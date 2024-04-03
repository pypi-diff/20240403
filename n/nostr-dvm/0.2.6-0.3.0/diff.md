# Comparing `tmp/nostr-dvm-0.2.6.tar.gz` & `tmp/nostr-dvm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostr-dvm-0.2.6.tar", last modified: Mon Mar  4 14:44:28 2024, max compression
+gzip compressed data, was "nostr-dvm-0.3.0.tar", last modified: Fri Mar 22 16:08:21 2024, max compression
```

## Comparing `nostr-dvm-0.2.6.tar` & `nostr-dvm-0.3.0.tar`

### file list

```diff
@@ -1,107 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.684015 nostr-dvm-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-04 14:44:28.684015 nostr-dvm-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.668015 nostr-dvm-0.2.6/nostr_dvm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.668015 nostr-dvm-0.2.6/nostr_dvm/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.668015 nostr-dvm-0.2.6/nostr_dvm/backends/mlx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/mlx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.668015 nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.668015 nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.668015 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.672015 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.672015 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/image_interrogator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.672015 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/image_upscale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.672015 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.672015 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/whisperx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/whisperx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    35304 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    32338 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/dvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.672015 nostr-dvm-0.2.6/nostr_dvm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/interfaces/dvmtaskinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.680015 nostr-dvm-0.2.6/nostr_dvm/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/advanced_search_wine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/convert_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/discovery_inactive_follows.py
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/discovery_nonfollowers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/imagegeneration_openai_dalle.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/imagegeneration_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/imageinterrogator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/imageupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/search_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/summarization_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/textextraction_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/textextraction_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/textextraction_whisperx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/textgeneration_huggingchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/textgeneration_llmlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/textgeneration_unleashed_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/texttospeech.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/translation_google.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/translation_libretranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/trending_notes_nostrband.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/videogeneration_replicate_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/tasks/videogeneration_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.680015 nostr-dvm-0.2.6/nostr_dvm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/cashu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/dvmconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/external_dvm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/mediasource_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/nip89_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/nostr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/nwc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/output_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.680015 nostr-dvm-0.2.6/nostr_dvm/utils/scrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/scrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/scrapper/media_scrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    14413 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/nostr_dvm/utils/zap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.680015 nostr-dvm-0.2.6/nostr_dvm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-04 14:44:28.000000 nostr-dvm-0.2.6/nostr_dvm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-03-04 14:44:28.000000 nostr-dvm-0.2.6/nostr_dvm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 14:44:28.000000 nostr-dvm-0.2.6/nostr_dvm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-04 14:44:28.000000 nostr-dvm-0.2.6/nostr_dvm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-04 14:44:28.000000 nostr-dvm-0.2.6/nostr_dvm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 14:44:28.684015 nostr-dvm-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:44:28.680015 nostr-dvm-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/tests/test_dvm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-03-04 14:44:23.000000 nostr-dvm-0.2.6/tests/test_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.466750 nostr-dvm-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-22 16:08:21.466750 nostr-dvm-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.450750 nostr-dvm-0.3.0/nostr_dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.450750 nostr-dvm-0.3.0/nostr_dvm/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.450750 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.450750 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.450750 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13685 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.454750 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.454750 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.454750 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_interrogator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_interrogator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_interrogator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.454750 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_upscale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.454750 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.454750 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/whisperx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/whisperx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/whisperx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36516 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39271 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/dvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.454750 nostr-dvm-0.3.0/nostr_dvm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/interfaces/dvmtaskinterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16345 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.458751 nostr-dvm-0.3.0/nostr_dvm/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/advanced_search_wine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/content_discovery_currently_popular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/convert_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/discovery_inactive_follows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/discovery_nonfollowers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/discovery_relevant_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/discovery_trending_notes_nostrband.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_openai_dalle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_sd21_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/imageinterrogator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/imageupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/search_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/summarization_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/summarization_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/textextraction_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/textextraction_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/textextraction_whisperx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/textgeneration_huggingchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/textgeneration_llmlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/textgeneration_unleashed_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/texttospeech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/translation_google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/translation_libretranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/videogeneration_replicate_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/tasks/videogeneration_svd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.462751 nostr-dvm-0.3.0/nostr_dvm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/cashu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/dvmconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/external_dvm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13403 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/mediasource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/nip88_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/nip89_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/nostr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/nwc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/output_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.462751 nostr-dvm-0.3.0/nostr_dvm/utils/scrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/scrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26119 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/scrapper/media_scrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/subscription_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/nostr_dvm/utils/zap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.462751 nostr-dvm-0.3.0/nostr_dvm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-22 16:08:21.000000 nostr-dvm-0.3.0/nostr_dvm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-22 16:08:21.000000 nostr-dvm-0.3.0/nostr_dvm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 16:08:21.000000 nostr-dvm-0.3.0/nostr_dvm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-22 16:08:21.000000 nostr-dvm-0.3.0/nostr_dvm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-22 16:08:21.000000 nostr-dvm-0.3.0/nostr_dvm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 16:08:21.466750 nostr-dvm-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:08:21.462751 nostr-dvm-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/tests/test_dvm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-03-22 16:08:13.000000 nostr-dvm-0.3.0/tests/test_events.py
```

### Comparing `nostr-dvm-0.2.6/LICENSE` & `nostr-dvm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/PKG-INFO` & `nostr-dvm-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.2.6
+Version: 0.3.0
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
-Requires-Dist: nostr-sdk==0.9.1
+Requires-Dist: nostr-sdk==0.10.0
 Requires-Dist: bech32
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: emoji==2.8.0
 Requires-Dist: eva-decord==0.6.1
 Requires-Dist: ffmpegio==0.8.5
 Requires-Dist: lnurl
```

### Comparing `nostr-dvm-0.2.6/README.md` & `nostr-dvm-0.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# NostrAI: Nostr NIP90 Data Vending Machine Framework
+# NostrDVM: Nostr NIP90 Data Vending Machine Framework
 
 This framework provides a way to easily build and/or run `Nostr NIP90 DVMs in Python`.
 
 This project is currently under development and additional tasks and features are added along the way. 
 This means the project is in alpha status, interfaces might still change/break at this stage.
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/clip.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/model_io.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/sampler.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/mlx/modules/stable_diffusion/vae.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_interrogator/image_interrogator.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_upscale/image_upscale_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/image_upscale/inference_realesrgan.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/lora.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl-img2img.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/stablediffusionxl/stablediffusionxl.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/backends/nova_server/utils.py` & `nostr-dvm-0.3.0/nostr_dvm/backends/nova_server/utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/bot.py` & `nostr-dvm-0.3.0/nostr_dvm/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import os
 import signal
 import time
 from datetime import timedelta
 
 from nostr_sdk import (Keys, Client, Timestamp, Filter, nip04_decrypt, HandleNotification, EventBuilder, PublicKey,
-                       Options, Tag, Event, nip04_encrypt, NostrSigner, EventId, Nip19Event)
+                       Options, Tag, Event, nip04_encrypt, NostrSigner, EventId, Nip19Event, Kind, KindEnum,
+                       UnsignedEvent, nip59_extract_rumor)
 
 from nostr_dvm.utils.admin_utils import admin_make_database_updates
 from nostr_dvm.utils.database_utils import get_or_add_user, update_user_balance, create_sql_table, update_sql_table
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.nip89_utils import nip89_fetch_events_pubkey, NIP89Config
 from nostr_dvm.utils.nostr_utils import send_event
 from nostr_dvm.utils.output_utils import PostProcessFunctionType, post_process_list_to_users, \
@@ -51,38 +52,56 @@
         self.client.connect()
 
         zap_filter = Filter().pubkey(pk).kinds([EventDefinitions.KIND_ZAP]).since(Timestamp.now())
         dm_filter = Filter().pubkey(pk).kinds([EventDefinitions.KIND_DM]).since(Timestamp.now())
         kinds = [EventDefinitions.KIND_NIP90_GENERIC, EventDefinitions.KIND_FEEDBACK]
         for dvm in self.dvm_config.SUPPORTED_DVMS:
             if dvm.KIND not in kinds:
-                kinds.append(dvm.KIND + 1000)
+                kinds.append(Kind(dvm.KIND.as_u64() + 1000))
         dvm_filter = (Filter().kinds(kinds).since(Timestamp.now()))
 
-        self.client.subscribe([zap_filter, dm_filter, dvm_filter])
+        self.client.subscribe([zap_filter, dm_filter, dvm_filter], None)
 
         create_sql_table(self.dvm_config.DB)
         admin_make_database_updates(adminconfig=self.admin_config, dvmconfig=self.dvm_config, client=self.client)
+        # add_sql_table_column(dvm_config.DB)
 
         class NotificationHandler(HandleNotification):
             client = self.client
             dvm_config = self.dvm_config
             keys = self.keys
 
-            def handle(self, relay_url, nostr_event):
-                if (EventDefinitions.KIND_NIP90_EXTRACT_TEXT + 1000 <= nostr_event.kind()
-                        <= EventDefinitions.KIND_NIP90_GENERIC + 1000):
+            def handle(self, relay_url, subscription_id, nostr_event):
+                if (EventDefinitions.KIND_NIP90_EXTRACT_TEXT.as_u64() + 1000 <= nostr_event.kind().as_u64()
+                        <= EventDefinitions.KIND_NIP90_GENERIC.as_u64() + 1000):
                     handle_nip90_response_event(nostr_event)
-                elif nostr_event.kind() == EventDefinitions.KIND_FEEDBACK:
+                elif nostr_event.kind().as_u64() == EventDefinitions.KIND_FEEDBACK.as_u64():
                     handle_nip90_feedback(nostr_event)
-                elif nostr_event.kind() == EventDefinitions.KIND_DM:
-                    handle_dm(nostr_event)
-                elif nostr_event.kind() == EventDefinitions.KIND_ZAP:
+
+                elif nostr_event.kind().as_u64() == EventDefinitions.KIND_ZAP.as_u64():
                     handle_zap(nostr_event)
 
+                elif nostr_event.kind().match_enum(KindEnum.ENCRYPTED_DIRECT_MESSAGE()):
+                    try:
+                        handle_dm(nostr_event)
+                    except Exception as e:
+                        print(f"Error during content NIP04 decryption: {e}")
+                elif nostr_event.kind().match_enum(KindEnum.GIFT_WRAP()):
+                    print("Decrypting NIP59 event")
+                    try:
+                        rumor: UnsignedEvent = nip59_extract_rumor(self.keys, nostr_event)
+                        if rumor.kind().match_enum(KindEnum.SEALED_DIRECT()):
+                            msg = rumor.content()
+                            print(f"Received new msg [sealed]: {msg}")
+                            self.client.send_sealed_msg(rumor.author(), "Nip44 is not supported yet, but coming soon", None)
+                        else:
+                            print(f"{rumor.as_json()}")
+                    except Exception as e:
+                        print(f"Error during content NIP59 decryption: {e}")
+
             def handle_msg(self, relay_url, msg):
                 return
 
         def handle_dm(nostr_event):
             sender = nostr_event.author().to_hex()
             if sender == self.keys.public_key().to_hex():
                 return
@@ -186,15 +205,15 @@
                     # Build an overview of known DVMs and send it to the user
                     answer_overview(nostr_event)
 
             except Exception as e:
                 print("Error in bot " + str(e))
 
         def handle_nip90_feedback(nostr_event):
-            print(nostr_event.as_json())
+            #print(nostr_event.as_json())
             try:
                 is_encrypted = False
                 status = ""
                 etag = ""
                 ptag = ""
                 content = nostr_event.content()
                 for tag in nostr_event.tags():
@@ -261,15 +280,15 @@
                                 user = get_or_add_user(db=self.dvm_config.DB, npub=entry["npub"],
                                                        client=self.client, config=self.dvm_config)
                                 if user.balance >= amount:
                                     balance = max(user.balance - amount, 0)
                                     update_sql_table(db=self.dvm_config.DB, npub=user.npub, balance=balance,
                                                      iswhitelisted=user.iswhitelisted, isblacklisted=user.isblacklisted,
                                                      nip05=user.nip05, lud16=user.lud16, name=user.name,
-                                                     lastactive=Timestamp.now().as_secs())
+                                                     lastactive=Timestamp.now().as_secs(), subscribed=user.subscribed)
                                     evt = EventBuilder.encrypted_direct_msg(self.keys,
                                                                                 PublicKey.from_hex(entry["npub"]),
                                                                                 "Paid " + str(
                                                                                     amount) + " Sats from balance to DVM. New balance is " +
                                                                                 str(balance)
                                                                                 + " Sats.\n",
                                                                                 None).to_event(self.keys)
@@ -342,15 +361,15 @@
                     if is_encrypted:
                         if ptag == self.keys.public_key().to_hex():
                             content = nip04_decrypt(self.keys.secret_key(), nostr_event.author(), content)
                         else:
                             return
 
                     dvms = [x for x in self.dvm_config.SUPPORTED_DVMS if
-                            x.PUBLIC_KEY == nostr_event.author().to_hex() and x.KIND == nostr_event.kind() - 1000]
+                            x.PUBLIC_KEY == nostr_event.author().to_hex() and x.KIND.as_u64() == nostr_event.kind().as_u64() - 1000]
                     if len(dvms) > 0:
                         dvm = dvms[0]
                         if dvm.dvm_config.EXTERNAL_POST_PROCESS_TYPE != PostProcessFunctionType.NONE:
                             if dvm.dvm_config.EXTERNAL_POST_PROCESS_TYPE == PostProcessFunctionType.LIST_TO_EVENTS:
                                 content = post_process_list_to_events(content)
                             elif dvm.dvm_config.EXTERNAL_POST_PROCESS_TYPE == PostProcessFunctionType.LIST_TO_USERS:
                                 content = post_process_list_to_users(content)
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/dvm.py` & `nostr-dvm-0.3.0/nostr_dvm/dvm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import json
 import os
 import subprocess
 from datetime import timedelta
 from sys import platform
 
 from nostr_sdk import PublicKey, Keys, Client, Tag, Event, EventBuilder, Filter, HandleNotification, Timestamp, \
-    init_logger, LogLevel, Options, nip04_encrypt, NostrSigner
+    init_logger, LogLevel, Options, nip04_encrypt, NostrSigner, Kind, SubscribeAutoCloseOptions
 
 import time
 
 from nostr_dvm.utils.definitions import EventDefinitions, RequiredJobToWatch, JobToWatch
 from nostr_dvm.utils.dvmconfig import DVMConfig
 from nostr_dvm.utils.admin_utils import admin_make_database_updates, AdminConfig
 from nostr_dvm.utils.backend_utils import get_amount_per_task, check_task_is_supported, get_task
-from nostr_dvm.utils.database_utils import create_sql_table, get_or_add_user, update_user_balance, update_sql_table
+from nostr_dvm.utils.database_utils import create_sql_table, get_or_add_user, update_user_balance, update_sql_table, \
+    update_user_subscription
 from nostr_dvm.utils.mediasource_utils import input_data_file_duration
+from nostr_dvm.utils.nip88_utils import nip88_has_active_subscription
 from nostr_dvm.utils.nostr_utils import get_event_by_id, get_referenced_event_by_id, send_event, check_and_decrypt_tags
 from nostr_dvm.utils.output_utils import build_status_reaction
 from nostr_dvm.utils.zap_utils import check_bolt11_ln_bits_is_paid, create_bolt11_ln_bits, parse_zap_event_tags, \
     parse_amount_from_bolt11_invoice, zaprequest, pay_bolt11_ln_bits, create_bolt11_lud16
 from nostr_dvm.utils.cashu_utils import redeem_cashu
 
 
@@ -30,235 +32,325 @@
     job_list: list
     jobs_on_hold_list: list
 
     def __init__(self, dvm_config, admin_config=None):
         self.dvm_config = dvm_config
         self.admin_config = admin_config
         self.keys = Keys.parse(dvm_config.PRIVATE_KEY)
-        wait_for_send = True
+        wait_for_send = False
         skip_disconnected_relays = True
         opts = (Options().wait_for_send(wait_for_send).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
                 .skip_disconnected_relays(skip_disconnected_relays))
 
         signer = NostrSigner.keys(self.keys)
         self.client = Client.with_opts(signer, opts)
 
         self.job_list = []
         self.jobs_on_hold_list = []
         pk = self.keys.public_key()
 
-        print("Nostr DVM public key: " + str(pk.to_bech32()) + " Hex: " + str(pk.to_hex()) + " Supported DVM tasks: " +
-              ', '.join(p.NAME + ":" + p.TASK for p in self.dvm_config.SUPPORTED_DVMS) + "\n")
+        print("Nostr DVM public key: " + str(pk.to_bech32()) + " Hex: " + str(pk.to_hex()) + "\n")
 
         for relay in self.dvm_config.RELAY_LIST:
             self.client.add_relay(relay)
         self.client.connect()
 
         zap_filter = Filter().pubkey(pk).kinds([EventDefinitions.KIND_ZAP]).since(Timestamp.now())
         kinds = [EventDefinitions.KIND_NIP90_GENERIC]
         for dvm in self.dvm_config.SUPPORTED_DVMS:
             if dvm.KIND not in kinds:
                 kinds.append(dvm.KIND)
         dvm_filter = (Filter().kinds(kinds).since(Timestamp.now()))
-        self.client.subscribe([dvm_filter, zap_filter])
+
+        self.client.subscribe([dvm_filter, zap_filter], None)
 
         create_sql_table(self.dvm_config.DB)
         admin_make_database_updates(adminconfig=self.admin_config, dvmconfig=self.dvm_config, client=self.client)
 
         class NotificationHandler(HandleNotification):
             client = self.client
             dvm_config = self.dvm_config
             keys = self.keys
 
-            def handle(self, relay_url, nostr_event):
-                if EventDefinitions.KIND_NIP90_EXTRACT_TEXT <= nostr_event.kind() <= EventDefinitions.KIND_NIP90_GENERIC:
+            def handle(self, relay_url, subscription_id, nostr_event: Event):
+
+                if EventDefinitions.KIND_NIP90_EXTRACT_TEXT.as_u64() <= nostr_event.kind().as_u64() <= EventDefinitions.KIND_NIP90_GENERIC.as_u64():
                     handle_nip90_job_event(nostr_event)
-                elif nostr_event.kind() == EventDefinitions.KIND_ZAP:
+                elif nostr_event.kind().as_u64() == EventDefinitions.KIND_ZAP.as_u64():
                     handle_zap(nostr_event)
 
             def handle_msg(self, relay_url, msg):
                 return
 
         def handle_nip90_job_event(nip90_event):
-
+            # decrypted encrypted events
             nip90_event = check_and_decrypt_tags(nip90_event, self.dvm_config)
+            # if event is encrypted, but we can't decrypt it (e.g. because its directed to someone else), return
             if nip90_event is None:
                 return
-
-            user = get_or_add_user(self.dvm_config.DB, nip90_event.author().to_hex(), client=self.client,
-                                   config=self.dvm_config)
+            
+            task_is_free = False
+            user_has_active_subscription = False
             cashu = ""
             p_tag_str = ""
+
             for tag in nip90_event.tags():
                 if tag.as_vec()[0] == "cashu":
                     cashu = tag.as_vec()[1]
                 elif tag.as_vec()[0] == "p":
                     p_tag_str = tag.as_vec()[1]
 
+            if p_tag_str != "" and p_tag_str != self.dvm_config.PUBLIC_KEY:
+                print("[" + self.dvm_config.NIP89.NAME + "] No public request, also not addressed to me.")
+                return
+
+
+            # check if task is supported by the current DVM
             task_supported, task = check_task_is_supported(nip90_event, client=self.client,
                                                            config=self.dvm_config)
+            # if task is supported, continue, else do nothing.
+            if task_supported:
+                # fetch or add user contacting the DVM from/to local database
+                user = get_or_add_user(self.dvm_config.DB, nip90_event.author().to_hex(), client=self.client,
+                                       config=self.dvm_config, skip_meta=False)
+                # if user is blacklisted for some reason, send an error reaction and return
+                if user.isblacklisted:
+                    send_job_status_reaction(nip90_event, "error", client=self.client, dvm_config=self.dvm_config)
+                    print("[" + self.dvm_config.NIP89.NAME + "] Request by blacklisted user, skipped")
+                    return
 
-            if user.isblacklisted:
-                send_job_status_reaction(nip90_event, "error", client=self.client, dvm_config=self.dvm_config)
-                print("[" + self.dvm_config.NIP89.NAME + "] Request by blacklisted user, skipped")
-
-            elif task_supported:
                 print("[" + self.dvm_config.NIP89.NAME + "] Received new Request: " + task + " from " + user.name)
                 duration = input_data_file_duration(nip90_event, dvm_config=self.dvm_config, client=self.client)
                 amount = get_amount_per_task(task, self.dvm_config, duration)
                 if amount is None:
                     return
 
-                task_is_free = False
+
+                # If this is a subscription DVM and the Task is directed to us, check for active subscription
+                if dvm_config.NIP88 is not None and p_tag_str == self.dvm_config.PUBLIC_KEY:
+                    send_job_status_reaction(nip90_event, "subscription-required", True, amount, self.client,
+                                             "Checking Subscription Status, please wait..",self.dvm_config)
+                    # if we stored in the database that the user has an active subscription, we don't need to check it
+                    print("User Subscription: " + str(user.subscribed) + " Current time: " + str(
+                        Timestamp.now().as_secs()))
+                    # if we have an entry in the db that user is subscribed, continue
+                    if int(user.subscribed) > int(Timestamp.now().as_secs()):
+                        print("User subscribed until: " + str(Timestamp.from_secs(user.subscribed).to_human_datetime()))
+                        user_has_active_subscription = True
+                        send_job_status_reaction(nip90_event, "subscription-required", True, amount,
+                                                 self.client, "User subscripton active until " +
+                                                 Timestamp.from_secs(int(user.subscribed)).to_human_datetime().replace("Z", " ").replace("T", " ") + " GMT", self.dvm_config)
+                    # otherwise we check for an active subscription by checking recipie events
+                    else:
+                        print("[" + self.dvm_config.NIP89.NAME + "] Checking Subscription status")
+                        send_job_status_reaction(nip90_event, "subscription-required", True, amount, self.client,
+                                                 "I Don't have information about subscription status, checking on the Nostr. This might take a few seconds",
+                                                 self.dvm_config)
+
+                        subscription_status = nip88_has_active_subscription(PublicKey.parse(user.npub),
+                                                                            self.dvm_config.NIP88.DTAG, self.client,
+                                                                            self.dvm_config.PUBLIC_KEY)
+
+                        if subscription_status["isActive"]:
+                            send_job_status_reaction(nip90_event, "subscription-required", True, amount, self.client,
+                                                     "User subscripton active until " + Timestamp.from_secs(int(subscription_status["validUntil"])).to_human_datetime().replace("Z", " ").replace("T", " ") + " GMT",
+                                                     self.dvm_config)
+                            print("Checked Recipe: User subscribed until: " + str(
+                                Timestamp.from_secs(int(subscription_status["validUntil"])).to_human_datetime()))
+                            user_has_active_subscription = True
+                            update_user_subscription(user.npub,
+                                                     int(subscription_status["validUntil"]),
+                                                     self.client, self.dvm_config)
+                        else:
+                            print("No active subscription found")
+                            send_job_status_reaction(nip90_event, "subscription-required", True, amount, self.client,
+                                                     "No active subscription found..",
+                                                     self.dvm_config)
+
                 for dvm in self.dvm_config.SUPPORTED_DVMS:
-                    if dvm.TASK == task and dvm.FIX_COST == 0 and dvm.PER_UNIT_COST == 0:
+                    if dvm.TASK == task and dvm.FIX_COST == 0 and dvm.PER_UNIT_COST == 0 and dvm_config.NIP88 is None:
                         task_is_free = True
 
                 cashu_redeemed = False
                 if cashu != "":
                     print(cashu)
                     cashu_redeemed, cashu_message, redeem_amount, fees = redeem_cashu(cashu, self.dvm_config,
                                                                                       self.client, int(amount))
                     print(cashu_message)
                     if cashu_message != "success":
                         send_job_status_reaction(nip90_event, "error", False, amount, self.client, cashu_message,
                                                  self.dvm_config)
                         return
                 # if user is whitelisted or task is free, just do the job
-                if (user.iswhitelisted or task_is_free or cashu_redeemed) and (p_tag_str == "" or p_tag_str ==
-                                                                               self.dvm_config.PUBLIC_KEY):
+                if (user.iswhitelisted or task_is_free or cashu_redeemed) and (
+                        p_tag_str == "" or p_tag_str ==
+                        self.dvm_config.PUBLIC_KEY):
                     print(
                         "[" + self.dvm_config.NIP89.NAME + "] Free task or Whitelisted for task " + task +
                         ". Starting processing..")
 
                     if dvm_config.SEND_FEEDBACK_EVENTS:
                         send_job_status_reaction(nip90_event, "processing", True, 0,
-                                                 client=self.client, dvm_config=self.dvm_config)
+                                                 client=self.client, dvm_config=self.dvm_config, user=user)
 
                     #  when we reimburse users on error make sure to not send anything if it was free
                     if user.iswhitelisted or task_is_free:
                         amount = 0
                     do_work(nip90_event, amount)
-                # if task is directed to us via p tag and user has balance, do the job and update balance
-                elif p_tag_str == self.dvm_config.PUBLIC_KEY and user.balance >= int(amount):
-                    balance = max(user.balance - int(amount), 0)
-                    update_sql_table(db=self.dvm_config.DB, npub=user.npub, balance=balance,
-                                     iswhitelisted=user.iswhitelisted, isblacklisted=user.isblacklisted,
-                                     nip05=user.nip05, lud16=user.lud16, name=user.name,
-                                     lastactive=Timestamp.now().as_secs())
+                # if task is directed to us via p tag and user has balance or is subscribed, do the job and update balance
+                elif (p_tag_str == self.dvm_config.PUBLIC_KEY and (
+                        user.balance >= int(
+                    amount) and dvm_config.NIP88 is None) or (
+                              p_tag_str == self.dvm_config.PUBLIC_KEY and user_has_active_subscription)):
+
+                    if not user_has_active_subscription:
+                        balance = max(user.balance - int(amount), 0)
+                        update_sql_table(db=self.dvm_config.DB, npub=user.npub, balance=balance,
+                                         iswhitelisted=user.iswhitelisted, isblacklisted=user.isblacklisted,
+                                         nip05=user.nip05, lud16=user.lud16, name=user.name,
+                                         lastactive=Timestamp.now().as_secs(), subscribed=user.subscribed)
 
-                    print(
-                        "[" + self.dvm_config.NIP89.NAME + "] Using user's balance for task: " + task +
-                        ". Starting processing.. New balance is: " + str(balance))
+                        print(
+                            "[" + self.dvm_config.NIP89.NAME + "] Using user's balance for task: " + task +
+                            ". Starting processing.. New balance is: " + str(balance))
+                    else:
+                        print("[" + self.dvm_config.NIP89.NAME + "] User has active subscription for task: " + task +
+                              ". Starting processing.. Balance remains at: " + str(user.balance))
 
                     send_job_status_reaction(nip90_event, "processing", True, 0,
                                              client=self.client, dvm_config=self.dvm_config)
 
                     do_work(nip90_event, amount)
 
                 # else send a payment required event to user
                 elif p_tag_str == "" or p_tag_str == self.dvm_config.PUBLIC_KEY:
-                    bid = 0
-                    for tag in nip90_event.tags():
-                        if tag.as_vec()[0] == 'bid':
-                            bid = int(tag.as_vec()[1])
-
-                    print(
-                        "[" + self.dvm_config.NIP89.NAME + "] Payment required: New Nostr " + task + " Job event: "
-                        + nip90_event.as_json())
-                    if bid > 0:
-                        bid_offer = int(bid / 1000)
-                        if bid_offer >= int(amount):
-                            send_job_status_reaction(nip90_event, "payment-required", False,
-                                                     int(amount),  # bid_offer
-                                                     client=self.client, dvm_config=self.dvm_config)
 
-                    else:  # If there is no bid, just request server rate from user
+                    if dvm_config.NIP88 is not None:
                         print(
-                            "[" + self.dvm_config.NIP89.NAME + "]  Requesting payment for Event: " +
+                            "[" + self.dvm_config.NIP89.NAME + "]  Hinting user for Subscription: " +
                             nip90_event.id().to_hex())
-                        send_job_status_reaction(nip90_event, "payment-required",
-                                                 False, int(amount), client=self.client, dvm_config=self.dvm_config)
+                        send_job_status_reaction(nip90_event, "subscription-required",
+                                                 False, 0, client=self.client,
+                                                 dvm_config=self.dvm_config)
+                    else:
+                        bid = 0
+                        for tag in nip90_event.tags():
+                            if tag.as_vec()[0] == 'bid':
+                                bid = int(tag.as_vec()[1])
+
+                        print(
+                            "[" + self.dvm_config.NIP89.NAME + "] Payment required: New Nostr " + task + " Job event: "
+                            + nip90_event.as_json())
+                        if bid > 0:
+                            bid_offer = int(bid / 1000)
+                            if bid_offer >= int(amount):
+                                send_job_status_reaction(nip90_event, "payment-required", False,
+                                                         int(amount),  # bid_offer
+                                                         client=self.client, dvm_config=self.dvm_config)
+
+                        else:  # If there is no bid, just request server rate from user
+                            print(
+                                "[" + self.dvm_config.NIP89.NAME + "]  Requesting payment for Event: " +
+                                nip90_event.id().to_hex())
+                            send_job_status_reaction(nip90_event, "payment-required",
+                                                     False, int(amount), client=self.client, dvm_config=self.dvm_config)
+
+
+
+
                 else:
                     print("[" + self.dvm_config.NIP89.NAME + "] Job addressed to someone else, skipping..")
             # else:
             # print("[" + self.dvm_config.NIP89.NAME + "] Task " + task + " not supported on this DVM, skipping..")
 
         def handle_zap(zap_event):
             try:
                 invoice_amount, zapped_event, sender, message, anon = parse_zap_event_tags(zap_event,
                                                                                            self.keys,
                                                                                            self.dvm_config.NIP89.NAME,
                                                                                            self.client, self.dvm_config)
                 user = get_or_add_user(db=self.dvm_config.DB, npub=sender, client=self.client, config=self.dvm_config)
 
                 if zapped_event is not None:
-                    if zapped_event.kind() == EventDefinitions.KIND_FEEDBACK:
+                    if zapped_event.kind().as_u64() == EventDefinitions.KIND_FEEDBACK.as_u64():
 
                         amount = 0
                         job_event = None
                         p_tag_str = ""
+                        status = ""
                         for tag in zapped_event.tags():
                             if tag.as_vec()[0] == 'amount':
                                 amount = int(float(tag.as_vec()[1]) / 1000)
                             elif tag.as_vec()[0] == 'e':
                                 job_event = get_event_by_id(tag.as_vec()[1], client=self.client, config=self.dvm_config)
                                 if job_event is not None:
                                     job_event = check_and_decrypt_tags(job_event, self.dvm_config)
                                     if job_event is None:
                                         return
                                 else:
                                     return
+                            elif tag.as_vec()[0] == 'status':
+                                status = tag.as_vec()[1]
+                                print(status)
 
                             # if a reaction by us got zapped
+                        print(status)
+                        if job_event.kind().as_u64() == EventDefinitions.KIND_NIP88_SUBSCRIBE_EVENT.as_u64():
+                            send_job_status_reaction(job_event, "subscription-success", client=self.client,
+                                                     dvm_config=self.dvm_config, user=user)
 
-                        task_supported, task = check_task_is_supported(job_event, client=self.client,
-                                                                       config=self.dvm_config)
-                        if job_event is not None and task_supported:
-                            print("Zap received for NIP90 task: " + str(invoice_amount) + " Sats from " + str(
-                                user.name))
-                            if amount <= invoice_amount:
-                                print("[" + self.dvm_config.NIP89.NAME + "]  Payment-request fulfilled...")
-                                send_job_status_reaction(job_event, "processing", client=self.client,
-                                                         dvm_config=self.dvm_config)
-                                indices = [i for i, x in enumerate(self.job_list) if
-                                           x.event == job_event]
-                                index = -1
-                                if len(indices) > 0:
-                                    index = indices[0]
-                                if index > -1:
-                                    if self.job_list[index].is_processed:  # If payment-required appears a processing
-                                        self.job_list[index].is_paid = True
-                                        check_and_return_event(self.job_list[index].result, job_event)
-                                    elif not (self.job_list[index]).is_processed:
-                                        # If payment-required appears before processing
-                                        self.job_list.pop(index)
-                                        print("Starting work...")
+
+
+                        else:
+                            task_supported, task = check_task_is_supported(job_event, client=self.client,
+                                                                           config=self.dvm_config)
+                            if job_event is not None and task_supported:
+                                print("Zap received for NIP90 task: " + str(invoice_amount) + " Sats from " + str(
+                                    user.name))
+                                if amount <= invoice_amount:
+                                    print("[" + self.dvm_config.NIP89.NAME + "]  Payment-request fulfilled...")
+                                    send_job_status_reaction(job_event, "processing", client=self.client,
+                                                             dvm_config=self.dvm_config, user=user)
+                                    indices = [i for i, x in enumerate(self.job_list) if
+                                               x.event == job_event]
+                                    index = -1
+                                    if len(indices) > 0:
+                                        index = indices[0]
+                                    if index > -1:
+                                        if self.job_list[index].is_processed:
+                                            self.job_list[index].is_paid = True
+                                            check_and_return_event(self.job_list[index].result, job_event)
+                                        elif not (self.job_list[index]).is_processed:
+                                            # If payment-required appears before processing
+                                            self.job_list.pop(index)
+                                            print("Starting work...")
+                                            do_work(job_event, invoice_amount)
+                                    else:
+                                        print("Job not in List, but starting work...")
                                         do_work(job_event, invoice_amount)
-                                else:
-                                    print("Job not in List, but starting work...")
-                                    do_work(job_event, invoice_amount)
 
-                            else:
-                                send_job_status_reaction(job_event, "payment-rejected",
-                                                         False, invoice_amount, client=self.client,
-                                                         dvm_config=self.dvm_config)
-                                print("[" + self.dvm_config.NIP89.NAME + "] Invoice was not paid sufficiently")
+                                else:
+                                    send_job_status_reaction(job_event, "payment-rejected",
+                                                             False, invoice_amount, client=self.client,
+                                                             dvm_config=self.dvm_config)
+                                    print("[" + self.dvm_config.NIP89.NAME + "] Invoice was not paid sufficiently")
+                    elif zapped_event.kind().as_u64() == EventDefinitions.KIND_NIP88_SUBSCRIBE_EVENT.as_u64():
+                        print("new subscription, doing nothing")
 
                     elif zapped_event.kind() in EventDefinitions.ANY_RESULT:
                         print("[" + self.dvm_config.NIP89.NAME + "] "
                                                                  "Someone zapped the result of an exisiting Task. Nice")
                     elif not anon:
                         print("[" + self.dvm_config.NIP89.NAME + "] Note Zap received for DVM balance: " +
                               str(invoice_amount) + " Sats from " + str(user.name))
                         update_user_balance(self.dvm_config.DB, sender, invoice_amount, client=self.client,
                                             config=self.dvm_config)
 
                         # a regular note
-                elif not anon:
+                elif not anon and dvm_config.NIP88 is None:
                     print("[" + self.dvm_config.NIP89.NAME + "] Profile Zap received for DVM balance: " +
                           str(invoice_amount) + " Sats from " + str(user.name))
                     update_user_balance(self.dvm_config.DB, sender, invoice_amount, client=self.client,
                                         config=self.dvm_config)
 
             except Exception as e:
                 print("[" + self.dvm_config.NIP89.NAME + "] Error during content decryption: " + str(e))
@@ -319,14 +411,15 @@
                 task = get_task(original_event, self.client, self.dvm_config)
                 for dvm in self.dvm_config.SUPPORTED_DVMS:
                     if task == dvm.TASK:
                         try:
                             post_processed = dvm.post_process(data, original_event)
                             send_nostr_reply_event(post_processed, original_event.as_json())
                         except Exception as e:
+                            print(e)
                             # Zapping back by error in post-processing is a risk for the DVM because work has been done,
                             # but maybe something with parsing/uploading failed. Try to avoid errors here as good as possible
                             send_job_status_reaction(original_event, "error",
                                                      content="Error in Post-processing: " + str(e),
                                                      dvm_config=self.dvm_config,
                                                      )
                             if amount > 0 and self.dvm_config.LNBITS_ADMIN_KEY != "":
@@ -346,15 +439,15 @@
 
         def send_nostr_reply_event(content, original_event_as_str):
             original_event = Event.from_json(original_event_as_str)
             request_tag = Tag.parse(["request", original_event_as_str])
             e_tag = Tag.parse(["e", original_event.id().to_hex()])
             p_tag = Tag.parse(["p", original_event.author().to_hex()])
             alt_tag = Tag.parse(["alt", "This is the result of a NIP90 DVM AI task with kind " + str(
-                original_event.kind()) + ". The task was: " + original_event.content()])
+                original_event.kind().as_u64()) + ". The task was: " + original_event.content()])
             status_tag = Tag.parse(["status", "success"])
             reply_tags = [request_tag, e_tag, p_tag, alt_tag, status_tag]
             encrypted = False
             for tag in original_event.tags():
                 if tag.as_vec()[0] == "encrypted":
                     encrypted = True
                     encrypted_tag = Tag.parse(["encrypted"])
@@ -367,23 +460,24 @@
                         reply_tags.append(i_tag)
 
             if encrypted:
                 print(content)
                 content = nip04_encrypt(self.keys.secret_key(), PublicKey.from_hex(original_event.author().to_hex()),
                                         content)
 
-            reply_event = EventBuilder(original_event.kind() + 1000, str(content), reply_tags).to_event(self.keys)
+            reply_event = EventBuilder(Kind(original_event.kind().as_u64() + 1000), str(content), reply_tags).to_event(
+                self.keys)
 
             send_event(reply_event, client=self.client, dvm_config=self.dvm_config)
             print("[" + self.dvm_config.NIP89.NAME + "] " + str(
-                original_event.kind() + 1000) + " Job Response event sent: " + reply_event.as_json())
+                original_event.kind().as_u64() + 1000) + " Job Response event sent: " + reply_event.as_json())
 
         def send_job_status_reaction(original_event, status, is_paid=True, amount=0, client=None,
                                      content=None,
-                                     dvm_config=None):
+                                     dvm_config=None, user=None):
 
             task = get_task(original_event, client=client, dvm_config=dvm_config)
             alt_description, reaction = build_status_reaction(status, task, amount, content, dvm_config)
 
             e_tag = Tag.parse(["e", original_event.id().to_hex()])
             p_tag = Tag.parse(["p", original_event.author().to_hex()])
             alt_tag = Tag.parse(["alt", alt_description])
@@ -396,28 +490,32 @@
                 if tag.as_vec()[0] == "encrypted":
                     encrypted = True
                     encrypted_tag = Tag.parse(["encrypted"])
                     encryption_tags.append(encrypted_tag)
 
             if encrypted:
                 encryption_tags.append(p_tag)
+                encryption_tags.append(e_tag)
+
             else:
                 reply_tags.append(p_tag)
 
+
             if status == "success" or status == "error":  #
                 for x in self.job_list:
                     if x.event == original_event:
                         is_paid = x.is_paid
                         amount = x.amount
                         break
 
             bolt11 = ""
             payment_hash = ""
             expires = original_event.created_at().as_secs() + (60 * 60 * 24)
-            if status == "payment-required" or (status == "processing" and not is_paid):
+            if status == "payment-required" or (
+                    status == "processing" and not is_paid):
                 if dvm_config.LNBITS_INVOICE_KEY != "":
                     try:
                         bolt11, payment_hash = create_bolt11_ln_bits(amount, dvm_config)
                     except Exception as e:
                         print(e)
                         try:
                             bolt11, payment_hash = create_bolt11_lud16(dvm_config.LN_ADDRESS,
@@ -467,20 +565,21 @@
             else:
                 content = reaction
 
             keys = Keys.parse(dvm_config.PRIVATE_KEY)
             reaction_event = EventBuilder(EventDefinitions.KIND_FEEDBACK, str(content), reply_tags).to_event(keys)
             send_event(reaction_event, client=self.client, dvm_config=self.dvm_config)
             print("[" + self.dvm_config.NIP89.NAME + "]" + ": Sent Kind " + str(
-                EventDefinitions.KIND_FEEDBACK) + " Reaction: " + status + " " + reaction_event.as_json())
+                EventDefinitions.KIND_FEEDBACK.as_u64()) + " Reaction: " + status + " " + reaction_event.as_json())
             return reaction_event.as_json()
 
         def do_work(job_event, amount):
-            if ((EventDefinitions.KIND_NIP90_EXTRACT_TEXT <= job_event.kind() <= EventDefinitions.KIND_NIP90_GENERIC)
-                    or job_event.kind() == EventDefinitions.KIND_DM):
+            if ((
+                    EventDefinitions.KIND_NIP90_EXTRACT_TEXT.as_u64() <= job_event.kind().as_u64() <= EventDefinitions.KIND_NIP90_GENERIC.as_u64())
+                    or job_event.kind().as_u64() == EventDefinitions.KIND_DM.as_u64()):
 
                 task = get_task(job_event, client=self.client, dvm_config=self.dvm_config)
 
                 for dvm in self.dvm_config.SUPPORTED_DVMS:
                     result = ""
                     try:
                         if task == dvm.TASK:
@@ -511,27 +610,29 @@
                             else:  # Some components might have issues with running code in otuside venv.
                                 # We install locally in these cases for now
                                 result = dvm.process(request_form)
                             try:
                                 post_processed = dvm.post_process(result, job_event)
                                 send_nostr_reply_event(post_processed, job_event.as_json())
                             except Exception as e:
+                                print(e)
                                 send_job_status_reaction(job_event, "error", content=str(e),
                                                          dvm_config=self.dvm_config)
                     except Exception as e:
+                        print(e)
                         # we could send the exception here to the user, but maybe that's not a good idea after all.
                         send_job_status_reaction(job_event, "error", content=result,
                                                  dvm_config=self.dvm_config)
                         # Zapping back the user on error
                         if amount > 0 and self.dvm_config.LNBITS_ADMIN_KEY != "":
                             user = get_or_add_user(self.dvm_config.DB, job_event.author().to_hex(),
                                                    client=self.client, config=self.dvm_config)
                             print(user.lud16 + " " + str(amount))
                             bolt11 = zaprequest(user.lud16, amount, "Couldn't finish job, returning sats", job_event,
-                                                user.npub,
+                                                PublicKey.parse(user.npub),
                                                 self.keys, self.dvm_config.RELAY_LIST, zaptype="private")
                             if bolt11 is None:
                                 print("Receiver has no Lightning address, can't zap back.")
                                 return
                             try:
                                 payment_hash = pay_bolt11_ln_bits(bolt11, self.dvm_config)
                             except Exception as e:
@@ -541,27 +642,27 @@
 
         self.client.handle_notifications(NotificationHandler())
         while True:
 
             for dvm in self.dvm_config.SUPPORTED_DVMS:
                 scheduled_result = dvm.schedule(self.dvm_config)
 
-
             for job in self.job_list:
                 if job.bolt11 != "" and job.payment_hash != "" and not job.payment_hash is None and not job.is_paid:
                     ispaid = check_bolt11_ln_bits_is_paid(job.payment_hash, self.dvm_config)
                     if ispaid and job.is_paid is False:
                         print("is paid")
+                        job.is_paid = True
+                        amount = parse_amount_from_bolt11_invoice(job.bolt11)
 
                         job.is_paid = True
                         send_job_status_reaction(job.event, "processing", True, 0,
                                                  client=self.client,
                                                  dvm_config=self.dvm_config)
                         print("[" + self.dvm_config.NIP89.NAME + "] doing work from joblist")
-                        amount = parse_amount_from_bolt11_invoice(job.bolt11)
                         do_work(job.event, amount)
                     elif ispaid is None:  # invoice expired
                         self.job_list.remove(job)
 
                 if Timestamp.now().as_secs() > job.expires:
                     self.job_list.remove(job)
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/interfaces/dvmtaskinterface.py` & `nostr-dvm-0.3.0/nostr_dvm/interfaces/dvmtaskinterface.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,44 +3,46 @@
 import subprocess
 import time
 from subprocess import run
 import sys
 from sys import platform
 from threading import Thread
 from venv import create
-from nostr_sdk import Keys
+from nostr_sdk import Keys, Kind
 from nostr_dvm.dvm import DVM
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.output_utils import post_process_result
 
 
 class DVMTaskInterface:
     NAME: str
-    KIND: int
+    KIND: Kind
     TASK: str = ""
     FIX_COST: float = 0
     PER_UNIT_COST: float = 0
     PRIVATE_KEY: str
     PUBLIC_KEY: str
     DVM = DVM
     SUPPORTS_ENCRYPTION = True  # DVMs build with this framework support encryption, but others might not.
     ACCEPTS_CASHU = True  # DVMs build with this framework support encryption, but others might not.
     dvm_config: DVMConfig
     admin_config: AdminConfig
     dependencies = []
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, admin_config: AdminConfig = None,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
+                 admin_config: AdminConfig = None,
                  options=None, task=None):
-        self.init(name, dvm_config, admin_config, nip89config, task)
+        self.init(name, dvm_config, admin_config, nip88config, nip89config, task)
         self.options = options
         self.install_dependencies(dvm_config)
 
-    def init(self, name, dvm_config, admin_config=None, nip89config=None, task=None):
+    def init(self, name, dvm_config, admin_config=None, nip88config=None, nip89config=None, task=None):
         self.NAME = name
         self.PRIVATE_KEY = dvm_config.PRIVATE_KEY
         if dvm_config.PUBLIC_KEY == "" or dvm_config.PUBLIC_KEY is None:
             dvm_config.PUBLIC_KEY = Keys.parse(dvm_config.PRIVATE_KEY).public_key().to_hex()
         self.PUBLIC_KEY = dvm_config.PUBLIC_KEY
         if dvm_config.FIX_COST is not None:
             self.FIX_COST = dvm_config.FIX_COST
@@ -51,14 +53,20 @@
 
         dvm_config.SUPPORTED_DVMS = [self]
         dvm_config.DB = "db/" + self.NAME + ".db"
         if nip89config.KIND is not None:
             self.KIND = nip89config.KIND
 
         dvm_config.NIP89 = self.NIP89_announcement(nip89config)
+
+        if nip88config is None:
+            dvm_config.NIP88 = None
+        else:
+            dvm_config.NIP88 = nip88config
+
         self.dvm_config = dvm_config
         self.admin_config = admin_config
 
     def install_dependencies(self, dvm_config):
         if dvm_config.SCRIPT != "":
             if self.dvm_config.USE_OWN_VENV:
                 dir = r'cache/venvs/' + os.path.basename(dvm_config.SCRIPT).split(".py")[0]
@@ -146,8 +154,7 @@
     dvm_config = build_default_config(args.identifier)
     dvm = identifier(name="", dvm_config=dvm_config, nip89config=NIP89Config(), admin_config=None)
     try:
         result = dvm.process(json.loads(args.request))
         DVMTaskInterface.write_output(result, args.output)
     except Exception as e:
         DVMTaskInterface.write_output("Error: " + str(e), args.output)
-
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/advanced_search.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/advanced_search_wine.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 import json
 import os
 from datetime import timedelta
-from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner
+
+import requests
+from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, Event, Kind
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.output_utils import post_process_list_to_events
 
 """
 This File contains a Module to search for notes
 Accepted Inputs: a search query
 Outputs: A list of events 
 Params:  None
 """
 
 
-class AdvancedSearch(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_CONTENT_SEARCH
+class AdvancedSearchWine(DVMTaskInterface):
+    KIND: Kind = EventDefinitions.KIND_NIP90_CONTENT_SEARCH
     TASK: str = "search-content"
     FIX_COST: float = 0
     dvm_config: DVMConfig
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
@@ -47,102 +51,86 @@
         # default values
         user = ""
         users = []
         since_seconds = Timestamp.now().as_secs() - (365 * 24 * 60 * 60)
         until_seconds = Timestamp.now().as_secs()
         search = ""
         max_results = 100
-        relay = "wss://relay.nostr.band"
-        
+
+
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 input_type = tag.as_vec()[2]
                 if input_type == "text":
                     search = tag.as_vec()[1]
             elif tag.as_vec()[0] == 'param':
                 param = tag.as_vec()[1]
                 if param == "user":  # check for param type
-                    #user = tag.as_vec()[2]
-                    users.append(Tag.parse(["p", tag.as_vec()[2]]))
+                    user = tag.as_vec()[2]
                 elif param == "users":  # check for param type
                     users = json.loads(tag.as_vec()[2])
                 elif param == "since":  # check for param type
                     since_seconds = int(tag.as_vec()[2])
                 elif param == "until":  # check for param type
-                    until_seconds = min(int(tag.as_vec()[2]), until_seconds)
+                    until_seconds = int(tag.as_vec()[2])
                 elif param == "max_results":  # check for param type
                     max_results = int(tag.as_vec()[2])
 
         options = {
             "search": search,
+            "user": user,
             "users": users,
             "since": since_seconds,
             "until": until_seconds,
             "max_results": max_results,
-            "relay": relay
+
         }
         request_form['options'] = json.dumps(options)
         return request_form
 
     def process(self, request_form):
         from nostr_sdk import Filter
         options = DVMTaskInterface.set_options(request_form)
-
-        opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
-        sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
-        keys = Keys.parse(sk.to_hex())
-        signer = NostrSigner.keys(keys)
-        cli = Client.with_opts(signer, opts)
-
-        cli.add_relay(options["relay"])
-        cli.connect()
-
-        #earch_since_seconds = int(options["since"]) * 24 * 60 * 60
-        #dif = Timestamp.now().as_secs() - search_since_seconds
-        #search_since = Timestamp.from_secs(dif)
-        search_since = Timestamp.from_secs(int(options["since"]))
-
-        #search_until_seconds = int(options["until"]) * 24 * 60 * 60
-        #dif = Timestamp.now().as_secs() - search_until_seconds
-        #search_until = Timestamp.from_secs(dif)
-        search_until = Timestamp.from_secs(int(options["until"]))
         userkeys = []
         for user in options["users"]:
             tag = Tag.parse(user)
             user = tag.as_vec()[1]
-            #user = user[1]
             user = str(user).lstrip("@")
             if str(user).startswith('npub'):
                 userkey = PublicKey.from_bech32(user)
             elif str(user).startswith("nostr:npub"):
                 userkey = PublicKey.from_nostr_uri(user)
             else:
                 userkey = PublicKey.from_hex(user)
 
             userkeys.append(userkey)
 
-        if not options["users"]:
-            notes_filter = Filter().kind(1).search(options["search"]).since(search_since).until(search_until).limit(options["max_results"])
-        elif options["search"] == "":
-                notes_filter = Filter().kind(1).authors(userkeys).since(search_since).until(
-                    search_until).limit(options["max_results"])
+        print("Sending job to nostr.wine API")
+        if options["users"]:
+            url = ('https://api.nostr.wine/search?query=' + options["search"] + '&kind=1' + '&pubkey=' + options["users"][0][1] + "&limit=100" + "&sort=time" + "&until=" + str(options["until"]) + "&since=" + str(options["since"]))
         else:
-                notes_filter = Filter().kind(1).authors(userkeys).search(options["search"]).since(
-                    search_since).until(search_until).limit(options["max_results"])
-
+            url = ('https://api.nostr.wine/search?query=' + options["search"] + '&kind=1' + "&limit=100" + "&sort=time" + "&until=" + str(options["until"]) + "&since=" + str(options["since"]))
 
-        events = cli.get_events_of([notes_filter], timedelta(seconds=5))
+        headers = {'Content-type': 'application/x-www-form-urlencoded'}
+        response = requests.get(url, headers=headers)
+        #print(response.text)
+
+        try:
+            ob = json.loads(response.text)
+            data = ob['data']
+            result_list = []
+            for el in data:
+                try:
+                    e_tag = Tag.parse(["e", el['id']])
+                    result_list.append(e_tag.as_vec())
+                except Exception as e:
+                    print("ERROR: " + str(e))
+        except Exception as e:
+            print(e)
 
-        result_list = []
-        if len(events) > 0:
-
-            for event in events:
-                e_tag = Tag.parse(["e", event.id().to_hex()])
-                #print(e_tag.as_vec())
-                result_list.append(e_tag.as_vec())
 
         return json.dumps(result_list)
 
     def post_process(self, result, event):
         """Overwrite the interface function to return a social client readable format, if requested"""
         for tag in event.tags():
             if tag.as_vec()[0] == 'output':
@@ -159,47 +147,45 @@
 # playground or elsewhere
 def build_example(name, identifier, admin_config):
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     # Add NIP89
     nip89info = {
         "name": name,
-        "image": "https://image.nostr.build/a99ab925084029d9468fef8330ff3d9be2cf67da473b024f2a6d48b5cd77197f.jpg",
-        "about": "I search notes on Nostr.band.",
+        "image": "https://image.nostr.build/d844d6a963724b9f9deb6b3326984fd95352343336718812424d5e99d93a6f2d.jpg",
+        "about": "I search notes on nostr.wine using the nostr-wine API",
         "encryptionSupported": True,
         "cashuAccepted": True,
         "nip90Params": {
             "users": {
                 "required": False,
                 "values": [],
                 "description": "Search for content from specific users"
             },
             "since": {
                 "required": False,
                 "values": [],
-                "description": "A unix timestamp in the past from where the search should start"
+                "description": "The number of days in the past from now the search should include"
             },
             "until": {
                 "required": False,
                 "values": [],
-                "description": "A unix timestamp that tells until the search should include results"
+                "description": "The number of days in the past from now the search should include up to"
             },
             "max_results": {
                 "required": False,
                 "values": [],
                 "description": "The number of maximum results to return (default currently 20)"
             }
         }
     }
 
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
-    options = {"relay": "wss://relay.nostr.band"}
-
-    return AdvancedSearch(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                          admin_config=admin_config, options=options)
+    return AdvancedSearchWine(name=name, dvm_config=dvm_config, nip89config=nip89config,
+                          admin_config=admin_config)
 
 
 if __name__ == '__main__':
-    process_venv(AdvancedSearch)
+    process_venv(AdvancedSearchWine)
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/advanced_search_wine.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_openai_dalle.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,189 +1,159 @@
 import json
 import os
-from datetime import timedelta
+import time
+from io import BytesIO
 
 import requests
-from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, Event
+from PIL import Image
+from nostr_sdk import Kind
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
-from nostr_dvm.utils.output_utils import post_process_list_to_events
+from nostr_dvm.utils.output_utils import upload_media_to_hoster
+from nostr_dvm.utils.zap_utils import get_price_per_sat
 
 """
-This File contains a Module to search for notes
-Accepted Inputs: a search query
-Outputs: A list of events 
-Params:  None
+This File contains a Module to transform Text input on OpenAI's servers with DALLE-3 and receive results back. 
+
+Accepted Inputs: Prompt (text)
+Outputs: An url to an Image
 """
 
 
-class AdvancedSearchWine(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_CONTENT_SEARCH
-    TASK: str = "search-content"
-    FIX_COST: float = 0
-    dvm_config: DVMConfig
+class ImageGenerationDALLE(DVMTaskInterface):
+    KIND: Kind = EventDefinitions.KIND_NIP90_GENERATE_IMAGE
+    TASK: str = "text-to-image"
+    FIX_COST: float = 120
+    dependencies = [("nostr-dvm", "nostr-dvm"),
+                    ("openai", "openai==1.3.5")]
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
                     return False
-        return True
-
-    def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
-        self.dvm_config = dvm_config
-        print(self.dvm_config.PRIVATE_KEY)
 
-        request_form = {"jobID": event.id().to_hex()}
+            elif tag.as_vec()[0] == 'output':
+                output = tag.as_vec()[1]
+                if (output == "" or
+                        not (output == "image/png" or "image/jpg"
+                             or output == "image/png;format=url" or output == "image/jpg;format=url")):
+                    print("Output format not supported, skipping..")
+                    return False
 
-        # default values
-        user = ""
-        users = []
-        since_seconds = Timestamp.now().as_secs() - (365 * 24 * 60 * 60)
-        until_seconds = Timestamp.now().as_secs()
-        search = ""
-        max_results = 100
+        return True
 
+    def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
+        request_form = {"jobID": event.id().to_hex() + "_" + self.NAME.replace(" ", "")}
+        prompt = ""
+        width = "1024"
+        height = "1024"
+        model = "dall-e-3"
+        quality = "standard"
 
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 input_type = tag.as_vec()[2]
                 if input_type == "text":
-                    search = tag.as_vec()[1]
+                    prompt = tag.as_vec()[1]
+
             elif tag.as_vec()[0] == 'param':
-                param = tag.as_vec()[1]
-                if param == "user":  # check for param type
-                    user = tag.as_vec()[2]
-                elif param == "users":  # check for param type
-                    users = json.loads(tag.as_vec()[2])
-                elif param == "since":  # check for param type
-                    since_seconds = int(tag.as_vec()[2])
-                elif param == "until":  # check for param type
-                    until_seconds = int(tag.as_vec()[2])
-                elif param == "max_results":  # check for param type
-                    max_results = int(tag.as_vec()[2])
+                print("Param: " + tag.as_vec()[1] + ": " + tag.as_vec()[2])
+                if tag.as_vec()[1] == "size":
+                    if len(tag.as_vec()) > 3:
+                        width = (tag.as_vec()[2])
+                        height = (tag.as_vec()[3])
+                    elif len(tag.as_vec()) == 3:
+                        split = tag.as_vec()[2].split("x")
+                        if len(split) > 1:
+                            width = split[0]
+                            height = split[1]
+                elif tag.as_vec()[1] == "quality":
+                    quality = tag.as_vec()[2]
 
         options = {
-            "search": search,
-            "user": user,
-            "users": users,
-            "since": since_seconds,
-            "until": until_seconds,
-            "max_results": max_results,
-
+            "prompt": prompt,
+            "size": width + "x" + height,
+            "model": model,
+            "quality": quality,
+            "number": 1
         }
         request_form['options'] = json.dumps(options)
+
         return request_form
 
     def process(self, request_form):
-        from nostr_sdk import Filter
-        options = DVMTaskInterface.set_options(request_form)
-        userkeys = []
-        for user in options["users"]:
-            tag = Tag.parse(user)
-            user = tag.as_vec()[1]
-            user = str(user).lstrip("@")
-            if str(user).startswith('npub'):
-                userkey = PublicKey.from_bech32(user)
-            elif str(user).startswith("nostr:npub"):
-                userkey = PublicKey.from_nostr_uri(user)
-            else:
-                userkey = PublicKey.from_hex(user)
-
-            userkeys.append(userkey)
-
-        print("Sending job to nostr.wine API")
-        if options["users"]:
-            url = ('https://api.nostr.wine/search?query=' + options["search"] + '&kind=1' + '&pubkey=' + options["users"][0][1] + "&limit=100" + "&sort=time" + "&until=" + str(options["until"]) + "&since=" + str(options["since"]))
-        else:
-            url = ('https://api.nostr.wine/search?query=' + options["search"] + '&kind=1' + "&limit=100" + "&sort=time" + "&until=" + str(options["until"]) + "&since=" + str(options["since"]))
-
-        headers = {'Content-type': 'application/x-www-form-urlencoded'}
-        response = requests.get(url, headers=headers)
-        #print(response.text)
-
         try:
-            ob = json.loads(response.text)
-            data = ob['data']
-            result_list = []
-            for el in data:
-                try:
-                    e_tag = Tag.parse(["e", el['id']])
-                    result_list.append(e_tag.as_vec())
-                except Exception as e:
-                    print("ERROR: " + str(e))
-        except Exception as e:
-            print(e)
-
-
-        return json.dumps(result_list)
-
-    def post_process(self, result, event):
-        """Overwrite the interface function to return a social client readable format, if requested"""
-        for tag in event.tags():
-            if tag.as_vec()[0] == 'output':
-                format = tag.as_vec()[1]
-                if format == "text/plain":  # check for output type
-                    result = post_process_list_to_events(result)
+            options = DVMTaskInterface.set_options(request_form)
 
-        # if not text/plain, don't post-process
-        return result
+            from openai import OpenAI
+            client = OpenAI()
+            print("Job " + request_form['jobID'] + " sent to OpenAI API..")
+
+            response = client.images.generate(
+                model=options['model'],
+                prompt=options['prompt'],
+                size=options['size'],
+                quality=options['quality'],
+                n=int(options['number']),
+            )
+
+            image_url = response.data[0].url
+            # rehost the result instead of relying on the openai link
+            response = requests.get(image_url)
+            image = Image.open(BytesIO(response.content)).convert("RGB")
+            image.save("./outputs/image.jpg")
+            result = upload_media_to_hoster("./outputs/image.jpg")
+            return result
 
+        except Exception as e:
+            if str(e).startswith("Error code: 400"):
+                raise Exception('Your request was rejected as a result of OpenAI´s safety system. Your prompt may '
+                                'contain text that is not allowed by their safety system.')
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
 def build_example(name, identifier, admin_config):
     dvm_config = build_default_config(identifier)
-    dvm_config.USE_OWN_VENV = False
-    # Add NIP89
+    dvm_config.USE_OWN_VENV = True
+    admin_config.LUD16 = dvm_config.LN_ADDRESS
+    profit_in_sats = 10
+    cost_in_cent = 4.0
+    dvm_config.FIX_COST = int(((cost_in_cent / (get_price_per_sat("USD") * 100)) + profit_in_sats))
+
     nip89info = {
         "name": name,
-        "image": "https://image.nostr.build/d844d6a963724b9f9deb6b3326984fd95352343336718812424d5e99d93a6f2d.jpg",
-        "about": "I search notes on nostr.wine using the nostr-wine API",
+        "image": "https://image.nostr.build/c33ca6fc4cc038ca4adb46fdfdfda34951656f87ee364ef59095bae1495ce669.jpg",
+        "about": "I use OpenAI's DALL·E 3",
         "encryptionSupported": True,
         "cashuAccepted": True,
         "nip90Params": {
-            "users": {
-                "required": False,
-                "values": [],
-                "description": "Search for content from specific users"
-            },
-            "since": {
-                "required": False,
-                "values": [],
-                "description": "The number of days in the past from now the search should include"
-            },
-            "until": {
-                "required": False,
-                "values": [],
-                "description": "The number of days in the past from now the search should include up to"
-            },
-            "max_results": {
+            "size": {
                 "required": False,
-                "values": [],
-                "description": "The number of maximum results to return (default currently 20)"
+                "values": ["1024:1024", "1024x1792", "1792x1024"]
             }
         }
     }
 
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
-    return AdvancedSearchWine(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                          admin_config=admin_config)
+    return ImageGenerationDALLE(name=name, dvm_config=dvm_config, nip89config=nip89config, admin_config=admin_config)
 
 
 if __name__ == '__main__':
-    process_venv(AdvancedSearchWine)
+    process_venv(ImageGenerationDALLE)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/convert_media.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/convert_media.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 import json
 import os
+
+from nostr_sdk import Kind
+
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config
 from nostr_dvm.utils.mediasource_utils import organize_input_media_data
 from nostr_dvm.utils.output_utils import upload_media_to_hoster
 
 """
 This File contains a Module convert media locally
 
 Accepted Inputs: Text, Events, Jobs (Text Extraction, Summary, Translation)
 Outputs: Text containing the TranslationGoogle in the desired language.
 Params:  -language The target language
 """
 
 
 class MediaConverter(DVMTaskInterface):
-    KIND = EventDefinitions.KIND_NIP90_CONVERT_VIDEO
+    KIND: Kind = EventDefinitions.KIND_NIP90_CONVERT_VIDEO
     TASK = "convert"
     FIX_COST = 20
     PER_UNIT_COST = 0.1
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "url":
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/discovery_inactive_follows.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/discovery_inactive_follows.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import json
 import os
 from datetime import timedelta
 from threading import Thread
 
-from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner
+from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, Kind
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.output_utils import post_process_list_to_users
 
 """
 This File contains a Module to find inactive follows for a user on nostr
 
 Accepted Inputs: None needed
 Outputs: A list of users that have been inactive 
 Params:  None
 """
 
 
 class DiscoverInactiveFollows(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_PEOPLE_DISCOVERY
+    KIND: Kind = EventDefinitions.KIND_NIP90_PEOPLE_DISCOVERY
     TASK: str = "inactive-follows"
     FIX_COST: float = 50
     client: Client
     dvm_config: DVMConfig
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         # no input required
         return True
 
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         self.dvm_config = dvm_config
@@ -74,15 +76,15 @@
         for relay in self.dvm_config.RELAY_LIST:
             cli.add_relay(relay)
         cli.connect()
 
         options = DVMTaskInterface.set_options(request_form)
         step = 20
 
-        followers_filter = Filter().author(PublicKey.from_hex(options["user"])).kind(3).limit(1)
+        followers_filter = Filter().author(PublicKey.from_hex(options["user"])).kind(Kind(3)).limit(1)
         followers = cli.get_events_of([followers_filter], timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
 
         if len(followers) > 0:
             result_list = []
             newest = 0
             best_entry = followers[0]
             for entry in followers:
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/discovery_nonfollowers.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/discovery_nonfollowers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import json
 import os
 from datetime import timedelta
 from threading import Thread
 
-from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner
+from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, Kind
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.output_utils import post_process_list_to_users
 
 """
 This File contains a Module to find inactive follows for a user on nostr
 
 Accepted Inputs: None needed
 Outputs: A list of users that have been inactive 
 Params:  None
 """
 
 
 class DiscoverNonFollowers(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_PEOPLE_DISCOVERY
+    KIND: Kind = EventDefinitions.KIND_NIP90_PEOPLE_DISCOVERY
     TASK: str = "non-followers"
     FIX_COST: float = 50
     client: Client
     dvm_config: DVMConfig
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         # no input required
         return True
 
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         self.dvm_config = dvm_config
@@ -62,23 +64,23 @@
         ns = SimpleNamespace()
 
         opts = (Options().wait_for_send(False).send_timeout(timedelta(seconds=self.dvm_config.RELAY_TIMEOUT)))
         sk = SecretKey.from_hex(self.dvm_config.PRIVATE_KEY)
         keys = Keys.parse(sk.to_hex())
         signer = NostrSigner.keys(keys)
         cli = Client.with_opts(signer, opts)
-        #cli.add_relay("wss://relay.nostr.band")
+        # cli.add_relay("wss://relay.nostr.band")
         for relay in self.dvm_config.RELAY_LIST:
-           cli.add_relay(relay)
+            cli.add_relay(relay)
         cli.connect()
 
         options = DVMTaskInterface.set_options(request_form)
         step = 20
 
-        followers_filter = Filter().author(PublicKey.from_hex(options["user"])).kind(3)
+        followers_filter = Filter().author(PublicKey.from_hex(options["user"])).kind(Kind(3))
         followers = cli.get_events_of([followers_filter], timedelta(seconds=self.dvm_config.RELAY_TIMEOUT))
 
         if len(followers) > 0:
             result_list = []
             newest = 0
             best_entry = followers[0]
             for entry in followers:
@@ -92,31 +94,29 @@
             for tag in best_entry.tags():
                 if tag.as_vec()[0] == "p":
                     following = tag.as_vec()[1]
                     followings.append(following)
                     ns.dic[following] = "True"
             print("Followings: " + str(len(followings)))
 
-
             def scanList(users, instance, i, st):
                 from nostr_sdk import Filter
 
                 keys = Keys.parse(self.dvm_config.PRIVATE_KEY)
                 opts = Options().wait_for_send(True).send_timeout(
                     timedelta(seconds=5)).skip_disconnected_relays(True)
                 signer = NostrSigner.keys(keys)
                 cli = Client.with_opts(signer, opts)
                 for relay in self.dvm_config.RELAY_LIST:
                     cli.add_relay(relay)
                 cli.connect()
 
-
                 for i in range(i, i + st):
                     filters = []
-                    filter1 = Filter().author(PublicKey.from_hex(users[i])).kind(3)
+                    filter1 = Filter().author(PublicKey.from_hex(users[i])).kind(Kind(3))
                     filters.append(filter1)
                     followers = cli.get_events_of(filters, timedelta(seconds=3))
 
                     if len(followers) > 0:
                         result_list = []
                         newest = 0
                         best_entry = followers[0]
@@ -126,32 +126,32 @@
                                 best_entry = entry
 
                         foundfollower = False
                         for tag in best_entry.tags():
                             if tag.as_vec()[0] == "p":
                                 if len(tag.as_vec()) > 1:
                                     if tag.as_vec()[1] == options["user"]:
-                                         foundfollower = True
-                                         break
+                                        foundfollower = True
+                                        break
 
                         if not foundfollower:
                             instance.dic[best_entry.author().to_hex()] = "False"
-                            print( "DIDNT FIND " + best_entry.author().to_nostr_uri())
+                            print("DIDNT FIND " + best_entry.author().to_nostr_uri())
 
                 print(str(i) + "/" + str(len(users)))
                 cli.disconnect()
 
             threads = []
             begin = 0
             # Spawn some threads to speed things up
             while begin < len(followings) - step:
                 args = [followings, ns, begin, step]
                 t = Thread(target=scanList, args=args)
                 threads.append(t)
-                begin = begin + step -1
+                begin = begin + step - 1
 
             # last to step size
             missing_scans = (len(followings) - begin)
             args = [followings, ns, begin, missing_scans]
             t = Thread(target=scanList, args=args)
             threads.append(t)
 
@@ -212,12 +212,12 @@
         }
     }
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
     return DiscoverNonFollowers(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                   admin_config=admin_config)
+                                admin_config=admin_config)
 
 
 if __name__ == '__main__':
     process_venv(DiscoverNonFollowers)
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/imagegeneration_openai_dalle.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 import json
 import os
-import time
 from io import BytesIO
-
 import requests
 from PIL import Image
+from nostr_sdk import Kind
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.output_utils import upload_media_to_hoster
 from nostr_dvm.utils.zap_utils import get_price_per_sat
 
 """
-This File contains a Module to transform Text input on OpenAI's servers with DALLE-3 and receive results back. 
+This File contains a Module to generate an Image on replicate and receive results back. 
 
 Accepted Inputs: Prompt (text)
 Outputs: An url to an Image
+Params: 
 """
 
 
-class ImageGenerationDALLE(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_GENERATE_IMAGE
+class ImageGenerationReplicateSDXL(DVMTaskInterface):
+    KIND: Kind = EventDefinitions.KIND_NIP90_GENERATE_IMAGE
     TASK: str = "text-to-image"
     FIX_COST: float = 120
     dependencies = [("nostr-dvm", "nostr-dvm"),
-                    ("openai", "openai==1.3.5")]
+                    ("replicate", "replicate")]
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
@@ -53,16 +55,14 @@
         return True
 
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         request_form = {"jobID": event.id().to_hex() + "_" + self.NAME.replace(" ", "")}
         prompt = ""
         width = "1024"
         height = "1024"
-        model = "dall-e-3"
-        quality = "standard"
 
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 input_type = tag.as_vec()[2]
                 if input_type == "text":
                     prompt = tag.as_vec()[1]
 
@@ -73,84 +73,80 @@
                         width = (tag.as_vec()[2])
                         height = (tag.as_vec()[3])
                     elif len(tag.as_vec()) == 3:
                         split = tag.as_vec()[2].split("x")
                         if len(split) > 1:
                             width = split[0]
                             height = split[1]
+                elif tag.as_vec()[1] == "model":
+                    model = tag.as_vec()[2]
                 elif tag.as_vec()[1] == "quality":
                     quality = tag.as_vec()[2]
 
         options = {
             "prompt": prompt,
             "size": width + "x" + height,
-            "model": model,
-            "quality": quality,
             "number": 1
         }
         request_form['options'] = json.dumps(options)
 
         return request_form
 
     def process(self, request_form):
         try:
             options = DVMTaskInterface.set_options(request_form)
 
-            from openai import OpenAI
-            client = OpenAI()
-            print("Job " + request_form['jobID'] + " sent to OpenAI API..")
-
-            response = client.images.generate(
-                model=options['model'],
-                prompt=options['prompt'],
-                size=options['size'],
-                quality=options['quality'],
-                n=int(options['number']),
+            import replicate
+            width = int(options["size"].split("x")[0])
+            height = int(options["size"].split("x")[1])
+            output = replicate.run(
+                "stability-ai/sdxl:39ed52f2a78e934b3ba6e2a89f5b1c712de7dfea535525255b1aa35c5565e08b",
+                input={"prompt": options["prompt"],
+                       "width": width,
+                       "height": height,
+                       "disable_safety_checker": True}
             )
-
-            image_url = response.data[0].url
-            # rehost the result instead of relying on the openai link
-            response = requests.get(image_url)
+            print(output[0])
+            response = requests.get(output[0])
             image = Image.open(BytesIO(response.content)).convert("RGB")
             image.save("./outputs/image.jpg")
             result = upload_media_to_hoster("./outputs/image.jpg")
             return result
 
         except Exception as e:
-            if str(e).startswith("Error code: 400"):
-                raise Exception('Your request was rejected as a result of OpenAI´s safety system. Your prompt may '
-                                'contain text that is not allowed by their safety system.')
+            print("Error in Module")
+            raise Exception(e)
+
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
 def build_example(name, identifier, admin_config):
     dvm_config = build_default_config(identifier)
-    dvm_config.USE_OWN_VENV = True
     admin_config.LUD16 = dvm_config.LN_ADDRESS
     profit_in_sats = 10
-    cost_in_cent = 4.0
-    dvm_config.FIX_COST = int(((cost_in_cent / (get_price_per_sat("USD") * 100)) + profit_in_sats))
+    dvm_config.FIX_COST = int(((4.0 / (get_price_per_sat("USD") * 100)) + profit_in_sats))
 
     nip89info = {
         "name": name,
         "image": "https://image.nostr.build/c33ca6fc4cc038ca4adb46fdfdfda34951656f87ee364ef59095bae1495ce669.jpg",
-        "about": "I use OpenAI's DALL·E 3",
+        "about": "I use Replicate to run StableDiffusion XL",
         "encryptionSupported": True,
         "cashuAccepted": True,
         "nip90Params": {
             "size": {
                 "required": False,
                 "values": ["1024:1024", "1024x1792", "1792x1024"]
             }
         }
     }
 
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
-    return ImageGenerationDALLE(name=name, dvm_config=dvm_config, nip89config=nip89config, admin_config=admin_config)
+    return ImageGenerationReplicateSDXL(name=name, dvm_config=dvm_config, nip89config=nip89config,
+                                        admin_config=admin_config)
 
 
 if __name__ == '__main__':
-    process_venv(ImageGenerationDALLE)
+    process_venv(ImageGenerationReplicateSDXL)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/imagegeneration_replicate_sdxl.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/videogeneration_replicate_svd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,149 +1,140 @@
 import json
 import os
 from io import BytesIO
 import requests
+import urllib.request
 from PIL import Image
+from nostr_sdk import Kind
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.output_utils import upload_media_to_hoster
 from nostr_dvm.utils.zap_utils import get_price_per_sat
 
 """
-This File contains a Module to generate an Image on replicate and receive results back. 
+This File contains a Module to transform an image to a short video clip using Stable Video Diffusion with replicate
 
 Accepted Inputs: Prompt (text)
 Outputs: An url to an Image
 Params: 
 """
 
 
-class ImageGenerationReplicateSDXL(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_GENERATE_IMAGE
-    TASK: str = "text-to-image"
+class VideoGenerationReplicateSVD(DVMTaskInterface):
+    KIND: Kind = EventDefinitions.KIND_NIP90_GENERATE_VIDEO
+    TASK: str = "image-to-video"
     FIX_COST: float = 120
     dependencies = [("nostr-dvm", "nostr-dvm"),
                     ("replicate", "replicate")]
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
-                if input_type != "text":
+                if input_type != "url":
                     return False
-
-            elif tag.as_vec()[0] == 'output':
-                output = tag.as_vec()[1]
-                if (output == "" or
-                        not (output == "image/png" or "image/jpg"
-                             or output == "image/png;format=url" or output == "image/jpg;format=url")):
-                    print("Output format not supported, skipping..")
-                    return False
-
         return True
 
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         request_form = {"jobID": event.id().to_hex() + "_" + self.NAME.replace(" ", "")}
-        prompt = ""
-        width = "1024"
-        height = "1024"
+        url = ""
+        frames = 14  # 25
+        if frames == 25:
+            length = "25_frames_with_svd_xt"
+        else:
+            length = "14_frames_with_svd"
+        sizing_strategy = "maintain_aspect_ratio"  # crop_to_16_9, use_image_dimensions
+        frames_per_second = 6
+        motion_bucket_id = 127  # Increase overall motion in the generated video
+        cond_aug = 0.02  # Amount of noise to add to input image
 
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 input_type = tag.as_vec()[2]
-                if input_type == "text":
-                    prompt = tag.as_vec()[1]
-
-            elif tag.as_vec()[0] == 'param':
-                print("Param: " + tag.as_vec()[1] + ": " + tag.as_vec()[2])
-                if tag.as_vec()[1] == "size":
-                    if len(tag.as_vec()) > 3:
-                        width = (tag.as_vec()[2])
-                        height = (tag.as_vec()[3])
-                    elif len(tag.as_vec()) == 3:
-                        split = tag.as_vec()[2].split("x")
-                        if len(split) > 1:
-                            width = split[0]
-                            height = split[1]
-                elif tag.as_vec()[1] == "model":
-                    model = tag.as_vec()[2]
-                elif tag.as_vec()[1] == "quality":
-                    quality = tag.as_vec()[2]
+                if input_type == "url":
+                    url = str(tag.as_vec()[1]).split('#')[0]
+        # TODO add params as defined above
 
         options = {
-            "prompt": prompt,
-            "size": width + "x" + height,
-            "number": 1
+            "url": url,
+            "length": length,
+            "sizing_strategy": sizing_strategy,
+            "frames_per_second": frames_per_second,
+            "motion_bucket_id": motion_bucket_id,
+            "cond_aug": cond_aug
+
         }
         request_form['options'] = json.dumps(options)
 
         return request_form
 
     def process(self, request_form):
         try:
             options = DVMTaskInterface.set_options(request_form)
+            print(options["url"])
+            response = requests.get(options["url"])
+            image = Image.open(BytesIO(response.content)).convert("RGB")
+            image.save("./outputs/input.jpg")
 
             import replicate
-            width = int(options["size"].split("x")[0])
-            height = int(options["size"].split("x")[1])
             output = replicate.run(
-                "stability-ai/sdxl:39ed52f2a78e934b3ba6e2a89f5b1c712de7dfea535525255b1aa35c5565e08b",
-                input={"prompt": options["prompt"],
-                       "width": width,
-                       "height": height,
-                       "disable_safety_checker": True}
+                "stability-ai/stable-video-diffusion:3f0457e4619daac51203dedb472816fd4af51f3149fa7a9e0b5ffcf1b8172438",
+                input={"input_image": open("./outputs/input.jpg", "rb"),
+                       "video_length": options["length"],
+                       "sizing_strategy": options["sizing_strategy"],
+                       "frames_per_second": options["frames_per_second"],
+                       "motion_bucket_id": options["motion_bucket_id"],
+                       "cond_aug": options["cond_aug"]
+                       }
             )
-            print(output[0])
-            response = requests.get(output[0])
-            image = Image.open(BytesIO(response.content)).convert("RGB")
-            image.save("./outputs/image.jpg")
-            result = upload_media_to_hoster("./outputs/image.jpg")
+            print(output)
+
+            urllib.request.urlretrieve(output, "./outputs/svd.mp4")
+            result = upload_media_to_hoster("./outputs/svd.mp4")
             return result
 
         except Exception as e:
             print("Error in Module")
             raise Exception(e)
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
 def build_example(name, identifier, admin_config):
     dvm_config = build_default_config(identifier)
     admin_config.LUD16 = dvm_config.LN_ADDRESS
     profit_in_sats = 10
-    dvm_config.FIX_COST = int(((4.0 / (get_price_per_sat("USD") * 100)) + profit_in_sats))
+    cost_in_cent = 4.0
+    dvm_config.FIX_COST = int(((cost_in_cent / (get_price_per_sat("USD") * 100)) + profit_in_sats))
 
     nip89info = {
         "name": name,
         "image": "https://image.nostr.build/c33ca6fc4cc038ca4adb46fdfdfda34951656f87ee364ef59095bae1495ce669.jpg",
         "about": "I use Replicate to run StableDiffusion XL",
         "encryptionSupported": True,
         "cashuAccepted": True,
-        "nip90Params": {
-            "size": {
-                "required": False,
-                "values": ["1024:1024", "1024x1792", "1792x1024"]
-            }
-        }
+        "nip90Params": {}
     }
 
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
 
-    return ImageGenerationReplicateSDXL(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                        admin_config=admin_config)
+    return VideoGenerationReplicateSVD(name=name, dvm_config=dvm_config, nip89config=nip89config,
+                                       admin_config=admin_config)
 
 
 if __name__ == '__main__':
-    process_venv(ImageGenerationReplicateSDXL)
+    process_venv(VideoGenerationReplicateSVD)
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/imagegeneration_sd21_mlx.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_sd21_mlx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 import json
 import os
 from PIL import Image
+from nostr_sdk import Kind
 from tqdm import tqdm
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.output_utils import upload_media_to_hoster
 from nostr_dvm.utils.zap_utils import get_price_per_sat
 
 """
 This File contains a Module to generate an Image on Macs with M1/M2/M3 chips and receive results back. 
 
 Accepted Inputs: Prompt (text)
 Outputs: An url to an Image
 Params: 
 """
 
 
 class ImageGenerationMLX(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_GENERATE_IMAGE
+    KIND: Kind = EventDefinitions.KIND_NIP90_GENERATE_IMAGE
     TASK: str = "text-to-image"
     FIX_COST: float = 120
     dependencies = [("nostr-dvm", "nostr-dvm"),
                     ("mlx", "mlx"),
                     ("safetensors", "safetensors"),
                     ("huggingface-hub", "huggingface-hub"),
                     ("regex", "regex"),
                     ("tqdm", "tqdm"),
                     ]
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/imagegeneration_sdxl.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_sdxl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import json
 from multiprocessing.pool import ThreadPool
 
+from nostr_sdk import Kind
+
 from nostr_dvm.backends.nova_server.utils import check_server_status, send_request_to_server
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.definitions import EventDefinitions
 
 """
 This File contains a module to transform Text input on n-server and receive results back. 
 
 Accepted Inputs: Prompt (text)
 Outputs: An url to an Image
 Params: -model         # models: juggernaut, dynavision, colossusProject, newreality, unstable
         -lora          # loras (weights on top of models) voxel, 
 """
 
 
 class ImageGenerationSDXL(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_GENERATE_IMAGE
+    KIND: Kind = EventDefinitions.KIND_NIP90_GENERATE_IMAGE
     TASK: str = "text-to-image"
-    FIX_COST: float = 70
+    FIX_COST: float = 50
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/imagegeneration_sdxlimg2img.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import json
 from multiprocessing.pool import ThreadPool
 
+from nostr_sdk import Kind
+
 from nostr_dvm.backends.nova_server.utils import check_server_status, send_request_to_server
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.definitions import EventDefinitions
 
 """
 This File contains a Module to transform Image (and Text) input on N-server and receive results back. 
 
 Accepted Inputs: Prompt (text)
 Outputs: An url to an Image
 Params: -model         # models: juggernaut, dynavision, colossusProject, newreality, unstable
         -lora          # loras (weights on top of models) voxel, 
 """
 
 
 class ImageGenerationSDXLIMG2IMG(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_GENERATE_IMAGE
+    KIND: Kind = EventDefinitions.KIND_NIP90_GENERATE_IMAGE
     TASK: str = "image-to-image"
     FIX_COST: float = 70
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         hasurl = False
         hasprompt = False
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/imageinterrogator.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/imageinterrogator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import json
 from multiprocessing.pool import ThreadPool
 
+from nostr_sdk import Kind
+
 from nostr_dvm.backends.nova_server.utils import check_server_status, send_request_to_server
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.definitions import EventDefinitions
 
 """
 This File contains a Module to extract a prompt from an image from an url.
 
 Accepted Inputs: link to image (url)
 Outputs: An textual description of the image
 
 """
 
 
 class ImageInterrogator(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_EXTRACT_TEXT
+    KIND: Kind = EventDefinitions.KIND_NIP90_EXTRACT_TEXT
     TASK: str = "image-to-text"
     FIX_COST: float = 80
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         hasurl = False
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/imageupscale.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/imageupscale.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import json
 from multiprocessing.pool import ThreadPool
 
+from nostr_sdk import Kind
+
 from nostr_dvm.backends.nova_server.utils import check_server_status, send_request_to_server
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.definitions import EventDefinitions
 
 """
 This File contains a Module to upscale an image from an url by factor 2-4 
 
 Accepted Inputs: link to image (url)
 Outputs: An url to an Image
 Params: -upscale        2,3,4
 """
 
 
 class ImageUpscale(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_GENERATE_IMAGE
+    KIND: Kind = EventDefinitions.KIND_NIP90_GENERATE_IMAGE
     TASK: str = "image-to-image"
     FIX_COST: float = 20
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         hasurl = False
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/search_users.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/search_users.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import json
 import os
 from datetime import timedelta
 from nostr_sdk import Client, Timestamp, PublicKey, Tag, Keys, Options, SecretKey, NostrSigner, NostrDatabase, \
-    ClientBuilder, Filter, NegentropyOptions, NegentropyDirection, init_logger, LogLevel
+    ClientBuilder, Filter, NegentropyOptions, NegentropyDirection, init_logger, LogLevel, Kind
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.output_utils import post_process_list_to_events, post_process_list_to_users
 
 """
 This File contains a Module to search for notes
 Accepted Inputs: a search query
 Outputs: A list of events 
 Params:  None
 """
 
 
 class SearchUser(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_USER_SEARCH
+    KIND: Kind = EventDefinitions.KIND_NIP90_USER_SEARCH
     TASK: str = "search-user"
     FIX_COST: float = 0
     dvm_config: DVMConfig
     last_schedule: int
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        self.last_schedule = Timestamp.now().as_secs()
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
         use_logger = False
         if use_logger:
             init_logger(LogLevel.DEBUG)
 
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
-
         self.sync_db()
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
@@ -91,15 +91,15 @@
         # cli.add_relay("wss://atl.purplerelay.com")
         cli.connect()
 
         # Negentropy reconciliation
 
         # Query events from database
 
-        filter1 = Filter().kind(0)
+        filter1 = Filter().kind(Kind(0))
         events = cli.database().query([filter1])
         # for event in events:
         #    print(event.as_json())
 
         # events = cli.get_events_of([notes_filter], timedelta(seconds=5))
 
         result_list = []
@@ -149,15 +149,15 @@
         signer = NostrSigner.keys(keys)
         database = NostrDatabase.sqlite("db/nostr_profiles.db")
         cli = ClientBuilder().signer(signer).database(database).opts(opts).build()
 
         cli.add_relay("wss://relay.damus.io")
         cli.connect()
 
-        filter1 = Filter().kind(0)
+        filter1 = Filter().kind(Kind(0))
 
         # filter = Filter().author(keys.public_key())
         print("Syncing Profile Database.. this might take a while..")
         dbopts = NegentropyOptions().direction(NegentropyDirection.DOWN)
         cli.reconcile(filter1, dbopts)
         print("Done Syncing Profile Database.")
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/summarization_huggingchat.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/summarization_huggingchat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import json
 import os
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.nostr_utils import get_referenced_event_by_id, get_event_by_id, get_events_by_ids
-from nostr_sdk import Tag
+from nostr_sdk import Tag, Kind
 
 """
 This File contains a Module to summarize Text, based on a prompt using a the HuggingChat LLM on Huggingface
 
 Accepted Inputs: Prompt (text)
 Outputs: Generated text
 """
 
 
 class TextSummarizationHuggingChat(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_SUMMARIZE_TEXT
+    KIND: Kind = EventDefinitions.KIND_NIP90_SUMMARIZE_TEXT
     TASK: str = "summarization"
     FIX_COST: float = 0
     dependencies = [("nostr-dvm", "nostr-dvm"),
                     ("hugchat", "hugchat")]
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "event" and input_type != "job" and input_type != "text":
@@ -119,15 +121,15 @@
 # playground or elsewhere
 def build_example(name, identifier, admin_config):
     dvm_config = build_default_config(identifier)
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
     nip89info = {
         "name": name,
-        "image": "https://image.nostr.build/c33ca6fc4cc038ca4adb46fdfdfda34951656f87ee364ef59095bae1495ce669.jpg",
+        "image": "https://image.nostr.build/720eadc9af89084bb09de659af43ad17fec1f4b0887084e83ac0ae708dfa83a6.png",
         "about": "I use a LLM connected via Huggingchat to summarize Inputs",
         "encryptionSupported": True,
         "cashuAccepted": True,
         "nip90Params": {}
     }
 
     nip89config = NIP89Config()
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/textextraction_google.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/textextraction_google.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 import json
 import os
 import time
 
+from nostr_sdk import Kind
+
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.mediasource_utils import organize_input_media_data
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.definitions import EventDefinitions
 
 """
 This File contains a Module to extract text form a media file input on Google Cloud
 
 Accepted Inputs: Url to media file (url)
 Outputs: Transcribed text
 
 """
 
 
 class SpeechToTextGoogle(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_EXTRACT_TEXT
+    KIND: Kind = EventDefinitions.KIND_NIP90_EXTRACT_TEXT
     TASK: str = "speech-to-text"
     FIX_COST: float = 10
     PER_UNIT_COST: float = 0.1
     dependencies = [("nostr-dvm", "nostr-dvm"),
                     ("speech_recognition", "SpeechRecognition==3.10.0")]
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
         if options is None:
             self.options = {}
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/textextraction_pdf.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/textextraction_pdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 import json
 import os
 import re
 
+from nostr_sdk import Kind
+
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.nostr_utils import get_event_by_id
 
 """
 This File contains a Module to extract Text from a PDF file locally on the DVM Machine
 
 Accepted Inputs: Url to pdf file, Event containing an URL to a PDF file
 Outputs: Text containing the extracted contents of the PDF file
 Params:  None
 """
 
 
 class TextExtractionPDF(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_EXTRACT_TEXT
+    KIND: Kind = EventDefinitions.KIND_NIP90_EXTRACT_TEXT
     TASK: str = "pdf-to-text"
     FIX_COST: float = 0
     dependencies = [("nostr-dvm", "nostr-dvm"),
                     ("pypdf", "pypdf==3.17.1")]
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "url" and input_type != "event":
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/textextraction_whisperx.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/textextraction_whisperx.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 import json
 import os
 import time
 from multiprocessing.pool import ThreadPool
+
+from nostr_sdk import Kind
+
 from nostr_dvm.backends.nova_server.utils import check_server_status, send_request_to_server, send_file_to_server
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
 from nostr_dvm.utils.mediasource_utils import organize_input_media_data
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.definitions import EventDefinitions
 
 """
 This File contains a Module to transform A media file input on n-server and receive results back. 
 
 Accepted Inputs: Url to media file (url)
 Outputs: Transcribed text
 
 """
 
 
 class SpeechToTextWhisperX(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_EXTRACT_TEXT
+    KIND: Kind = EventDefinitions.KIND_NIP90_EXTRACT_TEXT
     TASK: str = "speech-to-text"
     FIX_COST: float = 10
     PER_UNIT_COST: float = 0.1
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        dvm_config.SCRIPT = os.path.abspath(__file__)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "url":
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/textgeneration_huggingchat.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/textgeneration_huggingchat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import json
 import os
 
+from nostr_sdk import Kind
+
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 
 """
 This File contains a Module to generate Text, based on a prompt using a the HuggingChat LLM on Huggingface
 
 Accepted Inputs: Prompt (text)
 Outputs: Generated text
 """
 
 
 class TextGenerationHuggingChat(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_GENERATE_TEXT
+    KIND: Kind = EventDefinitions.KIND_NIP90_GENERATE_TEXT
     TASK: str = "text-to-text"
     FIX_COST: float = 0
     dependencies = [("nostr-dvm", "nostr-dvm"),
                     ("hugchat", "hugchat")]
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
@@ -85,15 +89,15 @@
 # playground or elsewhere
 def build_example(name, identifier, admin_config):
     dvm_config = build_default_config(identifier)
     admin_config.LUD16 = dvm_config.LN_ADDRESS
 
     nip89info = {
         "name": name,
-        "image": "https://image.nostr.build/c33ca6fc4cc038ca4adb46fdfdfda34951656f87ee364ef59095bae1495ce669.jpg",
+        "image": "https://image.nostr.build/720eadc9af89084bb09de659af43ad17fec1f4b0887084e83ac0ae708dfa83a6.png",
         "about": "I use a LLM connected via Huggingchat",
         "encryptionSupported": True,
         "cashuAccepted": True,
         "nip90Params": {}
     }
 
     nip89config = NIP89Config()
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/textgeneration_llmlite.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/textgeneration_llmlite.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import json
 import os
 
+from nostr_sdk import Kind
+
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 
 """
 This File contains a Module to generate Text, based on a prompt using a LLM (local or API) (Ollama, custom model, chatgpt)
 
 Accepted Inputs: Prompt (text)
 Outputs: Generated text
 """
 
 
 class TextGenerationLLMLite(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_GENERATE_TEXT
+    KIND: Kind = EventDefinitions.KIND_NIP90_GENERATE_TEXT
     TASK: str = "text-to-text"
     FIX_COST: float = 0
     dependencies = [("nostr-dvm", "nostr-dvm"),
                     ("litellm", "litellm==1.12.3")]
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/textgeneration_unleashed_chat.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/textgeneration_unleashed_chat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import json
 import os
 
+from nostr_sdk import Kind
+
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 
 """
 This File contains a Module to generate Text, based on a prompt using the Unleashed.chat API.
 
 Accepted Inputs: Prompt (text)
 Outputs: Generated text
 """
 
 
 class TextGenerationUnleashedChat(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_GENERATE_TEXT
+    KIND: Kind = EventDefinitions.KIND_NIP90_GENERATE_TEXT
     TASK: str = "text-to-text"
     FIX_COST: float = 10
     dependencies = [("nostr-dvm", "nostr-dvm"),
                     ("openai", "openai")]
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/texttospeech.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/texttospeech.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import json
 import os
 
+from nostr_sdk import Kind
+
+from nostr_dvm.utils.nip88_utils import NIP88Config
+
 os.environ["PYTORCH_ENABLE_MPS_FALLBACK"] = "1"
 from pathlib import Path
 import urllib.request
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
@@ -18,25 +22,26 @@
 
 Accepted Inputs: Text
 Outputs: Generated Audiofile
 """
 
 
 class TextToSpeech(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_TEXT_TO_SPEECH
+    KIND: Kind = EventDefinitions.KIND_NIP90_TEXT_TO_SPEECH
     TASK: str = "text-to-speech"
     FIX_COST: float = 50
     PER_UNIT_COST = 0.5
     dependencies = [("nostr-dvm", "nostr-dvm"),
                     ("TTS", "TTS==0.22.0")]
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "event" and input_type != "job" and input_type != "text":
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/translation_google.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/translation_google.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 import json
 import os
+
+from nostr_sdk import Kind
+
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.nostr_utils import get_referenced_event_by_id, get_event_by_id
 
 """
 This File contains a Module to call Google Translate Services on the DVM Machine
 
 Accepted Inputs: Text, Events, Jobs (Text Extraction, Summary, Translation)
 Outputs: Text containing the TranslationGoogle in the desired language.
 Params:  -language The target language
 """
 
 
 class TranslationGoogle(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_TRANSLATE_TEXT
+    KIND: Kind = EventDefinitions.KIND_NIP90_TRANSLATE_TEXT
     TASK: str = "translation"
     FIX_COST: float = 0
     dependencies = [("nostr-dvm", "nostr-dvm"),
                     ("translatepy", "translatepy==2.3")]
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "event" and input_type != "job" and input_type != "text":
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/translation_libretranslate.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/translation_libretranslate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 import os
 import requests
+from nostr_sdk import Kind
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.nostr_utils import get_referenced_event_by_id, get_event_by_id
 
 """
 This File contains a Module to call Libre Translate Services
 
 Accepted Inputs: Text, Events, Jobs (Text Extraction, Summary, Translation)
@@ -17,22 +19,23 @@
 Params:  -language The target language
 
 Requires API key or self-hosted instance
 """
 
 
 class TranslationLibre(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_TRANSLATE_TEXT
+    KIND: Kind = EventDefinitions.KIND_NIP90_TRANSLATE_TEXT
     TASK: str = "translation"
     FIX_COST: float = 0
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
-                 admin_config: AdminConfig = None, options=None, task=None):
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
+                 admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options, task)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "event" and input_type != "job" and input_type != "text":
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/trending_notes_nostrband.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/discovery_trending_notes_nostrband.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import json
 import os
-from nostr_sdk import Tag
+from nostr_sdk import Tag, Kind
 
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.output_utils import post_process_list_to_events
 
 """
 This File contains a Module to search for notes
 Accepted Inputs: a search query
 Outputs: A list of events 
 Params:  None
 """
 
 
 class TrendingNotesNostrBand(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_CONTENT_DISCOVERY
+    KIND: Kind = EventDefinitions.KIND_NIP90_CONTENT_DISCOVERY
     TASK: str = "trending-content"
     FIX_COST: float = 0
     dvm_config: DVMConfig
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "text":
@@ -72,16 +74,17 @@
                         print(e_tag.as_vec())
                         result_list.append(e_tag.as_vec())
                     else:
                         break
 
             return json.dumps(result_list)
 
-        except:
-            return "error"
+        except Exception as e:
+            print(e)
+            return json.dumps([])
 
     def post_process(self, result, event):
         """Overwrite the interface function to return a social client readable format, if requested"""
         for tag in event.tags():
             if tag.as_vec()[0] == 'output':
                 format = tag.as_vec()[1]
                 if format == "text/plain":  # check for output type
@@ -98,16 +101,17 @@
     dvm_config = build_default_config(identifier)
     dvm_config.USE_OWN_VENV = False
     admin_config.LUD16 = dvm_config.LN_ADDRESS
     # Add NIP89
 
     nip89info = {
         "name": name,
-        "image": "https://image.nostr.build/c33ca6fc4cc038ca4adb46fdfdfda34951656f87ee364ef59095bae1495ce669.jpg",
+        "image": "https://nostr.band/android-chrome-192x192.png",
         "about": "I show trending notes from nostr.band",
+        "amount": "Free",
         "encryptionSupported": True,
         "cashuAccepted": True,
         "nip90Params": {}
     }
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/videogeneration_replicate_svd.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/summarization_unleashed_chat.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,137 +1,171 @@
 import json
 import os
-from io import BytesIO
-import requests
-import urllib.request
-from PIL import Image
-
+import re
+from nostr_sdk import Tag, Kind
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
-from nostr_dvm.utils.definitions import EventDefinitions
+from nostr_dvm.utils.definitions  import EventDefinitions
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
-from nostr_dvm.utils.output_utils import upload_media_to_hoster
-from nostr_dvm.utils.zap_utils import get_price_per_sat
+from nostr_dvm.utils.nostr_utils import get_referenced_event_by_id, get_events_by_ids, get_event_by_id
 
 """
-This File contains a Module to transform an image to a short video clip using Stable Video Diffusion with replicate
+This File contains a Module to generate Text, based on a prompt using the Unleashed.chat API.
 
 Accepted Inputs: Prompt (text)
-Outputs: An url to an Image
-Params: 
+Outputs: Generated text
 """
 
 
-class VideoGenerationReplicateSVD(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_GENERATE_VIDEO
-    TASK: str = "image-to-video"
-    FIX_COST: float = 120
+class SummarizationUnleashedChat(DVMTaskInterface):
+    KIND: Kind = EventDefinitions.KIND_NIP90_SUMMARIZE_TEXT
+    TASK: str = "text-to-text"
+    FIX_COST: float = 10
     dependencies = [("nostr-dvm", "nostr-dvm"),
-                    ("replicate", "replicate")]
+                    ("openai", "openai")]
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
         dvm_config.SCRIPT = os.path.abspath(__file__)
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
+                print(tag.as_vec())
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
-                if input_type != "url":
+                if input_type != "event" and input_type != "job" and input_type != "text":
                     return False
+
         return True
 
     def create_request_from_nostr_event(self, event, client=None, dvm_config=None):
         request_form = {"jobID": event.id().to_hex() + "_" + self.NAME.replace(" ", "")}
-        url = ""
-        frames = 14  # 25
-        if frames == 25:
-            length = "25_frames_with_svd_xt"
-        else:
-            length = "14_frames_with_svd"
-        sizing_strategy = "maintain_aspect_ratio"  # crop_to_16_9, use_image_dimensions
-        frames_per_second = 6
-        motion_bucket_id = 127  # Increase overall motion in the generated video
-        cond_aug = 0.02  # Amount of noise to add to input image
+        prompt = ""
+        collect_events = []
+        nostr_mode = True
 
         for tag in event.tags():
             if tag.as_vec()[0] == 'i':
                 input_type = tag.as_vec()[2]
-                if input_type == "url":
-                    url = str(tag.as_vec()[1]).split('#')[0]
-        # TODO add params as defined above
+                if input_type == "text":
+                    prompt += tag.as_vec()[1] + "\n"
+                elif input_type == "event":
+                    collect_events.append(tag.as_vec()[1])
+                    # evt = get_event_by_id(tag.as_vec()[1], client=client, config=dvm_config)
+                    # prompt += evt.content() + "\n"
+                elif input_type == "job":
+                    evt = get_referenced_event_by_id(event_id=tag.as_vec()[1], client=client,
+                                                     kinds=[EventDefinitions.KIND_NIP90_RESULT_EXTRACT_TEXT,
+                                                            EventDefinitions.KIND_NIP90_RESULT_SUMMARIZE_TEXT,
+                                                            EventDefinitions.KIND_NIP90_RESULT_TRANSLATE_TEXT,
+                                                            EventDefinitions.KIND_NIP90_RESULT_CONTENT_DISCOVERY],
+                                                     dvm_config=dvm_config)
+                    if evt is None:
+                        print("Event not found")
+                        raise Exception
+
+                    if evt.kind() == EventDefinitions.KIND_NIP90_RESULT_CONTENT_DISCOVERY:
+                        result_list = json.loads(evt.content())
+                        prompt = ""
+                        for tag in result_list:
+                            e_tag = Tag.parse(tag)
+                            evt = get_event_by_id(e_tag.as_vec()[1], client=client, config=dvm_config)
+                            prompt += evt.content() + "\n"
+
+                    else:
+                        prompt = evt.content()
+
+        evts = get_events_by_ids(collect_events, client=client, config=dvm_config)
+        if evts is not None:
+            for evt in evts:
+                prompt += evt.content() + "\n"
 
+        prompt = re.sub(r'http\S+', '', prompt)
         options = {
-            "url": url,
-            "length": length,
-            "sizing_strategy": sizing_strategy,
-            "frames_per_second": frames_per_second,
-            "motion_bucket_id": motion_bucket_id,
-            "cond_aug": cond_aug
-
+            "prompt": prompt,
+            "nostr": nostr_mode,
         }
         request_form['options'] = json.dumps(options)
 
         return request_form
 
     def process(self, request_form):
+        from openai import OpenAI
+        temp_open_ai_api_key = os.environ["OPENAI_API_KEY"]
+        os.environ["OPENAI_API_KEY"] = os.getenv("UNLEASHED_API_KEY")
+        options = DVMTaskInterface.set_options(request_form)
+
         try:
-            options = DVMTaskInterface.set_options(request_form)
-            print(options["url"])
-            response = requests.get(options["url"])
-            image = Image.open(BytesIO(response.content)).convert("RGB")
-            image.save("./outputs/input.jpg")
-
-            import replicate
-            output = replicate.run(
-                "stability-ai/stable-video-diffusion:3f0457e4619daac51203dedb472816fd4af51f3149fa7a9e0b5ffcf1b8172438",
-                input={"input_image": open("./outputs/input.jpg", "rb"),
-                       "video_length": options["length"],
-                       "sizing_strategy": options["sizing_strategy"],
-                       "frames_per_second": options["frames_per_second"],
-                       "motion_bucket_id": options["motion_bucket_id"],
-                       "cond_aug": options["cond_aug"]
-                       }
+            client = OpenAI(
+                base_url='https://unleashed.chat/api/v1',
+            )
+
+            print('Models:\n')
+
+            for model in client.models.list():
+                print('- ' + model.id)
+
+            content = "Summarize the following notes: " + str(options["prompt"])[:3500]
+            normal_stream = client.chat.completions.create(
+                messages=[
+                    {
+                        'role': 'user',
+                        'content':content,
+                    }
+                ],
+                model='dolphin-2.2.1-mistral-7b',
+                stream=True,
+                extra_body={
+                    'nostr_mode': options["nostr"],
+                },
             )
-            print(output)
 
-            urllib.request.urlretrieve(output, "./outputs/svd.mp4")
-            result = upload_media_to_hoster("./outputs/svd.mp4")
+            print('\nChat response: ', end='')
+
+            result = ""
+            for chunk in normal_stream:
+                result += chunk.choices[0].delta.content
+                print(chunk.choices[0].delta.content, end='')
+
+            os.environ["OPENAI_API_KEY"] = temp_open_ai_api_key
             return result
 
         except Exception as e:
-            print("Error in Module")
+            print("Error in Module: " + str(e))
             raise Exception(e)
 
 
 # We build an example here that we can call by either calling this file directly from the main directory,
 # or by adding it to our playground. You can call the example and adjust it to your needs or redefine it in the
 # playground or elsewhere
 def build_example(name, identifier, admin_config):
     dvm_config = build_default_config(identifier)
+    dvm_config.SEND_FEEDBACK_EVENTS = True
     admin_config.LUD16 = dvm_config.LN_ADDRESS
-    profit_in_sats = 10
-    cost_in_cent = 4.0
-    dvm_config.FIX_COST = int(((cost_in_cent / (get_price_per_sat("USD") * 100)) + profit_in_sats))
+
 
     nip89info = {
         "name": name,
-        "image": "https://image.nostr.build/c33ca6fc4cc038ca4adb46fdfdfda34951656f87ee364ef59095bae1495ce669.jpg",
-        "about": "I use Replicate to run StableDiffusion XL",
+        "image": "https://unleashed.chat/_app/immutable/assets/hero.pehsu4x_.jpeg",
+        "about": "I summarize Text with https://unleashed.chat",
         "encryptionSupported": True,
         "cashuAccepted": True,
         "nip90Params": {}
     }
 
     nip89config = NIP89Config()
     nip89config.DTAG = check_and_set_d_tag(identifier, name, dvm_config.PRIVATE_KEY, nip89info["image"])
     nip89config.CONTENT = json.dumps(nip89info)
+    admin_config2 = AdminConfig()
+    admin_config2.REBROADCAST_NIP89 = False
 
-    return VideoGenerationReplicateSVD(name=name, dvm_config=dvm_config, nip89config=nip89config,
-                                       admin_config=admin_config)
+    return SummarizationUnleashedChat(name=name, dvm_config=dvm_config, nip89config=nip89config, admin_config=admin_config2)
 
 
 if __name__ == '__main__':
-    process_venv(VideoGenerationReplicateSVD)
+    process_venv(SummarizationUnleashedChat)
+
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/tasks/videogeneration_svd.py` & `nostr-dvm-0.3.0/nostr_dvm/tasks/videogeneration_svd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import json
+import os
 from multiprocessing.pool import ThreadPool
 
+from nostr_sdk import Kind
+
 from nostr_dvm.backends.nova_server.utils import check_server_status, send_request_to_server
 from nostr_dvm.interfaces.dvmtaskinterface import DVMTaskInterface, process_venv
 from nostr_dvm.utils.admin_utils import AdminConfig
 from nostr_dvm.utils.dvmconfig import DVMConfig, build_default_config
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config, check_and_set_d_tag
 from nostr_dvm.utils.definitions import EventDefinitions
 
 """
 This File contains a module to transform an Image to a short Video Clip on n-server and receive results back. 
 
 Accepted Inputs: An url to an Image
 Outputs: An url to a video
 , 
 """
 
 
 class VideoGenerationSVD(DVMTaskInterface):
-    KIND: int = EventDefinitions.KIND_NIP90_GENERATE_VIDEO
+    KIND: Kind = EventDefinitions.KIND_NIP90_GENERATE_VIDEO
     TASK: str = "image-to-video"
     FIX_COST: float = 120
 
-    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config,
+    def __init__(self, name, dvm_config: DVMConfig, nip89config: NIP89Config, nip88config: NIP88Config = None,
                  admin_config: AdminConfig = None, options=None):
-        super().__init__(name, dvm_config, nip89config, admin_config, options)
+        super().__init__(name=name, dvm_config=dvm_config, nip89config=nip89config, nip88config=nip88config,
+                         admin_config=admin_config, options=options)
 
     def is_input_supported(self, tags, client=None, dvm_config=None):
         for tag in tags:
             if tag.as_vec()[0] == 'i':
                 input_value = tag.as_vec()[1]
                 input_type = tag.as_vec()[2]
                 if input_type != "url":
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/utils/admin_utils.py` & `nostr-dvm-0.3.0/nostr_dvm/utils/admin_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 # ADMINISTRARIVE DB MANAGEMENT
 
 from nostr_sdk import Keys, PublicKey, Client
 
 from nostr_dvm.utils.database_utils import get_from_sql_table, list_db, delete_from_sql_table, update_sql_table, \
     get_or_add_user, clean_db
 from nostr_dvm.utils.dvmconfig import DVMConfig
-from nostr_dvm.utils.nip89_utils import nip89_announce_tasks, fetch_nip89_paramters_for_deletion
+from nostr_dvm.utils.nip88_utils import nip88_announce_tier, fetch_nip88_parameters_for_deletion, fetch_nip88_event, \
+    check_and_set_tiereventid_nip88
+from nostr_dvm.utils.nip89_utils import nip89_announce_tasks, fetch_nip89_parameters_for_deletion
 from nostr_dvm.utils.nostr_utils import update_profile
 
 
 class AdminConfig:
     REBROADCAST_NIP89: bool = False
+    REBROADCAST_NIP88: bool = False
     UPDATE_PROFILE: bool = False
     DELETE_NIP89: bool = False
+    DELETE_NIP88: bool = False
+    FETCH_NIP88: bool = False
     WHITELISTUSER: bool = False
     UNWHITELISTUSER: bool = False
     BLACKLISTUSER: bool = False
     DELETEUSER: bool = False
     LISTDATABASE: bool = False
     ClEANDB: bool = False
+    INDEX: str = "1"
 
-    USERNPUB: str = ""
-    LUD16: str = ""
+    USERNPUBS: list = []
 
     EVENTID: str = ""
     PRIVKEY: str = ""
 
 
 def admin_make_database_updates(adminconfig: AdminConfig = None, dvmconfig: DVMConfig = None, client: Client = None):
     # This is called on start of Server, Admin function to manually whitelist/blacklist/add balance/delete users
@@ -33,57 +38,74 @@
         return
 
     if not isinstance(adminconfig, AdminConfig):
         return
 
     if ((
             adminconfig.WHITELISTUSER is True or adminconfig.UNWHITELISTUSER is True or adminconfig.BLACKLISTUSER is True or adminconfig.DELETEUSER is True)
-            and adminconfig.USERNPUB == ""):
+            and adminconfig.USERNPUBS == []):
         return
 
     if adminconfig.UPDATE_PROFILE and (dvmconfig.NIP89 is None):
         return
 
     if adminconfig.DELETE_NIP89 and (adminconfig.EVENTID == "" or adminconfig.EVENTID == ""):
         return
 
     db = dvmconfig.DB
 
-    if str(adminconfig.USERNPUB).startswith("npub"):
-        publickey = PublicKey.from_bech32(adminconfig.USERNPUB).to_hex()
-    else:
-        publickey = adminconfig.USERNPUB
-
-    if adminconfig.WHITELISTUSER:
-        user = get_or_add_user(db, publickey, client=client, config=dvmconfig)
-        update_sql_table(db, user.npub, user.balance, True, False, user.nip05, user.lud16, user.name, user.lastactive)
-        user = get_from_sql_table(db, publickey)
-        print(str(user.name) + " is whitelisted: " + str(user.iswhitelisted))
-
-    if adminconfig.UNWHITELISTUSER:
-        user = get_from_sql_table(db, publickey)
-        update_sql_table(db, user.npub, user.balance, False, False, user.nip05, user.lud16, user.name, user.lastactive)
-
-    if adminconfig.BLACKLISTUSER:
-        user = get_from_sql_table(db, publickey)
-        update_sql_table(db, user.npub, user.balance, False, True, user.nip05, user.lud16, user.name, user.lastactive)
+    for npub in adminconfig.USERNPUBS:
+        if str(npub).startswith("npub"):
+            publickey = PublicKey.from_bech32(npub).to_hex()
+        else:
+            publickey = npub
+
+        if adminconfig.WHITELISTUSER:
+            user = get_or_add_user(db, publickey, client=client, config=dvmconfig)
+            update_sql_table(db, user.npub, user.balance, True, False, user.nip05, user.lud16, user.name, user.lastactive, user.subscribed)
+            user = get_from_sql_table(db, publickey)
+            print(str(user.name) + " is whitelisted: " + str(user.iswhitelisted))
+
+        if adminconfig.UNWHITELISTUSER:
+            user = get_from_sql_table(db, publickey)
+            update_sql_table(db, user.npub, user.balance, False, False, user.nip05, user.lud16, user.name, user.lastactive, user.subscribed)
+
+        if adminconfig.BLACKLISTUSER:
+            user = get_from_sql_table(db, publickey)
+            update_sql_table(db, user.npub, user.balance, False, True, user.nip05, user.lud16, user.name, user.lastactive, user.subscribed)
 
-    if adminconfig.DELETEUSER:
-        delete_from_sql_table(db, publickey)
+        if adminconfig.DELETEUSER:
+            delete_from_sql_table(db, publickey)
 
     if adminconfig.ClEANDB:
         clean_db(db)
 
     if adminconfig.LISTDATABASE:
         list_db(db)
 
     if adminconfig.REBROADCAST_NIP89:
         nip89_announce_tasks(dvmconfig, client=client)
 
+    if adminconfig.REBROADCAST_NIP88:
+        annotier_id = nip88_announce_tier(dvmconfig, client=client)
+        check_and_set_tiereventid_nip88(dvmconfig.IDENTIFIER, adminconfig.INDEX, annotier_id.to_hex())
+
     if adminconfig.DELETE_NIP89:
         event_id = adminconfig.EVENTID
         keys = Keys.parse(
             adminconfig.PRIVKEY)  # Private key from sender of Event (e.g. the key of an nip89 announcement you want to delete)
-        fetch_nip89_paramters_for_deletion(keys, event_id, client, dvmconfig)
+        fetch_nip89_parameters_for_deletion(keys, event_id, client, dvmconfig)
+
+    if adminconfig.DELETE_NIP88:
+        event_id = adminconfig.EVENTID
+        keys = Keys.parse(
+            adminconfig.PRIVKEY)  # Private key from sender of Event (e.g. the key of an nip89 announcement you want to delete)
+        fetch_nip88_parameters_for_deletion(keys, event_id, client, dvmconfig)
+
+    if adminconfig.FETCH_NIP88:
+        event_id = adminconfig.EVENTID
+        keys = Keys.parse(
+            adminconfig.PRIVKEY)
+        fetch_nip88_event(keys, event_id, client, dvmconfig)
 
     if adminconfig.UPDATE_PROFILE:
-        update_profile(dvmconfig, client, lud16=adminconfig.LUD16)
+        update_profile(dvmconfig, client, lud16=dvmconfig.LN_ADDRESS)
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/utils/backend_utils.py` & `nostr-dvm-0.3.0/nostr_dvm/utils/backend_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 from nostr_dvm.utils.definitions import EventDefinitions
 from nostr_dvm.utils.mediasource_utils import check_source_type, media_source
 from nostr_dvm.utils.nostr_utils import get_event_by_id, get_referenced_event_by_id
 
 
 def get_task(event, client, dvm_config):
     try:
-        if event.kind() == EventDefinitions.KIND_NIP90_GENERIC:  # use this for events that have no id yet, inclufr j tag
+        if event.kind().as_u64() == EventDefinitions.KIND_NIP90_GENERIC.as_u64():  # use this for events that have no id yet, inclufr j tag
             for tag in event.tags():
                 if tag.as_vec()[0] == 'j':
                     return tag.as_vec()[1]
             else:
                 return "unknown job: " + event.as_json()
         elif event.kind() == EventDefinitions.KIND_DM:  # dm
             for tag in event.tags():
                 if tag.as_vec()[0] == 'j':
                     return tag.as_vec()[1]
             else:
                 return "unknown job: " + event.as_json()
 
         # This looks a bit more complicated, but we do several tasks for text-extraction in the future
-        elif event.kind() == EventDefinitions.KIND_NIP90_EXTRACT_TEXT:
+        elif event.kind().as_u64() == EventDefinitions.KIND_NIP90_EXTRACT_TEXT.as_u64():
             for tag in event.tags():
                 if tag.as_vec()[0] == "i":
                     if tag.as_vec()[2] == "url":
                         file_type = check_url_is_readable(tag.as_vec()[1])
                         print(file_type)
                         if file_type == "pdf":
                             return "pdf-to-text"
@@ -53,15 +53,15 @@
                                             return "speech-to-text"
                                         else:
                                             return "unknown job"
                             else:
                                 return "unknown type"
                     else:
                         return "unknown job"
-        elif event.kind() == EventDefinitions.KIND_NIP90_GENERATE_IMAGE:
+        elif event.kind().as_u64() == EventDefinitions.KIND_NIP90_GENERATE_IMAGE.as_u64():
             has_image_tag = False
             has_text_tag = False
             for tag in event.tags():
                 if tag.as_vec()[0] == "i":
                     if tag.as_vec()[2] == "url":
                         file_type = check_url_is_readable(tag.as_vec()[1])
                         if file_type == "image":
@@ -88,15 +88,15 @@
         #  TODO if a task can consist of multiple inputs add them here
         #  This is not ideal. Maybe such events should have their own kind
 
         #  else if kind is supported, simply return task
         else:
 
             for dvm in dvm_config.SUPPORTED_DVMS:
-                if dvm.KIND == event.kind():
+                if dvm.KIND.as_u64() == event.kind().as_u64():
                     return dvm.TASK
     except Exception as e:
         print("Get task: " + str(e))
 
     return "unknown type"
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/utils/cashu_utils.py` & `nostr-dvm-0.3.0/nostr_dvm/utils/cashu_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/utils/database_utils.py` & `nostr-dvm-0.3.0/nostr_dvm/utils/database_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 import sqlite3
 
 from _sqlite3 import Error
 from dataclasses import dataclass
 from datetime import timedelta
 from logging import Filter
 
-from nostr_sdk import Timestamp, Keys, PublicKey, EventBuilder, Filter
+from nostr_sdk import Timestamp, Keys, PublicKey, EventBuilder, Filter, Kind
 from nostr_dvm.utils.nostr_utils import send_event
 
 
 @dataclass
 class User:
     npub: str
     balance: int
     iswhitelisted: bool
     isblacklisted: bool
     name: str
     nip05: str
     lud16: str
     lastactive: int
+    subscribed: int
 
 
 def create_sql_table(db):
     try:
         import os
         if not os.path.exists(r'db'):
             os.makedirs(r'db')
@@ -36,59 +37,61 @@
                                             npub text PRIMARY KEY,
                                             sats integer NOT NULL,
                                             iswhitelisted boolean,
                                             isblacklisted boolean,
                                             nip05 text,
                                             lud16 text,
                                             name text,
-                                            lastactive integer
+                                            lastactive integer,
+                                            subscribed integer
                                         ); """)
         cur.execute("SELECT name FROM sqlite_master")
         con.close()
 
     except Error as e:
         print(e)
 
 
 def add_sql_table_column(db):
     try:
         con = sqlite3.connect(db)
         cur = con.cursor()
-        cur.execute(""" ALTER TABLE users ADD COLUMN lastactive 'integer' """)
+        cur.execute(""" ALTER TABLE users ADD COLUMN subscribed 'integer' """)
         con.close()
     except Error as e:
         print(e)
 
 
-def add_to_sql_table(db, npub, sats, iswhitelisted, isblacklisted, nip05, lud16, name, lastactive):
+def add_to_sql_table(db, npub, sats, iswhitelisted, isblacklisted, nip05, lud16, name, lastactive, subscribed):
     try:
         con = sqlite3.connect(db)
         cur = con.cursor()
-        data = (npub, sats, iswhitelisted, isblacklisted, nip05, lud16, name, lastactive)
-        cur.execute("INSERT or IGNORE INTO users VALUES(?, ?, ?, ?, ?, ?, ?, ?)", data)
+        data = (npub, sats, iswhitelisted, isblacklisted, nip05, lud16, name, lastactive, subscribed)
+        cur.execute("INSERT or IGNORE INTO users VALUES(?, ?, ?, ?, ?, ?, ?, ?, ?)", data)
         con.commit()
         con.close()
     except Error as e:
         print("Error when Adding to DB: " + str(e))
 
 
-def update_sql_table(db, npub, balance, iswhitelisted, isblacklisted, nip05, lud16, name, lastactive):
+def update_sql_table(db, npub, balance, iswhitelisted, isblacklisted, nip05, lud16, name, lastactive, subscribed):
     try:
         con = sqlite3.connect(db)
         cur = con.cursor()
-        data = (balance, iswhitelisted, isblacklisted, nip05, lud16, name, lastactive, npub)
+        data = (balance, iswhitelisted, isblacklisted, nip05, lud16, name, lastactive, subscribed, npub)
 
         cur.execute(""" UPDATE users
                   SET sats = ? ,
                       iswhitelisted = ? ,
                       isblacklisted = ? ,
                       nip05 = ? ,
                       lud16 = ? ,
                       name = ? ,
-                      lastactive = ?
+                      lastactive = ?,
+                      subscribed = ?
                   WHERE npub = ?""", data)
         con.commit()
         con.close()
     except Error as e:
         print("Error Updating DB: " + str(e))
 
 
@@ -98,23 +101,32 @@
         cur = con.cursor()
         cur.execute("SELECT * FROM users WHERE npub=?", (npub,))
         row = cur.fetchone()
         con.close()
         if row is None:
             return None
         else:
+
+            if len(row) < 9:
+                add_sql_table_column(db)
+                # Migrate 
+
+
             user = User
             user.npub = row[0]
             user.balance = row[1]
             user.iswhitelisted = row[2]
             user.isblacklisted = row[3]
             user.nip05 = row[4]
             user.lud16 = row[5]
             user.name = row[6]
             user.lastactive = row[7]
+            user.subscribed = row[8]
+            if user.subscribed is None:
+                user.subscribed = 0
 
             return user
 
     except Error as e:
         print("Error Getting from DB: " + str(e))
 
 
@@ -158,69 +170,103 @@
 
 
 def update_user_balance(db, npub, additional_sats, client, config):
     user = get_from_sql_table(db, npub)
     if user is None:
         name, nip05, lud16 = fetch_user_metadata(npub, client)
         add_to_sql_table(db, npub, (int(additional_sats) + config.NEW_USER_BALANCE), False, False,
-                         nip05, lud16, name, Timestamp.now().as_secs())
+                         nip05, lud16, name, Timestamp.now().as_secs(), 0)
         print("Adding User: " + npub + " (" + npub + ")")
     else:
         user = get_from_sql_table(db, npub)
         new_balance = int(user.balance) + int(additional_sats)
         update_sql_table(db, npub, new_balance, user.iswhitelisted, user.isblacklisted, user.nip05, user.lud16,
                          user.name,
-                         Timestamp.now().as_secs())
+                         Timestamp.now().as_secs(), user.subscribed)
         print("Updated user balance for: " + str(user.name) +
-              " Zap amount: " + str(additional_sats) + " Sats. New balance: " + str(new_balance) +" Sats")
+              " Zap amount: " + str(additional_sats) + " Sats. New balance: " + str(new_balance) + " Sats")
 
         if config is not None:
             keys = Keys.parse(config.PRIVATE_KEY)
-            #time.sleep(1.0)
+            # time.sleep(1.0)
 
-            message = ("Added " + str(additional_sats) + " Sats to balance. New balance is " + str(new_balance) + " Sats.")
+            message = ("Added " + str(additional_sats) + " Sats to balance. New balance is " + str(
+                new_balance) + " Sats.")
 
             evt = EventBuilder.encrypted_direct_msg(keys, PublicKey.from_hex(npub), message,
-                                                        None).to_event(keys)
+                                                    None).to_event(keys)
             send_event(evt, client=client, dvm_config=config)
 
 
-def get_or_add_user(db, npub, client, config, update=False):
+def update_user_subscription(npub, subscribed_until, client, dvm_config):
+    user = get_from_sql_table(dvm_config.DB, npub)
+    if user is None:
+        name, nip05, lud16 = fetch_user_metadata(npub, client)
+        add_to_sql_table(dvm_config.DB, npub, dvm_config.NEW_USER_BALANCE, False, False,
+                         nip05, lud16, name, Timestamp.now().as_secs(), 0)
+        print("Adding User: " + npub + " (" + npub + ")")
+    else:
+        user = get_from_sql_table(dvm_config.DB, npub)
+
+        update_sql_table(dvm_config.DB, npub, user.balance, user.iswhitelisted, user.isblacklisted, user.nip05,
+                         user.lud16,
+                         user.name,
+                         Timestamp.now().as_secs(), subscribed_until)
+        print("Updated user subscription for: " + str(user.name))
+
+        if dvm_config is not None:
+            keys = Keys.parse(dvm_config.PRIVATE_KEY)
+            # time.sleep(1.0)
+
+            message = ("Subscribed to DVM " + dvm_config.NIP89.NAME + " until: " + str(
+                Timestamp.from_secs(subscribed_until).to_human_datetime().replace("Z", " ").replace("T", " ")))
+
+            evt = EventBuilder.encrypted_direct_msg(keys, PublicKey.from_hex(npub), message,
+                                                    None).to_event(keys)
+            send_event(evt, client=client, dvm_config=dvm_config)
+
+
+def get_or_add_user(db, npub, client, config, update=False, skip_meta = False):
     user = get_from_sql_table(db, npub)
     if user is None:
         try:
-            name, nip05, lud16 = fetch_user_metadata(npub, client)
+            if skip_meta:
+                name = npub
+                nip05 = ""
+                lud16 = ""
+            else:
+                name, nip05, lud16 = fetch_user_metadata(npub, client)
             print("Adding User: " + npub + " (" + npub + ")")
             add_to_sql_table(db, npub, config.NEW_USER_BALANCE, False, False, nip05,
-                             lud16, name, Timestamp.now().as_secs())
+                             lud16, name, Timestamp.now().as_secs(), 0)
             user = get_from_sql_table(db, npub)
             return user
         except Exception as e:
             print("Error Adding User to DB: " + str(e))
     elif update:
         try:
             name, nip05, lud16 = fetch_user_metadata(npub, client)
             print("Updating User: " + npub + " (" + npub + ")")
             update_sql_table(db, user.npub, user.balance, user.iswhitelisted, user.isblacklisted, nip05,
-                             lud16, name, Timestamp.now().as_secs())
+                             lud16, name, Timestamp.now().as_secs(), user.subscribed)
             user = get_from_sql_table(db, npub)
             return user
         except Exception as e:
             print("Error Updating User in DB: " + str(e))
 
     return user
 
 
 def fetch_user_metadata(npub, client):
     name = ""
     nip05 = ""
     lud16 = ""
-    pk = PublicKey.from_hex(npub)
+    pk = PublicKey.parse(npub)
     print(f"\nGetting profile metadata for {pk.to_bech32()}...")
-    profile_filter = Filter().kind(0).author(pk).limit(1)
+    profile_filter = Filter().kind(Kind(0)).author(pk).limit(1)
     events = client.get_events_of([profile_filter], timedelta(seconds=1))
     if len(events) > 0:
         latest_entry = events[0]
         latest_time = 0
         try:
             for entry in events:
                 if entry.created_at().as_secs() > latest_time:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/utils/dvmconfig.py` & `nostr-dvm-0.3.0/nostr_dvm/utils/dvmconfig.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import os
 
 from nostr_sdk import Keys
 
+from nostr_dvm.utils.nip88_utils import NIP88Config
 from nostr_dvm.utils.nip89_utils import NIP89Config
 from nostr_dvm.utils.nostr_utils import check_and_set_private_key
 from nostr_dvm.utils.output_utils import PostProcessFunctionType
 from nostr_dvm.utils.zap_utils import check_and_set_ln_bits_keys
 
 
 class DVMConfig:
     SUPPORTED_DVMS = []
     PRIVATE_KEY: str = ""
     PUBLIC_KEY: str = ""
     FIX_COST: float = None
     PER_UNIT_COST: float = None
 
-
     RELAY_LIST = ["wss://relay.damus.io", "wss://nos.lol", "wss://nostr.wine",
                   "wss://nostr.mom", "wss://nostr.oxtr.dev", "wss://relay.nostr.bg",
                   "wss://relay.f7z.io", "wss://pablof7z.nostr1.com", "wss://relay.nostr.net", "wss://140.f7z.io",
-                  "wss://relay.snort.social", "wss://offchain.pub/", "wss://relay.nostr.band"]
+                  "wss://relay.snort.social", "wss://offchain.pub/"]
 
     RELAY_TIMEOUT = 5
     EXTERNAL_POST_PROCESS_TYPE = PostProcessFunctionType.NONE  # Leave this on None, except the DVM is external
-    LNBITS_INVOICE_KEY = '' # Will all automatically generated by default, or read from .env
+    LNBITS_INVOICE_KEY = ''  # Will all automatically generated by default, or read from .env
     LNBITS_ADMIN_KEY = ''  # In order to pay invoices, e.g. from the bot to DVMs, or reimburse users.
     LNBITS_URL = 'https://lnbits.com'
     LN_ADDRESS = ''
     SCRIPT = ''
     IDENTIFIER = ''
-    USE_OWN_VENV = True # Make an own venv for each dvm's process function.Disable if you want to install packages into main venv. Only recommended if you dont want to run dvms with different dependency versions
+    USE_OWN_VENV = True  # Make an own venv for each dvm's process function.Disable if you want to install packages into main venv. Only recommended if you dont want to run dvms with different dependency versions
     DB: str
     NEW_USER_BALANCE: int = 0  # Free credits for new users
+    NIP88: NIP88Config
     NIP89: NIP89Config
     SEND_FEEDBACK_EVENTS = True
     SHOW_RESULT_BEFORE_PAYMENT: bool = False  # if this is true show results even when not paid right after autoprocess
     SCHEDULE_UPDATES_SECONDS = 0
 
 
 def build_default_config(identifier):
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/utils/external_dvm_utils.py` & `nostr-dvm-0.3.0/nostr_dvm/utils/external_dvm_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/utils/mediasource_utils.py` & `nostr-dvm-0.3.0/nostr_dvm/utils/mediasource_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/utils/nip89_utils.py` & `nostr-dvm-0.3.0/nostr_dvm/utils/nip89_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 def nip89_create_d_tag(name, pubkey, image):
     key_str = str(name + image + pubkey)
     d_tag = sha256(key_str.encode('utf-8')).hexdigest()[:16]
     return d_tag
 
 
 def nip89_announce_tasks(dvm_config, client):
-    k_tag = Tag.parse(["k", str(dvm_config.NIP89.KIND)])
+    k_tag = Tag.parse(["k", str(dvm_config.NIP89.KIND.as_u64())])
     d_tag = Tag.parse(["d", dvm_config.NIP89.DTAG])
     keys = Keys.parse(dvm_config.NIP89.PK)
     content = dvm_config.NIP89.CONTENT
     event = EventBuilder(EventDefinitions.KIND_ANNOUNCEMENT, content, [k_tag, d_tag]).to_event(keys)
     send_event(event, client=client, dvm_config=dvm_config)
     print("Announced NIP 89 for " + dvm_config.NIP89.NAME)
 
 
-def fetch_nip89_paramters_for_deletion(keys, eventid, client, dvmconfig):
+def fetch_nip89_parameters_for_deletion(keys, eventid, client, dvmconfig):
     idfilter = Filter().id(EventId.from_hex(eventid)).limit(1)
     nip89events = client.get_events_of([idfilter], timedelta(seconds=dvmconfig.RELAY_TIMEOUT))
     d_tag = ""
     if len(nip89events) == 0:
         print("Event not found. Potentially gone.")
 
     for event in nip89events:
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/utils/nostr_utils.py` & `nostr-dvm-0.3.0/nostr_dvm/utils/nostr_utils.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/utils/nwc_tools.py` & `nostr-dvm-0.3.0/nostr_dvm/utils/nwc_tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,88 @@
 import json
 import os
+from datetime import timedelta
 
 import requests
-from nostr_sdk import Keys, PublicKey, Client, nip04_encrypt, EventBuilder, Tag, NostrSigner
+from nostr_sdk import Keys, PublicKey, Client, nip04_encrypt, EventBuilder, Tag, NostrSigner, Filter, Timestamp, \
+    NostrWalletConnectUri, Nwc
 
 from nostr_dvm.utils.dvmconfig import DVMConfig
 from nostr_dvm.utils.nostr_utils import check_and_set_private_key
 from nostr_dvm.utils.zap_utils import zaprequest
 
 
-def nwc_zap(connectionstr, bolt11, keys):
-    target_pubkey, relay, secret = parse_connection_str(connectionstr)
-    SecretSK = Keys.parse(secret)
-
-    content = {
-        "method": "pay_invoice",
-        "params": {
-            "invoice": bolt11
-        }
-    }
-
-    signer = NostrSigner.keys(keys)
-    client = Client(signer)
-    client.add_relay(relay)
-    client.connect()
-
-    client_public_key = PublicKey.from_hex(target_pubkey)
-    encrypted_content = nip04_encrypt(SecretSK.secret_key(), client_public_key, json.dumps(content))
-
-    pTag = Tag.parse(["p", client_public_key.to_hex()])
-    event = EventBuilder(23194, encrypted_content,
-                         [pTag]).to_event(keys)
+def nwc_zap(connectionstr, bolt11, keys, externalrelay=None):
+    uri = NostrWalletConnectUri.parse(connectionstr)
 
-    event_id = client.send_event(event)
-    print(event_id.to_hex())
+    # Initialize NWC client
+    nwc = Nwc(uri)
+
+    info = nwc.get_info()
+    print(info)
+
+    balance = nwc.get_balance()
+    print(f"Balance: {balance} SAT")
+
+    event_id = nwc.pay_invoice(bolt11)
+    print("NWC event: " + event_id)
+
+
+    #target_pubkey, relay, secret = parse_connection_str(connectionstr)
+    #print(target_pubkey)
+    #print(relay)
+    #print(secret)
+    #SecretSK = Keys.parse(secret)
+
+    #content = {
+    #    "method": "pay_invoice",
+    #    "params": {
+    #        "invoice": bolt11
+    #    }
+    #}
+
+    #signer = NostrSigner.keys(keys)
+    #client = Client(signer)
+    #client.add_relay(relay)
+    #if externalrelay is not None:
+    #    client.add_relay(externalrelay)
+
+    #client.connect()
+
+    #client_public_key = PublicKey.from_hex(target_pubkey)
+    #encrypted_content = nip04_encrypt(SecretSK.secret_key(), client_public_key, json.dumps(content))
+
+    #pTag = Tag.parse(["p", client_public_key.to_hex()])
+
+    #event = EventBuilder(23194, encrypted_content,
+    #                     [pTag]).to_event(keys)
+
+    #ts = Timestamp.now()
+    #event_id = client.send_event(event)
+
+
+
+
+
+
+    #nwc_response_filter = Filter().kind(23195).since(ts)
+    #events = client.get_events_of([nwc_response_filter], timedelta(seconds=5))
+
+    #if len(events) > 0:
+    #    for evt in events:
+    #        print(evt.as_json())
+    #else:
+    #    print("No response found")
+
+    return event_id
 
 
 def parse_connection_str(connectionstring):
     split = connectionstring.split("?")
-    targetpubkey = split[0].split(":")[1]
+    targetpubkey = split[0].split(":")[1].replace("//", "")
     split2 = split[1].split("&")
     relay = split2[0].split("=")[1]
     relay = relay.replace("%3A%2F%2F", "://")
     secret = split2[1].split("=")[1]
     return targetpubkey, relay, secret
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/utils/output_utils.py` & `nostr-dvm-0.3.0/nostr_dvm/utils/output_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -182,16 +182,20 @@
                 raise Exception("Upload not possible, all hosters didn't work or couldn't generate output")
 
 
 def build_status_reaction(status, task, amount, content, dvm_config):
     alt_description = "This is a reaction to a NIP90 DVM AI task. "
 
     if status == "processing":
-        alt_description = "NIP90 DVM AI task " + task + " started processing. "
-        reaction = alt_description + emoji.emojize(":thumbs_up:")
+        if content is not None and content != "":
+            alt_description = content
+            reaction = alt_description
+        else:
+            alt_description = "NIP90 DVM AI task " + task + " started processing. "
+            reaction = alt_description + emoji.emojize(":thumbs_up:")
     elif status == "success":
         alt_description = "NIP90 DVM AI task " + task + " finished successfully. "
         reaction = alt_description + emoji.emojize(":call_me_hand:")
     elif status == "chain-scheduled":
         alt_description = "NIP90 DVM AI task " + task + " Chain Task scheduled"
         reaction = alt_description + emoji.emojize(":thumbs_up:")
     elif status == "error":
@@ -202,14 +206,25 @@
             reaction = alt_description + emoji.emojize(":thumbs_down:") + " " + content
 
     elif status == "payment-required":
         alt_description = "NIP90 DVM AI task " + task + " requires payment of min " + str(
             amount) + " Sats. "
         reaction = alt_description + emoji.emojize(":orange_heart:")
 
+    elif status == "subscription-required":
+        if content is not None and content != "":
+            alt_description = content
+            reaction = alt_description
+
+        else:
+            alt_description = "NIP90 DVM AI task " + task + " requires payment for subscription"
+            reaction = alt_description + emoji.emojize(":orange_heart:")
+
+
+
     elif status == "payment-rejected":
         alt_description = "NIP90 DVM AI task " + task + " payment is below required amount of " + str(
             amount) + " Sats. "
         reaction = alt_description + emoji.emojize(":thumbs_down:")
     elif status == "user-blocked-from-service":
         alt_description = "NIP90 DVM AI task " + task + " can't be performed. User has been blocked from Service. "
         reaction = alt_description + emoji.emojize(":thumbs_down:")
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm/utils/scrapper/media_scrapper.py` & `nostr-dvm-0.3.0/nostr_dvm/utils/scrapper/media_scrapper.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/nostr_dvm/utils/zap_utils.py` & `nostr-dvm-0.3.0/nostr_dvm/utils/zap_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import urllib.parse
 from pathlib import Path
 
 import requests
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad
 from bech32 import bech32_decode, convertbits, bech32_encode
-from nostr_sdk import nostr_sdk, PublicKey, SecretKey, Event, EventBuilder, Tag, Keys, generate_shared_key
+from nostr_sdk import nostr_sdk, PublicKey, SecretKey, Event, EventBuilder, Tag, Keys, generate_shared_key, Kind
 
 from nostr_dvm.utils.nostr_utils import get_event_by_id, check_and_decrypt_own_tags
 import lnurl
 from hashlib import sha256
 import dotenv
 
 # TODO tor connection to lnbits
@@ -46,15 +46,15 @@
                 if z_tag.as_vec()[0] == 'anon':
                     if len(z_tag.as_vec()) > 1:
                         # print("[" + name + "] Private Zap received.")
                         decrypted_content = decrypt_private_zap_message(z_tag.as_vec()[1],
                                                                         keys.secret_key(),
                                                                         zap_request_event.author())
                         decrypted_private_event = Event.from_json(decrypted_content)
-                        if decrypted_private_event.kind() == 9733:
+                        if decrypted_private_event.kind().as_u64() == 9733:
                             sender = decrypted_private_event.author().to_hex()
                             message = decrypted_private_event.content()
                             # if message != "":
                             #    print("Zap Message: " + message)
                     else:
                         anon = True
                         print(
@@ -128,15 +128,15 @@
         print("LUD16: " + e)
         return None
 
 
 def create_lnbits_account(name):
     if os.getenv("LNBITS_ADMIN_ID") is None or os.getenv("LNBITS_ADMIN_ID") == "":
         print("No admin id set, no wallet created.")
-        return "","","","", "failed"
+        return "", "", "", "", "failed"
     data = {
         'admin_id': os.getenv("LNBITS_ADMIN_ID"),
         'wallet_name': name,
         'user_name': name,
     }
     try:
         json_object = json.dumps(data)
@@ -236,61 +236,66 @@
         decoded = plaintext.rsplit("}", 1)[0] + "}"  # weird symbols at the end
         return decoded
     except Exception as ex:
         return str(ex)
 
 
 def zaprequest(lud16: str, amount: int, content, zapped_event, zapped_user, keys, relay_list, zaptype="public"):
+    print(lud16)
+    print(str(amount))
+    print(content)
+    print(zapped_user.to_hex())
     if lud16.startswith("LNURL") or lud16.startswith("lnurl"):
         url = lnurl.decode(lud16)
     elif '@' in lud16:  # LNaddress
         url = 'https://' + str(lud16).split('@')[1] + '/.well-known/lnurlp/' + str(lud16).split('@')[0]
     else:  # No lud16 set or format invalid
         return None
     try:
         response = requests.get(url)
         ob = json.loads(response.content)
         callback = ob["callback"]
+        print(ob["callback"])
         encoded_lnurl = lnurl.encode(url)
         amount_tag = Tag.parse(['amount', str(amount * 1000)])
         relays_tag = Tag.parse(['relays', str(relay_list)])
         lnurl_tag = Tag.parse(['lnurl', encoded_lnurl])
         if zapped_event is not None:
             p_tag = Tag.parse(['p', zapped_event.author().to_hex()])
             e_tag = Tag.parse(['e', zapped_event.id().to_hex()])
             tags = [amount_tag, relays_tag, p_tag, e_tag, lnurl_tag]
         else:
             p_tag = Tag.parse(['p', zapped_user.to_hex()])
             tags = [amount_tag, relays_tag, p_tag, lnurl_tag]
 
-
         if zaptype == "private":
             key_str = keys.secret_key().to_hex() + zapped_event.id().to_hex() + str(zapped_event.created_at().as_secs())
             encryption_key = sha256(key_str.encode('utf-8')).hexdigest()
 
-            zap_request = EventBuilder(9733, content,
+            zap_request = EventBuilder(Kind(9733), content,
                                        [p_tag, e_tag]).to_event(keys).as_json()
             keys = Keys.parse(encryption_key)
             encrypted_content = enrypt_private_zap_message(zap_request, keys.secret_key(), zapped_event.author())
             anon_tag = Tag.parse(['anon', encrypted_content])
             tags.append(anon_tag)
             content = ""
 
-        zap_request = EventBuilder(9734, content,
+        zap_request = EventBuilder(Kind(9734), content,
                                    tags).to_event(keys).as_json()
 
         response = requests.get(callback + "?amount=" + str(int(amount) * 1000) + "&nostr=" + urllib.parse.quote_plus(
             zap_request) + "&lnurl=" + encoded_lnurl)
         ob = json.loads(response.content)
         return ob["pr"]
 
     except Exception as e:
         print("ZAP REQUEST: " + e)
         return None
 
+
 def get_price_per_sat(currency):
     import requests
 
     url = "https://openapiv1.coinstats.app/coins/bitcoin"
     params = {"skip": 0, "limit": 1, "currency": currency}
     price_currency_per_sat = 0.0004
     if os.getenv("COINSTATSOPENAPI_KEY"):
@@ -330,16 +335,14 @@
         if obj.get("ok"):
             return identifier + "@" + nostdressdomain, obj["pin"]
     except Exception as e:
         print(e)
         return "", ""
 
 
-
-
 def check_and_set_ln_bits_keys(identifier, npub):
     if not os.getenv("LNBITS_INVOICE_KEY_" + identifier.upper()):
         invoicekey, adminkey, walletid, userid, success = create_lnbits_account(identifier)
         add_key_to_env_file("LNBITS_INVOICE_KEY_" + identifier.upper(), invoicekey)
         add_key_to_env_file("LNBITS_ADMIN_KEY_" + identifier.upper(), adminkey)
         add_key_to_env_file("LNBITS_USER_ID_" + identifier.upper(), userid)
         add_key_to_env_file("LNBITS_WALLET_ID_" + identifier.upper(), userid)
@@ -361,8 +364,8 @@
                 os.getenv("LNADDRESS_" + identifier.upper()))
 
 
 def add_key_to_env_file(value, oskey):
     env_path = Path('.env')
     if env_path.is_file():
         dotenv.load_dotenv(env_path, verbose=True, override=True)
-        dotenv.set_key(env_path, value, oskey)
+        dotenv.set_key(env_path, value, oskey)
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm.egg-info/PKG-INFO` & `nostr-dvm-0.3.0/nostr_dvm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nostr-dvm
-Version: 0.2.6
+Version: 0.3.0
 Summary: A framework to build and run Nostr NIP90 Data Vending Machines
 Home-page: https://github.com/believethehype/nostrdvm
 Author: Believethehype
 Author-email: believethehypeonnostr@proton.me
 License: MIT
 Keywords: nostr,nip90,dvm,data vending machine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
-Requires-Dist: nostr-sdk==0.9.1
+Requires-Dist: nostr-sdk==0.10.0
 Requires-Dist: bech32
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: emoji==2.8.0
 Requires-Dist: eva-decord==0.6.1
 Requires-Dist: ffmpegio==0.8.5
 Requires-Dist: lnurl
```

### Comparing `nostr-dvm-0.2.6/nostr_dvm.egg-info/SOURCES.txt` & `nostr-dvm-0.3.0/nostr_dvm.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 nostr_dvm/__init__.py
 nostr_dvm/bot.py
 nostr_dvm/dvm.py
+nostr_dvm/subscription.py
 nostr_dvm.egg-info/PKG-INFO
 nostr_dvm.egg-info/SOURCES.txt
 nostr_dvm.egg-info/dependency_links.txt
 nostr_dvm.egg-info/requires.txt
 nostr_dvm.egg-info/top_level.txt
 nostr_dvm/backends/__init__.py
 nostr_dvm/backends/mlx/__init__.py
@@ -39,49 +40,54 @@
 nostr_dvm/backends/nova_server/modules/whisperx/version.py
 nostr_dvm/backends/nova_server/modules/whisperx/whisperx_transcript.py
 nostr_dvm/interfaces/__init__.py
 nostr_dvm/interfaces/dvmtaskinterface.py
 nostr_dvm/tasks/__init__.py
 nostr_dvm/tasks/advanced_search.py
 nostr_dvm/tasks/advanced_search_wine.py
+nostr_dvm/tasks/content_discovery_currently_popular.py
 nostr_dvm/tasks/convert_media.py
 nostr_dvm/tasks/discovery_inactive_follows.py
 nostr_dvm/tasks/discovery_nonfollowers.py
+nostr_dvm/tasks/discovery_relevant_notes.py
+nostr_dvm/tasks/discovery_trending_notes_nostrband.py
 nostr_dvm/tasks/imagegeneration_openai_dalle.py
 nostr_dvm/tasks/imagegeneration_replicate_sdxl.py
 nostr_dvm/tasks/imagegeneration_sd21_mlx.py
 nostr_dvm/tasks/imagegeneration_sdxl.py
 nostr_dvm/tasks/imagegeneration_sdxlimg2img.py
 nostr_dvm/tasks/imageinterrogator.py
 nostr_dvm/tasks/imageupscale.py
 nostr_dvm/tasks/search_users.py
 nostr_dvm/tasks/summarization_huggingchat.py
+nostr_dvm/tasks/summarization_unleashed_chat.py
 nostr_dvm/tasks/textextraction_google.py
 nostr_dvm/tasks/textextraction_pdf.py
 nostr_dvm/tasks/textextraction_whisperx.py
 nostr_dvm/tasks/textgeneration_huggingchat.py
 nostr_dvm/tasks/textgeneration_llmlite.py
 nostr_dvm/tasks/textgeneration_unleashed_chat.py
 nostr_dvm/tasks/texttospeech.py
 nostr_dvm/tasks/translation_google.py
 nostr_dvm/tasks/translation_libretranslate.py
-nostr_dvm/tasks/trending_notes_nostrband.py
 nostr_dvm/tasks/videogeneration_replicate_svd.py
 nostr_dvm/tasks/videogeneration_svd.py
 nostr_dvm/utils/__init__.py
 nostr_dvm/utils/admin_utils.py
 nostr_dvm/utils/backend_utils.py
 nostr_dvm/utils/cashu_utils.py
 nostr_dvm/utils/database_utils.py
 nostr_dvm/utils/definitions.py
 nostr_dvm/utils/dvmconfig.py
 nostr_dvm/utils/external_dvm_utils.py
 nostr_dvm/utils/mediasource_utils.py
+nostr_dvm/utils/nip88_utils.py
 nostr_dvm/utils/nip89_utils.py
 nostr_dvm/utils/nostr_utils.py
 nostr_dvm/utils/nwc_tools.py
 nostr_dvm/utils/output_utils.py
+nostr_dvm/utils/subscription_utils.py
 nostr_dvm/utils/zap_utils.py
 nostr_dvm/utils/scrapper/__init__.py
 nostr_dvm/utils/scrapper/media_scrapper.py
 tests/test_dvm_client.py
 tests/test_events.py
```

### Comparing `nostr-dvm-0.2.6/setup.py` & `nostr-dvm-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.6'
+VERSION = '0.3.0'
 DESCRIPTION = 'A framework to build and run Nostr NIP90 Data Vending Machines'
 LONG_DESCRIPTION = ('A framework to build and run Nostr NIP90 Data Vending Machines. '
                     'This is an early stage release. Interfaces might change/brick')
 
 # Setting up
 setup(
     name="nostr-dvm",
     version=VERSION,
     author="Believethehype",
     author_email="believethehypeonnostr@proton.me",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(include=['nostr_dvm', 'nostr_dvm.*']),
 
-    install_requires=["nostr-sdk==0.9.1",
+    install_requires=["nostr-sdk==0.10.0",
                       "bech32",
                       "pycryptodome==3.20.0",
                       "python-dotenv==1.0.0",
                       "emoji==2.8.0",
                       "eva-decord==0.6.1",
                       "ffmpegio==0.8.5",
                       "lnurl",
```

### Comparing `nostr-dvm-0.2.6/tests/test_dvm_client.py` & `nostr-dvm-0.3.0/tests/test_dvm_client.py`

 * *Files identical despite different names*

### Comparing `nostr-dvm-0.2.6/tests/test_events.py` & `nostr-dvm-0.3.0/tests/test_events.py`

 * *Files identical despite different names*

