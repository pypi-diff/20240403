# Comparing `tmp/xklb-2.5.8.tar.gz` & `tmp/xklb-2.5.9.tar.gz`

## Comparing `xklb-2.5.8.tar` & `xklb-2.5.9.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.5.8/.gitattributes
--rw-r--r--   0        0        0   203078 2020-02-02 00:00:00.000000 xklb-2.5.8/pdm.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.5.8/.github/FUNDING.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.5.8/.github/LICENSE
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 xklb-2.5.8/.github/Windows.md
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.5.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.5.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.5.8/.github/examples/extract.svg
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.5.8/.github/examples/tubeadd.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.5.8/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 xklb-2.5.8/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/__init__.py
--rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/db_media.py
--rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/db_playlists.py
--rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/dl_extract.py
--rw-r--r--   0        0        0    16853 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/fs_extract.py
--rw-r--r--   0        0        0     8133 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/gdl_backend.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/gdl_extract.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/history.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/hn_extract.py
--rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/lb.py
--rw-r--r--   0        0        0    24696 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/play_actions.py
--rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/post_actions.py
--rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/readme.py
--rw-r--r--   0        0        0    13292 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/reddit_extract.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/rss_extract.py
--rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/search.py
--rw-r--r--   0        0        0     6810 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/site_extract.py
--rw-r--r--   0        0        0     6951 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/tabs_extract.py
--rw-r--r--   0        0        0    19687 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/tube_backend.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/tube_extract.py
--rw-r--r--   0        0        0   111312 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/usage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/data/__init__.py
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/data/dl_config.py
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/data/wordbank.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/media/__init__.py
--rw-r--r--   0        0        0     9165 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/media/av.py
--rw-r--r--   0        0        0     7484 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/media/books.py
--rw-r--r--   0        0        0    16296 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/media/dedupe.py
--rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/media/media_check.py
--rw-r--r--   0        0        0    23526 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/media/media_player.py
--rw-r--r--   0        0        0     9411 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/media/media_printer.py
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/media/subtitle.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scratch/__init__.py
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scratch/javguru.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scratch/javtiful.py
--rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scratch/mam_search.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scratch/mam_slots.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     8314 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/big_dirs.py
--rw-r--r--   0        0        0    12252 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/block.py
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/christen.py
--rw-r--r--   0        0        0    14173 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0    14120 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/dedupe_czkawka.py
--rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/disk_usage.py
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/eda.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/export_text.py
--rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/history.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/incremental_diff.py
--rw-r--r--   0        0        0    13991 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/links_db.py
--rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/mcda.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/merge_folders.py
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/move_list.py
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/open_links.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/places_import.py
--rw-r--r--   0        0        0     9972 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/process_audio.py
--rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/rel_mv.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/sample_compare.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/sample_hash.py
--rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/search_db.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/web_add.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     9591 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/mining/extract_text.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/mining/markdown_links.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/mining/substack.py
--rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/scripts/mining/tildes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/__init__.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/arg_utils.py
--rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/consts.py
--rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/db_utils.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/devices.py
--rw-r--r--   0        0        0    15155 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/file_utils.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/gui.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/iterables.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/log_utils.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/mpv_utils.py
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/nums.py
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/objects.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/path_utils.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/pd_utils.py
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/printing.py
--rw-r--r--   0        0        0     7347 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/processes.py
--rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/sql_utils.py
--rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/strings.py
--rw-r--r--   0        0        0    21269 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/utils/web.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.5.8/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 xklb-2.5.8/.gitignore
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 xklb-2.5.8/pyproject.toml
--rw-r--r--   0        0        0   149705 2020-02-02 00:00:00.000000 xklb-2.5.8/.github/README.md
--rw-r--r--   0        0        0   153466 2020-02-02 00:00:00.000000 xklb-2.5.8/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.5.9/.gitattributes
+-rw-r--r--   0        0        0   203078 2020-02-02 00:00:00.000000 xklb-2.5.9/pdm.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/LICENSE
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/Windows.md
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/examples/extract.svg
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/examples/tubeadd.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/__init__.py
+-rw-r--r--   0        0        0    18248 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/db_media.py
+-rw-r--r--   0        0        0     8230 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/db_playlists.py
+-rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/dl_extract.py
+-rw-r--r--   0        0        0    16853 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/fs_extract.py
+-rw-r--r--   0        0        0     8133 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/gdl_extract.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/history.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/hn_extract.py
+-rw-r--r--   0        0        0    13098 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/lb.py
+-rw-r--r--   0        0        0    24696 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/play_actions.py
+-rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/post_actions.py
+-rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/readme.py
+-rw-r--r--   0        0        0    13292 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/reddit_extract.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/rss_extract.py
+-rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/search.py
+-rw-r--r--   0        0        0     6810 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/site_extract.py
+-rw-r--r--   0        0        0     6951 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    19687 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/tube_backend.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/tube_extract.py
+-rw-r--r--   0        0        0   111452 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/usage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/data/__init__.py
+-rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/data/dl_config.py
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/data/wordbank.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/__init__.py
+-rw-r--r--   0        0        0     9165 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/av.py
+-rw-r--r--   0        0        0     7484 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/books.py
+-rw-r--r--   0        0        0    16296 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/dedupe.py
+-rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/media_check.py
+-rw-r--r--   0        0        0    23526 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/media_player.py
+-rw-r--r--   0        0        0     9411 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/media_printer.py
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/media/subtitle.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scratch/__init__.py
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scratch/javguru.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scratch/javtiful.py
+-rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scratch/mam_search.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scratch/mam_slots.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     8314 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/big_dirs.py
+-rw-r--r--   0        0        0    12252 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/christen.py
+-rw-r--r--   0        0        0    14173 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0    14120 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/dedupe_czkawka.py
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/disk_usage.py
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/eda.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/export_text.py
+-rw-r--r--   0        0        0     7920 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/history.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/incremental_diff.py
+-rw-r--r--   0        0        0    13991 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/links_db.py
+-rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mcda.py
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/merge_folders.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/open_links.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/places_import.py
+-rw-r--r--   0        0        0     9972 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/process_audio.py
+-rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/rel_mv.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/sample_compare.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/sample_hash.py
+-rw-r--r--   0        0        0    11797 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/search_db.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0    14110 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/web_add.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0     9591 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/extract_text.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/markdown_links.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/substack.py
+-rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/scripts/mining/tildes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/__init__.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/arg_utils.py
+-rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/consts.py
+-rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/db_utils.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/devices.py
+-rw-r--r--   0        0        0    15155 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/file_utils.py
+-rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/gui.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/iterables.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/log_utils.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/mpv_utils.py
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/nums.py
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/objects.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/path_utils.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/pd_utils.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/printing.py
+-rw-r--r--   0        0        0     7347 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/processes.py
+-rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/sql_utils.py
+-rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/strings.py
+-rw-r--r--   0        0        0    21269 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/utils/web.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.5.9/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 xklb-2.5.9/.gitignore
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 xklb-2.5.9/pyproject.toml
+-rw-r--r--   0        0        0   149845 2020-02-02 00:00:00.000000 xklb-2.5.9/.github/README.md
+-rw-r--r--   0        0        0   153606 2020-02-02 00:00:00.000000 xklb-2.5.9/PKG-INFO
```

### Comparing `xklb-2.5.8/pdm.lock` & `xklb-2.5.9/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1879,24 +1879,24 @@
 files = [
     {file = "requests-2.31.0-py3-none-any.whl", hash = "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f"},
     {file = "requests-2.31.0.tar.gz", hash = "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"},
 ]
 
 [[package]]
 name = "rich"
-version = "13.7.0"
+version = "13.7.1"
 requires_python = ">=3.7.0"
 summary = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
 dependencies = [
     "markdown-it-py>=2.2.0",
     "pygments<3.0.0,>=2.13.0",
 ]
 files = [
-    {file = "rich-13.7.0-py3-none-any.whl", hash = "sha256:6da14c108c4866ee9520bbffa71f6fe3962e193b7da68720583850cd4548e235"},
-    {file = "rich-13.7.0.tar.gz", hash = "sha256:5cb5123b5cf9ee70584244246816e9114227e0b98ad9176eede6ad54bf5403fa"},
+    {file = "rich-13.7.1-py3-none-any.whl", hash = "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222"},
+    {file = "rich-13.7.1.tar.gz", hash = "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"},
 ]
 
 [[package]]
 name = "ruff"
 version = "0.2.2"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter and code formatter, written in Rust."
```

### Comparing `xklb-2.5.8/.github/LICENSE` & `xklb-2.5.9/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/.github/Windows.md` & `xklb-2.5.9/.github/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-2.5.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-2.5.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/.github/examples/extract.svg` & `xklb-2.5.9/.github/examples/extract.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/.github/examples/tubeadd.svg` & `xklb-2.5.9/.github/examples/tubeadd.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/.github/workflows/push.yaml` & `xklb-2.5.9/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/db_media.py` & `xklb-2.5.9/xklb/db_media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/db_playlists.py` & `xklb-2.5.9/xklb/db_playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/dl_extract.py` & `xklb-2.5.9/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/fs_extract.py` & `xklb-2.5.9/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/gdl_backend.py` & `xklb-2.5.9/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/gdl_extract.py` & `xklb-2.5.9/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/history.py` & `xklb-2.5.9/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/hn_extract.py` & `xklb-2.5.9/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/lb.py` & `xklb-2.5.9/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/play_actions.py` & `xklb-2.5.9/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/post_actions.py` & `xklb-2.5.9/xklb/post_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/readme.py` & `xklb-2.5.9/xklb/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/reddit_extract.py` & `xklb-2.5.9/xklb/reddit_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/rss_extract.py` & `xklb-2.5.9/xklb/rss_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/search.py` & `xklb-2.5.9/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/site_extract.py` & `xklb-2.5.9/xklb/site_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/tabs_actions.py` & `xklb-2.5.9/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/tabs_extract.py` & `xklb-2.5.9/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/tube_backend.py` & `xklb-2.5.9/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/tube_extract.py` & `xklb-2.5.9/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/usage.py` & `xklb-2.5.9/xklb/usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -523,14 +523,17 @@
         To prevent confusion, normal post-actions will be skipped if the exit-code is greater than 4.
         Exit-codes 0, 1, 2, 3, and 4: the external post-action will run after normal post-actions. Be careful of conflicting player-exit-code command and post-action behavior when using these!
 
     Experimental options:
         Duration to play (in seconds) while changing the channel
         library {action} --interdimensional-cable 40
         library {action} -4dtv 40
+        You can open two terminals to replicate AMV Hell somewhat
+        library watch --volume 0 -4dtv 30
+        library listen -4dtv 30
 
         Playback multiple files at once
         library {action} --multiple-playback    # one per display; or two if only one display detected
         library {action} --multiple-playback 4  # play four media at once, divide by available screens
         library {action} -m 4 --screen-name eDP # play four media at once on specific screen
         library {action} -m 4 --loop --crop     # play four cropped videos on a loop
         library {action} -m 4 --hstack          # use hstack style
```

### Comparing `xklb-2.5.8/xklb/data/dl_config.py` & `xklb-2.5.9/xklb/data/dl_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 .*geo-restricted
 .*geolocation
 .*your country
 .*No such file or directory
 .*The downloaded file is empty
 .*Invalid data found
 .*fragment 1 not found
+.*Got error: 0 bytes read
 .*HTTP Error 429
 .*HTTP Error 400
 .*HTTP Error 503: Service Unavailable
 .*Origin Error
 .*API is not granting access
 .*Did not get any data blocks
 .*Too Many Requests
```

### Comparing `xklb-2.5.8/xklb/data/wordbank.py` & `xklb-2.5.9/xklb/data/wordbank.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/media/av.py` & `xklb-2.5.9/xklb/media/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/media/books.py` & `xklb-2.5.9/xklb/media/books.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/media/dedupe.py` & `xklb-2.5.9/xklb/media/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/media/media_check.py` & `xklb-2.5.9/xklb/media/media_check.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/media/media_player.py` & `xklb-2.5.9/xklb/media/media_player.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/media/media_printer.py` & `xklb-2.5.9/xklb/media/media_printer.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/media/subtitle.py` & `xklb-2.5.9/xklb/media/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scratch/javguru.py` & `xklb-2.5.9/xklb/scratch/javguru.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scratch/javtiful.py` & `xklb-2.5.9/xklb/scratch/javtiful.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scratch/mam_search.py` & `xklb-2.5.9/xklb/scratch/mam_search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scratch/mam_slots.py` & `xklb-2.5.9/xklb/scratch/mam_slots.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/big_dirs.py` & `xklb-2.5.9/xklb/scripts/big_dirs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/block.py` & `xklb-2.5.9/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/christen.py` & `xklb-2.5.9/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/cluster_sort.py` & `xklb-2.5.9/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/copy_play_counts.py` & `xklb-2.5.9/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/dedupe_czkawka.py` & `xklb-2.5.9/xklb/scripts/dedupe_czkawka.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/dedupe_db.py` & `xklb-2.5.9/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/disk_usage.py` & `xklb-2.5.9/xklb/scripts/disk_usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/download_status.py` & `xklb-2.5.9/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/eda.py` & `xklb-2.5.9/xklb/scripts/eda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/export_text.py` & `xklb-2.5.9/xklb/scripts/export_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/history.py` & `xklb-2.5.9/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/incremental_diff.py` & `xklb-2.5.9/xklb/scripts/incremental_diff.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/links_db.py` & `xklb-2.5.9/xklb/scripts/links_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/mcda.py` & `xklb-2.5.9/xklb/scripts/mcda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/merge_dbs.py` & `xklb-2.5.9/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/merge_folders.py` & `xklb-2.5.9/xklb/scripts/merge_folders.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/merge_online_local.py` & `xklb-2.5.9/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/move_list.py` & `xklb-2.5.9/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/open_links.py` & `xklb-2.5.9/xklb/scripts/open_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/optimize_db.py` & `xklb-2.5.9/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/places_import.py` & `xklb-2.5.9/xklb/scripts/places_import.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/playback_control.py` & `xklb-2.5.9/xklb/scripts/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/playlists.py` & `xklb-2.5.9/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/process_audio.py` & `xklb-2.5.9/xklb/scripts/process_audio.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/redownload.py` & `xklb-2.5.9/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/rel_mv.py` & `xklb-2.5.9/xklb/scripts/rel_mv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/sample_compare.py` & `xklb-2.5.9/xklb/scripts/sample_compare.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/sample_hash.py` & `xklb-2.5.9/xklb/scripts/sample_hash.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/scatter.py` & `xklb-2.5.9/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/search_db.py` & `xklb-2.5.9/xklb/scripts/search_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/streaming_tab_loader.py` & `xklb-2.5.9/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/web_add.py` & `xklb-2.5.9/xklb/scripts/web_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/mining/extract_links.py` & `xklb-2.5.9/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/mining/extract_text.py` & `xklb-2.5.9/xklb/scripts/mining/extract_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/mining/markdown_links.py` & `xklb-2.5.9/xklb/scripts/mining/markdown_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.5.9/xklb/scripts/mining/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/mining/nouns.py` & `xklb-2.5.9/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/mining/pushshift.py` & `xklb-2.5.9/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.5.9/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/mining/substack.py` & `xklb-2.5.9/xklb/scripts/mining/substack.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/scripts/mining/tildes.py` & `xklb-2.5.9/xklb/scripts/mining/tildes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/arg_utils.py` & `xklb-2.5.9/xklb/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/consts.py` & `xklb-2.5.9/xklb/utils/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/db_utils.py` & `xklb-2.5.9/xklb/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/devices.py` & `xklb-2.5.9/xklb/utils/devices.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/file_utils.py` & `xklb-2.5.9/xklb/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/gui.py` & `xklb-2.5.9/xklb/utils/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/iterables.py` & `xklb-2.5.9/xklb/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/log_utils.py` & `xklb-2.5.9/xklb/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/mpv_utils.py` & `xklb-2.5.9/xklb/utils/mpv_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/nums.py` & `xklb-2.5.9/xklb/utils/nums.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/objects.py` & `xklb-2.5.9/xklb/utils/objects.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/path_utils.py` & `xklb-2.5.9/xklb/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/pd_utils.py` & `xklb-2.5.9/xklb/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/printing.py` & `xklb-2.5.9/xklb/utils/printing.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/processes.py` & `xklb-2.5.9/xklb/utils/processes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/sql_utils.py` & `xklb-2.5.9/xklb/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/strings.py` & `xklb-2.5.9/xklb/utils/strings.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/utils/web.py` & `xklb-2.5.9/xklb/utils/web.py`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/xklb/assets/kotobago.png` & `xklb-2.5.9/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/.gitignore` & `xklb-2.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/pyproject.toml` & `xklb-2.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.5.8/.github/README.md` & `xklb-2.5.9/.github/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.5.008)
+    xk media library subcommands (v2.5.009)
 
     Create database subcommands:
     ╭───────────────┬────────────────────────────────────────────────────╮
     │ fsadd         │ Add local media                                    │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ tubeadd       │ Add online video media (yt-dlp)                    │
     ├───────────────┼────────────────────────────────────────────────────┤
@@ -1325,14 +1325,17 @@
         To prevent confusion, normal post-actions will be skipped if the exit-code is greater than 4.
         Exit-codes 0, 1, 2, 3, and 4: the external post-action will run after normal post-actions. Be careful of conflicting player-exit-code command and post-action behavior when using these!
 
     Experimental options:
         Duration to play (in seconds) while changing the channel
         library watch --interdimensional-cable 40
         library watch -4dtv 40
+        You can open two terminals to replicate AMV Hell somewhat
+        library watch --volume 0 -4dtv 30
+        library listen -4dtv 30
 
         Playback multiple files at once
         library watch --multiple-playback    # one per display; or two if only one display detected
         library watch --multiple-playback 4  # play four media at once, divide by available screens
         library watch -m 4 --screen-name eDP # play four media at once on specific screen
         library watch -m 4 --loop --crop     # play four cropped videos on a loop
         library watch -m 4 --hstack          # use hstack style
```

### Comparing `xklb-2.5.8/PKG-INFO` & `xklb-2.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 2.5.8
+Version: 2.5.9
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -179,15 +179,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.5.008)
+    xk media library subcommands (v2.5.009)
 
     Create database subcommands:
     ╭───────────────┬────────────────────────────────────────────────────╮
     │ fsadd         │ Add local media                                    │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ tubeadd       │ Add online video media (yt-dlp)                    │
     ├───────────────┼────────────────────────────────────────────────────┤
@@ -1413,14 +1413,17 @@
         To prevent confusion, normal post-actions will be skipped if the exit-code is greater than 4.
         Exit-codes 0, 1, 2, 3, and 4: the external post-action will run after normal post-actions. Be careful of conflicting player-exit-code command and post-action behavior when using these!
 
     Experimental options:
         Duration to play (in seconds) while changing the channel
         library watch --interdimensional-cable 40
         library watch -4dtv 40
+        You can open two terminals to replicate AMV Hell somewhat
+        library watch --volume 0 -4dtv 30
+        library listen -4dtv 30
 
         Playback multiple files at once
         library watch --multiple-playback    # one per display; or two if only one display detected
         library watch --multiple-playback 4  # play four media at once, divide by available screens
         library watch -m 4 --screen-name eDP # play four media at once on specific screen
         library watch -m 4 --loop --crop     # play four cropped videos on a loop
         library watch -m 4 --hstack          # use hstack style
```

