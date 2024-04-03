# Comparing `tmp/ai-datahive-0.1.4.tar.gz` & `tmp/ai-datahive-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-datahive-0.1.4.tar", last modified: Tue Mar 19 18:15:11 2024, max compression
+gzip compressed data, was "ai-datahive-0.1.5.tar", last modified: Wed Apr  3 18:08:53 2024, max compression
```

## Comparing `ai-datahive-0.1.4.tar` & `ai-datahive-0.1.5.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.287470 ai-datahive-0.1.4/
--rw-rw-rw-   0        0        0     1085 2024-02-28 17:54:56.000000 ai-datahive-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       93 2024-03-19 18:04:54.000000 ai-datahive-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      570 2024-03-19 18:15:11.286579 ai-datahive-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4998 2024-03-09 15:08:20.000000 ai-datahive-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.246989 ai-datahive-0.1.4/ai_datahive/
--rw-rw-rw-   0        0        0        0 2024-03-11 14:33:26.000000 ai-datahive-0.1.4/ai_datahive/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.256988 ai-datahive-0.1.4/ai_datahive/collectors/
--rw-rw-rw-   0        0        0      231 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/collectors/__init__.py
--rw-rw-rw-   0        0        0     3726 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/collectors/arxiv_collector.py
--rw-rw-rw-   0        0        0     2423 2024-03-11 14:53:05.000000 ai-datahive-0.1.4/ai_datahive/collectors/base_collector.py
--rw-rw-rw-   0        0        0     4997 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/collectors/civitai_collector.py
--rw-rw-rw-   0        0        0     3862 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/collectors/github_collector.py
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.258988 ai-datahive-0.1.4/ai_datahive/collectors/models/
--rw-rw-rw-   0        0        0      112 2024-03-05 20:56:45.000000 ai-datahive-0.1.4/ai_datahive/collectors/models/__init__.py
--rw-rw-rw-   0        0        0     1005 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/collectors/models/github_project.py
--rw-rw-rw-   0        0        0     2641 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/collectors/models/media.py
--rw-rw-rw-   0        0        0      528 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/collectors/models/research_paper.py
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.262988 ai-datahive-0.1.4/ai_datahive/collectors/utils/
--rw-rw-rw-   0        0        0        0 2024-02-28 13:53:11.000000 ai-datahive-0.1.4/ai_datahive/collectors/utils/__init__.py
--rw-rw-rw-   0        0        0    19908 2024-02-20 18:30:47.000000 ai-datahive-0.1.4/ai_datahive/collectors/utils/allowed_github_parameter.py
--rw-rw-rw-   0        0        0    25962 2024-03-09 15:05:32.000000 ai-datahive-0.1.4/ai_datahive/collectors/utils/arxiv_helper.py
--rw-rw-rw-   0        0        0      483 2024-02-19 18:48:46.000000 ai-datahive-0.1.4/ai_datahive/collectors/utils/custom_exceptions.py
--rw-rw-rw-   0        0        0     7633 2024-02-28 13:58:34.000000 ai-datahive-0.1.4/ai_datahive/collectors/utils/github_helper.py
--rw-rw-rw-   0        0        0      833 2024-02-25 13:35:06.000000 ai-datahive-0.1.4/ai_datahive/collectors/utils/scraping_helper.py
--rw-rw-rw-   0        0        0     4947 2024-02-20 17:00:33.000000 ai-datahive-0.1.4/ai_datahive/collectors/utils/zotero_helper.py
--rw-rw-rw-   0        0        0     3793 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/collectors/zotero_collector.py
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.263987 ai-datahive-0.1.4/ai_datahive/dao/
--rw-rw-rw-   0        0        0      119 2024-03-11 14:23:44.000000 ai-datahive-0.1.4/ai_datahive/dao/__init__.py
--rw-rw-rw-   0        0        0     1257 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/dao/base_dao.py
--rw-rw-rw-   0        0        0      251 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/dao/dao_factory.py
--rw-rw-rw-   0        0        0     8848 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/dao/supabase_dao.py
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.265988 ai-datahive-0.1.4/ai_datahive/models/
--rw-rw-rw-   0        0        0       93 2024-03-04 19:54:55.000000 ai-datahive-0.1.4/ai_datahive/models/__init__.py
--rw-rw-rw-   0        0        0      341 2024-03-05 14:19:38.000000 ai-datahive-0.1.4/ai_datahive/models/base_model.py
--rw-rw-rw-   0        0        0      424 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/models/content_base_model.py
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.266989 ai-datahive-0.1.4/ai_datahive/publishers/
--rw-rw-rw-   0        0        0        0 2024-03-04 15:35:13.000000 ai-datahive-0.1.4/ai_datahive/publishers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.269987 ai-datahive-0.1.4/ai_datahive/publishers/loader/
--rw-rw-rw-   0        0        0       54 2024-03-06 20:28:03.000000 ai-datahive-0.1.4/ai_datahive/publishers/loader/__init__.py
--rw-rw-rw-   0        0        0     2695 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/publishers/loader/telegram_base_loader.py
--rw-rw-rw-   0        0        0     1006 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/publishers/loader/telegram_daily_arxiv_loader.py
--rw-rw-rw-   0        0        0     1144 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/publishers/loader/telegram_daily_trending_github_projects_loader.py
--rw-rw-rw-   0        0        0     1040 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/publishers/loader/telegram_top_daily_image_critique_loader.py
--rw-rw-rw-   0        0        0      968 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/publishers/loader/telegram_top_daily_image_loader.py
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.271988 ai-datahive-0.1.4/ai_datahive/publishers/models/
--rw-rw-rw-   0        0        0      144 2024-03-04 20:28:30.000000 ai-datahive-0.1.4/ai_datahive/publishers/models/__init__.py
--rw-rw-rw-   0        0        0      171 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/publishers/models/telegram_group.py
--rw-rw-rw-   0        0        0      211 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/publishers/models/telegram_group_topic.py
--rw-rw-rw-   0        0        0      514 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/publishers/models/telegram_message.py
--rw-rw-rw-   0        0        0     7262 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/publishers/telegram_bot.py
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.275988 ai-datahive-0.1.4/ai_datahive/services/
--rw-rw-rw-   0        0        0      266 2024-03-09 14:16:03.000000 ai-datahive-0.1.4/ai_datahive/services/__init__.py
--rw-rw-rw-   0        0        0      494 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/services/ai_backed_translation_service.py
--rw-rw-rw-   0        0        0      523 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/services/ai_service_factory.py
--rw-rw-rw-   0        0        0      337 2024-03-09 13:52:41.000000 ai-datahive-0.1.4/ai_datahive/services/base_ai_vision_service.py
--rw-rw-rw-   0        0        0      423 2024-03-09 14:14:43.000000 ai-datahive-0.1.4/ai_datahive/services/base_llm_service.py
--rw-rw-rw-   0        0        0      314 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/services/data_service.py
--rw-rw-rw-   0        0        0     2681 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/services/openai_service.py
--rw-rw-rw-   0        0        0     1947 2024-03-09 16:04:56.000000 ai-datahive-0.1.4/ai_datahive/services/prompt_service.py
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.277987 ai-datahive-0.1.4/ai_datahive/services/prompts/
--rw-rw-rw-   0        0        0     2133 2024-03-09 16:06:57.000000 ai-datahive-0.1.4/ai_datahive/services/prompts/js_style_image_critique_prompt.txt
--rw-rw-rw-   0        0        0       50 2024-03-06 19:11:41.000000 ai-datahive-0.1.4/ai_datahive/services/prompts/summarize_prompt.txt
--rw-rw-rw-   0        0        0       49 2024-03-06 19:11:41.000000 ai-datahive-0.1.4/ai_datahive/services/prompts/translate_prompt.txt
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.280986 ai-datahive-0.1.4/ai_datahive/transformers/
--rw-rw-rw-   0        0        0       62 2024-03-09 14:18:22.000000 ai-datahive-0.1.4/ai_datahive/transformers/__init__.py
--rw-rw-rw-   0        0        0     1715 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/transformers/base_content_transformer.py
--rw-rw-rw-   0        0        0     3266 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/transformers/daily_arxiv_paper_transformer.py
--rw-rw-rw-   0        0        0     3018 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/transformers/daily_trending_github_project_transformer.py
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.282070 ai-datahive-0.1.4/ai_datahive/transformers/models/
--rw-rw-rw-   0        0        0       30 2024-03-04 16:57:55.000000 ai-datahive-0.1.4/ai_datahive/transformers/models/__init__.py
--rw-rw-rw-   0        0        0      641 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/transformers/models/content.py
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.283579 ai-datahive-0.1.4/ai_datahive/transformers/templates/
--rw-rw-rw-   0        0        0       96 2024-03-06 19:41:54.000000 ai-datahive-0.1.4/ai_datahive/transformers/templates/daily_arxiv_paper_template.html
--rw-rw-rw-   0        0        0      138 2024-03-09 14:45:56.000000 ai-datahive-0.1.4/ai_datahive/transformers/templates/github_loader_trending_template.html
--rw-rw-rw-   0        0        0       88 2024-03-09 16:10:33.000000 ai-datahive-0.1.4/ai_datahive/transformers/templates/top_daily_image_critique_template.html
--rw-rw-rw-   0        0        0      136 2024-03-04 21:29:24.000000 ai-datahive-0.1.4/ai_datahive/transformers/templates/top_daily_image_template.html
--rw-rw-rw-   0        0        0     2854 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/transformers/top_daily_image_critique_transformer.py
--rw-rw-rw-   0        0        0     3151 2024-03-11 14:22:40.000000 ai-datahive-0.1.4/ai_datahive/transformers/top_daily_image_transformer.py
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.285579 ai-datahive-0.1.4/ai_datahive/utils/
--rw-rw-rw-   0        0        0        0 2024-02-25 13:31:44.000000 ai-datahive-0.1.4/ai_datahive/utils/__init__.py
--rw-rw-rw-   0        0        0      650 2024-03-04 19:36:47.000000 ai-datahive-0.1.4/ai_datahive/utils/datetime_helper.py
--rw-rw-rw-   0        0        0      842 2024-03-09 14:32:24.000000 ai-datahive-0.1.4/ai_datahive/utils/text_helper.py
-drwxrwxrwx   0        0        0        0 2024-03-19 18:15:11.285579 ai-datahive-0.1.4/ai_datahive.egg-info/
--rw-rw-rw-   0        0        0      570 2024-03-19 18:15:11.000000 ai-datahive-0.1.4/ai_datahive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3163 2024-03-19 18:15:11.000000 ai-datahive-0.1.4/ai_datahive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 18:15:11.000000 ai-datahive-0.1.4/ai_datahive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2024-03-19 18:15:11.000000 ai-datahive-0.1.4/ai_datahive.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-19 18:15:11.000000 ai-datahive-0.1.4/ai_datahive.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 18:15:11.287470 ai-datahive-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      652 2024-03-19 18:14:17.000000 ai-datahive-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.621750 ai-datahive-0.1.5/
+-rw-rw-rw-   0        0        0     1085 2024-02-28 17:54:56.000000 ai-datahive-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       93 2024-03-19 18:04:54.000000 ai-datahive-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      570 2024-04-03 18:08:53.620750 ai-datahive-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4998 2024-03-09 15:08:20.000000 ai-datahive-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.426169 ai-datahive-0.1.5/ai_datahive/
+-rw-rw-rw-   0        0        0        0 2024-03-11 14:33:26.000000 ai-datahive-0.1.5/ai_datahive/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.458678 ai-datahive-0.1.5/ai_datahive/collectors/
+-rw-rw-rw-   0        0        0      231 2024-03-11 14:22:40.000000 ai-datahive-0.1.5/ai_datahive/collectors/__init__.py
+-rw-rw-rw-   0        0        0     3618 2024-04-02 16:37:45.000000 ai-datahive-0.1.5/ai_datahive/collectors/arxiv_collector.py
+-rw-rw-rw-   0        0        0     1871 2024-04-02 16:28:44.000000 ai-datahive-0.1.5/ai_datahive/collectors/base_collector.py
+-rw-rw-rw-   0        0        0     5096 2024-04-02 16:37:20.000000 ai-datahive-0.1.5/ai_datahive/collectors/civitai_collector.py
+-rw-rw-rw-   0        0        0     3913 2024-04-02 16:36:56.000000 ai-datahive-0.1.5/ai_datahive/collectors/github_collector.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.471674 ai-datahive-0.1.5/ai_datahive/collectors/models/
+-rw-rw-rw-   0        0        0      112 2024-03-05 20:56:45.000000 ai-datahive-0.1.5/ai_datahive/collectors/models/__init__.py
+-rw-rw-rw-   0        0        0     1023 2024-04-01 16:46:30.000000 ai-datahive-0.1.5/ai_datahive/collectors/models/github_project.py
+-rw-rw-rw-   0        0        0     2483 2024-04-01 16:30:52.000000 ai-datahive-0.1.5/ai_datahive/collectors/models/media.py
+-rw-rw-rw-   0        0        0      483 2024-04-01 16:12:36.000000 ai-datahive-0.1.5/ai_datahive/collectors/models/research_paper.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.494674 ai-datahive-0.1.5/ai_datahive/collectors/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-28 13:53:11.000000 ai-datahive-0.1.5/ai_datahive/collectors/utils/__init__.py
+-rw-rw-rw-   0        0        0    19908 2024-02-20 18:30:47.000000 ai-datahive-0.1.5/ai_datahive/collectors/utils/allowed_github_parameter.py
+-rw-rw-rw-   0        0        0    25962 2024-03-09 15:05:32.000000 ai-datahive-0.1.5/ai_datahive/collectors/utils/arxiv_helper.py
+-rw-rw-rw-   0        0        0      483 2024-02-19 18:48:46.000000 ai-datahive-0.1.5/ai_datahive/collectors/utils/custom_exceptions.py
+-rw-rw-rw-   0        0        0     7633 2024-02-28 13:58:34.000000 ai-datahive-0.1.5/ai_datahive/collectors/utils/github_helper.py
+-rw-rw-rw-   0        0        0      833 2024-02-25 13:35:06.000000 ai-datahive-0.1.5/ai_datahive/collectors/utils/scraping_helper.py
+-rw-rw-rw-   0        0        0     4947 2024-02-20 17:00:33.000000 ai-datahive-0.1.5/ai_datahive/collectors/utils/zotero_helper.py
+-rw-rw-rw-   0        0        0     3784 2024-04-02 16:28:44.000000 ai-datahive-0.1.5/ai_datahive/collectors/zotero_collector.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.504673 ai-datahive-0.1.5/ai_datahive/dao/
+-rw-rw-rw-   0        0        0       81 2024-04-02 15:51:26.000000 ai-datahive-0.1.5/ai_datahive/dao/__init__.py
+-rw-rw-rw-   0        0        0     1245 2024-04-01 16:54:42.000000 ai-datahive-0.1.5/ai_datahive/dao/base_dao.py
+-rw-rw-rw-   0        0        0     8183 2024-04-01 16:56:49.000000 ai-datahive-0.1.5/ai_datahive/dao/supabase_dao.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.512674 ai-datahive-0.1.5/ai_datahive/models/
+-rw-rw-rw-   0        0        0       93 2024-03-04 19:54:55.000000 ai-datahive-0.1.5/ai_datahive/models/__init__.py
+-rw-rw-rw-   0        0        0      395 2024-04-01 16:16:17.000000 ai-datahive-0.1.5/ai_datahive/models/base_model.py
+-rw-rw-rw-   0        0        0      543 2024-04-01 15:28:04.000000 ai-datahive-0.1.5/ai_datahive/models/content_base_model.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.517674 ai-datahive-0.1.5/ai_datahive/publishers/
+-rw-rw-rw-   0        0        0        0 2024-03-04 15:35:13.000000 ai-datahive-0.1.5/ai_datahive/publishers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.538745 ai-datahive-0.1.5/ai_datahive/publishers/loader/
+-rw-rw-rw-   0        0        0       54 2024-03-06 20:28:03.000000 ai-datahive-0.1.5/ai_datahive/publishers/loader/__init__.py
+-rw-rw-rw-   0        0        0     3282 2024-04-02 16:20:47.000000 ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_base_loader.py
+-rw-rw-rw-   0        0        0     1377 2024-04-02 15:31:13.000000 ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_daily_arxiv_loader.py
+-rw-rw-rw-   0        0        0     1464 2024-04-02 15:18:12.000000 ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_daily_trending_github_projects_loader.py
+-rw-rw-rw-   0        0        0     1391 2024-04-02 15:38:15.000000 ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_top_daily_image_critique_loader.py
+-rw-rw-rw-   0        0        0     1322 2024-04-02 15:30:50.000000 ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_top_daily_image_loader.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.549745 ai-datahive-0.1.5/ai_datahive/publishers/models/
+-rw-rw-rw-   0        0        0      144 2024-03-04 20:28:30.000000 ai-datahive-0.1.5/ai_datahive/publishers/models/__init__.py
+-rw-rw-rw-   0        0        0      171 2024-03-11 14:22:40.000000 ai-datahive-0.1.5/ai_datahive/publishers/models/telegram_group.py
+-rw-rw-rw-   0        0        0      211 2024-03-11 14:22:40.000000 ai-datahive-0.1.5/ai_datahive/publishers/models/telegram_group_topic.py
+-rw-rw-rw-   0        0        0      532 2024-04-01 15:40:56.000000 ai-datahive-0.1.5/ai_datahive/publishers/models/telegram_message.py
+-rw-rw-rw-   0        0        0     7256 2024-04-02 15:53:48.000000 ai-datahive-0.1.5/ai_datahive/publishers/telegram_bot.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.573745 ai-datahive-0.1.5/ai_datahive/services/
+-rw-rw-rw-   0        0        0      266 2024-03-09 14:16:03.000000 ai-datahive-0.1.5/ai_datahive/services/__init__.py
+-rw-rw-rw-   0        0        0      494 2024-03-11 14:22:40.000000 ai-datahive-0.1.5/ai_datahive/services/ai_backed_translation_service.py
+-rw-rw-rw-   0        0        0      523 2024-03-11 14:22:40.000000 ai-datahive-0.1.5/ai_datahive/services/ai_service_factory.py
+-rw-rw-rw-   0        0        0      337 2024-03-09 13:52:41.000000 ai-datahive-0.1.5/ai_datahive/services/base_ai_vision_service.py
+-rw-rw-rw-   0        0        0      423 2024-03-09 14:14:43.000000 ai-datahive-0.1.5/ai_datahive/services/base_llm_service.py
+-rw-rw-rw-   0        0        0      314 2024-03-11 14:22:40.000000 ai-datahive-0.1.5/ai_datahive/services/data_service.py
+-rw-rw-rw-   0        0        0     2681 2024-03-11 14:22:40.000000 ai-datahive-0.1.5/ai_datahive/services/openai_service.py
+-rw-rw-rw-   0        0        0     1947 2024-03-09 16:04:56.000000 ai-datahive-0.1.5/ai_datahive/services/prompt_service.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.575747 ai-datahive-0.1.5/ai_datahive/services/prompts/
+-rw-rw-rw-   0        0        0     2133 2024-03-09 16:06:57.000000 ai-datahive-0.1.5/ai_datahive/services/prompts/js_style_image_critique_prompt.txt
+-rw-rw-rw-   0        0        0       50 2024-03-06 19:11:41.000000 ai-datahive-0.1.5/ai_datahive/services/prompts/summarize_prompt.txt
+-rw-rw-rw-   0        0        0       49 2024-03-06 19:11:41.000000 ai-datahive-0.1.5/ai_datahive/services/prompts/translate_prompt.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.599747 ai-datahive-0.1.5/ai_datahive/transformers/
+-rw-rw-rw-   0        0        0       62 2024-03-09 14:18:22.000000 ai-datahive-0.1.5/ai_datahive/transformers/__init__.py
+-rw-rw-rw-   0        0        0     2600 2024-04-02 16:20:28.000000 ai-datahive-0.1.5/ai_datahive/transformers/base_content_transformer.py
+-rw-rw-rw-   0        0        0     2710 2024-04-02 16:41:37.000000 ai-datahive-0.1.5/ai_datahive/transformers/daily_arxiv_paper_transformer.py
+-rw-rw-rw-   0        0        0     2907 2024-04-02 16:28:44.000000 ai-datahive-0.1.5/ai_datahive/transformers/daily_trending_github_project_transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.606745 ai-datahive-0.1.5/ai_datahive/transformers/models/
+-rw-rw-rw-   0        0        0       30 2024-03-04 16:57:55.000000 ai-datahive-0.1.5/ai_datahive/transformers/models/__init__.py
+-rw-rw-rw-   0        0        0      610 2024-03-20 16:46:25.000000 ai-datahive-0.1.5/ai_datahive/transformers/models/content.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.608747 ai-datahive-0.1.5/ai_datahive/transformers/templates/
+-rw-rw-rw-   0        0        0       96 2024-03-06 19:41:54.000000 ai-datahive-0.1.5/ai_datahive/transformers/templates/daily_arxiv_paper_template.html
+-rw-rw-rw-   0        0        0      132 2024-04-02 16:40:23.000000 ai-datahive-0.1.5/ai_datahive/transformers/templates/github_loader_trending_template.html
+-rw-rw-rw-   0        0        0       88 2024-03-09 16:10:33.000000 ai-datahive-0.1.5/ai_datahive/transformers/templates/top_daily_image_critique_template.html
+-rw-rw-rw-   0        0        0      136 2024-03-04 21:29:24.000000 ai-datahive-0.1.5/ai_datahive/transformers/templates/top_daily_image_template.html
+-rw-rw-rw-   0        0        0     2858 2024-04-02 16:41:37.000000 ai-datahive-0.1.5/ai_datahive/transformers/top_daily_image_critique_transformer.py
+-rw-rw-rw-   0        0        0     2463 2024-04-02 17:15:38.000000 ai-datahive-0.1.5/ai_datahive/transformers/top_daily_image_transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.619753 ai-datahive-0.1.5/ai_datahive/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-25 13:31:44.000000 ai-datahive-0.1.5/ai_datahive/utils/__init__.py
+-rw-rw-rw-   0        0        0      247 2024-04-02 15:55:29.000000 ai-datahive-0.1.5/ai_datahive/utils/dao_factory.py
+-rw-rw-rw-   0        0        0     1957 2024-04-02 15:59:25.000000 ai-datahive-0.1.5/ai_datahive/utils/datetime_helper.py
+-rw-rw-rw-   0        0        0      842 2024-03-09 14:32:24.000000 ai-datahive-0.1.5/ai_datahive/utils/text_helper.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:08:53.620750 ai-datahive-0.1.5/ai_datahive.egg-info/
+-rw-rw-rw-   0        0        0      570 2024-04-03 18:08:53.000000 ai-datahive-0.1.5/ai_datahive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3165 2024-04-03 18:08:53.000000 ai-datahive-0.1.5/ai_datahive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 18:08:53.000000 ai-datahive-0.1.5/ai_datahive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2024-04-03 18:08:53.000000 ai-datahive-0.1.5/ai_datahive.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-03 18:08:53.000000 ai-datahive-0.1.5/ai_datahive.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 18:08:53.621750 ai-datahive-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      652 2024-04-03 18:08:41.000000 ai-datahive-0.1.5/setup.py
```

### Comparing `ai-datahive-0.1.4/LICENSE` & `ai-datahive-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.4/PKG-INFO` & `ai-datahive-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-datahive
-Version: 0.1.4
+Version: 0.1.5
 Summary: ETL Package for crawling data, transform it with AI and store it in a datastorage.
 Author: Danny Gerst
 Author-email: d.gerst@bizrock.de
 License-File: LICENSE
 Requires-Dist: python-dotenv
 Requires-Dist: pydantic
 Requires-Dist: inflect
```

### Comparing `ai-datahive-0.1.4/README.md` & `ai-datahive-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.4/ai_datahive/collectors/arxiv_collector.py` & `ai-datahive-0.1.5/ai_datahive/collectors/arxiv_collector.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 from ai_datahive.collectors.models import ResearchPaper
 
 
 class ArxivCollector(BaseCollector):
 
     VALID_PERIODS = ['Day']
 
-    def __init__(self, creator_name='ArxivCollector', arxiv_category='cs.AI', period='Day', tags=None, limit=3):
+    def __init__(self, creator='ArxivCollector', arxiv_category='cs.AI', period='Day', tags=None, limit=3):
         self.validate_parameters(arxiv_category, period)
 
-        self.creator_name = creator_name
+        self.creator = creator
         self.limit = limit
         self.arxiv_category = arxiv_category
         self.period = period
 
         if tags is None:
             self.tags = self.build_tags(arxiv_category, period)
         else:
             self.tags = tags
 
-        super().__init__(creator_name=self.creator_name, content_type=ResearchPaper)
+        super().__init__(creator=self.creator, content_type=ResearchPaper)
 
     def validate_parameters(self, arxiv_category, period) -> None:
         if arxiv_category not in ah.ALL_CATEGORIES:
             raise ValueError(f"category must be one of {ah.ALL_CATEGORIES}")
         if period not in self.VALID_PERIODS:
             raise ValueError(f"period must be one of {self.VALID_PERIODS}")
 
@@ -70,32 +70,29 @@
                     now = datetime.now(timezone.utc)
                     paper = ResearchPaper(
                         title=item['title'],
                         abstract=item['description'],
                         source_id=item['guid'],
                         authors=item['authors'],
                         license=item['rights'],
-                        source='Arxiv',
-                        creator=self.creator_name,
+                        source_name='Arxiv',
+                        creator=self.creator,
                         tags=self.tags,
                         paper_submitted_at=now,
                         paper_url=item['link'],
-                        # TODO rework function call
-                        reference_url=ah.search_day_submissions(self.arxiv_category, os.getenv('ARXIV_RSS_LINK'))
+                        # TODO rework function call to get the RSS LINK
+                        source_url=ah.search_day_submissions(self.arxiv_category, os.getenv('ARXIV_RSS_LINK'))
                     )
                     result.append(paper)
         return result
 
 
 def main():
     load_dotenv()
     arxiv_collector = ArxivCollector()
     data = arxiv_collector.run()
-    #result = arxiv_collector.save(data)
-    print(data)
-    #media = civitai_collector.convert_to_media(data)
-
-    #print(media)
+    if data:
+        print(data)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ai-datahive-0.1.4/ai_datahive/collectors/base_collector.py` & `ai-datahive-0.1.5/ai_datahive/collectors/base_collector.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from typing import Optional, Type, Union
 from collections.abc import Collection
 
-from datetime import datetime, timezone, timedelta
+from datetime import timedelta
 
 from ai_datahive.models import ContentBaseModel
+from ai_datahive.utils import datetime_helper
 
 
 class BaseCollector:
 
-    def __init__(self, content_type: Optional[Type[ContentBaseModel]], creator_name: str,
+    def __init__(self, content_type: Optional[Type[ContentBaseModel]], creator: str,
                  run_interval: timedelta = timedelta(days=1)):
-        from ai_datahive.dao.dao_factory import dao_factory
+        from ai_datahive.utils.dao_factory import get_dao
 
-        self.creator_name = creator_name
+        self.creator = creator
         self.content_type = content_type
         self.run_interval = run_interval
 
-        self.dao = dao_factory()
+        self.dao = get_dao()
 
     def get_latest_message_date(self):
         # Get date from the latest message to the telegram table - using topic / reporter
         if self.content_type is None:
             raise NotImplementedError('If no content_type is defined, you have to implement this method.')
 
-        result = self.dao.get_latest_entity_date(self.content_type, self.creator_name)
+        result = self.dao.get_latest_entity_date(self.content_type, self.creator)
+
         return result
 
     def retrieve(self) -> Union[ContentBaseModel, Collection[ContentBaseModel]]:
         # Get data from the source
         raise NotImplementedError
 
     def save(self, data: Union[ContentBaseModel, Collection[ContentBaseModel]]):
@@ -35,32 +37,16 @@
             result = []
             for item in data:
                 result.append(self.dao.create(item))
             return result
         else:
             return self.dao.create(data)
 
-    def is_due(self):
-        latest_entity_date = self.get_latest_message_date()
-        if latest_entity_date is None:
-            return True
-
-        latest_entity_date = latest_entity_date.astimezone(timezone.utc)
-        now = datetime.now(timezone.utc)
-        time_diff = now - latest_entity_date
-
-        if time_diff < self.run_interval:
-            total_seconds = time_diff.total_seconds()
-            hours = int(total_seconds // 3600)
-            minutes = int((total_seconds % 3600) // 60)
-            print(f"Weniger als 24 Stunden seit der letzten Nachricht vergangen: "
-                  f"Vergangen bisher: {hours:02d}:{minutes:02d}")
-            return False
-        return True
-
     def run(self):
-        if self.is_due():
+        is_due = datetime_helper.is_due(content_type=self.content_type, creator=self.creator,
+                                        run_interval=self.run_interval)
+        if is_due:
             try:
                 data = self.retrieve()
-                self.save(data=data)
+                return self.save(data=data)
             except Exception as e:
-                print(f"Error in {self.creator_name}: {e}")
+                print(f"Error in {self.creator}: {e}")
```

### Comparing `ai-datahive-0.1.4/ai_datahive/collectors/civitai_collector.py` & `ai-datahive-0.1.5/ai_datahive/collectors/civitai_collector.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 class CivitaiCollector(BaseCollector):
     VALID_PERIODS = ['AllTime', 'Year', 'Month', 'Week', 'Day']
     VALID_MEDIA_TYPES = ['image', 'video', 'model']
     VALID_NSFW_LEVELS = [None, 'Soft', 'Mature', 'X']
     VALID_SORTS = ['Most Reactions', 'Most Buzz', 'Most Comments', 'Most Collected', 'Oldest']
 
-    def __init__(self, creator_name='CivitaiCollector', media_type='image', period='Day', sort='Most Reactions',
+    def __init__(self, creator='CivitaiCollector', media_type='image', period='Day', sort='Most Reactions',
                  nsfw=None, tags=None, limit=1):
-        self.creator_name = creator_name
+        self.creator = creator
         if tags is None:
             self.tags = self.build_tags(media_type, period, sort, nsfw)
         else:
             self.tags = tags
         self.limit = limit
 
         self.validate_parameters(media_type, period, nsfw, sort)
@@ -33,15 +33,15 @@
         else:
             self.media_type = media_type
         # END - Workaround as long as there is no way to get videos directly from Civitai
 
         base_url = os.getenv('CIVITAI_API_URL', '')
         self.civitai_url = self.build_url(base_url, media_type, sort, nsfw, period, limit)
 
-        super().__init__(creator_name=self.creator_name, content_type=Media)
+        super().__init__(creator=self.creator, content_type=Media)
 
     def build_tags(self, media_type, period, sort, nsfw):
         tags = 'civitai, '
         tags += media_type.lower() + ', '
         tags += to_periodic_format(period) + ', '
         tags += sort.lower() + ', '
 
@@ -82,37 +82,42 @@
             print(f"Es gab einen Fehler bei der Anfrage: {data}")
 
     def convert_to_media(self, data):
         result = []
         if data:
             for item in data['items']:
                 media = Media(
-                    creator=self.creator_name,
+                    creator=self.creator,
                     media_url=item['url'],
                     media_type=self.media_type,
                     likes=item['stats']['likeCount'],
                     hearts=item['stats']['heartCount'],
                     prompt=item['meta'].get('prompt') if item.get('meta') is not None else None,
                     model=item['meta'].get('Model').split('.')[0] if item.get('meta') is not None and
                                                                      item['meta'].get('Model') is not None else None,
                     author=item['username'],
                     tags=self.tags,
-                    source='Civitai',
+                    source_name='Civitai',
+                    source_url=self.civitai_url,
                     media_created_at=item['createdAt']
                 )
                 result.append(media)
         return result
 
 
 def main():
     load_dotenv()
 
-    civitai_image_loader = CivitaiCollector(creator_name='CivitAIDailyTopImage', media_type='image', period='Day',
+    civitai_image_loader = CivitaiCollector(creator='CivitAIDailyTopImage', media_type='image', period='Day',
                                             nsfw=None, limit=3)
-    civitai_image_loader.run()
-    civitai_hot_image_loader = CivitaiCollector(creator_name='CivitAIDailyTopHotImage', media_type='image',
+    data = civitai_image_loader.run()
+    if data:
+        print(data)
+    civitai_hot_image_loader = CivitaiCollector(creator='CivitAIDailyTopHotImage', media_type='image',
                                                 period='Day', nsfw='Mature', limit=3)
-    civitai_hot_image_loader.run()
+    data = civitai_hot_image_loader.run()
+    if data:
+        print(data)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ai-datahive-0.1.4/ai_datahive/collectors/github_collector.py` & `ai-datahive-0.1.5/ai_datahive/collectors/github_collector.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 
 
 class GithubCollector(BaseCollector):
 
     VALID_PERIODS = ['Day', 'Week', 'Month']
 
     #TODO if needed use more parameters, right now fixed to github trending repos
-    def __init__(self, creator_name='GithubCollector', period='Day', tags=None, limit=3):
-        self.creator_name = creator_name
+    def __init__(self, creator='GithubCollector', period='Day', tags=None, limit=3):
+        self.creator = creator
         self.limit = limit
         self.period = period
         self.media_type = 'github_project'
         self.github_url = os.getenv('GITHUB_TRENDS_URL')
 
         if tags is None:
             self.tags = self.build_tags(period)
         else:
             self.tags = tags
 
         self.validate_parameters(period)
 
-        super().__init__(creator_name=self.creator_name, content_type=GithubProject)
+        super().__init__(creator=self.creator, content_type=GithubProject)
 
     def validate_parameters(self, period):
         if period not in self.VALID_PERIODS:
             raise ValueError(f"period must be one of {self.VALID_PERIODS}")
 
     def build_tags(self, period):
         tags = 'github, '
@@ -75,37 +75,38 @@
                 # Format output
                 if len(contributors) > 3:
                     output = ', '.join(contributors[:3]) + ', et al.'
                 else:
                     output = ', '.join(contributors)
 
                 project = GithubProject(
-                    creator=self.creator_name,
+                    creator=self.creator,
                     rank=item['rank'],
                     username=item['username'],
                     name=item['repositoryName'],
                     url=item['url'],
                     description=item['description'],
                     program_language=item['language'],
-                    language=item['language'],
+                    lang='en',  # TODO Determine language with AI based on the title and description
                     total_stars=item['totalStars'],
                     forks=item['forks'],
                     new_stars=item['starsSince'],
-                    since=item['since'],
+                    periodicity=item['since'],
                     tags=self.tags,
-                    source='GitHub Trending',
+                    source_name='GitHub Trends',
+                    source_url=self.github_url,
                     contributors=output
                 )
                 result.append(project)
         return result
 
 
 def main():
     load_dotenv()
     github_collector = GithubCollector()
-    data = github_collector.retrieve()
-    result = github_collector.save(data)
-    print(result)
+    data = github_collector.run()
+    if data:
+        print(data)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ai-datahive-0.1.4/ai_datahive/collectors/models/github_project.py` & `ai-datahive-0.1.5/ai_datahive/collectors/models/github_project.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,20 +12,20 @@
     name: str = Field(..., max_length=255)
     url: HttpUrl
     description: Optional[str] = None
     program_language: Optional[str] = Field(None, max_length=255)
     total_stars: Optional[int] = None
     forks: Optional[int] = None
     new_stars: Optional[int] = None
-    since: str = Field(..., max_length=50)
+    periodicity: str = Field(..., max_length=50)
     contributors: Optional[str] = None
 
     class Config:
         json_encoders = {
             HttpUrl: lambda v: str(v)
         }
 
-    @field_validator('since')
-    def check_since(cls, v: str) -> str:
+    @field_validator('periodicity')
+    def check_periodicity(cls, v: str) -> str:
         if v not in cls.VALID_PERIODICITY:
             raise ValueError(f"since must be one of {cls.VALID_PERIODICITY}")
         return v
```

### Comparing `ai-datahive-0.1.4/ai_datahive/collectors/models/media.py` & `ai-datahive-0.1.5/ai_datahive/collectors/models/media.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,30 +2,26 @@
 from typing import Union, Optional, ClassVar
 from ai_datahive.models import ContentBaseModel
 from pydantic import HttpUrl, field_validator
 import base64
 
 
 class Media(ContentBaseModel):
-    VALID_MEDIA_TYPES: ClassVar[list[str]] = ['image', 'video', 'model', 'text', 'paper', 'news', 'prompt',
-                                              'website', 'pdf']
-
+    VALID_MEDIA_TYPES: ClassVar[list[str]] = ['image', 'video', 'audio', 'text', 'pdf']
     media_url: Optional[HttpUrl] = None
     media_b64_content: Optional[str] = None
     media_type: str
     title: Optional[str] = None
     description: Optional[str] = None
     likes: int = 0
     hearts: int = 0
     prompt: Optional[str] = None
     model: Optional[str] = None
     author: Optional[str] = None
-    source: Optional[str] = None
-    reference_url: Optional[HttpUrl] = None
-    media_reference_id: Optional[Union['Media', str]] = None  # TODO To low leve, should refernce the media object
+    # media_reference_id: Optional[Union['Media', str]] = None  # TODO To low level, should reference another media object
     media_created_at: Union[datetime, str]
 
     class Config:
         json_encoders = {
             HttpUrl: lambda v: str(v),
             datetime: lambda v: v.isoformat(),
         }
```

### Comparing `ai-datahive-0.1.4/ai_datahive/collectors/utils/allowed_github_parameter.py` & `ai-datahive-0.1.5/ai_datahive/collectors/utils/allowed_github_parameter.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.4/ai_datahive/collectors/utils/arxiv_helper.py` & `ai-datahive-0.1.5/ai_datahive/collectors/utils/arxiv_helper.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.4/ai_datahive/collectors/utils/github_helper.py` & `ai-datahive-0.1.5/ai_datahive/collectors/utils/github_helper.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.4/ai_datahive/collectors/utils/scraping_helper.py` & `ai-datahive-0.1.5/ai_datahive/collectors/utils/scraping_helper.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.4/ai_datahive/collectors/utils/zotero_helper.py` & `ai-datahive-0.1.5/ai_datahive/collectors/utils/zotero_helper.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.4/ai_datahive/collectors/zotero_collector.py` & `ai-datahive-0.1.5/ai_datahive/collectors/zotero_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import os
 from dotenv import load_dotenv
 from datetime import datetime, timedelta
 
-from ai_datahive.models import Media
+from ai_datahive.collectors.models import Media
 from ai_datahive.collectors import BaseCollector
 from ai_datahive.collectors.utils.zotero_helper import ZoteroHelper
 
 
 class ZoteroCollector(BaseCollector):
 
-    def __init__(self, collection_name, content_type='media', creator_name='ZoteroCollector', zotero_api_key=None,
+    def __init__(self, collection_name, content_type='media', creator='ZoteroCollector', zotero_api_key=None,
                  zotero_library_id=None, zotero_library_type='user', all_types=False, tags=None, limit=3):
 
         zotero_api_key = os.getenv('ZOTERO_API_KEY') if zotero_api_key is None else zotero_api_key
         zotero_library_id = os.getenv('ZOTERO_USER_ID') if zotero_library_id is None else zotero_library_id
 
         self.zotero_library_id = zotero_library_id
         self.collection_name = collection_name
         self.limit = limit
         self.all_types = all_types
         self.content_type = content_type
         self.zotero_helper = ZoteroHelper(zotero_api_key, zotero_library_id, zotero_library_type)
 
-        super().__init__(creator_name=creator_name, content_type=content_type)
+        super().__init__(creator=creator, content_type=content_type)
 
     def build_tags(self, itemType, repository):
         tags = 'zotero, '
         if itemType:
             tags += itemType + ', '
         if repository:
             tags += repository + ', '
@@ -60,15 +60,15 @@
                 # Format output
                 if len(full_names) > 3:
                     output_creators = ', '.join(full_names[:3]) + ', et al.'
                 else:
                     output_creators = ', '.join(full_names)
 
                 media = Media(
-                    creator=self.creator_name,
+                    creator=self.creator,
                     media_type='paper',
                     title=data['data'].get('title', ''),
                     description=data['data'].get('abstractNote', ''),
                     author=output_creators,
                     tags=self.build_tags(data['data'].get('itemType'), data['data'].get('repository')),
                     source='Zotero - ' + self.zotero_library_id,
                     media_created_at=data['data'].get('date', ''),
```

### Comparing `ai-datahive-0.1.4/ai_datahive/dao/base_dao.py` & `ai-datahive-0.1.5/ai_datahive/dao/base_dao.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
     def update(self, entity: DataHiveBaseModel, id=None) -> DataHiveBaseModel:
         raise NotImplementedError
 
     def delete(self, entity: DataHiveBaseModel, id=None):
         raise NotImplementedError
 
-    def get_latest_entity_date(self, entity: Type[DataHiveBaseModel], creator_name: str) -> Union[datetime, None]:
-        entity = self.read(entity, filters=[['creator', creator_name]], order_by='created_at', order_dir='desc',
-                             limit=1)
+    def get_latest_entity_date(self, entity: Type[DataHiveBaseModel], creator: str) -> Union[datetime, None]:
+        entity = self.read(entity, filters=[['creator', creator]], order_by='created_at', order_dir='desc',
+                           limit=1)
 
         if entity:
             entity = entity[0]
             return entity.created_at
         else:
             return None
```

### Comparing `ai-datahive-0.1.4/ai_datahive/dao/supabase_dao.py` & `ai-datahive-0.1.5/ai_datahive/dao/supabase_dao.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,22 +43,22 @@
                     # Nun müssen wir operator_criteria in Operator und Kriterium aufteilen
                     operator, criteria = operator_criteria.split('.', 1)
                     result = result.filter(field, operator, criteria)
                 else:
                     # Fallback, falls das Format ungültig ist
                     print(f"Fehler: Filterformat ist ungültig: '{query}'")
 
+            # Order By und Richtung anwenden, wenn spezifiziert
+        if order_by is not None:
+            result = result.order(order_by, desc=(order_dir == 'desc'))
+
             # Limit anwenden, wenn spezifiziert
         if limit is not None:
             result = result.limit(limit)
 
-            # Order By und Richtung anwenden, wenn spezifiziert
-        if order_by is not None:
-            result = result.order(order_by, desc=(order_dir == 'asc'))
-
         return [self._row_to_model_instance(row, entity) for row in result.execute().data]
 
     def update(self, entity: T, id=None):
         table_name = self.table_name_from_model(type(entity))
         row_data = self._model_instance_to_row(entity)
         if id is None:
             id = entity.id
@@ -128,14 +128,16 @@
         p = inflect.engine()
         model_name = model.__name__
         table_name_snake_case = re.sub(r'(?<!^)(?=[A-Z])', '_', model_name).lower()
 
         # TODO find a better way to handle pluralization
         if 'media' in table_name_snake_case:
             table_name_plural = 'media'
+        elif 'content' in table_name_snake_case:
+            table_name_plural = 'content'
         else:
             table_name_plural = p.plural_noun(table_name_snake_case)
 
         table_name = f"t_{table_name_plural}"
         return table_name
 
     def convert_filters_to_query(self, filters: List[Filter]) -> List[str]:
@@ -165,32 +167,14 @@
             if isinstance(result, list):
                 query_filters.extend(result)
             else:
                 query_filters.append(result)
 
         return query_filters
 
-    #def get_latest_data_date(self, creator_name: str, table_name: str):
-    #    # Get date from the latest message to the telegram table - using topic / reporter
-    #    #table_name = f't_{content_type}'
-    #    result = self.supabase_client.table(table_name) \
-    #        .select('created_at') \
-    #        .eq('creator', creator_name) \
-    #        .order('created_at', desc=True) \
-    #        .limit(1) \
-    #        .execute()
-
-    #    if result.data:
-            # Gehe davon aus, dass `created_at` das Datum beinhaltet
-    #        return datetime.fromisoformat(result.data[0]['created_at'])
-    #    else:
-    #        return datetime.now() - timedelta(weeks=1)
-
-    # Implementiere die restlichen Methoden entsprechend
-
 
 def main():
     from dotenv import load_dotenv
     from ai_datahive.publishers.models import TelegramMessage
 
     load_dotenv()
```

### Comparing `ai-datahive-0.1.4/ai_datahive/publishers/loader/telegram_base_loader.py` & `ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_base_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from typing import Union, List
+from datetime import timedelta
 
 from ai_datahive.publishers.models import TelegramMessage, TelegramGroup, TelegramGroupTopic
 
 from ai_datahive.transformers.models import Content
 
+from ai_datahive.utils import datetime_helper
+
 
 class TelegramBaseLoader:
-    def __init__(self, telegram_group_name, telegram_group_topic_id):
-        from ai_datahive.dao.dao_factory import dao_factory
-        self.dao = dao_factory()
+    def __init__(self, creator, language, telegram_group_name, telegram_group_topic_id,
+                 run_interval: timedelta = timedelta(days=1)):
+        from ai_datahive.utils.dao_factory import get_dao
+        self.dao = get_dao()
 
         tgr = self.dao.read(TelegramGroup, [["telegram_group_name", telegram_group_name]], limit=1)
         if not tgr:
             raise ValueError(f"Telegram-Gruppe '{telegram_group_name}' nicht gefunden.")
 
         self.telegram_group_uuid = tgr[0].id
         self.telegram_group_topic_id = telegram_group_topic_id
+        self.creator = creator
+        self.language = language
+        self.run_interval = run_interval
 
     def retrieve(self):
-        raise NotImplementedError
+        raise NotImplementedError()
 
     def find_group_topic_uuid(self):
         filters = [
             ["telegram_group_topic_id", self.telegram_group_topic_id],
             ["telegram_group_fk", self.telegram_group_uuid]
         ]
 
@@ -44,15 +51,15 @@
         else:
             str_content = content.content
 
         # Datenstruktur für die neue Nachricht
         message_data = {
             'telegram_group_topic_fk': group_topic_uuid,
             'content': f"<b>{content.title}</b>\n\n{str_content}",
-            'creator': content.creator,
+            'creator': self.creator,
             'status': 'planned'
         }
 
         if content.media_type and (content.media_url or content.media_content):
             message_data['media_type'] = content.media_type
             if content.media_url:
                 message_data['media_url'] = content.media_url
@@ -63,9 +70,13 @@
         if content.scheduled_for:
             message_data['schedule_for'] = content.schedule_for
 
         # Speichern der Nachricht in der Tabelle `t_telegram_messages`
         result = self.dao.create(TelegramMessage(**message_data))
 
     def load(self):
-        content = self.retrieve()
-        self.save_content_as_telegram_message(content)
+        is_due = datetime_helper.is_due(content_type=TelegramMessage, creator=self.creator,
+                                        run_interval=self.run_interval)
+        if is_due:
+            content = self.retrieve()
+            if (isinstance(content, list) and len(content) > 0) or (content is not None and not isinstance(content, list)):
+                self.save_content_as_telegram_message(content)
```

### Comparing `ai-datahive-0.1.4/ai_datahive/publishers/loader/telegram_daily_arxiv_loader.py` & `ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_top_daily_image_critique_loader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 from ai_datahive.transformers.models import Content
 
-from ai_datahive.utils.datetime_helper import today_as_start_and_enddate_str
+from ai_datahive.utils.datetime_helper import today_as_start_and_enddate_str, get_start_and_end_times_based_on_interval
 
 from ai_datahive.publishers.loader import TelegramBaseLoader
 
 
-class TelegramDailyArxivLoader(TelegramBaseLoader):
+class TelegramTopDailyImageCritiqueLoader(TelegramBaseLoader):
 
-    def __init__(self, telegram_group_name, telegram_group_topic_id):
-        super().__init__(telegram_group_name, telegram_group_topic_id)
+    def __init__(self, telegram_group_name, telegram_group_topic_id, creator='TelegramTopDailyImageCritiqueLoader',
+                 language='de'):
+        super().__init__(creator, language, telegram_group_name, telegram_group_topic_id)
 
     def retrieve(self):
-        start_date_str, end_date_str = today_as_start_and_enddate_str()
+        if self.run_interval:
+            start_date_str, end_date_str = get_start_and_end_times_based_on_interval(self.run_interval)
+        else:
+            start_date_str, end_date_str = today_as_start_and_enddate_str()
+
         filters = [
-            ["creator", "DailyArxivPaper"],
-            ["language", "de"],
+            ["creator", "DailyImageCritiqueJS"],
+            ["lang", self.language],
             ["created_at", "between", start_date_str, end_date_str]
         ]
 
-        paper = self.dao.read(Content, filters, limit=1)
-        return paper[0]
+        topimage = self.dao.read(Content, filters, limit=1)
+        if topimage:
+            return topimage[0]
+        return None
 
 
 def main():
     from dotenv import load_dotenv
     load_dotenv()
-    ARXIV_GROUP_TOPIC_ID = 2
-    loader = TelegramDailyArxivLoader('KI & Business', ARXIV_GROUP_TOPIC_ID)
+    IMAGE_GROUP_TOPIC_ID = 27
+    loader = TelegramTopDailyImageCritiqueLoader('KI & Business', IMAGE_GROUP_TOPIC_ID)
     loader.load()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ai-datahive-0.1.4/ai_datahive/publishers/loader/telegram_daily_trending_github_projects_loader.py` & `ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_daily_trending_github_projects_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from ai_datahive.transformers.models import Content
 
 from ai_datahive.publishers.loader import TelegramBaseLoader
-from ai_datahive.utils.datetime_helper import today_as_start_and_enddate_str
+from ai_datahive.utils.datetime_helper import today_as_start_and_enddate_str, get_start_and_end_times_based_on_interval
 
 
 class TelegramDailyTrendingGithubProjectsLoader(TelegramBaseLoader):
-    def __init__(self, telegram_group_name, telegram_group_topic_id):
-        super().__init__(telegram_group_name, telegram_group_topic_id)
+    def __init__(self, telegram_group_name, telegram_group_topic_id,
+                 creator='TelegramDailyTrendingGithubProjectsLoader', language='de'):
+        super().__init__(creator, language, telegram_group_name, telegram_group_topic_id)
 
     def retrieve(self):
-        start_date_str, end_date_str = today_as_start_and_enddate_str()
+        if self.run_interval:
+            start_date_str, end_date_str = get_start_and_end_times_based_on_interval(self.run_interval)
+        else:
+            start_date_str, end_date_str = today_as_start_and_enddate_str()
+
         filters = [
-            ["creator", "DailyTrendingGithubProjects"],
-            ["language", "de"],
+            ["creator", "DailyTrendingGithubProjectTransformer"],
+            ["lang", self.language],
             ["created_at", "between", start_date_str, end_date_str]
         ]
 
         projects = self.dao.read(Content, filters, limit=3)
 
         for project in projects:
             project.title = 'Aktuelle GitHub-Trends'
```

### Comparing `ai-datahive-0.1.4/ai_datahive/publishers/loader/telegram_top_daily_image_critique_loader.py` & `ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_top_daily_image_loader.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 from ai_datahive.transformers.models import Content
 
-from ai_datahive.utils.datetime_helper import today_as_start_and_enddate_str
+from ai_datahive.utils.datetime_helper import today_as_start_and_enddate_str, get_start_and_end_times_based_on_interval
 
 from ai_datahive.publishers.loader import TelegramBaseLoader
 
 
-class TelegramTopDailyImageCritiqueLoader(TelegramBaseLoader):
+class TelegramTopDailyImageLoader(TelegramBaseLoader):
 
-    def __init__(self, telegram_group_name, telegram_group_topic_id):
-        super().__init__(telegram_group_name, telegram_group_topic_id)
+    def __init__(self, telegram_group_name, telegram_group_topic_id, creator='TelegramTopDailyImageLoader',
+                 language='de'):
+        super().__init__(creator, language, telegram_group_name, telegram_group_topic_id)
 
     def retrieve(self):
-        start_date_str, end_date_str = today_as_start_and_enddate_str()
+        if self.run_interval:
+            start_date_str, end_date_str = get_start_and_end_times_based_on_interval(self.run_interval)
+        else:
+            start_date_str, end_date_str = today_as_start_and_enddate_str()
+
         filters = [
-            ["creator", "DailyImageCritiqueJS"],
-            ["language", "de"],
+            ["creator", "TopDailyImageTransformer"],
+            ["lang", self.language],
             ["created_at", "between", start_date_str, end_date_str]
         ]
 
         topimage = self.dao.read(Content, filters, limit=1)
-        return topimage[0]
+        if topimage:
+            return topimage[0]
+        return None
 
 
 def main():
     from dotenv import load_dotenv
     load_dotenv()
-    IMAGE_GROUP_TOPIC_ID = 27
-    loader = TelegramTopDailyImageCritiqueLoader('KI & Business', IMAGE_GROUP_TOPIC_ID)
+    loader = TelegramTopDailyImageLoader('KI & Business', 27)
     loader.load()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ai-datahive-0.1.4/ai_datahive/publishers/loader/telegram_top_daily_image_loader.py` & `ai-datahive-0.1.5/ai_datahive/publishers/loader/telegram_daily_arxiv_loader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 from ai_datahive.transformers.models import Content
 
-from ai_datahive.utils.datetime_helper import today_as_start_and_enddate_str
-
 from ai_datahive.publishers.loader import TelegramBaseLoader
+from ai_datahive.utils.datetime_helper import get_start_and_end_times_based_on_interval, today_as_start_and_enddate_str
 
 
-class TelegramTopDailyImageLoader(TelegramBaseLoader):
+class TelegramDailyArxivLoader(TelegramBaseLoader):
 
-    def __init__(self, telegram_group_name, telegram_group_topic_id):
-        super().__init__(telegram_group_name, telegram_group_topic_id)
+    def __init__(self, telegram_group_name, telegram_group_topic_id, creator='TelegramDailyArxivLoader', language='de'):
+        super().__init__(creator, language, telegram_group_name, telegram_group_topic_id)
 
     def retrieve(self):
-        start_date_str, end_date_str = today_as_start_and_enddate_str()
+        if self.run_interval:
+            start_date_str, end_date_str = get_start_and_end_times_based_on_interval(self.run_interval)
+        else:
+            start_date_str, end_date_str = today_as_start_and_enddate_str()
+
         filters = [
-            ["creator", "TopDailyImage"],
-            ["language", "de"],
-            ["created_at", "between", start_date_str, end_date_str]
+            ["creator", "DailyArxivPaperTransformer"],
+            ["lang", self.language],
+            ["created_at", "between", start_date_str, end_date_str]  # TODO extract from run_interval
         ]
 
-        topimage = self.dao.read(Content, filters, limit=1)
-        return topimage[0]
+        paper = self.dao.read(Content, filters, limit=1)
+        if len(paper) > 0:
+            return paper[0]
+        return None
 
 
 def main():
     from dotenv import load_dotenv
     load_dotenv()
-    loader = TelegramTopDailyImageLoader('KI & Business', 27)
+    ARXIV_GROUP_TOPIC_ID = 2
+    loader = TelegramDailyArxivLoader('KI & Business', ARXIV_GROUP_TOPIC_ID)
     loader.load()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ai-datahive-0.1.4/ai_datahive/publishers/models/telegram_message.py` & `ai-datahive-0.1.5/ai_datahive/publishers/models/telegram_message.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,10 +8,11 @@
 
 class TelegramMessage(DataHiveBaseModel):
     telegram_group_topic_fk: str
     content: Optional[str] = None
     media_content: Optional[str] = None
     media_url: Optional[HttpUrl] = None
     media_type: Optional[str] = None
+    creator: str
     scheduled_for: Optional[Union[datetime, str]] = None
     sent_at: Optional[Union[datetime, str]] = None
     status: str
```

### Comparing `ai-datahive-0.1.4/ai_datahive/publishers/telegram_bot.py` & `ai-datahive-0.1.5/ai_datahive/publishers/telegram_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from dotenv import load_dotenv
 
 from telegram import Update
 from telegram.ext import Application, ContextTypes, CallbackContext
 
 from ai_datahive.publishers.models import TelegramMessage, TelegramGroupTopic
 
-from ai_datahive.dao.dao_factory import dao_factory
+from ai_datahive.utils.dao_factory import get_dao
 from ai_datahive.dao import BaseDAO
 
 
 def setup_logging():
     logging.basicConfig(
         format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
         level=logging.INFO
@@ -164,15 +164,15 @@
     dao.update(message)
 
 
 def main():
     setup_logging()
     load_dotenv()
 
-    dao: BaseDAO = dao_factory()
+    dao: BaseDAO = get_dao()
     telegram_application: Application = create_telegram_application()
 
     (telegram_application.job_queue.run_repeating(process_and_send_new_messages,
                                                   interval=10, first=0, data={'dao': dao}))
 
     print('Telegram Bot started ...')
     # Run the bot until the user presses Ctrl-C
```

### Comparing `ai-datahive-0.1.4/ai_datahive/services/ai_service_factory.py` & `ai-datahive-0.1.5/ai_datahive/services/ai_service_factory.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.4/ai_datahive/services/openai_service.py` & `ai-datahive-0.1.5/ai_datahive/services/openai_service.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.4/ai_datahive/services/prompt_service.py` & `ai-datahive-0.1.5/ai_datahive/services/prompt_service.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.4/ai_datahive/services/prompts/js_style_image_critique_prompt.txt` & `ai-datahive-0.1.5/ai_datahive/services/prompts/js_style_image_critique_prompt.txt`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.4/ai_datahive/transformers/base_content_transformer.py` & `ai-datahive-0.1.5/ai_datahive/transformers/base_content_transformer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 import os
-from typing import Union, Collection
+import inspect
+from typing import Union, Collection, List
 
+from datetime import timedelta
 from string import Template
 from ai_datahive.utils.text_helper import escape_html
 
 from ai_datahive.transformers.models import Content
+from ai_datahive.utils import datetime_helper
 
 
 class BaseContentTransformer:
-    def __init__(self, creator_name, template_file_name, language):
-        from ai_datahive.dao.dao_factory import dao_factory
-        self.dao = dao_factory()
+    def __init__(self, creator, template_file_name, language, run_interval: timedelta = timedelta(days=1)):
+        from ai_datahive.utils.dao_factory import get_dao
+        self.dao = get_dao()
         self.language = language
-        self.creator_name = creator_name
-        self.template_path = os.path.join(os.path.dirname(__file__), 'templates', template_file_name)
+        self.creator = creator
+        self.run_interval = run_interval
+        caller_file = inspect.getfile(self.__class__)
+        template_file_path = os.path.join(caller_file, 'templates', template_file_name)
+        if os.path.exists(template_file_path):
+            self.template_path = os.path.join(caller_file, 'templates', template_file_name)
+        elif os.path.exists(os.path.join(os.path.dirname(__file__), 'templates', template_file_name)):
+            self.template_path = os.path.join(os.path.dirname(__file__), 'templates', template_file_name)
+        else:
+            self.template_path = os.path.join('templates', template_file_name)
 
     def save(self, content: Union[Content, Collection[Content]]):
         if isinstance(content, Collection):
             results = [self.dao.create(c) for c in content]
             return results
         else:
             result = self.dao.create(content)
@@ -31,18 +42,21 @@
 
         template = Template(template_content)
         return template.safe_substitute(template_data)
 
     def retrieve(self):
         raise NotImplementedError
 
-    def transform(self, data):
+    def transform(self, data) -> List[Content]:
         raise NotImplementedError
 
     def run(self):
-        # get top image
-        # check if top image was already top image
-        # if yes try next top image until three tries
-        # If all already top images write a message with the first one to say it is again the winner. in a row.
-        entities = self.retrieve()
-        content = self.transform(entities)
-        self.save(content)
+        is_due = datetime_helper.is_due(content_type=Content, creator=self.creator,
+                                        run_interval=self.run_interval)
+        if is_due:
+            # get top image
+            # check if top image was already top image
+            # if yes try next top image until three tries
+            # If all already top images write a message with the first one to say it is again the winner. in a row.
+            entities = self.retrieve()
+            content = self.transform(entities)
+            return self.save(content)
```

### Comparing `ai-datahive-0.1.4/ai_datahive/transformers/daily_arxiv_paper_transformer.py` & `ai-datahive-0.1.5/ai_datahive/transformers/daily_arxiv_paper_transformer.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,79 +7,67 @@
 from ai_datahive.collectors.models import ResearchPaper
 from ai_datahive.transformers.models import Content
 
 from ai_datahive.services import OpenAIService, PromptService
 
 
 class DailyArxivPaperTransformer(BaseContentTransformer):
-    def __init__(self, creator_name='DailyArxivPaper', template_file_name='daily_arxiv_paper_template.html', language='de'):
-        from ai_datahive.dao.dao_factory import dao_factory
-        self.dao = dao_factory()
+    def __init__(self, creator='DailyArxivPaperTransformer', template_file_name='daily_arxiv_paper_template.html',
+                 language='de'):
 
         self.ps = PromptService()
         self.oais = OpenAIService()
 
-        super().__init__(creator_name=creator_name, template_file_name=template_file_name, language=language)
+        super().__init__(creator=creator, template_file_name=template_file_name, language=language)
 
     def retrieve(self) -> List[ResearchPaper]:
         start_date_str, end_date_str = today_as_start_and_enddate_str()
 
         filters = [["creator", "ArxivCollector"], ['created_at', 'between', start_date_str, end_date_str]]
         papers = self.dao.read(ResearchPaper, filters, limit=3, order_by='created_at')
         return papers
 
     def transform(self, papers: list[ResearchPaper]) -> List[Content]:
-        # TODO make a language system. Getting the language from Paper and Check language in this transformer
-        # TODO If different make a translation
-        # Hardcoded for now
-        paper_language = 'en'
         result = []
 
         for paper in papers:
-            system_msg = self.ps.create_summarize_system_prompt()
+            paper_language = paper.lang
 
+            system_msg = self.ps.create_summarize_system_prompt()
             if self.language != paper_language:
                 system_msg += self.ps.create_translate_system_prompt(language=self.language)
 
             self.oais.switch_text_model('gpt-3.5-turbo')
             abstract = self.oais.chat_response(system_msg, paper.abstract)
             self.oais.switch_to_default_text_model()
 
             template_data = {
                 'title': paper.title,
                 'abstract': abstract,
                 'authors': paper.authors,
-                'date': paper.created_at,
+                'date': paper.created_at.strftime('%d.%m.%Y %H:%M'),
                 'url': paper.paper_url
             }
             str_content = self.create_content(template_data)
 
             content = Content(
                 title=paper.title,
                 content=str_content,
                 reference_url=paper.paper_url,
                 reference_type='paper',
                 reference_created_at=paper.created_at,
-                source=paper.source,
-                language=self.language,
-                creator=self.creator_name,
+                source_name=paper.source_name,
+                source_url=paper.source_url,
+                lang=self.language,
+                creator=self.creator,
                 tags=paper.tags,
             )
             result.append(content)
         return result
 
-    def run(self):
-        # get top image
-        # check if top image was already top image
-        # if yes try next top image until three tries
-        # If all already top images write a message with the first one to say it is again the winner. in a row.
-        papers = self.retrieve()
-        content = self.transform(papers)
-        self.save(content)
-
 
 def main():
     from dotenv import load_dotenv
     load_dotenv()
 
     transformer = DailyArxivPaperTransformer()
     transformer.run()
```

### Comparing `ai-datahive-0.1.4/ai_datahive/transformers/daily_trending_github_project_transformer.py` & `ai-datahive-0.1.5/ai_datahive/transformers/daily_trending_github_project_transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,42 +2,39 @@
 
 from ai_datahive.collectors.models import GithubProject
 from ai_datahive.transformers import BaseContentTransformer
 from ai_datahive.transformers.models import Content
 
 from ai_datahive.services import AIBackedTranslationService
 
-from ai_datahive.utils.datetime_helper import today_as_start_and_enddate_str
+from ai_datahive.utils.datetime_helper import get_start_and_end_times_based_on_interval
 from ai_datahive.utils.text_helper import replace_numbers_with_emojis
 
+
 class DailyTrendingGithubProjectTransformer(BaseContentTransformer):
-    def __init__(self, creator_name='DailyTrendingGithubProjects',
+    def __init__(self, creator='DailyTrendingGithubProjectTransformer',
                  template_file_name='github_loader_trending_template.html', language='de'):
-        from ai_datahive.dao.dao_factory import dao_factory
-        self.dao = dao_factory()
 
         self.ts = AIBackedTranslationService()
 
-        super().__init__(creator_name=creator_name, template_file_name=template_file_name, language=language)
+        super().__init__(creator=creator, template_file_name=template_file_name, language=language)
 
     def retrieve(self) -> List[GithubProject]:
-        start_date_str, end_date_str = today_as_start_and_enddate_str()
+        # start_date_str, end_date_str = today_as_start_and_enddate_str()
+        start_date_str, end_date_str = get_start_and_end_times_based_on_interval(self.run_interval)
 
         filters = [["creator", "GithubCollector"], ['created_at', 'between', start_date_str, end_date_str]]
         projects = self.dao.read(GithubProject, filters, limit=3, order_by='created_at')
         return projects
 
     def transform(self, projects: list[GithubProject]) -> List[Content]:
-        # TODO make a language system. Getting the language from Paper and Check language in this transformer
-        # TODO If different make a translation
-        # Hardcoded for now
-        project_language = 'en'
         result = []
 
         for project in projects:
+            project_language = project.lang
             if self.language != project_language:
                 translated_description = self.ts.translate(project.description, self.language)
                 project.description = translated_description
 
             template_data = {
                 'rank': replace_numbers_with_emojis(str(project.rank)),
                 'username': project.username,
@@ -52,17 +49,18 @@
 
             content = Content(
                 title=project.name,
                 content=str_content,
                 reference_url=project.url,
                 reference_type='github_project',
                 reference_created_at=project.created_at,
-                source=project.source,
-                language=self.language,
-                creator=self.creator_name,
+                source_name=project.source_name,
+                source_url=project.source_url,
+                lang=self.language,
+                creator=self.creator,
                 tags=project.tags,
             )
             result.append(content)
         return result
 
 
 def main():
```

### Comparing `ai-datahive-0.1.4/ai_datahive/transformers/models/content.py` & `ai-datahive-0.1.5/ai_datahive/transformers/models/content.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from pydantic import HttpUrl
 from datetime import datetime
 
 
 class Content(ContentBaseModel):
     title: Optional[str] = None
     content: Optional[str] = None
-    language: str # ISO 639-1
     media_url: Optional[HttpUrl] = None
     media_type: Optional[str] = None
     media_created_at: Optional[Union[datetime, str]] = None
     reference_url: Optional[HttpUrl] = None
     reference_type: Optional[str] = None
     reference_created_at: Optional[Union[datetime, str]] = None
     scheduled_for: Optional[Union[datetime, str]] = None
```

### Comparing `ai-datahive-0.1.4/ai_datahive/transformers/top_daily_image_critique_transformer.py` & `ai-datahive-0.1.5/ai_datahive/transformers/top_daily_image_critique_transformer.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,61 +5,61 @@
 from ai_datahive.collectors.models import Media
 from ai_datahive.transformers.models import Content
 
 from ai_datahive.services import OpenAIService, PromptService, AIBackedTranslationService
 
 
 class TopDailyImageCritiqueTransformer(BaseContentTransformer):
-    def __init__(self, creator_name='DailyImageCritiqueJS', template_file_name='top_daily_image_critique_template.html',
+    def __init__(self, creator='DailyImageCritiqueJS', template_file_name='top_daily_image_critique_template.html',
                  language='de'):
-        from ai_datahive.dao.dao_factory import dao_factory
-        self.dao = dao_factory()
 
         self.ps = PromptService()
         self.oais = OpenAIService()
         self.ts = AIBackedTranslationService()
 
-        super().__init__(creator_name=creator_name, template_file_name=template_file_name, language=language)
+        super().__init__(creator=creator, template_file_name=template_file_name, language=language)
 
     def retrieve(self) -> Media:
         start_date_str, end_date_str = today_as_start_and_enddate_str()
 
         filters = [["creator", "CivitAIDailyTopImage"], ['created_at', 'between', start_date_str, end_date_str]]
         media = self.dao.read(Media, filters, limit=1, order_by='likes')
         return media[0] if media else None
 
     def transform(self, topdailyimage: Media) -> Content:
 
         if topdailyimage:
+            image_language = topdailyimage.lang
             system_prompt = self.ps.create_system_prompt_from_file('js_style_image_critique_prompt.txt')
 
             user_prompt = f"Prompt: {topdailyimage.prompt}\nartist: {topdailyimage.author}"
             critique = self.oais.vision_response(system_prompt=system_prompt, user_prompt=user_prompt,
                                                  image_url=topdailyimage.media_url)
-            if self.language != 'en':
+            if self.language != image_language:
                 critique = self.ts.translate(critique, self.language)
 
             template_data = {
                 'critique': critique,
                 'author': topdailyimage.author,
                 'created_at': topdailyimage.media_created_at,
                 'media_url': topdailyimage.media_url,
             }
             str_content = self.create_content(template_data)
 
             content = Content(
-                creator=self.creator_name,
+                creator=self.creator,
                 tags=topdailyimage.tags+', critique, JS style',
                 title=f'Die Bildkritik mit Saltz',
                 content=str_content,
                 media_url=topdailyimage.media_url,
                 media_type='image',
                 media_created_at=topdailyimage.media_created_at,
-                source=topdailyimage.source,
-                language=self.language
+                source_name=topdailyimage.source_name,
+                source_url=topdailyimage.source_url,
+                lang=self.language
             )
             return content
 
 
 def main():
     from dotenv import load_dotenv
     load_dotenv()
```

### Comparing `ai-datahive-0.1.4/ai_datahive/utils/text_helper.py` & `ai-datahive-0.1.5/ai_datahive/utils/text_helper.py`

 * *Files identical despite different names*

### Comparing `ai-datahive-0.1.4/ai_datahive.egg-info/PKG-INFO` & `ai-datahive-0.1.5/ai_datahive.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-datahive
-Version: 0.1.4
+Version: 0.1.5
 Summary: ETL Package for crawling data, transform it with AI and store it in a datastorage.
 Author: Danny Gerst
 Author-email: d.gerst@bizrock.de
 License-File: LICENSE
 Requires-Dist: python-dotenv
 Requires-Dist: pydantic
 Requires-Dist: inflect
```

### Comparing `ai-datahive-0.1.4/ai_datahive.egg-info/SOURCES.txt` & `ai-datahive-0.1.5/ai_datahive.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 ai_datahive/collectors/utils/arxiv_helper.py
 ai_datahive/collectors/utils/custom_exceptions.py
 ai_datahive/collectors/utils/github_helper.py
 ai_datahive/collectors/utils/scraping_helper.py
 ai_datahive/collectors/utils/zotero_helper.py
 ai_datahive/dao/__init__.py
 ai_datahive/dao/base_dao.py
-ai_datahive/dao/dao_factory.py
 ai_datahive/dao/supabase_dao.py
 ai_datahive/models/__init__.py
 ai_datahive/models/base_model.py
 ai_datahive/models/content_base_model.py
 ai_datahive/publishers/__init__.py
 ai_datahive/publishers/telegram_bot.py
 ai_datahive/publishers/loader/__init__.py
@@ -64,9 +63,10 @@
 ai_datahive/transformers/models/__init__.py
 ai_datahive/transformers/models/content.py
 ai_datahive/transformers/templates/daily_arxiv_paper_template.html
 ai_datahive/transformers/templates/github_loader_trending_template.html
 ai_datahive/transformers/templates/top_daily_image_critique_template.html
 ai_datahive/transformers/templates/top_daily_image_template.html
 ai_datahive/utils/__init__.py
+ai_datahive/utils/dao_factory.py
 ai_datahive/utils/datetime_helper.py
 ai_datahive/utils/text_helper.py
```

### Comparing `ai-datahive-0.1.4/setup.py` & `ai-datahive-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_requirements():
     with open('requirements.txt') as f:
         return [line.strip() for line in f.readlines() if not line.startswith('#')]
 
 
 setup(
     name='ai-datahive',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     package_data={
         'ai_datahive': ['transformers/templates/*.html', 'services/prompts/*.txt'],
     },
     include_package_data=True,
     description='ETL Package for crawling data, transform it with AI and store it in a datastorage.',
     author='Danny Gerst',
```

