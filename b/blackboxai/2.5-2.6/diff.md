# Comparing `tmp/blackboxai-2.5.tar.gz` & `tmp/blackboxai-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboxai-2.5.tar", last modified: Sat Mar 23 15:38:06 2024, max compression
+gzip compressed data, was "blackboxai-2.6.tar", last modified: Wed Apr  3 19:17:52 2024, max compression
```

## Comparing `blackboxai-2.5.tar` & `blackboxai-2.6.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.814078 blackboxai-2.5/
--rw-r--r--   0 rizkrichard   (501) staff       (20)    33813 2024-03-23 14:46:01.000000 blackboxai-2.5/LICENSE
--rw-r--r--   0 rizkrichard   (501) staff       (20)      804 2024-03-23 15:38:06.813917 blackboxai-2.5/PKG-INFO
--rw-r--r--   0 rizkrichard   (501) staff       (20)      635 2024-03-23 14:46:01.000000 blackboxai-2.5/README.md
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.793436 blackboxai-2.5/blackboxai/
--rw-r--r--   0 rizkrichard   (501) staff       (20)       25 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1725 2024-03-23 15:33:42.000000 blackboxai-2.5/blackboxai/chat.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.793573 blackboxai-2.5/blackboxai/interpreter/
--rw-r--r--   0 rizkrichard   (501) staff       (20)      601 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/__init__.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.795274 blackboxai-2.5/blackboxai/interpreter/core/
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2820 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.795938 blackboxai-2.5/blackboxai/interpreter/core/ARCHIVE_rag/
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1293 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     3138 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/ARCHIVE_rag/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/__init__.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.796185 blackboxai-2.5/blackboxai/interpreter/core/computer/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/__init__.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.796567 blackboxai-2.5/blackboxai/interpreter/core/computer/ai/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/ai/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     5688 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/ai/ai.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.796954 blackboxai-2.5/blackboxai/interpreter/core/computer/browser/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/browser/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      399 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/browser/browser.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.797326 blackboxai-2.5/blackboxai/interpreter/core/computer/clipboard/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/clipboard/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      879 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/clipboard/clipboard.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2526 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/computer.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.797651 blackboxai-2.5/blackboxai/interpreter/core/computer/display/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/display/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     9531 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/display/display.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.798050 blackboxai-2.5/blackboxai/interpreter/core/computer/docs/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/docs/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      749 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/docs/docs.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.798469 blackboxai-2.5/blackboxai/interpreter/core/computer/files/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/files/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1698 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/files/files.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.798902 blackboxai-2.5/blackboxai/interpreter/core/computer/keyboard/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/keyboard/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     3553 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/keyboard/keyboard.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.799228 blackboxai-2.5/blackboxai/interpreter/core/computer/mouse/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/mouse/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)    12449 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/mouse/mouse.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.799648 blackboxai-2.5/blackboxai/interpreter/core/computer/os/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/os/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2961 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/os/os.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.799924 blackboxai-2.5/blackboxai/interpreter/core/computer/skills/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/skills/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     3586 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/skills/skills.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.800500 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1090 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/base_language.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.802803 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/
--rw-r--r--   0 rizkrichard   (501) staff       (20)     5164 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1812 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/applescript.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      858 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/html.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1924 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/javascript.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)    15293 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2193 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/powershell.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      293 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/python.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2360 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/r.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2500 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/react.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2727 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/shell.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     6715 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     4946 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/terminal.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.803642 blackboxai-2.5/blackboxai/interpreter/core/computer/utils/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/utils/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     7043 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/utils/computer_vision.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1479 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/utils/get_active_window.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      929 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      396 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/computer/utils/recipient_utils.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)    13438 2024-03-23 15:34:18.000000 blackboxai-2.5/blackboxai/interpreter/core/core.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1647 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/default_system_message.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.804612 blackboxai-2.5/blackboxai/interpreter/core/llm/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/llm/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     8524 2024-03-23 15:34:51.000000 blackboxai-2.5/blackboxai/interpreter/core/llm/llm.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     5120 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/llm/run_function_calling_llm.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2616 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/llm/run_text_llm.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.805349 blackboxai-2.5/blackboxai/interpreter/core/llm/utils/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/llm/utils/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     8613 2024-03-23 15:36:57.000000 blackboxai-2.5/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      711 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/llm/utils/merge_deltas.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1800 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/llm/utils/parse_partial_json.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      538 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/llm/vision_for_text_llms.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1288 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/render_message.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)    14088 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/respond.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     6162 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/server.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.807102 blackboxai-2.5/blackboxai/interpreter/core/utils/
--rw-r--r--   0 rizkrichard   (501) staff       (20)      630 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/utils/ARCHIVE_embed.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      360 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/utils/ARCHIVE_get_user_info_string.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1096 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/utils/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      920 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/utils/lazy_import.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2118 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/utils/scan_code.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     4415 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/utils/system_debug_info.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1736 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/utils/telemetry.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1098 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/utils/temporary_file.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      510 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/core/utils/truncate_output.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.808750 blackboxai-2.5/blackboxai/interpreter/terminal_interface/
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2433 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/__init__.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.809424 blackboxai-2.5/blackboxai/interpreter/terminal_interface/components/
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/components/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      611 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/components/base_block.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2664 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/components/code_block.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1386 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/components/message_block.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2905 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/conversation_navigator.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)    10586 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/magic_commands.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2304 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/render_past_conversation.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)    14679 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/start_terminal_interface.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)    20298 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/terminal_interface.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.812916 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/
--rw-r--r--   0 rizkrichard   (501) staff       (20)    25835 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     3099 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/__init__.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      512 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/check_for_package.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      481 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/check_for_update.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      419 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/cli_input.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1939 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/count_tokens.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      884 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     3069 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/display_output.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      459 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/find_image_path.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      250 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/get_conversations.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      184 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/in_jupyter_notebook.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)      316 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/local_storage_path.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)       79 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/oi_dir.py
--rw-r--r--   0 rizkrichard   (501) staff       (20)     2899 2024-03-23 14:46:01.000000 blackboxai-2.5/blackboxai/interpreter/terminal_interface/validate_llm_settings.py
-drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-03-23 15:38:06.813721 blackboxai-2.5/blackboxai.egg-info/
--rw-r--r--   0 rizkrichard   (501) staff       (20)      804 2024-03-23 15:38:06.000000 blackboxai-2.5/blackboxai.egg-info/PKG-INFO
--rw-r--r--   0 rizkrichard   (501) staff       (20)     6297 2024-03-23 15:38:06.000000 blackboxai-2.5/blackboxai.egg-info/SOURCES.txt
--rw-r--r--   0 rizkrichard   (501) staff       (20)        1 2024-03-23 15:38:06.000000 blackboxai-2.5/blackboxai.egg-info/dependency_links.txt
--rw-r--r--   0 rizkrichard   (501) staff       (20)       50 2024-03-23 15:38:06.000000 blackboxai-2.5/blackboxai.egg-info/entry_points.txt
--rw-r--r--   0 rizkrichard   (501) staff       (20)       11 2024-03-23 15:38:06.000000 blackboxai-2.5/blackboxai.egg-info/top_level.txt
--rw-r--r--   0 rizkrichard   (501) staff       (20)     1959 2024-03-23 14:46:01.000000 blackboxai-2.5/pyproject.toml
--rw-r--r--   0 rizkrichard   (501) staff       (20)       38 2024-03-23 15:38:06.814125 blackboxai-2.5/setup.cfg
--rw-r--r--   0 rizkrichard   (501) staff       (20)      523 2024-03-23 15:37:55.000000 blackboxai-2.5/setup.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.920207 blackboxai-2.6/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)    33813 2024-04-03 18:37:22.000000 blackboxai-2.6/LICENSE
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      804 2024-04-03 19:17:52.920036 blackboxai-2.6/PKG-INFO
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      635 2024-04-03 18:37:22.000000 blackboxai-2.6/README.md
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.896251 blackboxai-2.6/blackboxai/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)       25 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1725 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/chat.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.896529 blackboxai-2.6/blackboxai/interpreter/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      601 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/__init__.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.898255 blackboxai-2.6/blackboxai/interpreter/core/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2820 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.899172 blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_rag/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1293 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     3138 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_rag/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/__init__.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.899372 blackboxai-2.6/blackboxai/interpreter/core/computer/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/__init__.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.899800 blackboxai-2.6/blackboxai/interpreter/core/computer/ai/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/ai/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     5688 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/ai/ai.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.900157 blackboxai-2.6/blackboxai/interpreter/core/computer/browser/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/browser/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      399 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/browser/browser.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.900515 blackboxai-2.6/blackboxai/interpreter/core/computer/clipboard/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/clipboard/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      879 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/clipboard/clipboard.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2526 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/computer.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.900878 blackboxai-2.6/blackboxai/interpreter/core/computer/display/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/display/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     9531 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/display/display.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.901254 blackboxai-2.6/blackboxai/interpreter/core/computer/docs/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/docs/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      749 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/docs/docs.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.901624 blackboxai-2.6/blackboxai/interpreter/core/computer/files/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/files/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1698 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/files/files.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.902005 blackboxai-2.6/blackboxai/interpreter/core/computer/keyboard/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/keyboard/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     3553 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/keyboard/keyboard.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.902248 blackboxai-2.6/blackboxai/interpreter/core/computer/mouse/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/mouse/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)    12449 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/mouse/mouse.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.902680 blackboxai-2.6/blackboxai/interpreter/core/computer/os/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/os/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2961 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/os/os.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.903101 blackboxai-2.6/blackboxai/interpreter/core/computer/skills/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/skills/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     3586 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/skills/skills.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.903631 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1090 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/base_language.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.906907 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     5164 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1812 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/applescript.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      858 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/html.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1924 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/javascript.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)    15293 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2193 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/powershell.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      293 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/python.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2360 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/r.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2500 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/react.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2727 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/shell.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     6715 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     4946 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/terminal.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.907969 blackboxai-2.6/blackboxai/interpreter/core/computer/utils/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/utils/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     7043 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/utils/computer_vision.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1479 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/utils/get_active_window.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      929 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      396 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/computer/utils/recipient_utils.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)    13458 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/core.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1647 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/default_system_message.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.908939 blackboxai-2.6/blackboxai/interpreter/core/llm/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     8998 2024-04-03 19:17:36.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/llm.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     5120 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/run_function_calling_llm.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2616 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/run_text_llm.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.909867 blackboxai-2.6/blackboxai/interpreter/core/llm/utils/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/utils/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     7838 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      711 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/utils/merge_deltas.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1800 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/utils/parse_partial_json.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      538 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/llm/vision_for_text_llms.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1288 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/render_message.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)    14088 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/respond.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     6162 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/server.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.912296 blackboxai-2.6/blackboxai/interpreter/core/utils/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      630 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/ARCHIVE_embed.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      360 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/ARCHIVE_get_user_info_string.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1096 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      920 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/lazy_import.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2118 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/scan_code.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     4415 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/system_debug_info.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1736 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/telemetry.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1098 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/temporary_file.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      510 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/core/utils/truncate_output.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.914719 blackboxai-2.6/blackboxai/interpreter/terminal_interface/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2433 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/__init__.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.915480 blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      611 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/base_block.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2664 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/code_block.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1386 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/message_block.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2905 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/conversation_navigator.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)    10586 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/magic_commands.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2304 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/render_past_conversation.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)    14679 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/start_terminal_interface.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)    20298 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/terminal_interface.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.919063 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)    25835 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     3099 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        0 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/__init__.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      512 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/check_for_package.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      481 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/check_for_update.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      419 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/cli_input.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1939 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/count_tokens.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      884 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     3069 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/display_output.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      459 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/find_image_path.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      250 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/get_conversations.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      184 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/in_jupyter_notebook.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      316 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/local_storage_path.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)       79 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/oi_dir.py
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     2899 2024-04-03 18:37:22.000000 blackboxai-2.6/blackboxai/interpreter/terminal_interface/validate_llm_settings.py
+drwxr-xr-x   0 rizkrichard   (501) staff       (20)        0 2024-04-03 19:17:52.919821 blackboxai-2.6/blackboxai.egg-info/
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      804 2024-04-03 19:17:52.000000 blackboxai-2.6/blackboxai.egg-info/PKG-INFO
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     6297 2024-04-03 19:17:52.000000 blackboxai-2.6/blackboxai.egg-info/SOURCES.txt
+-rw-r--r--   0 rizkrichard   (501) staff       (20)        1 2024-04-03 19:17:52.000000 blackboxai-2.6/blackboxai.egg-info/dependency_links.txt
+-rw-r--r--   0 rizkrichard   (501) staff       (20)       50 2024-04-03 19:17:52.000000 blackboxai-2.6/blackboxai.egg-info/entry_points.txt
+-rw-r--r--   0 rizkrichard   (501) staff       (20)       11 2024-04-03 19:17:52.000000 blackboxai-2.6/blackboxai.egg-info/top_level.txt
+-rw-r--r--   0 rizkrichard   (501) staff       (20)     1959 2024-04-03 18:37:22.000000 blackboxai-2.6/pyproject.toml
+-rw-r--r--   0 rizkrichard   (501) staff       (20)       38 2024-04-03 19:17:52.920254 blackboxai-2.6/setup.cfg
+-rw-r--r--   0 rizkrichard   (501) staff       (20)      523 2024-04-03 19:12:05.000000 blackboxai-2.6/setup.py
```

### Comparing `blackboxai-2.5/LICENSE` & `blackboxai-2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/PKG-INFO` & `blackboxai-2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboxai
-Version: 2.5
+Version: 2.6
 Summary: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">BlackboxAI Interpreter</h1>
```

### Comparing `blackboxai-2.5/README.md` & `blackboxai-2.6/README.md`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/chat.py` & `blackboxai-2.6/blackboxai/chat.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/__init__.py` & `blackboxai-2.6/blackboxai/interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py` & `blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_extend_system_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py` & `blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_get_relevant_procedures_string.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py` & `blackboxai-2.6/blackboxai/interpreter/core/ARCHIVE_rag/ARCHIVE_local_get_relevant_procedures_string.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/ai/ai.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/ai/ai.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/clipboard/clipboard.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/clipboard/clipboard.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/computer.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/computer.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/display/display.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/display/display.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/docs/docs.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/docs/docs.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/files/files.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/files/files.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/keyboard/keyboard.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/keyboard/keyboard.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/mouse/mouse.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/mouse/mouse.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/os/os.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/os/os.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/skills/skills.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/skills/skills.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/base_language.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/base_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/ARCHIVE_subprocess_python.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/applescript.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/applescript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/html.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/html.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/javascript.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/javascript.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/jupyter_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/powershell.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/powershell.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/r.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/r.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/react.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/react.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/shell.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/shell.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/languages/subprocess_language.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/terminal/terminal.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/utils/computer_vision.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/utils/computer_vision.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/utils/get_active_window.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/utils/get_active_window.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py` & `blackboxai-2.6/blackboxai/interpreter/core/computer/utils/html_to_png_base64.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/core.py` & `blackboxai-2.6/blackboxai/interpreter/core/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         in_terminal_interface=False,
         conversation_history=True,
         conversation_filename=None,
         conversation_history_path=get_storage_path("conversations"),
         os=False,
         speak_messages=False,
         llm=None,
-        system_message="",
+        system_message=default_system_message,
         custom_instructions="",
         computer=None,
         sync_computer=True,
         import_computer_api=True,
         skills_path=None,
         import_skills=True,
         multi_line=False,
```

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/default_system_message.py` & `blackboxai-2.6/blackboxai/interpreter/core/default_system_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/llm/llm.py` & `blackboxai-2.6/blackboxai/interpreter/core/llm/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,32 @@
     display_markdown_message,
 )
 from .run_function_calling_llm import run_function_calling_llm
 from .run_text_llm import run_text_llm
 from .utils.convert_to_openai_messages import convert_to_openai_messages
 
 litellm.suppress_debug_info = True
+import requests
+import json
 
+def selectionFct(event):
+    try:
+        url = "https://www.useblackbox.io/selection"
+
+        payload = json.dumps({
+            "selected": event,
+            "source": "terminal"
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+    except Exception as e:
+        print(f"An error occurred: {e}")
 
 class Llm:
     """
     A stateless LMC-style LLM with some helpful properties.
     """
 
     def __init__(self, interpreter):
@@ -175,36 +192,38 @@
         if self.api_key:
             params["api_key"] = self.api_key
         if self.api_base:
             params["api_base"] = self.api_base
             params["custom_llm_provider"] = "openai"
         if self.api_version:
             params["api_version"] = self.api_version
-        if self.max_tokens is not None:
+        if self.max_tokens:
             params["max_tokens"] = self.max_tokens
         if self.temperature:
             params["temperature"] = self.temperature
 
         # Set some params directly on LiteLLM
         if self.max_budget:
             litellm.max_budget = self.max_budget
         if self.interpreter.verbose:
             litellm.set_verbose = True
 
         # print("=====>")
         # print(params)
         # exit()
+        selectionFct('Chat Request')
         if supports_functions:
             # print("--------------->")
             yield from run_function_calling_llm(self, params)
         else:
             # print("---===========>")
             yield from run_text_llm(self, params)
 
 
+
 def fixed_litellm_completions(**params):
     """
     Just uses a dummy API key, since we use litellm without an API key sometimes.
     Hopefully they will fix this!
     """
 
     # Run completion
```

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/llm/run_function_calling_llm.py` & `blackboxai-2.6/blackboxai/interpreter/core/llm/run_function_calling_llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/llm/run_text_llm.py` & `blackboxai-2.6/blackboxai/interpreter/core/llm/run_text_llm.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py` & `blackboxai-2.6/blackboxai/interpreter/core/llm/utils/convert_to_openai_messages.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,13 @@
 import base64
 import io
 import json
 
 from PIL import Image
 
-def combine_assistant_messages(new_messages):
-    messages_to_remove = []
-    i = 0
-    while i < len(new_messages):
-        if new_messages[i]['role']=="assistant":
-            j = i+1
-            while j < len(new_messages) and new_messages[j]["role"] == "assistant":
-                new_messages[i]['content']+=(new_messages[j]['content']+"\n")
-                messages_to_remove.append(j)
-                j+=1
-            new_messages[i]['content'] = new_messages[i]['content'].replace("\nexecute>","")
-            i = j+1
-        else:
-            i+=1
-
-    retained_messages = [_i for idx, _i in enumerate(new_messages) if idx not in messages_to_remove]
-    return retained_messages
 
 def convert_to_openai_messages(
     messages, function_calling=True, vision=False, shrink_images=True
 ):
     """
     Converts LMC messages into OpenAI messages
     """
@@ -60,15 +43,15 @@
                 }
                 # Add empty content to avoid error "openai.error.InvalidRequestError: 'content' is a required property - 'messages.*'"
                 # especially for the OpenAI service hosted on Azure
                 new_message["content"] = ""
             else:
                 new_message[
                     "content"
-                ] = f"""<execute>\n```{message["format"]}\n{message["content"]}\n```\n</execute>"""
+                ] = f"""```{message["format"]}\n{message["content"]}\n```"""
 
         elif message["type"] == "console" and message["format"] == "output":
             if function_calling:
                 new_message["role"] = "function"
                 new_message["name"] = "execute"
                 if message["content"].strip() == "":
                     new_message[
@@ -168,15 +151,14 @@
             new_message = {"role": "user", "content": message["content"]}
 
         else:
             raise Exception(f"Unable to convert this message type: {message}")
 
         new_messages.append(new_message)
 
-    new_messages = combine_assistant_messages(new_messages[:])
     """
     # Combine adjacent user messages
     combined_messages = []
     i = 0
     while i < len(new_messages):
         message = new_messages[i]
         if message["role"] == "user":
```

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/llm/utils/merge_deltas.py` & `blackboxai-2.6/blackboxai/interpreter/core/llm/utils/merge_deltas.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/llm/utils/parse_partial_json.py` & `blackboxai-2.6/blackboxai/interpreter/core/llm/utils/parse_partial_json.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/llm/vision_for_text_llms.py` & `blackboxai-2.6/blackboxai/interpreter/core/llm/vision_for_text_llms.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/render_message.py` & `blackboxai-2.6/blackboxai/interpreter/core/render_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/respond.py` & `blackboxai-2.6/blackboxai/interpreter/core/respond.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/server.py` & `blackboxai-2.6/blackboxai/interpreter/core/server.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/utils/ARCHIVE_embed.py` & `blackboxai-2.6/blackboxai/interpreter/core/utils/ARCHIVE_embed.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py` & `blackboxai-2.6/blackboxai/interpreter/core/utils/ARCHIVE_vector_search.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/utils/lazy_import.py` & `blackboxai-2.6/blackboxai/interpreter/core/utils/lazy_import.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/utils/scan_code.py` & `blackboxai-2.6/blackboxai/interpreter/core/utils/scan_code.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/utils/system_debug_info.py` & `blackboxai-2.6/blackboxai/interpreter/core/utils/system_debug_info.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/utils/telemetry.py` & `blackboxai-2.6/blackboxai/interpreter/core/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/core/utils/temporary_file.py` & `blackboxai-2.6/blackboxai/interpreter/core/utils/temporary_file.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/ARCHIVE_start_terminal_interface_proto_profiles.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/components/base_block.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/base_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/components/code_block.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/code_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/components/message_block.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/components/message_block.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/conversation_navigator.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/conversation_navigator.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/magic_commands.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/magic_commands.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/render_past_conversation.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/render_past_conversation.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/start_terminal_interface.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/start_terminal_interface.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/terminal_interface.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/terminal_interface.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_apply_config.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/ARCHIVE_get_config.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/check_for_package.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/check_for_package.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/count_tokens.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/count_tokens.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/display_markdown_message.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/utils/display_output.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/utils/display_output.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai/interpreter/terminal_interface/validate_llm_settings.py` & `blackboxai-2.6/blackboxai/interpreter/terminal_interface/validate_llm_settings.py`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/blackboxai.egg-info/PKG-INFO` & `blackboxai-2.6/blackboxai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboxai
-Version: 2.5
+Version: 2.6
 Summary: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">BlackboxAI Interpreter</h1>
```

### Comparing `blackboxai-2.5/blackboxai.egg-info/SOURCES.txt` & `blackboxai-2.6/blackboxai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/pyproject.toml` & `blackboxai-2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboxai-2.5/setup.py` & `blackboxai-2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="blackboxai",
-    version="2.5",
+    version="2.6",
     packages=find_packages(),
     package_dir = {'': '.'},
     include_package_data=True,
     setup_requires= ['requests'],
     entry_points={
         "console_scripts": [
             "blackboxai = blackboxai:runChat"
```

