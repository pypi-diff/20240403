# Comparing `tmp/elevenlabs-1.0.3.tar.gz` & `tmp/elevenlabs-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-1.0.3.tar", max compression
+gzip compressed data, was "elevenlabs-1.0.4.tar", max compression
```

## Comparing `elevenlabs-1.0.3.tar` & `elevenlabs-1.0.4.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0     1067 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/LICENSE
--rw-r--r--   0        0        0     9366 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/README.md
--rw-r--r--   0        0        0      659 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4689 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/__init__.py
--rw-r--r--   0        0        0       65 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/audio_native/__init__.py
--rw-r--r--   0        0        0    13565 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/audio_native/client.py
--rw-r--r--   0        0        0     7523 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/base_client.py
--rw-r--r--   0        0        0       65 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/chapters/__init__.py
--rw-r--r--   0        0        0    34318 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/chapters/client.py
--rw-r--r--   0        0        0    20910 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/client.py
--rw-r--r--   0        0        0      790 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/core/__init__.py
--rw-r--r--   0        0        0      426 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/core/api_error.py
--rw-r--r--   0        0        0     1683 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/core/file.py
--rw-r--r--   0        0        0     5059 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/core/request_options.py
--rw-r--r--   0        0        0       65 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/dubbing/__init__.py
--rw-r--r--   0        0        0    27796 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/dubbing/client.py
--rw-r--r--   0        0        0      164 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/environment.py
--rw-r--r--   0        0        0      170 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/history/__init__.py
--rw-r--r--   0        0        0    27725 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/history/client.py
--rw-r--r--   0        0        0       65 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/models/__init__.py
--rw-r--r--   0        0        0     5069 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/models/client.py
--rw-r--r--   0        0        0     2715 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/play.py
--rw-r--r--   0        0        0       65 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/projects/__init__.py
--rw-r--r--   0        0        0    54697 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/projects/client.py
--rw-r--r--   0        0        0       65 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/pronunciation_dictionary/__init__.py
--rw-r--r--   0        0        0    13080 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/pronunciation_dictionary/client.py
--rw-r--r--   0        0        0        0 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/py.typed
--rw-r--r--   0        0        0     5093 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/realtime_tts.py
--rw-r--r--   0        0        0       65 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/samples/__init__.py
--rw-r--r--   0        0        0    11145 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/samples/client.py
--rw-r--r--   0        0        0       65 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/speech_to_speech/__init__.py
--rw-r--r--   0        0        0    20960 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/speech_to_speech/client.py
--rw-r--r--   0        0        0       65 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/text_to_speech/__init__.py
--rw-r--r--   0        0        0    23093 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/text_to_speech/client.py
--rw-r--r--   0        0        0     6114 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/__init__.py
--rw-r--r--   0        0        0      191 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/accent.py
--rw-r--r--   0        0        0      978 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/add_project_response_model.py
--rw-r--r--   0        0        0     1058 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py
--rw-r--r--   0        0        0      919 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/add_voice_response_model.py
--rw-r--r--   0        0        0      161 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/age.py
--rw-r--r--   0        0        0      980 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/audio_native_create_project_response_model.py
--rw-r--r--   0        0        0      130 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/audio_native_get_embed_code_response_model.py
--rw-r--r--   0        0        0     1560 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/audio_output.py
--rw-r--r--   0        0        0     1196 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/chapter_response.py
--rw-r--r--   0        0        0     1011 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/chapter_snapshot_response.py
--rw-r--r--   0        0        0     1019 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/chapter_snapshots_response.py
--rw-r--r--   0        0        0      164 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/chapter_state.py
--rw-r--r--   0        0        0     1029 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/chapter_statistics_response.py
--rw-r--r--   0        0        0      149 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/currency.py
--rw-r--r--   0        0        0      950 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/do_dubbing_response.py
--rw-r--r--   0        0        0      214 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/extended_subscription_response_model_billing_period.py
--rw-r--r--   0        0        0     1082 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/feedback_item.py
--rw-r--r--   0        0        0     1837 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/fine_tuning_response.py
--rw-r--r--   0        0        0      223 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/finetuning_state.py
--rw-r--r--   0        0        0      151 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/gender.py
--rw-r--r--   0        0        0     2288 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/generation_config.py
--rw-r--r--   0        0        0      988 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/get_chapters_response.py
--rw-r--r--   0        0        0     1048 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/get_library_voices_response.py
--rw-r--r--   0        0        0      988 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/get_projects_response.py
--rw-r--r--   0        0        0     1041 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py
--rw-r--r--   0        0        0     1073 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/get_speech_history_response.py
--rw-r--r--   0        0        0      953 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/get_voices_response.py
--rw-r--r--   0        0        0      101 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/history.py
--rw-r--r--   0        0        0      992 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/history_item.py
--rw-r--r--   0        0        0     1010 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/http_validation_error.py
--rw-r--r--   0        0        0      948 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/invoice.py
--rw-r--r--   0        0        0      931 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/language_response.py
--rw-r--r--   0        0        0     1639 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/library_voice_response.py
--rw-r--r--   0        0        0     1011 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/manual_verification_file_response.py
--rw-r--r--   0        0        0     1086 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/manual_verification_response.py
--rw-r--r--   0        0        0     1671 2024-03-28 16:25:39.410899 elevenlabs-1.0.3/src/elevenlabs/types/model.py
--rw-r--r--   0        0        0     2207 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/normalized_alignment.py
--rw-r--r--   0        0        0      176 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/optimize_streaming_latency.py
--rw-r--r--   0        0        0      408 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/output_format.py
--rw-r--r--   0        0        0     1278 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/project_extended_response_model.py
--rw-r--r--   0        0        0     1259 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/project_response.py
--rw-r--r--   0        0        0      991 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/project_snapshot_response.py
--rw-r--r--   0        0        0     1019 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/project_snapshots_response.py
--rw-r--r--   0        0        0      164 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/project_state.py
--rw-r--r--   0        0        0      974 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/pronunciation_dictionary_version_locator.py
--rw-r--r--   0        0        0     1477 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/realtime_voice_settings.py
--rw-r--r--   0        0        0     1007 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/recording_response.py
--rw-r--r--   0        0        0      220 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/review_status.py
--rw-r--r--   0        0        0     2353 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/send_text.py
--rw-r--r--   0        0        0      147 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/source.py
--rw-r--r--   0        0        0     1865 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/speech_history_item_response.py
--rw-r--r--   0        0        0      226 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/speech_history_item_response_model_voice_category.py
--rw-r--r--   0        0        0     1079 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/sso_provider_db_model.py
--rw-r--r--   0        0        0      173 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/sso_provider_db_model_provider_type.py
--rw-r--r--   0        0        0     1879 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/subscription.py
--rw-r--r--   0        0        0     1611 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/subscription_response.py
--rw-r--r--   0        0        0      200 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/subscription_response_model_billing_period.py
--rw-r--r--   0        0        0      256 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/subscription_status.py
--rw-r--r--   0        0        0     1141 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/user.py
--rw-r--r--   0        0        0     1029 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1120 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/verification_attempt_response.py
--rw-r--r--   0        0        0     1991 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/voice.py
--rw-r--r--   0        0        0      946 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/voice_generation_parameter_option_response.py
--rw-r--r--   0        0        0     1325 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/voice_generation_parameter_response.py
--rw-r--r--   0        0        0      216 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/voice_response_model_safety_control.py
--rw-r--r--   0        0        0     1102 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/voice_sample.py
--rw-r--r--   0        0        0     1083 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/voice_settings.py
--rw-r--r--   0        0        0     2354 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/voice_sharing_response.py
--rw-r--r--   0        0        0      196 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/voice_sharing_state.py
--rw-r--r--   0        0        0     1245 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/types/voice_verification_response.py
--rw-r--r--   0        0        0       65 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/user/__init__.py
--rw-r--r--   0        0        0     9207 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/user/client.py
--rw-r--r--   0        0        0       78 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/version.py
--rw-r--r--   0        0        0       65 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/voice_generation/__init__.py
--rw-r--r--   0        0        0    20238 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/voice_generation/client.py
--rw-r--r--   0        0        0       65 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/voices/__init__.py
--rw-r--r--   0        0        0    58857 2024-03-28 16:25:39.414899 elevenlabs-1.0.3/src/elevenlabs/voices/client.py
--rw-r--r--   0        0        0     9958 1970-01-01 00:00:00.000000 elevenlabs-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/LICENSE
+-rw-r--r--   0        0        0     9356 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/README.md
+-rw-r--r--   0        0        0      659 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4689 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/audio_native/__init__.py
+-rw-r--r--   0        0        0    13565 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/audio_native/client.py
+-rw-r--r--   0        0        0     7523 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/base_client.py
+-rw-r--r--   0        0        0       65 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/chapters/__init__.py
+-rw-r--r--   0        0        0    34318 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/chapters/client.py
+-rw-r--r--   0        0        0    20882 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/client.py
+-rw-r--r--   0        0        0      790 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/api_error.py
+-rw-r--r--   0        0        0     1683 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/dubbing/__init__.py
+-rw-r--r--   0        0        0    27796 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/dubbing/client.py
+-rw-r--r--   0        0        0      164 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/environment.py
+-rw-r--r--   0        0        0      170 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/history/__init__.py
+-rw-r--r--   0        0        0    27725 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/history/client.py
+-rw-r--r--   0        0        0       65 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/models/__init__.py
+-rw-r--r--   0        0        0     5069 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/models/client.py
+-rw-r--r--   0        0        0     2715 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/play.py
+-rw-r--r--   0        0        0       65 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/projects/__init__.py
+-rw-r--r--   0        0        0    54697 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/projects/client.py
+-rw-r--r--   0        0        0       65 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/pronunciation_dictionary/__init__.py
+-rw-r--r--   0        0        0    13080 2024-04-03 11:22:47.979294 elevenlabs-1.0.4/src/elevenlabs/pronunciation_dictionary/client.py
+-rw-r--r--   0        0        0        0 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/py.typed
+-rw-r--r--   0        0        0     5093 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/realtime_tts.py
+-rw-r--r--   0        0        0       65 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/samples/__init__.py
+-rw-r--r--   0        0        0    11145 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/samples/client.py
+-rw-r--r--   0        0        0       65 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/speech_to_speech/__init__.py
+-rw-r--r--   0        0        0    20960 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/speech_to_speech/client.py
+-rw-r--r--   0        0        0       65 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/text_to_speech/__init__.py
+-rw-r--r--   0        0        0    23081 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/text_to_speech/client.py
+-rw-r--r--   0        0        0     6114 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/accent.py
+-rw-r--r--   0        0        0      978 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/add_project_response_model.py
+-rw-r--r--   0        0        0     1058 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py
+-rw-r--r--   0        0        0      919 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/add_voice_response_model.py
+-rw-r--r--   0        0        0      161 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/age.py
+-rw-r--r--   0        0        0      980 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/audio_native_create_project_response_model.py
+-rw-r--r--   0        0        0      130 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/audio_native_get_embed_code_response_model.py
+-rw-r--r--   0        0        0     1560 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/audio_output.py
+-rw-r--r--   0        0        0     1196 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/chapter_response.py
+-rw-r--r--   0        0        0     1011 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/chapter_snapshot_response.py
+-rw-r--r--   0        0        0     1019 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/chapter_snapshots_response.py
+-rw-r--r--   0        0        0      164 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/chapter_state.py
+-rw-r--r--   0        0        0     1029 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/chapter_statistics_response.py
+-rw-r--r--   0        0        0      149 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/currency.py
+-rw-r--r--   0        0        0      950 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/do_dubbing_response.py
+-rw-r--r--   0        0        0      214 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/extended_subscription_response_model_billing_period.py
+-rw-r--r--   0        0        0     1082 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/feedback_item.py
+-rw-r--r--   0        0        0     1837 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/fine_tuning_response.py
+-rw-r--r--   0        0        0      223 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/finetuning_state.py
+-rw-r--r--   0        0        0      151 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/gender.py
+-rw-r--r--   0        0        0     2288 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/generation_config.py
+-rw-r--r--   0        0        0      988 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/get_chapters_response.py
+-rw-r--r--   0        0        0     1048 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/get_library_voices_response.py
+-rw-r--r--   0        0        0      988 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/get_projects_response.py
+-rw-r--r--   0        0        0     1041 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py
+-rw-r--r--   0        0        0     1073 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/get_speech_history_response.py
+-rw-r--r--   0        0        0      953 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/get_voices_response.py
+-rw-r--r--   0        0        0      101 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/history.py
+-rw-r--r--   0        0        0      992 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/history_item.py
+-rw-r--r--   0        0        0     1010 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/http_validation_error.py
+-rw-r--r--   0        0        0      948 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/invoice.py
+-rw-r--r--   0        0        0      931 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/language_response.py
+-rw-r--r--   0        0        0     1639 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/library_voice_response.py
+-rw-r--r--   0        0        0     1011 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/manual_verification_file_response.py
+-rw-r--r--   0        0        0     1086 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/manual_verification_response.py
+-rw-r--r--   0        0        0     1671 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/model.py
+-rw-r--r--   0        0        0     2207 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/normalized_alignment.py
+-rw-r--r--   0        0        0      176 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/optimize_streaming_latency.py
+-rw-r--r--   0        0        0      408 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/output_format.py
+-rw-r--r--   0        0        0     1278 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/project_extended_response_model.py
+-rw-r--r--   0        0        0     1259 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/project_response.py
+-rw-r--r--   0        0        0      991 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/project_snapshot_response.py
+-rw-r--r--   0        0        0     1019 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/project_snapshots_response.py
+-rw-r--r--   0        0        0      164 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/project_state.py
+-rw-r--r--   0        0        0      974 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/pronunciation_dictionary_version_locator.py
+-rw-r--r--   0        0        0     1477 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/realtime_voice_settings.py
+-rw-r--r--   0        0        0     1007 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/recording_response.py
+-rw-r--r--   0        0        0      220 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/review_status.py
+-rw-r--r--   0        0        0     2353 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/send_text.py
+-rw-r--r--   0        0        0      147 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/source.py
+-rw-r--r--   0        0        0     1865 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/speech_history_item_response.py
+-rw-r--r--   0        0        0      226 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/speech_history_item_response_model_voice_category.py
+-rw-r--r--   0        0        0     1079 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/sso_provider_db_model.py
+-rw-r--r--   0        0        0      173 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/sso_provider_db_model_provider_type.py
+-rw-r--r--   0        0        0     1879 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/subscription.py
+-rw-r--r--   0        0        0     1611 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/subscription_response.py
+-rw-r--r--   0        0        0      200 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/subscription_response_model_billing_period.py
+-rw-r--r--   0        0        0      256 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/subscription_status.py
+-rw-r--r--   0        0        0     1141 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/user.py
+-rw-r--r--   0        0        0     1029 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1120 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/verification_attempt_response.py
+-rw-r--r--   0        0        0     1991 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice.py
+-rw-r--r--   0        0        0      946 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_generation_parameter_option_response.py
+-rw-r--r--   0        0        0     1325 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_generation_parameter_response.py
+-rw-r--r--   0        0        0      216 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_response_model_safety_control.py
+-rw-r--r--   0        0        0     1102 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_sample.py
+-rw-r--r--   0        0        0     1083 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_settings.py
+-rw-r--r--   0        0        0     2354 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_sharing_response.py
+-rw-r--r--   0        0        0      196 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_sharing_state.py
+-rw-r--r--   0        0        0     1245 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/types/voice_verification_response.py
+-rw-r--r--   0        0        0       65 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/user/__init__.py
+-rw-r--r--   0        0        0     9207 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/user/client.py
+-rw-r--r--   0        0        0       78 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/version.py
+-rw-r--r--   0        0        0       65 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/voice_generation/__init__.py
+-rw-r--r--   0        0        0    20238 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/voice_generation/client.py
+-rw-r--r--   0        0        0       65 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/voices/__init__.py
+-rw-r--r--   0        0        0    58857 2024-04-03 11:22:47.983294 elevenlabs-1.0.4/src/elevenlabs/voices/client.py
+-rw-r--r--   0        0        0     9948 1970-01-01 00:00:00.000000 elevenlabs-1.0.4/PKG-INFO
```

### Comparing `elevenlabs-1.0.3/LICENSE` & `elevenlabs-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/README.md` & `elevenlabs-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ## 📖 API & Docs
 
 Check out the [HTTP API documentation](https://elevenlabs.io/docs/api-reference).
 
 ## ⚙️ Install
 
 ```bash
-pip install elevenlabs==v1.0.0b1
+pip install elevenlabs
 ```
 
 ## v0.x to v1.x Migration Guide
 > The SDK was rewritten in v1 and is now programatically generated from our OpenAPI spec. As part of this release 
 > there are some breaking changes.
```

### Comparing `elevenlabs-1.0.3/src/elevenlabs/__init__.py` & `elevenlabs-1.0.4/src/elevenlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/audio_native/client.py` & `elevenlabs-1.0.4/src/elevenlabs/audio_native/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/base_client.py` & `elevenlabs-1.0.4/src/elevenlabs/base_client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/chapters/client.py` & `elevenlabs-1.0.4/src/elevenlabs/chapters/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/client.py` & `elevenlabs-1.0.4/src/elevenlabs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
       optimize_streaming_latency: typing.Optional[int] = 0,
       stream: bool = False,
       output_format: Optional[str] = "mp3_44100_128",
       pronunciation_dictionary_locators: typing.Optional[
             typing.Sequence[PronunciationDictionaryVersionLocator]
         ] = OMIT,
       request_options: typing.Optional[RequestOptions] = None
-    ) -> Union[bytes, Iterator[bytes]]:
+    ) -> Iterator[bytes]:
         """
             - text: Union[str, Iterator[str]]. The string or stream of strings that will get converted into speech.
 
             - voice: str. A voice id, name, or voice response. Defaults to the Rachel voice. 
 
             - model: typing.Optional[str]. Identifier of the model that will be used, you can query them using GET /v1/models. 
                                            The model needs to have support for text to speech, you can check this using the 
@@ -179,15 +179,15 @@
             voices_response = self.voices.get_all(request_options=request_options)
             maybe_voice_id = next((v.voice_id for v in voices_response.voices if v.name == voice), None)
             if maybe_voice_id is None:
                 raise ApiError(body=f"Voice {voice} not found.")
             voice_id = maybe_voice_id
         elif isinstance(voice, Voice):
             voice_id = voice.voice_id
-            if voice_settings != DEFAULT_VOICE.settings \
+            if voice_settings == DEFAULT_VOICE.settings \
                     and voice.settings is not None:
                 voice_settings = voice.settings
         else:
             voice_id = DEFAULT_VOICE.voice_id
 
         if isinstance(model, str):
             model_id = model
@@ -304,15 +304,15 @@
       optimize_streaming_latency: typing.Optional[int] = 0,
       stream: bool = False,
       output_format: Optional[str] = "mp3_44100_128",
       pronunciation_dictionary_locators: typing.Optional[
             typing.Sequence[PronunciationDictionaryVersionLocator]
         ] = OMIT,
       request_options: typing.Optional[RequestOptions] = None
-    ) -> Union[bytes, AsyncIterator[bytes]]:
+    ) -> AsyncIterator[bytes]:
         """
           This is a manually mnaintained helper function that generates a 
           voice from provided text.
 
           **NOTE**: This function is a helper function and is simply making 
           calls to the `text_to_speech.convert` and`text_to_speech.convert_as_stream`
           functions.
@@ -365,15 +365,15 @@
             voices_response = await self.voices.get_all(request_options=request_options)
             maybe_voice_id = next((v.voice_id for v in voices_response.voices if v.name == voice), None)
             if not maybe_voice_id:
                 raise ApiError(body=f"Voice {voice} not found.")
             voice_id = maybe_voice_id
         elif isinstance(voice, Voice):
             voice_id = voice.voice_id
-            if voice_settings != DEFAULT_VOICE.settings \
+            if voice_settings == DEFAULT_VOICE.settings \
                     and voice.settings is not None:
                 voice_settings = voice.settings
         else:
             voice_id = DEFAULT_VOICE.voice_id
 
         if isinstance(model, str):
             model_id = model
```

### Comparing `elevenlabs-1.0.3/src/elevenlabs/core/__init__.py` & `elevenlabs-1.0.4/src/elevenlabs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/core/client_wrapper.py` & `elevenlabs-1.0.4/src/elevenlabs/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "elevenlabs",
-            "X-Fern-SDK-Version": "v1.0.3",
+            "X-Fern-SDK-Version": "v1.0.4",
         }
         if self._api_key is not None:
             headers["xi-api-key"] = self._api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `elevenlabs-1.0.3/src/elevenlabs/core/datetime_utils.py` & `elevenlabs-1.0.4/src/elevenlabs/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/core/file.py` & `elevenlabs-1.0.4/src/elevenlabs/core/file.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/core/http_client.py` & `elevenlabs-1.0.4/src/elevenlabs/core/http_client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/core/jsonable_encoder.py` & `elevenlabs-1.0.4/src/elevenlabs/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/core/request_options.py` & `elevenlabs-1.0.4/src/elevenlabs/core/request_options.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/dubbing/client.py` & `elevenlabs-1.0.4/src/elevenlabs/dubbing/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/history/client.py` & `elevenlabs-1.0.4/src/elevenlabs/history/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/models/client.py` & `elevenlabs-1.0.4/src/elevenlabs/models/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/play.py` & `elevenlabs-1.0.4/src/elevenlabs/play.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/projects/client.py` & `elevenlabs-1.0.4/src/elevenlabs/projects/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/pronunciation_dictionary/client.py` & `elevenlabs-1.0.4/src/elevenlabs/pronunciation_dictionary/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/realtime_tts.py` & `elevenlabs-1.0.4/src/elevenlabs/realtime_tts.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/samples/client.py` & `elevenlabs-1.0.4/src/elevenlabs/samples/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/speech_to_speech/client.py` & `elevenlabs-1.0.4/src/elevenlabs/speech_to_speech/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/text_to_speech/client.py` & `elevenlabs-1.0.4/src/elevenlabs/text_to_speech/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
         _request: typing.Dict[str, typing.Any] = {"text": text}
         if model_id is not OMIT:
             _request["model_id"] = model_id
         if voice_settings is not OMIT:
             _request["voice_settings"] = voice_settings
         if pronunciation_dictionary_locators is not OMIT:
             _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
-        async with await self._client_wrapper.httpx_client.stream(
+        async with self._client_wrapper.httpx_client.stream(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -438,15 +438,15 @@
         _request: typing.Dict[str, typing.Any] = {"text": text}
         if model_id is not OMIT:
             _request["model_id"] = model_id
         if voice_settings is not OMIT:
             _request["voice_settings"] = voice_settings
         if pronunciation_dictionary_locators is not OMIT:
             _request["pronunciation_dictionary_locators"] = pronunciation_dictionary_locators
-        async with await self._client_wrapper.httpx_client.stream(
+        async with self._client_wrapper.httpx_client.stream(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v1/text-to-speech/{jsonable_encoder(voice_id)}/stream"
             ),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
```

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/__init__.py` & `elevenlabs-1.0.4/src/elevenlabs/types/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/add_project_response_model.py` & `elevenlabs-1.0.4/src/elevenlabs/types/add_project_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py` & `elevenlabs-1.0.4/src/elevenlabs/types/add_pronunciation_dictionary_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/add_voice_response_model.py` & `elevenlabs-1.0.4/src/elevenlabs/types/add_voice_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/audio_native_create_project_response_model.py` & `elevenlabs-1.0.4/src/elevenlabs/types/audio_native_create_project_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/audio_output.py` & `elevenlabs-1.0.4/src/elevenlabs/types/audio_output.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/chapter_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/chapter_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/chapter_snapshot_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/chapter_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/chapter_snapshots_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/chapter_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/chapter_statistics_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/chapter_statistics_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/do_dubbing_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/do_dubbing_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/feedback_item.py` & `elevenlabs-1.0.4/src/elevenlabs/types/feedback_item.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/fine_tuning_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/fine_tuning_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/generation_config.py` & `elevenlabs-1.0.4/src/elevenlabs/types/generation_config.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/get_chapters_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/get_chapters_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/get_library_voices_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/get_library_voices_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/get_projects_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/get_projects_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/get_pronunciation_dictionary_metadata_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/get_speech_history_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/get_speech_history_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/get_voices_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/get_voices_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/history_item.py` & `elevenlabs-1.0.4/src/elevenlabs/types/history_item.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/http_validation_error.py` & `elevenlabs-1.0.4/src/elevenlabs/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/invoice.py` & `elevenlabs-1.0.4/src/elevenlabs/types/invoice.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/language_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/language_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/library_voice_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/library_voice_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/manual_verification_file_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/manual_verification_file_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/manual_verification_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/manual_verification_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/model.py` & `elevenlabs-1.0.4/src/elevenlabs/types/model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/normalized_alignment.py` & `elevenlabs-1.0.4/src/elevenlabs/types/normalized_alignment.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/project_extended_response_model.py` & `elevenlabs-1.0.4/src/elevenlabs/types/project_extended_response_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/project_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/project_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/project_snapshot_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/project_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/project_snapshots_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/project_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/pronunciation_dictionary_version_locator.py` & `elevenlabs-1.0.4/src/elevenlabs/types/pronunciation_dictionary_version_locator.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/realtime_voice_settings.py` & `elevenlabs-1.0.4/src/elevenlabs/types/realtime_voice_settings.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/recording_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/recording_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/send_text.py` & `elevenlabs-1.0.4/src/elevenlabs/types/send_text.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/speech_history_item_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/speech_history_item_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/sso_provider_db_model.py` & `elevenlabs-1.0.4/src/elevenlabs/types/sso_provider_db_model.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/subscription.py` & `elevenlabs-1.0.4/src/elevenlabs/types/subscription.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/subscription_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/subscription_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/user.py` & `elevenlabs-1.0.4/src/elevenlabs/types/user.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/validation_error.py` & `elevenlabs-1.0.4/src/elevenlabs/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/verification_attempt_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/verification_attempt_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/voice.py` & `elevenlabs-1.0.4/src/elevenlabs/types/voice.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/voice_generation_parameter_option_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/voice_generation_parameter_option_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/voice_generation_parameter_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/voice_generation_parameter_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/voice_sample.py` & `elevenlabs-1.0.4/src/elevenlabs/types/voice_sample.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/voice_settings.py` & `elevenlabs-1.0.4/src/elevenlabs/types/voice_settings.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/voice_sharing_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/voice_sharing_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/types/voice_verification_response.py` & `elevenlabs-1.0.4/src/elevenlabs/types/voice_verification_response.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/user/client.py` & `elevenlabs-1.0.4/src/elevenlabs/user/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/voice_generation/client.py` & `elevenlabs-1.0.4/src/elevenlabs/voice_generation/client.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-1.0.3/src/elevenlabs/voices/client.py` & `elevenlabs-1.0.4/src/elevenlabs/voices/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -549,15 +549,15 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_voices(
+    def get_shared(
         self,
         *,
         page_size: typing.Optional[int] = None,
         category: typing.Optional[str] = None,
         gender: typing.Optional[str] = None,
         age: typing.Optional[str] = None,
         accent: typing.Optional[str] = None,
@@ -598,15 +598,15 @@
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from elevenlabs.client import ElevenLabs
 
         client = ElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        client.voices.get_voices()
+        client.voices.get_shared()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/shared-voices"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -1178,15 +1178,15 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_voices(
+    async def get_shared(
         self,
         *,
         page_size: typing.Optional[int] = None,
         category: typing.Optional[str] = None,
         gender: typing.Optional[str] = None,
         age: typing.Optional[str] = None,
         accent: typing.Optional[str] = None,
@@ -1227,15 +1227,15 @@
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from elevenlabs.client import AsyncElevenLabs
 
         client = AsyncElevenLabs(
             api_key="YOUR_API_KEY",
         )
-        await client.voices.get_voices()
+        await client.voices.get_shared()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/shared-voices"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
```

### Comparing `elevenlabs-1.0.3/PKG-INFO` & `elevenlabs-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -31,15 +31,15 @@
 ## 📖 API & Docs
 
 Check out the [HTTP API documentation](https://elevenlabs.io/docs/api-reference).
 
 ## ⚙️ Install
 
 ```bash
-pip install elevenlabs==v1.0.0b1
+pip install elevenlabs
 ```
 
 ## v0.x to v1.x Migration Guide
 > The SDK was rewritten in v1 and is now programatically generated from our OpenAPI spec. As part of this release 
 > there are some breaking changes.
```

