# Comparing `tmp/ytdl-sub-2024.4.1.tar.gz` & `tmp/ytdl-sub-2024.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-sub-2024.4.1.tar", last modified: Mon Apr  1 11:25:38 2024, max compression
+gzip compressed data, was "ytdl-sub-2024.4.3.tar", last modified: Wed Apr  3 00:34:23 2024, max compression
```

## Comparing `ytdl-sub-2024.4.1.tar` & `ytdl-sub-2024.4.3.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.046893 ytdl-sub-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-04-01 11:25:38.046893 ytdl-sub-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-01 11:25:38.046893 ytdl-sub-2024.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.014893 ytdl-sub-2024.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.018893 ytdl-sub-2024.4.1/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 11:25:22.000000 ytdl-sub-2024.4.1/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.018893 ytdl-sub-2024.4.1/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/cli/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/cli/output_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/cli/output_transaction_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.018893 ytdl-sub-2024.4.1/src/ytdl_sub/cli/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/cli/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/cli/parsers/dl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/cli/parsers/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.022893 ytdl-sub-2024.4.1/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.022893 ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/plugin_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/plugin_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/preset_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.022893 ytdl-sub-2024.4.1/src/ytdl_sub/config/validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/validators/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/config/validators/variable_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.022893 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.022893 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/source_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.022893 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.022893 ytdl-sub-2024.4.1/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.026893 ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/custom_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/function_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    42267 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/variable_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/variable_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.026893 ytdl-sub-2024.4.1/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/entries/variables/override_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.030893 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/embed_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/file_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/filter_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/filter_include.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.030893 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/throttle_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.030893 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.030893 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    23681 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/url.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.030893 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.030893 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/singles.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.030893 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music_videos/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music_videos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.034893 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    34839 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.034893 ytdl-sub-2024.4.1/src/ytdl_sub/script/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.034893 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/array_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/boolean_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/conditional_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/date_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/json_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/map_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/numeric_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/regex_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/string_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21401 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22535 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/script_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.038893 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/resolvable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/syntax_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/types/variable_dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.038893 ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/exception_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/name_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/type_checking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.038893 ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    16254 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.038893 ytdl-sub-2024.4.1/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.042893 ytdl-sub-2024.4.1/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/scriptable.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.042893 ytdl-sub-2024.4.1/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.042893 ytdl-sub-2024.4.1/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-04-01 11:25:21.000000 ytdl-sub-2024.4.1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:25:38.042893 ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-04-01 11:25:37.000000 ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-04-01 11:25:38.000000 ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:25:37.000000 ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 11:25:37.000000 ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-01 11:25:37.000000 ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 11:25:37.000000 ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.359598 ytdl-sub-2024.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-04-03 00:34:23.359598 ytdl-sub-2024.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-03 00:34:23.359598 ytdl-sub-2024.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.327597 ytdl-sub-2024.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.331597 ytdl-sub-2024.4.3/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.331597 ytdl-sub-2024.4.3/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/output_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/output_transaction_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.331597 ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/dl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/preset_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/variable_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/source_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.335597 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20678 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.339598 ytdl-sub-2024.4.3/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.339598 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6896 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/custom_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/function_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42267 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/variable_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/variable_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.339598 ytdl-sub-2024.4.3/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/entries/variables/override_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/embed_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/file_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/filter_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/filter_include.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/throttle_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    23681 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/url.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/singles.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.343598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.347598 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34839 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.347598 ytdl-sub-2024.4.3/src/ytdl_sub/script/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.347598 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/boolean_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/conditional_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/json_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/numeric_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/regex_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/string_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21712 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22535 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/script_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.347598 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/resolvable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/syntax_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/types/variable_dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.351598 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/exception_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/name_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/type_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.351598 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16254 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.351598 ytdl-sub-2024.4.3/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.355598 ytdl-sub-2024.4.3/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/scriptable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.355598 ytdl-sub-2024.4.3/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.355598 ytdl-sub-2024.4.3/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-04-03 00:34:05.000000 ytdl-sub-2024.4.3/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:34:23.355598 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 00:34:23.000000 ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl-sub-2024.4.1/LICENSE` & `ytdl-sub-2024.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/PKG-INFO` & `ytdl-sub-2024.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2024.4.1
+Version: 2024.4.3
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2024.4.1/README.md` & `ytdl-sub-2024.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/pyproject.toml` & `ytdl-sub-2024.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/setup.cfg` & `ytdl-sub-2024.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/cli/entrypoint.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/cli/output_summary.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/cli/output_summary.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/cli/output_transaction_log.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/cli/output_transaction_log.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/cli/parsers/dl.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/dl.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/cli/parsers/main.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/cli/parsers/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/config/config_file.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/config/config_validator.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/config/defaults.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/config/overrides.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/overrides.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/plugin.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/plugin_mapping.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/plugin_mapping.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/config/plugin/preset_plugins.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/plugin/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/config/preset.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/preset.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/config/preset_options.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/config/validators/options.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/config/validators/variable_validation.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/config/validators/variable_validation.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/source_plugin.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/source_plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/url/validators.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/url/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,16 @@
                 uid: "banner_uncropped"
               - name: "season{season_index}-poster.jpg"
                 uid: "latest_entry"
           - url: "https://www.youtube.com/playlist?list=UCsvn_Po0SmunchJYtttWpOxMg"
             variables:
               season_index: "2"
               season_name: "Playlist as Season"
+            ytdl_options:
+              break_on_existing: False
             playlist_thumbnails:
               - name: "season{season_index}-poster.jpg"
                 uid: "latest_entry"
     """
 
     @classmethod
     def partial_validate(cls, name: str, value: Any) -> None:
```

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/entries/base_entry.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/entries/entry.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/entries/entry_parent.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/custom_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/custom_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/function_scripts.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/function_scripts.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/variable_definitions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/variable_definitions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/entries/script/variable_types.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/script/variable_types.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/entries/variables/override_variables.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/entries/variables/override_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/main.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/audio_extract.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/chapters.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/date_range.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/embed_thumbnail.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/embed_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/file_convert.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/filter_exclude.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/filter_exclude.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/filter_include.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/filter_include.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/format.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/format.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/internal/view.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/match_filters.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/music_tags.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/regex.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/subtitles.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/throttle_protection.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/throttle_protection.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/plugins/video_tags.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/players.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/players.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/url.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/url.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music/singles.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music/singles.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl-sub-2024.4.3/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/__init__.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/array_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/array_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/boolean_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/boolean_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/conditional_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/conditional_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/error_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/error_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/json_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/json_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/map_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/map_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/numeric_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/numeric_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/regex_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/regex_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/functions/string_functions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/functions/string_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/parser.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 
 CUSTOM_FUNCTION_ARGUMENTS_ONLY_ARGS = InvalidSyntaxException(
     "Custom function arguments can only be used as arguments to functions, maps, or arrays"
 )
 
 FUNCTION_INVALID_CHAR = InvalidSyntaxException("Invalid value when parsing a function")
 
+BRACKET_INVALID_CHAR = InvalidSyntaxException("Invalid value within brackets")
+
 
 def _UNEXPECTED_CHAR_ARGUMENT(arg_type: ParsedArgType):
     return InvalidSyntaxException(f"Unexpected character when parsing {arg_type.value} arguments")
 
 
 def _UNEXPECTED_COMMA_ARGUMENT(arg_type: ParsedArgType):
     return InvalidSyntaxException(f"Unexpected comma when parsing {arg_type.value} arguments")
@@ -501,14 +503,18 @@
 
                 output[key] = value_args[0]
                 key = None
             else:
                 raise UNREACHABLE
 
     def _parse_main_loop(self, ch: str) -> bool:
+        if ch == "\\" and self._read(increment_pos=False) in {"{", "}"}:
+            # Escape brackets are \{ and \}, only add the second char
+            self._literal_str += self._read()
+            return True
         if ch == "}":
             if self._bracket_counter == 0:
                 raise BRACKET_NOT_CLOSED
 
             del self._bracket_counter_pos_stack[-1]
             self._bracket_counter -= 1
             return True
@@ -554,17 +560,17 @@
             elif _is_custom_function_argument_start(self._read(increment_pos=False)):
                 raise CUSTOM_FUNCTION_ARGUMENTS_ONLY_ARGS
             else:
                 raise _UNEXPECTED_CHAR_ARGUMENT(arg_type=ParsedArgType.SCRIPT)
         elif self._bracket_counter == 0:
             # Only accumulate literal str if not in brackets
             self._literal_str += ch
-        else:
-            # Should only be possible to get here if it's a space
-            assert ch.isspace()
+        elif not ch.isspace():
+            self._set_highlight_position(pos=self._pos - 1)
+            raise BRACKET_INVALID_CHAR
 
         return True
 
     def _parse(self) -> SyntaxTree:
 
         while ch := self._read():
             continue_parse = self._parse_main_loop(ch)
```

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/script.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/script.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/script_output.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/script_output.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/types/array.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/array.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/types/function.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/function.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/types/map.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/map.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/types/resolvable.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/resolvable.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/types/syntax_tree.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/syntax_tree.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/types/variable.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/variable.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/types/variable_dependency.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/types/variable_dependency.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/exception_formatters.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/exception_formatters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/exceptions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/name_validation.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/name_validation.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/script/utils/type_checking.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/script/utils/type_checking.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription_validators.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/utils/chapters.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/utils/datetime.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/utils/exceptions.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/utils/ffmpeg.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/utils/file_handler.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/utils/file_lock.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/utils/file_path.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/file_path.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/utils/logger.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/utils/retry.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/retry.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,20 +30,22 @@
 
     def decorator(func):
         def newfn(*args, **kwargs):
             attempt = 0
             while attempt < times:
                 try:
                     return func(*args, **kwargs)
-                except exceptions:
+                except exceptions as exc:
                     logger.debug(
-                        "Exception thrown when attempting to run %s, attempt %d of %d",
+                        "Exception thrown when attempting to run %s, attempt %d of %d\n"
+                        "Exception:\n%s",
                         func.__name__,
                         attempt + 1,
                         times,
+                        str(exc),
                     )
                     attempt += 1
                     sleep(wait_sec)
             return None
 
         return newfn
```

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/utils/script.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/script.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/utils/scriptable.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/scriptable.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/utils/thumbnail.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/utils/xml.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/utils/yaml.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/validators/file_path_validators.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/validators/nfo_validators.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/validators/regex_validator.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/validators/string_datetime.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/validators/string_select_validator.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/validators/validators.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl-sub-2024.4.3/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2024.4.1
+Version: 2024.4.3
 Summary: Automate downloading and metadata generation with YoutubeDL
 Home-page: https://github.com/jmbannon/ytdl-sub
 Author: Jesse Bannon
 Author-email: use_github_issues@nope.com
 License: GNUv3
 Platform: Unix
 Classifier: Topic :: Multimedia :: Sound/Audio
```

### Comparing `ytdl-sub-2024.4.1/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl-sub-2024.4.3/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

