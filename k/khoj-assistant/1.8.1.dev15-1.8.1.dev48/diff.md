# Comparing `tmp/khoj_assistant-1.8.1.dev15.tar.gz` & `tmp/khoj_assistant-1.8.1.dev48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Apr  2 11:31:31 2024, max compression
+gzip compressed data, last modified: Wed Apr  3 11:43:31 2024, max compression
```

## Comparing `khoj_assistant-1.8.1.dev15.tar` & `khoj_assistant-1.8.1.dev48.tar`

### file list

```diff
@@ -1,183 +1,183 @@
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/__init__.py
--rw-r--r--   0        0        0    14822 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/configure.py
--rw-r--r--   0        0        0     5330 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/main.py
--rwxr-xr-x   0        0        0      664 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/manage.py
--rw-r--r--   0        0        0     2832 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/app/README.md
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/app/__init__.py
--rw-r--r--   0        0        0     4534 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/app/settings.py
--rw-r--r--   0        0        0      869 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/app/urls.py
--rw-r--r--   0        0        0      388 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/app/wsgi.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/__init__.py
--rw-r--r--   0        0        0     5419 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/admin.py
--rw-r--r--   0        0        0      153 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/apps.py
--rw-r--r--   0        0        0       60 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/tests.py
--rw-r--r--   0        0        0    33288 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/adapters/__init__.py
--rw-r--r--   0        0        0     4077 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0001_khojuser.py
--rw-r--r--   0        0        0     1195 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0002_googleuser.py
--rw-r--r--   0        0        0      224 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0003_vector_extension.py
--rw-r--r--   0        0        0     8202 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0004_content_types_and_more.py
--rw-r--r--   0        0        0      429 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0005_embeddings_corpus_id.py
--rw-r--r--   0        0        0     1131 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0006_embeddingsdates.py
--rw-r--r--   0        0        0      917 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0007_add_conversation.py
--rw-r--r--   0        0        0      399 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0008_alter_conversation_conversation_log.py
--rw-r--r--   0        0        0      876 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0009_khojapiuser.py
--rw-r--r--   0        0        0     3347 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py
--rw-r--r--   0        0        0      773 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py
--rw-r--r--   0        0        0      331 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0011_merge_20231102_0138.py
--rw-r--r--   0        0        0      552 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0012_entry_file_source.py
--rw-r--r--   0        0        0     1311 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0013_subscription.py
--rw-r--r--   0        0        0      411 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0014_alter_googleuser_picture.py
--rw-r--r--   0        0        0      584 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0015_alter_subscription_user.py
--rw-r--r--   0        0        0      429 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0016_alter_subscription_renewal_date.py
--rw-r--r--   0        0        0     1219 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0017_searchmodel.py
--rw-r--r--   0        0        0     1152 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py
--rw-r--r--   0        0        0      843 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py
--rw-r--r--   0        0        0     1190 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0020_reflectivequestion.py
--rw-r--r--   0        0        0     1504 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py
--rw-r--r--   0        0        0      904 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0022_texttoimagemodelconfig.py
--rw-r--r--   0        0        0     1122 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0023_usersearchmodelconfig.py
--rw-r--r--   0        0        0      405 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0024_alter_entry_embeddings.py
--rw-r--r--   0        0        0     1573 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py
--rw-r--r--   0        0        0      691 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py
--rw-r--r--   0        0        0      731 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py
--rw-r--r--   0        0        0      375 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0027_merge_20240118_1324.py
--rw-r--r--   0        0        0      405 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0028_khojuser_verified_phone_number.py
--rw-r--r--   0        0        0      934 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0029_userrequests.py
--rw-r--r--   0        0        0     1252 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0030_conversation_slug_and_title.py
--rw-r--r--   0        0        0     2033 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0031_agent_conversation_agent.py
--rw-r--r--   0        0        0      812 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0031_alter_googleuser_locale.py
--rw-r--r--   0        0        0      317 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0032_merge_20240322_0427.py
--rw-r--r--   0        0        0      369 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0033_rename_tuning_agent_personality.py
--rw-r--r--   0        0        0     1251 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/__init__.py
--rw-r--r--   0        0        0    11129 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/database/models/__init__.py
--rw-r--r--   0        0        0     1651 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     8953 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/agent.html
--rw-r--r--   0        0        0     6672 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/agents.html
--rw-r--r--   0        0        0    11089 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0   100892 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    37581 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     5367 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/content_source_computer_input.html
--rw-r--r--   0        0        0     7225 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/content_source_github_input.html
--rw-r--r--   0        0        0     3655 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/content_source_notion_input.html
--rw-r--r--   0        0        0     1628 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0     4218 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/login.html
--rw-r--r--   0        0        0     2910 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0    18326 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/search.html
--rw-r--r--   0        0        0     2168 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/utils.html
--rw-r--r--   0        0        0     5160 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73396 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0     1222 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/utils.js
--rw-r--r--   0        0        0    51584 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0    10517 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/computer.png
--rw-r--r--   0        0        0      549 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0      503 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/copy-solid.svg
--rw-r--r--   0        0        0      746 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/copy_button.svg
--rw-r--r--   0        0        0    19662 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/credit-card.png
--rw-r--r--   0        0        0   205167 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    30234 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/favicon-256x256.png
--rw-r--r--   0        0        0    31531 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0     1100 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/key.svg
--rw-r--r--   0        0        0    13011 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0    29856 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png
--rw-r--r--   0        0        0  1301428 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0      616 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/microphone-solid.svg
--rw-r--r--   0        0        0     1578 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/notion.svg
--rw-r--r--   0        0        0     1736 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/openai-logomark.svg
--rw-r--r--   0        0        0     7946 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0     2945 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/plaintext.svg
--rw-r--r--   0        0        0     1877 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/question-mark-icon.svg
--rw-r--r--   0        0        0     1319 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/stop-solid.svg
--rw-r--r--   0        0        0      503 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/trash-solid.svg
--rw-r--r--   0        0        0     2233 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/user-silhouette.svg
--rw-r--r--   0        0        0      951 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/web.svg
--rw-r--r--   0        0        0     2417 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/whatsapp.svg
--rw-r--r--   0        0        0   591182 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png
--rw-r--r--   0        0        0   197173 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png
--rw-r--r--   0        0        0   268309 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png
--rw-r--r--   0        0        0   406179 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png
--rw-r--r--   0        0        0    82985 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png
--rw-r--r--   0        0        0   236285 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/migrations/__init__.py
--rw-r--r--   0        0        0     1928 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/migrations/migrate_offline_chat_default_model.py
--rw-r--r--   0        0        0     2034 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/migrations/migrate_offline_chat_default_model_2.py
--rw-r--r--   0        0        0     2510 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/migrations/migrate_offline_chat_schema.py
--rw-r--r--   0        0        0      975 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/migrations/migrate_offline_model.py
--rw-r--r--   0        0        0     2025 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/migrations/migrate_processor_config_openai.py
--rw-r--r--   0        0        0     5132 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/migrations/migrate_server_pg.py
--rw-r--r--   0        0        0      569 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/migrations/migrate_version.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4715 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/content/__init__.py
--rw-r--r--   0        0        0    12604 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/content/text_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/content/github/__init__.py
--rw-r--r--   0        0        0    13721 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/content/github/github_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/content/markdown/__init__.py
--rw-r--r--   0        0        0     5690 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/content/markdown/markdown_to_entries.py
--rw-r--r--   0        0        0     9871 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/content/notion/notion_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/content/org_mode/__init__.py
--rw-r--r--   0        0        0     6377 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/content/org_mode/org_to_entries.py
--rw-r--r--   0        0        0    18246 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/content/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/content/pdf/__init__.py
--rw-r--r--   0        0        0     4660 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/content/pdf/pdf_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/content/plaintext/__init__.py
--rw-r--r--   0        0        0     3717 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/content/plaintext/plaintext_to_entries.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0    20895 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0    10226 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/offline/__init__.py
--rw-r--r--   0        0        0     8615 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/offline/chat_model.py
--rw-r--r--   0        0        0     1793 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/offline/utils.py
--rw-r--r--   0        0        0      470 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/offline/whisper.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/openai/__init__.py
--rw-r--r--   0        0        0     6854 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/openai/gpt.py
--rw-r--r--   0        0        0     3284 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/openai/utils.py
--rw-r--r--   0        0        0      432 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/openai/whisper.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/tools/__init__.py
--rw-r--r--   0        0        0     5929 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/processor/tools/online_search.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    14588 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1443 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/routers/api_agents.py
--rw-r--r--   0        0        0    14988 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/routers/api_chat.py
--rw-r--r--   0        0        0    10614 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/routers/api_config.py
--rw-r--r--   0        0        0     2208 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/routers/api_phone.py
--rw-r--r--   0        0        0     4569 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/routers/auth.py
--rw-r--r--   0        0        0    28306 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/routers/helpers.py
--rw-r--r--   0        0        0    12706 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/routers/indexer.py
--rw-r--r--   0        0        0     1151 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/routers/storage.py
--rw-r--r--   0        0        0     4285 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/routers/subscription.py
--rw-r--r--   0        0        0     1081 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/routers/twilio.py
--rw-r--r--   0        0        0    13166 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      358 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0    10101 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0      939 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     1005 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11451 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0     8916 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     3466 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     1866 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/utils/config.py
--rw-r--r--   0        0        0      791 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     9519 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/utils/fs_syncer.py
--rw-r--r--   0        0        0    12034 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     7245 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/utils/initialization.py
--rw-r--r--   0        0        0     1192 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2009 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4028 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1354 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1430 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      565 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/.gitignore
--rw-r--r--   0        0        0    34523 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/LICENSE
--rw-r--r--   0        0        0     2007 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/README.md
--rw-r--r--   0        0        0     3430 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/pyproject.toml
--rw-r--r--   0        0        0     5227 2024-04-02 11:31:31.000000 khoj_assistant-1.8.1.dev15/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/__init__.py
+-rw-r--r--   0        0        0    14822 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/configure.py
+-rw-r--r--   0        0        0     5330 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/main.py
+-rwxr-xr-x   0        0        0      664 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/manage.py
+-rw-r--r--   0        0        0     2832 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/app/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/app/__init__.py
+-rw-r--r--   0        0        0     4534 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/app/settings.py
+-rw-r--r--   0        0        0      869 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/app/urls.py
+-rw-r--r--   0        0        0      388 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/app/wsgi.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/__init__.py
+-rw-r--r--   0        0        0     5419 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/admin.py
+-rw-r--r--   0        0        0      153 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/apps.py
+-rw-r--r--   0        0        0       60 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/tests.py
+-rw-r--r--   0        0        0    33288 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/adapters/__init__.py
+-rw-r--r--   0        0        0     4077 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0001_khojuser.py
+-rw-r--r--   0        0        0     1195 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0002_googleuser.py
+-rw-r--r--   0        0        0      224 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0003_vector_extension.py
+-rw-r--r--   0        0        0     8202 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0004_content_types_and_more.py
+-rw-r--r--   0        0        0      429 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0005_embeddings_corpus_id.py
+-rw-r--r--   0        0        0     1131 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0006_embeddingsdates.py
+-rw-r--r--   0        0        0      917 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0007_add_conversation.py
+-rw-r--r--   0        0        0      399 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0008_alter_conversation_conversation_log.py
+-rw-r--r--   0        0        0      876 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0009_khojapiuser.py
+-rw-r--r--   0        0        0     3347 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py
+-rw-r--r--   0        0        0      773 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py
+-rw-r--r--   0        0        0      331 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0011_merge_20231102_0138.py
+-rw-r--r--   0        0        0      552 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0012_entry_file_source.py
+-rw-r--r--   0        0        0     1311 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0013_subscription.py
+-rw-r--r--   0        0        0      411 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0014_alter_googleuser_picture.py
+-rw-r--r--   0        0        0      584 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0015_alter_subscription_user.py
+-rw-r--r--   0        0        0      429 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0016_alter_subscription_renewal_date.py
+-rw-r--r--   0        0        0     1219 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0017_searchmodel.py
+-rw-r--r--   0        0        0     1152 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py
+-rw-r--r--   0        0        0      843 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py
+-rw-r--r--   0        0        0     1190 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0020_reflectivequestion.py
+-rw-r--r--   0        0        0     1504 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py
+-rw-r--r--   0        0        0      904 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0022_texttoimagemodelconfig.py
+-rw-r--r--   0        0        0     1122 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0023_usersearchmodelconfig.py
+-rw-r--r--   0        0        0      405 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0024_alter_entry_embeddings.py
+-rw-r--r--   0        0        0     1573 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py
+-rw-r--r--   0        0        0      691 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py
+-rw-r--r--   0        0        0      731 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py
+-rw-r--r--   0        0        0      375 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0027_merge_20240118_1324.py
+-rw-r--r--   0        0        0      405 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0028_khojuser_verified_phone_number.py
+-rw-r--r--   0        0        0      934 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0029_userrequests.py
+-rw-r--r--   0        0        0     1252 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0030_conversation_slug_and_title.py
+-rw-r--r--   0        0        0     2033 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0031_agent_conversation_agent.py
+-rw-r--r--   0        0        0      812 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0031_alter_googleuser_locale.py
+-rw-r--r--   0        0        0      317 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0032_merge_20240322_0427.py
+-rw-r--r--   0        0        0      369 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0033_rename_tuning_agent_personality.py
+-rw-r--r--   0        0        0     1251 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/__init__.py
+-rw-r--r--   0        0        0    11129 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/database/models/__init__.py
+-rw-r--r--   0        0        0     1651 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     8953 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/agent.html
+-rw-r--r--   0        0        0     6672 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/agents.html
+-rw-r--r--   0        0        0    11089 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0   110890 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    37581 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     5367 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/content_source_computer_input.html
+-rw-r--r--   0        0        0     7225 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/content_source_github_input.html
+-rw-r--r--   0        0        0     3655 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/content_source_notion_input.html
+-rw-r--r--   0        0        0     1628 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0     4218 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/login.html
+-rw-r--r--   0        0        0     2910 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0    18326 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/search.html
+-rw-r--r--   0        0        0     2168 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/utils.html
+-rw-r--r--   0        0        0     5160 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73396 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0     1222 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/utils.js
+-rw-r--r--   0        0        0    51584 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0    10517 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/computer.png
+-rw-r--r--   0        0        0      549 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0      503 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/copy-solid.svg
+-rw-r--r--   0        0        0      746 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/copy_button.svg
+-rw-r--r--   0        0        0    19662 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/credit-card.png
+-rw-r--r--   0        0        0   205167 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    30234 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/favicon-256x256.png
+-rw-r--r--   0        0        0    31531 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0     1100 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/key.svg
+-rw-r--r--   0        0        0    13011 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0    29856 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png
+-rw-r--r--   0        0        0  1301428 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0      616 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/microphone-solid.svg
+-rw-r--r--   0        0        0     1578 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/notion.svg
+-rw-r--r--   0        0        0     1736 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/openai-logomark.svg
+-rw-r--r--   0        0        0     7946 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0     2945 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/plaintext.svg
+-rw-r--r--   0        0        0     1877 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/question-mark-icon.svg
+-rw-r--r--   0        0        0     1319 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/stop-solid.svg
+-rw-r--r--   0        0        0      503 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/trash-solid.svg
+-rw-r--r--   0        0        0     2233 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/user-silhouette.svg
+-rw-r--r--   0        0        0      951 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/web.svg
+-rw-r--r--   0        0        0     2417 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/whatsapp.svg
+-rw-r--r--   0        0        0   591182 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png
+-rw-r--r--   0        0        0   197173 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png
+-rw-r--r--   0        0        0   268309 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png
+-rw-r--r--   0        0        0   406179 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png
+-rw-r--r--   0        0        0    82985 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png
+-rw-r--r--   0        0        0   236285 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/migrations/__init__.py
+-rw-r--r--   0        0        0     1928 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/migrations/migrate_offline_chat_default_model.py
+-rw-r--r--   0        0        0     2034 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/migrations/migrate_offline_chat_default_model_2.py
+-rw-r--r--   0        0        0     2510 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/migrations/migrate_offline_chat_schema.py
+-rw-r--r--   0        0        0      975 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/migrations/migrate_offline_model.py
+-rw-r--r--   0        0        0     2025 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/migrations/migrate_processor_config_openai.py
+-rw-r--r--   0        0        0     5132 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/migrations/migrate_server_pg.py
+-rw-r--r--   0        0        0      569 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/migrations/migrate_version.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4715 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/content/__init__.py
+-rw-r--r--   0        0        0    12604 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/content/text_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/content/github/__init__.py
+-rw-r--r--   0        0        0    13721 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/content/github/github_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/content/markdown/__init__.py
+-rw-r--r--   0        0        0     5690 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/content/markdown/markdown_to_entries.py
+-rw-r--r--   0        0        0     9871 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/content/notion/notion_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/content/org_mode/__init__.py
+-rw-r--r--   0        0        0     6377 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/content/org_mode/org_to_entries.py
+-rw-r--r--   0        0        0    18246 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/content/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/content/pdf/__init__.py
+-rw-r--r--   0        0        0     4660 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/content/pdf/pdf_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/content/plaintext/__init__.py
+-rw-r--r--   0        0        0     3717 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/content/plaintext/plaintext_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0    20895 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0    10226 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/offline/__init__.py
+-rw-r--r--   0        0        0     8615 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/offline/chat_model.py
+-rw-r--r--   0        0        0     1793 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/offline/utils.py
+-rw-r--r--   0        0        0      470 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/offline/whisper.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/openai/__init__.py
+-rw-r--r--   0        0        0     6854 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/openai/gpt.py
+-rw-r--r--   0        0        0     3284 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/openai/utils.py
+-rw-r--r--   0        0        0      432 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/openai/whisper.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/tools/__init__.py
+-rw-r--r--   0        0        0     5929 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/processor/tools/online_search.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    15036 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1443 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/routers/api_agents.py
+-rw-r--r--   0        0        0    24398 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/routers/api_chat.py
+-rw-r--r--   0        0        0    10614 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/routers/api_config.py
+-rw-r--r--   0        0        0     2208 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/routers/api_phone.py
+-rw-r--r--   0        0        0     4569 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/routers/auth.py
+-rw-r--r--   0        0        0    28306 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/routers/helpers.py
+-rw-r--r--   0        0        0    12706 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/routers/indexer.py
+-rw-r--r--   0        0        0     1151 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/routers/storage.py
+-rw-r--r--   0        0        0     4285 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/routers/subscription.py
+-rw-r--r--   0        0        0     1081 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/routers/twilio.py
+-rw-r--r--   0        0        0    13166 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      358 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0    10101 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0      939 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     1005 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11451 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0     8916 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     3466 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     1866 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/utils/config.py
+-rw-r--r--   0        0        0      791 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     9519 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/utils/fs_syncer.py
+-rw-r--r--   0        0        0    12034 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     7245 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/utils/initialization.py
+-rw-r--r--   0        0        0     1192 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2009 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4028 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1354 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1430 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      565 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/.gitignore
+-rw-r--r--   0        0        0    34523 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/LICENSE
+-rw-r--r--   0        0        0     2007 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/README.md
+-rw-r--r--   0        0        0     3456 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/pyproject.toml
+-rw-r--r--   0        0        0     5259 2024-04-03 11:43:31.000000 khoj_assistant-1.8.1.dev48/PKG-INFO
```

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/configure.py` & `khoj_assistant-1.8.1.dev48/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/main.py` & `khoj_assistant-1.8.1.dev48/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/manage.py` & `khoj_assistant-1.8.1.dev48/src/khoj/manage.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/app/README.md` & `khoj_assistant-1.8.1.dev48/src/khoj/app/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/app/settings.py` & `khoj_assistant-1.8.1.dev48/src/khoj/app/settings.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/app/urls.py` & `khoj_assistant-1.8.1.dev48/src/khoj/app/urls.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/admin.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/admin.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/adapters/__init__.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0001_khojuser.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0001_khojuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0002_googleuser.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0002_googleuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0004_content_types_and_more.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0004_content_types_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0006_embeddingsdates.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0006_embeddingsdates.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0007_add_conversation.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0007_add_conversation.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0009_khojapiuser.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0009_khojapiuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0012_entry_file_source.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0012_entry_file_source.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0013_subscription.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0013_subscription.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0015_alter_subscription_user.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0015_alter_subscription_user.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0017_searchmodel.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0017_searchmodel.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0020_reflectivequestion.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0020_reflectivequestion.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0022_texttoimagemodelconfig.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0022_texttoimagemodelconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0023_usersearchmodelconfig.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0023_usersearchmodelconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0029_userrequests.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0029_userrequests.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0030_conversation_slug_and_title.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0030_conversation_slug_and_title.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0031_agent_conversation_agent.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0031_agent_conversation_agent.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0031_alter_googleuser_locale.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0031_alter_googleuser_locale.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/migrations/0034_alter_chatmodeloptions_chat_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/database/models/__init__.py` & `khoj_assistant-1.8.1.dev48/src/khoj/database/models/__init__.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/404.html` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/agent.html` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/agent.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/agents.html` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/agents.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/base_config.html` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/chat.html` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/chat.html`

 * *Files 4% similar despite different names*

```diff
@@ -43,19 +43,30 @@
                 console.error("Error copying programmatic output to clipboard:", error);
                 button.textContent = "⛔️ Failed to copy!";
                 setTimeout(() => {
                     button.textContent = "⛔️";
                 }, 1000);
             });
         }
+        var websocket = null;
+        var timeout = null;
+        var timeoutDuration = 600000; // 10 minutes
 
         let region = null;
         let city = null;
         let countryName = null;
 
+        let websocketState = {
+            newResponseText: null,
+            newResponseElement: null,
+            loadingEllipsis: null,
+            references: {},
+            rawResponse: "",
+        }
+
         fetch("https://ipapi.co/json")
             .then(response => response.json())
             .then(data => {
                 region = data.region;
                 city = data.city;
                 countryName = data.country_name;
             })
@@ -411,14 +422,20 @@
             referencesDiv.appendChild(referenceSection);
 
             return referencesDiv;
         }
 
         async function chat() {
             // Extract required fields for search from form
+
+            if (websocket) {
+                sendMessageViaWebSocket();
+                return;
+            }
+
             let query = document.getElementById("chat-input").value.trim();
             let resultsCount = localStorage.getItem("khojResultsCount") || 5;
             console.log(`Query: ${query}`);
 
             // Short circuit on empty query
             if (query.length === 0)
                 return;
@@ -436,157 +453,192 @@
                 let response = await fetch('/api/chat/sessions', { method: "POST" });
                 let data = await response.json();
                 conversationID = data.conversation_id;
                 chat_body.dataset.conversationId = conversationID;
                 refreshChatSessionsPanel();
             }
 
-            // Generate backend API URL to execute query
-            let url = `/api/chat?q=${encodeURIComponent(query)}&n=${resultsCount}&client=web&stream=true&conversation_id=${conversationID}&region=${region}&city=${city}&country=${countryName}`;
-
             let new_response = document.createElement("div");
             new_response.classList.add("chat-message", "khoj");
             new_response.attributes["data-meta"] = "🏮 Khoj at " + formatDate(new Date());
             chat_body.appendChild(new_response);
 
             let newResponseText = document.createElement("div");
             newResponseText.classList.add("chat-message-text", "khoj");
             new_response.appendChild(newResponseText);
 
             // Temporary status message to indicate that Khoj is thinking
-            let loadingEllipsis = document.createElement("div");
-            loadingEllipsis.classList.add("lds-ellipsis");
-
-            let firstEllipsis = document.createElement("div");
-            firstEllipsis.classList.add("lds-ellipsis-item");
-
-            let secondEllipsis = document.createElement("div");
-            secondEllipsis.classList.add("lds-ellipsis-item");
-
-            let thirdEllipsis = document.createElement("div");
-            thirdEllipsis.classList.add("lds-ellipsis-item");
-
-            let fourthEllipsis = document.createElement("div");
-            fourthEllipsis.classList.add("lds-ellipsis-item");
-
-            loadingEllipsis.appendChild(firstEllipsis);
-            loadingEllipsis.appendChild(secondEllipsis);
-            loadingEllipsis.appendChild(thirdEllipsis);
-            loadingEllipsis.appendChild(fourthEllipsis);
+            let loadingEllipsis = createLoadingEllipse();
 
             newResponseText.appendChild(loadingEllipsis);
             document.getElementById("chat-body").scrollTop = document.getElementById("chat-body").scrollHeight;
 
             let chatTooltip = document.getElementById("chat-tooltip");
             chatTooltip.style.display = "none";
 
             let chatInput = document.getElementById("chat-input");
             chatInput.classList.remove("option-enabled");
 
+            // Generate backend API URL to execute query
+            let url = `/api/chat?q=${encodeURIComponent(query)}&n=${resultsCount}&client=web&stream=true&conversation_id=${conversationID}&region=${region}&city=${city}&country=${countryName}`;
+
             // Call specified Khoj API
             let response = await fetch(url);
             let rawResponse = "";
             let references = null;
             const contentType = response.headers.get("content-type");
 
             if (contentType === "application/json") {
                 // Handle JSON response
                 try {
                     const responseAsJson = await response.json();
-                    if (responseAsJson.image) {
-                        // If response has image field, response is a generated image.
-                        if (responseAsJson.intentType === "text-to-image") {
-                            rawResponse += `![${query}](data:image/png;base64,${responseAsJson.image})`;
-                        } else if (responseAsJson.intentType === "text-to-image2") {
-                            rawResponse += `![${query}](${responseAsJson.image})`;
-                        }
-                        const inferredQuery = responseAsJson.inferredQueries?.[0];
-                        if (inferredQuery) {
-                            rawResponse += `\n\n**Inferred Query**:\n\n${inferredQuery}`;
-                        }
-                    }
-                    if (responseAsJson.context && responseAsJson.context.length > 0) {
-                        const rawReferenceAsJson = responseAsJson.context;
-                        references = createReferenceSection(rawReferenceAsJson);
-                    }
-                    if (responseAsJson.detail) {
-                        // If response has detail field, response is an error message.
-                        rawResponse += responseAsJson.detail;
+                    if (responseAsJson.image || responseAsJson.detail) {
+                        ({rawResponse, references } = handleImageResponse(responseAsJson, rawResponse));
+                    } else {
+                        rawResponse = responseAsJson.response;
                     }
                 } catch (error) {
                     // If the chunk is not a JSON object, just display it as is
                     rawResponse += chunk;
                 } finally {
-                    newResponseText.innerHTML = "";
-                    newResponseText.appendChild(formatHTMLMessage(rawResponse));
-
-                    if (references != null) {
-                        newResponseText.appendChild(references);
-                    }
-
-                    document.getElementById("chat-body").scrollTop = document.getElementById("chat-body").scrollHeight;
-                    document.getElementById("chat-input").removeAttribute("disabled");
+                    addMessageToChatBody(rawResponse, newResponseText, references);
                 }
             } else {
                 // Handle streamed response of type text/event-stream or text/plain
                 const reader = response.body.getReader();
                 const decoder = new TextDecoder();
                 let references = {};
 
                 readStream();
 
                 function readStream() {
                     reader.read().then(({ done, value }) => {
                         if (done) {
                             // Append any references after all the data has been streamed
-                            if (references != {}) {
-                                newResponseText.appendChild(createReferenceSection(references));
-                            }
-                            document.getElementById("chat-body").scrollTop = document.getElementById("chat-body").scrollHeight;
-                            document.getElementById("chat-input").removeAttribute("disabled");
+                            finalizeChatBodyResponse(references, newResponseText);
                             return;
                         }
 
                         // Decode message chunk from stream
                         const chunk = decoder.decode(value, { stream: true });
 
                         if (chunk.includes("### compiled references:")) {
-                            const additionalResponse = chunk.split("### compiled references:")[0];
-                            rawResponse += additionalResponse;
-                            newResponseText.innerHTML = "";
-                            newResponseText.appendChild(formatHTMLMessage(rawResponse));
-
-                            const rawReference = chunk.split("### compiled references:")[1];
-                            const rawReferenceAsJson = JSON.parse(rawReference);
-                            if (rawReferenceAsJson instanceof Array) {
-                                references["notes"] = rawReferenceAsJson;
-                            } else if (typeof rawReferenceAsJson === "object" && rawReferenceAsJson !== null) {
-                                references["online"] = rawReferenceAsJson;
-                            }
+                            ({ rawResponse, references } = handleCompiledReferences(newResponseText, chunk, references, rawResponse));
                             readStream();
                         } else {
-                            // Display response from Khoj
-                            if (newResponseText.getElementsByClassName("lds-ellipsis").length > 0) {
-                                newResponseText.removeChild(loadingEllipsis);
-                            }
-
                             // If the chunk is not a JSON object, just display it as is
                             rawResponse += chunk;
-                            newResponseText.innerHTML = "";
-                            newResponseText.appendChild(formatHTMLMessage(rawResponse));
+                            handleStreamResponse(newResponseText, rawResponse, loadingEllipsis);
                             readStream();
                         }
                     });
 
                     // Scroll to bottom of chat window as chat response is streamed
                     document.getElementById("chat-body").scrollTop = document.getElementById("chat-body").scrollHeight;
                 };
             }
         };
 
+        function createLoadingEllipse() {
+            // Temporary status message to indicate that Khoj is thinking
+            let loadingEllipsis = document.createElement("div");
+            loadingEllipsis.classList.add("lds-ellipsis");
+
+            let firstEllipsis = document.createElement("div");
+            firstEllipsis.classList.add("lds-ellipsis-item");
+
+            let secondEllipsis = document.createElement("div");
+            secondEllipsis.classList.add("lds-ellipsis-item");
+
+            let thirdEllipsis = document.createElement("div");
+            thirdEllipsis.classList.add("lds-ellipsis-item");
+
+            let fourthEllipsis = document.createElement("div");
+            fourthEllipsis.classList.add("lds-ellipsis-item");
+
+            loadingEllipsis.appendChild(firstEllipsis);
+            loadingEllipsis.appendChild(secondEllipsis);
+            loadingEllipsis.appendChild(thirdEllipsis);
+            loadingEllipsis.appendChild(fourthEllipsis);
+
+            return loadingEllipsis;
+        }
+
+        function handleStreamResponse(newResponseElement, rawResponse, loadingEllipsis, replace=true) {
+            if (newResponseElement.getElementsByClassName("lds-ellipsis").length > 0 && loadingEllipsis) {
+                newResponseElement.removeChild(loadingEllipsis);
+            }
+            if (replace) {
+                newResponseElement.innerHTML = "";
+            }
+            newResponseElement.appendChild(formatHTMLMessage(rawResponse));
+            document.getElementById("chat-body").scrollTop = document.getElementById("chat-body").scrollHeight;
+        }
+
+        function handleCompiledReferences(rawResponseElement, chunk, references, rawResponse) {
+            const additionalResponse = chunk.split("### compiled references:")[0];
+            rawResponse += additionalResponse;
+            rawResponseElement.innerHTML = "";
+            rawResponseElement.appendChild(formatHTMLMessage(rawResponse));
+
+            const rawReference = chunk.split("### compiled references:")[1];
+            const rawReferenceAsJson = JSON.parse(rawReference);
+            if (rawReferenceAsJson instanceof Array) {
+                references["notes"] = rawReferenceAsJson;
+            } else if (typeof rawReferenceAsJson === "object" && rawReferenceAsJson !== null) {
+                references["online"] = rawReferenceAsJson;
+            }
+            return { rawResponse, references };
+        }
+
+        function handleImageResponse(imageJson, rawResponse) {
+            if (imageJson.image) {
+                const inferredQuery = imageJson.inferredQueries?.[0] ?? "generated image";
+
+                // If response has image field, response is a generated image.
+                if (imageJson.intentType === "text-to-image") {
+                    rawResponse += `![generated_image](data:image/png;base64,${imageJson.image})`;
+                } else if (imageJson.intentType === "text-to-image2") {
+                    rawResponse += `![generated_image](${imageJson.image})`;
+                }
+                if (inferredQuery) {
+                    rawResponse += `\n\n**Inferred Query**:\n\n${inferredQuery}`;
+                }
+            }
+            let references = {};
+            if (imageJson.context && imageJson.context.length > 0) {
+                const rawReferenceAsJson = imageJson.context;
+                if (rawReferenceAsJson instanceof Array) {
+                    references["notes"] = rawReferenceAsJson;
+                } else if (typeof rawReferenceAsJson === "object" && rawReferenceAsJson !== null) {
+                    references["online"] = rawReferenceAsJson;
+                }
+            }
+            if (imageJson.detail) {
+                // If response has detail field, response is an error message.
+                rawResponse += imageJson.detail;
+            }
+            return { rawResponse, references };
+        }
+
+        function addMessageToChatBody(rawResponse, newResponseElement, references) {
+            newResponseElement.innerHTML = "";
+            newResponseElement.appendChild(formatHTMLMessage(rawResponse));
+
+            finalizeChatBodyResponse(references, newResponseElement);
+        }
+
+        function finalizeChatBodyResponse(references, newResponseElement) {
+            if (references != null && Object.keys(references).length > 0) {
+                newResponseElement.appendChild(createReferenceSection(references));
+            }
+            document.getElementById("chat-body").scrollTop = document.getElementById("chat-body").scrollHeight;
+            document.getElementById("chat-input").removeAttribute("disabled");
+        }
+
         function incrementalChat(event) {
             if (!event.shiftKey && event.key === 'Enter') {
                 event.preventDefault();
                 chat();
             }
         }
 
@@ -794,21 +846,196 @@
                 var file = event.dataTransfer.files[0];
                 uploadDataForIndexing(file);
             };
         }
 
         window.onload = loadChat;
 
+        function setupWebSocket() {
+            let chatBody = document.getElementById("chat-body");
+            let wsProtocol = window.location.protocol === 'https:' ? 'wss:' : 'ws:';
+            let webSocketUrl = `${wsProtocol}//${window.location.host}/api/chat/ws`;
+
+            websocketState = {
+                newResponseText: null,
+                newResponseElement: null,
+                loadingEllipsis: null,
+                references: {},
+                rawResponse: "",
+            }
+
+            function resetTimeout() {
+                if (timeout) {
+                    clearTimeout(timeout);
+                }
+
+                timeout = setTimeout(function() {
+                    if (websocket) {
+                        websocket.close();
+                    }
+                }, timeoutDuration);
+            }
+
+            if (chatBody.dataset.conversationId) {
+                webSocketUrl += `?conversation_id=${chatBody.dataset.conversationId}`;
+                webSocketUrl += `&region=${region}&city=${city}&country=${countryName}`;
+
+                websocket = new WebSocket(webSocketUrl);
+                websocket.onmessage = function(event) {
+                    resetTimeout();
+
+                    // Get the last element in the chat-body
+                    let chunk = event.data;
+                    if (chunk == "start_llm_response") {
+                        console.log("Started streaming", new Date());
+                    } else if(chunk == "end_llm_response") {
+                        console.log("Stopped streaming", new Date());
+                        // Append any references after all the data has been streamed
+                        finalizeChatBodyResponse(websocketState.references, websocketState.newResponseText);
+
+                        // Reset variables
+                        websocketState = {
+                            newResponseText: null,
+                            newResponseElement: null,
+                            loadingEllipsis: null,
+                            references: {},
+                            rawResponse: "",
+                        }
+                    } else {
+                        try {
+                            if (chunk.includes("application/json"))
+                            {
+                                chunk = JSON.parse(chunk);
+                            }
+                        } catch (error) {
+                            // If the chunk is not a JSON object, continue.
+                        }
+
+                        const contentType = chunk["content-type"]
+
+                        if (contentType === "application/json") {
+                            // Handle JSON response
+                            try {
+                                if (chunk.image || chunk.detail) {
+                                    ({rawResponse, references } = handleImageResponse(chunk, websocketState.rawResponse));
+                                    websocketState.rawResponse = rawResponse;
+                                    websocketState.references = references;
+                                } else if (chunk.type == "status") {
+                                    handleStreamResponse(websocketState.newResponseText, chunk.message, null, false);
+                                } else {
+                                    rawResponse = chunk.response;
+                                }
+                            } catch (error) {
+                                // If the chunk is not a JSON object, just display it as is
+                                websocketState.rawResponse += chunk;
+                            } finally {
+                                if (chunk.type != "status") {
+                                    addMessageToChatBody(websocketState.rawResponse, websocketState.newResponseText, websocketState.references);
+                                }
+                            }
+                        } else {
+
+                            // Handle streamed response of type text/event-stream or text/plain
+                            if (chunk && chunk.includes("### compiled references:")) {
+                                ({ rawResponse, references } = handleCompiledReferences(websocketState.newResponseText, chunk, websocketState.references, websocketState.rawResponse));
+                                websocketState.rawResponse = rawResponse;
+                                websocketState.references = references;
+                            } else {
+                                // If the chunk is not a JSON object, just display it as is
+                                websocketState.rawResponse += chunk;
+                                if (websocketState.newResponseText) {
+                                    handleStreamResponse(websocketState.newResponseText, websocketState.rawResponse, websocketState.loadingEllipsis);
+                                }
+                            }
+
+                            // Scroll to bottom of chat window as chat response is streamed
+                            document.getElementById("chat-body").scrollTop = document.getElementById("chat-body").scrollHeight;
+                        };
+                    }
+                }
+            };
+            websocket.onclose = function(event) {
+                websocket = null;
+                console.log("WebSocket is closed now.");
+                let greenDot = document.getElementById("connected-green-dot");
+                greenDot.style.display = "none";
+            }
+            websocket.onerror = function(event) {
+                console.log("WebSocket error observed:", event);
+            }
+
+            websocket.onopen = function(event) {
+                console.log("WebSocket is open now.")
+                let greenDot = document.getElementById("connected-green-dot");
+                greenDot.style.display = "flex";
+
+                // Setup the timeout to close the connection after inactivity.
+                resetTimeout();
+            }
+        }
+
+        function sendMessageViaWebSocket(event) {
+            if (event) {
+                event.preventDefault();
+            }
+
+            let chatBody = document.getElementById("chat-body");
+
+            var query = document.getElementById("chat-input").value.trim();
+            console.log(`Query: ${query}`);
+
+            // Add message by user to chat body
+            renderMessage(query, "you");
+            document.getElementById("chat-input").value = "";
+            autoResize();
+            document.getElementById("chat-input").setAttribute("disabled", "disabled");
+
+            let newResponseElement = document.createElement("div");
+            newResponseElement.classList.add("chat-message", "khoj");
+            newResponseElement.attributes["data-meta"] = "🏮 Khoj at " + formatDate(new Date());
+            chatBody.appendChild(newResponseElement);
+
+            let newResponseText = document.createElement("div");
+            newResponseText.classList.add("chat-message-text", "khoj");
+            newResponseElement.appendChild(newResponseText);
+
+            // Temporary status message to indicate that Khoj is thinking
+            let loadingEllipsis = createLoadingEllipse();
+
+            newResponseText.appendChild(loadingEllipsis);
+            document.getElementById("chat-body").scrollTop = document.getElementById("chat-body").scrollHeight;
+
+            let chatTooltip = document.getElementById("chat-tooltip");
+            chatTooltip.style.display = "none";
+
+            let chatInput = document.getElementById("chat-input");
+            chatInput.classList.remove("option-enabled");
+
+            // Call specified Khoj API
+            websocket.send(query);
+            let rawResponse = "";
+            let references = {};
+
+            websocketState = {
+                newResponseText,
+                newResponseElement,
+                loadingEllipsis,
+                references,
+                rawResponse,
+            }
+        }
+
         function loadChat() {
             let chatBody = document.getElementById("chat-body");
             chatBody.innerHTML = "";
             chatBody.classList.add("relative-position");
             let chatHistoryUrl = `/api/chat/history?client=web`;
             if (chatBody.dataset.conversationId) {
                 chatHistoryUrl += `&conversation_id=${chatBody.dataset.conversationId}`;
+                setupWebSocket();
             }
 
             if (window.screen.width < 700) {
                 handleCollapseSidePanel();
             }
 
             // Create loading screen and add it to chat-body
@@ -837,14 +1064,15 @@
                     }
                     return data.response;
                 })
                 .then(response => {
                     // Render conversation history, if any
                     let chatBody = document.getElementById("chat-body");
                     chatBody.dataset.conversationId = response.conversation_id;
+                    setupWebSocket();
                     chatBody.dataset.conversationTitle = response.slug || `New conversation 🌱`;
 
                     let agentMetadata = response.agent;
                     if (agentMetadata) {
                         let agentName = agentMetadata.name;
                         let agentAvatar = agentMetadata.avatar;
                         let agentOwnedByUser = agentMetadata.isCreator;
@@ -1319,14 +1547,18 @@
         <!--Add Header Logo and Nav Pane-->
         {% import 'utils.html' as utils %}
         {{ utils.heading_pane(user_photo, username, is_active, has_documents) }}
         <div id="chat-section-wrapper">
             <div id="side-panel-wrapper">
                 <div id="side-panel">
                     <div id="new-conversation">
+                        <div id="connected-green-dot" style="display: none; align-items: center; margin-bottom: 10px;">
+                            <div style="width: 10px; height: 10px; background-color: green; border-radius: 50%; margin-right: 5px;"></div>
+                            <div>Connected</div>
+                        </div>
                         <button class="side-panel-button" id="new-conversation-button" onclick="createNewConversation()">
                             New Topic
                             <svg class="new-convo-button" viewBox="0 0 35 35" fill="#000000" viewBox="0 0 32 32" version="1.1" xmlns="http://www.w3.org/2000/svg">
                                 <path d="M16 0c-8.836 0-16 7.163-16 16s7.163 16 16 16c8.837 0 16-7.163 16-16s-7.163-16-16-16zM16 30.032c-7.72 0-14-6.312-14-14.032s6.28-14 14-14 14 6.28 14 14-6.28 14.032-14 14.032zM23 15h-6v-6c0-0.552-0.448-1-1-1s-1 0.448-1 1v6h-6c-0.552 0-1 0.448-1 1s0.448 1 1 1h6v6c0 0.552 0.448 1 1 1s1-0.448 1-1v-6h6c0.552 0 1-0.448 1-1s-0.448-1-1-1z"></path>
                             </svg>
                         </button>
                         <div id="conversation-list-header" style="display: none;">Conversations</div>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 {% import 'utils.html' as utils %} {{ utils.heading_pane(user_photo, username,
 is_active, has_documents) }}
+Connected
 New Topic
 Conversations
 Active
 [Agent Avatar]
 Edit
```

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/config.html` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/content_source_computer_input.html` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/content_source_computer_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/content_source_github_input.html` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/content_source_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/content_source_notion_input.html` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/content_source_notion_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/khoj.webmanifest` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/khoj.webmanifest`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/login.html` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/login.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/search.html` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/search.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/utils.html` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/utils.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/utils.js` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/utils.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/computer.png` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/computer.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/copy_button.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/copy_button.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/credit-card.png` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/credit-card.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/favicon-256x256.png` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/favicon-256x256.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/key.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/key.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/microphone-solid.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/microphone-solid.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/notion.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/notion.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/openai-logomark.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/openai-logomark.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/plaintext.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/plaintext.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/question-mark-icon.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/question-mark-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/stop-solid.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/stop-solid.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/user-silhouette.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/user-silhouette.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/web.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/web.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/icons/whatsapp.svg` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/icons/whatsapp.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png` & `khoj_assistant-1.8.1.dev48/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/migrations/migrate_offline_chat_default_model.py` & `khoj_assistant-1.8.1.dev48/src/khoj/migrations/migrate_offline_chat_default_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/migrations/migrate_offline_chat_default_model_2.py` & `khoj_assistant-1.8.1.dev48/src/khoj/migrations/migrate_offline_chat_default_model_2.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/migrations/migrate_offline_chat_schema.py` & `khoj_assistant-1.8.1.dev48/src/khoj/migrations/migrate_offline_chat_schema.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/migrations/migrate_offline_model.py` & `khoj_assistant-1.8.1.dev48/src/khoj/migrations/migrate_offline_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/migrations/migrate_processor_config_openai.py` & `khoj_assistant-1.8.1.dev48/src/khoj/migrations/migrate_processor_config_openai.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/migrations/migrate_server_pg.py` & `khoj_assistant-1.8.1.dev48/src/khoj/migrations/migrate_server_pg.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/migrations/migrate_version.py` & `khoj_assistant-1.8.1.dev48/src/khoj/migrations/migrate_version.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/embeddings.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/embeddings.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/content/text_to_entries.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/content/text_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/content/github/github_to_entries.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/content/github/github_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/content/markdown/markdown_to_entries.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/content/markdown/markdown_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/content/notion/notion_to_entries.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/content/notion/notion_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/content/org_mode/org_to_entries.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/content/org_mode/org_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/content/org_mode/orgnode.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/content/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/content/pdf/pdf_to_entries.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/content/pdf/pdf_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/content/plaintext/plaintext_to_entries.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/content/plaintext/plaintext_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/utils.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/offline/chat_model.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/offline/chat_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/offline/utils.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/offline/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/openai/gpt.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/openai/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/conversation/openai/utils.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/conversation/openai/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/processor/tools/online_search.py` & `khoj_assistant-1.8.1.dev48/src/khoj/processor/tools/online_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/routers/api.py` & `khoj_assistant-1.8.1.dev48/src/khoj/routers/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,44 @@
     n: Optional[int] = 5,
     t: Optional[SearchType] = SearchType.All,
     r: Optional[bool] = False,
     max_distance: Optional[Union[float, None]] = None,
     dedupe: Optional[bool] = True,
 ):
     user = request.user.object
+
+    results = await execute_search(
+        user=user,
+        q=q,
+        n=n,
+        t=t,
+        r=r,
+        max_distance=max_distance,
+        dedupe=dedupe,
+    )
+
+    update_telemetry_state(
+        request=request,
+        telemetry_type="api",
+        api="search",
+        **common.__dict__,
+    )
+
+    return results
+
+
+async def execute_search(
+    user: KhojUser,
+    q: str,
+    n: Optional[int] = 5,
+    t: Optional[SearchType] = SearchType.All,
+    r: Optional[bool] = False,
+    max_distance: Optional[Union[float, None]] = None,
+    dedupe: Optional[bool] = True,
+):
     start_time = time.time()
 
     # Run validation checks
     results: List[SearchResponse] = []
     if q is None or q == "":
         logger.warning(f"No query param (q) passed in API call to initiate search")
         return results
@@ -151,21 +181,14 @@
                         results, query=defiltered_query, rank_results=r, search_model_name=search_model.name
                     )[:results_count]
 
     # Cache results
     if user:
         state.query_cache[user.uuid][query_cache_key] = results
 
-    update_telemetry_state(
-        request=request,
-        telemetry_type="api",
-        api="search",
-        **common.__dict__,
-    )
-
     end_time = time.time()
     logger.debug(f"🔍 Search took: {end_time - start_time:.3f} seconds")
 
     return results
 
 
 @api.get("/update")
@@ -346,22 +369,22 @@
     # Collate search results as context for GPT
     with timer("Searching knowledge base took", logger):
         result_list = []
         logger.info(f"🔍 Searching knowledge base with queries: {inferred_queries}")
         for query in inferred_queries:
             n_items = min(n, 3) if using_offline_chat else n
             result_list.extend(
-                await search(
+                await execute_search(
+                    user,
                     f"{query} {filters_in_query}",
-                    request=request,
                     n=n_items,
+                    t=SearchType.All,
                     r=True,
                     max_distance=d,
                     dedupe=False,
-                    common=common,
                 )
             )
         result_list = text_search.deduplicated_search_responses(result_list)
         compiled_references = [item.additional["compiled"] for item in result_list]
 
     return compiled_references, inferred_queries, defiltered_query
```

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/routers/api_agents.py` & `khoj_assistant-1.8.1.dev48/src/khoj/routers/api_agents.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/routers/api_chat.py` & `khoj_assistant-1.8.1.dev48/src/khoj/routers/api_chat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import json
 import logging
 import math
 from typing import Dict, Optional
 from urllib.parse import unquote
 
 from asgiref.sync import sync_to_async
-from fastapi import APIRouter, Depends, Request
+from fastapi import APIRouter, Depends, Request, WebSocket
 from fastapi.requests import Request
 from fastapi.responses import Response, StreamingResponse
 from starlette.authentication import requires
+from starlette.websockets import WebSocketDisconnect
+from websockets import ConnectionClosedOK
 
 from khoj.database.adapters import ConversationAdapters, EntryAdapters, aget_user_name
 from khoj.database.models import KhojUser
 from khoj.processor.conversation.prompts import (
     help_message,
     no_entries_found,
     no_notes_found,
@@ -238,14 +240,238 @@
     )
 
     return Response(
         content=json.dumps({"status": "ok", "success": success}), media_type="application/json", status_code=200
     )
 
 
+@api_chat.websocket("/ws")
+async def websocket_endpoint(
+    websocket: WebSocket,
+    conversation_id: int,
+    city: Optional[str] = None,
+    region: Optional[str] = None,
+    country: Optional[str] = None,
+):
+    connection_alive = True
+
+    async def send_status_update(message: str):
+        nonlocal connection_alive
+        if not connection_alive:
+            return
+
+        status_packet = {
+            "type": "status",
+            "message": message,
+            "content-type": "application/json",
+        }
+        try:
+            await websocket.send_text(json.dumps(status_packet))
+        except ConnectionClosedOK:
+            connection_alive = False
+            logger.info(f"User {user} disconnected web socket. Emitting rest of responses to clear thread")
+
+    async def send_complete_llm_response(llm_response: str):
+        nonlocal connection_alive
+        if not connection_alive:
+            return
+        try:
+            await websocket.send_text("start_llm_response")
+            await websocket.send_text(llm_response)
+            await websocket.send_text("end_llm_response")
+        except ConnectionClosedOK:
+            connection_alive = False
+            logger.info(f"User {user} disconnected web socket. Emitting rest of responses to clear thread")
+
+    async def send_message(message: str):
+        nonlocal connection_alive
+        if not connection_alive:
+            return
+        try:
+            await websocket.send_text(message)
+        except ConnectionClosedOK:
+            connection_alive = False
+            logger.info(f"User {user} disconnected web socket. Emitting rest of responses to clear thread")
+
+    user: KhojUser = websocket.user.object
+    conversation = await ConversationAdapters.aget_conversation_by_user(
+        user, client_application=websocket.user.client_app, conversation_id=conversation_id
+    )
+
+    hourly_limiter = ApiUserRateLimiter(requests=5, subscribed_requests=60, window=60, slug="chat_minute")
+
+    daily_limiter = ApiUserRateLimiter(requests=5, subscribed_requests=600, window=60 * 60 * 24, slug="chat_day")
+
+    await is_ready_to_chat(user)
+
+    user_name = await aget_user_name(user)
+
+    location = None
+
+    if city or region or country:
+        location = LocationData(city=city, region=region, country=country)
+
+    await websocket.accept()
+    while connection_alive:
+        try:
+            q = await websocket.receive_text()
+        except WebSocketDisconnect:
+            logger.debug(f"User {user} disconnected web socket")
+            break
+
+        await sync_to_async(hourly_limiter)(websocket)
+        await sync_to_async(daily_limiter)(websocket)
+
+        conversation_commands = [get_conversation_command(query=q, any_references=True)]
+
+        await send_status_update(f"**Processing query**: {q}")
+
+        if conversation_commands == [ConversationCommand.Help]:
+            conversation_config = await ConversationAdapters.aget_user_conversation_config(user)
+            if conversation_config == None:
+                conversation_config = await ConversationAdapters.aget_default_conversation_config()
+            model_type = conversation_config.model_type
+            formatted_help = help_message.format(model=model_type, version=state.khoj_version, device=get_device())
+            await send_complete_llm_response(formatted_help)
+            continue
+
+        meta_log = conversation.conversation_log
+
+        if conversation_commands == [ConversationCommand.Default]:
+            conversation_commands = await aget_relevant_information_sources(q, meta_log)
+            mode = await aget_relevant_output_modes(q, meta_log)
+            if mode not in conversation_commands:
+                conversation_commands.append(mode)
+
+        for cmd in conversation_commands:
+            await conversation_command_rate_limiter.update_and_check_if_valid(websocket, cmd)
+            q = q.replace(f"/{cmd.value}", "").strip()
+
+        await send_status_update(
+            f"**Using conversation commands:** {', '.join([cmd.value for cmd in conversation_commands])}"
+        )
+
+        compiled_references, inferred_queries, defiltered_query = await extract_references_and_questions(
+            websocket, None, meta_log, q, 7, 0.18, conversation_commands, location
+        )
+
+        if compiled_references:
+            headings = set([c.split("\n")[0] for c in compiled_references])
+            await send_status_update(f"**Searching references**: {headings}")
+
+        online_results: Dict = dict()
+
+        if conversation_commands == [ConversationCommand.Notes] and not await EntryAdapters.auser_has_entries(user):
+            await send_complete_llm_response(f"{no_entries_found.format()}")
+            continue
+
+        if ConversationCommand.Notes in conversation_commands and is_none_or_empty(compiled_references):
+            conversation_commands.remove(ConversationCommand.Notes)
+
+        if ConversationCommand.Online in conversation_commands:
+            if not online_search_enabled():
+                conversation_commands.remove(ConversationCommand.Online)
+                # If online search is not enabled, try to read webpages directly
+                if ConversationCommand.Webpage not in conversation_commands:
+                    conversation_commands.append(ConversationCommand.Webpage)
+            else:
+                try:
+                    await send_status_update("**Operation**: Searching the web for relevant information...")
+                    online_results = await search_online(defiltered_query, meta_log, location)
+                    online_searches = ", ".join([f"{query}" for query in online_results.keys()])
+                    await send_status_update(f"**Online searches**: {online_searches}")
+                except ValueError as e:
+                    logger.warning(f"Error searching online: {e}. Attempting to respond without online results")
+                    await send_complete_llm_response(
+                        f"Error searching online: {e}. Attempting to respond without online results"
+                    )
+                    continue
+
+        if ConversationCommand.Image in conversation_commands:
+            update_telemetry_state(
+                request=websocket,
+                telemetry_type="api",
+                api="chat",
+                metadata={"conversation_command": conversation_commands[0].value},
+            )
+            await send_status_update("**Operation**: Augmenting your query and generating a superb image...")
+            intent_type = "text-to-image"
+            image, status_code, improved_image_prompt, image_url = await text_to_image(
+                q, user, meta_log, location_data=location, references=compiled_references, online_results=online_results
+            )
+            if image is None or status_code != 200:
+                content_obj = {
+                    "image": image,
+                    "intentType": intent_type,
+                    "detail": improved_image_prompt,
+                    "content-type": "application/json",
+                }
+                await send_complete_llm_response(json.dumps(content_obj))
+                continue
+
+            if image_url:
+                intent_type = "text-to-image2"
+                image = image_url
+            await sync_to_async(save_to_conversation_log)(
+                q,
+                image,
+                user,
+                meta_log,
+                intent_type=intent_type,
+                inferred_queries=[improved_image_prompt],
+                client_application=websocket.user.client_app,
+                conversation_id=conversation_id,
+                compiled_references=compiled_references,
+                online_results=online_results,
+            )
+            content_obj = {"image": image, "intentType": intent_type, "inferredQueries": [improved_image_prompt], "context": compiled_references, "content-type": "application/json", "online_results": online_results}  # type: ignore
+
+            await send_complete_llm_response(json.dumps(content_obj))
+            continue
+
+        llm_response, chat_metadata = await agenerate_chat_response(
+            defiltered_query,
+            meta_log,
+            conversation,
+            compiled_references,
+            online_results,
+            inferred_queries,
+            conversation_commands,
+            user,
+            websocket.user.client_app,
+            conversation_id,
+            location,
+            user_name,
+        )
+
+        chat_metadata["agent"] = conversation.agent.slug if conversation.agent else None
+
+        update_telemetry_state(
+            request=websocket,
+            telemetry_type="api",
+            api="chat",
+            metadata=chat_metadata,
+        )
+        iterator = AsyncIteratorWrapper(llm_response)
+
+        await send_message("start_llm_response")
+
+        async for item in iterator:
+            if item is None:
+                break
+            if connection_alive:
+                try:
+                    await send_message(f"{item}")
+                except ConnectionClosedOK:
+                    connection_alive = False
+                    logger.info(f"User {user} disconnected web socket. Emitting rest of responses to clear thread")
+
+        await send_message("end_llm_response")
+
+
 @api_chat.get("", response_class=Response)
 @requires(["authenticated"])
 async def chat(
     request: Request,
     common: CommonQueryParams,
     q: str,
     n: Optional[int] = 5,
```

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/routers/api_config.py` & `khoj_assistant-1.8.1.dev48/src/khoj/routers/api_config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/routers/api_phone.py` & `khoj_assistant-1.8.1.dev48/src/khoj/routers/api_phone.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/routers/auth.py` & `khoj_assistant-1.8.1.dev48/src/khoj/routers/auth.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/routers/helpers.py` & `khoj_assistant-1.8.1.dev48/src/khoj/routers/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/routers/indexer.py` & `khoj_assistant-1.8.1.dev48/src/khoj/routers/indexer.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/routers/storage.py` & `khoj_assistant-1.8.1.dev48/src/khoj/routers/storage.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/routers/subscription.py` & `khoj_assistant-1.8.1.dev48/src/khoj/routers/subscription.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/routers/twilio.py` & `khoj_assistant-1.8.1.dev48/src/khoj/routers/twilio.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/routers/web_client.py` & `khoj_assistant-1.8.1.dev48/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/search_filter/date_filter.py` & `khoj_assistant-1.8.1.dev48/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/search_filter/file_filter.py` & `khoj_assistant-1.8.1.dev48/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/search_filter/word_filter.py` & `khoj_assistant-1.8.1.dev48/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/search_type/image_search.py` & `khoj_assistant-1.8.1.dev48/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/search_type/text_search.py` & `khoj_assistant-1.8.1.dev48/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/utils/cli.py` & `khoj_assistant-1.8.1.dev48/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/utils/config.py` & `khoj_assistant-1.8.1.dev48/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/utils/constants.py` & `khoj_assistant-1.8.1.dev48/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/utils/fs_syncer.py` & `khoj_assistant-1.8.1.dev48/src/khoj/utils/fs_syncer.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/utils/helpers.py` & `khoj_assistant-1.8.1.dev48/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/utils/initialization.py` & `khoj_assistant-1.8.1.dev48/src/khoj/utils/initialization.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/utils/jsonl.py` & `khoj_assistant-1.8.1.dev48/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/utils/models.py` & `khoj_assistant-1.8.1.dev48/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/utils/rawconfig.py` & `khoj_assistant-1.8.1.dev48/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/utils/state.py` & `khoj_assistant-1.8.1.dev48/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/src/khoj/utils/yaml.py` & `khoj_assistant-1.8.1.dev48/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/.gitignore` & `khoj_assistant-1.8.1.dev48/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/LICENSE` & `khoj_assistant-1.8.1.dev48/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/README.md` & `khoj_assistant-1.8.1.dev48/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.1.dev15/pyproject.toml` & `khoj_assistant-1.8.1.dev48/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     "lxml == 4.9.3",
     "tzdata == 2023.3",
     "rapidocr-onnxruntime == 1.3.11",
     "openai-whisper >= 20231117",
     "django-phonenumber-field == 7.3.0",
     "phonenumbers == 8.13.27",
     "markdownify ~= 0.11.6",
+    "websockets == 12.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://khoj.dev"
 Documentation = "https://docs.khoj.dev"
 Code = "https://github.com/khoj-ai/khoj"
```

### Comparing `khoj_assistant-1.8.1.dev15/PKG-INFO` & `khoj_assistant-1.8.1.dev48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: khoj-assistant
-Version: 1.8.1.dev15
+Version: 1.8.1.dev48
 Summary: An AI copilot for your Second Brain
 Project-URL: Homepage, https://khoj.dev
 Project-URL: Documentation, https://docs.khoj.dev
 Project-URL: Code, https://github.com/khoj-ai/khoj
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: AGPL-3.0-or-later
 License-File: LICENSE
@@ -56,14 +56,15 @@
 Requires-Dist: sentence-transformers==2.5.1
 Requires-Dist: tenacity>=8.2.2
 Requires-Dist: tiktoken>=0.3.2
 Requires-Dist: torch==2.0.1
 Requires-Dist: transformers>=4.28.0
 Requires-Dist: tzdata==2023.3
 Requires-Dist: uvicorn==0.17.6
+Requires-Dist: websockets==12.0
 Provides-Extra: dev
 Requires-Dist: black>=23.1.0; extra == 'dev'
 Requires-Dist: factory-boy>=3.2.1; extra == 'dev'
 Requires-Dist: freezegun>=1.2.0; extra == 'dev'
 Requires-Dist: khoj-assistant[prod]; extra == 'dev'
 Requires-Dist: mypy>=1.0.1; extra == 'dev'
 Requires-Dist: pre-commit>=3.0.4; extra == 'dev'
```

