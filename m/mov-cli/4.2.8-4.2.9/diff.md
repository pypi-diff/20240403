# Comparing `tmp/mov-cli-4.2.8.tar.gz` & `tmp/mov-cli-4.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-4.2.8.tar", last modified: Mon Apr  1 04:21:29 2024, max compression
+gzip compressed data, was "mov-cli-4.2.9.tar", last modified: Wed Apr  3 20:55:36 2024, max compression
```

## Comparing `mov-cli-4.2.8.tar` & `mov-cli-4.2.9.tar`

### file list

```diff
@@ -1,56 +1,73 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:29.016891 mov-cli-4.2.8/
--rw-rw-rw-   0        0        0     1085 2024-03-31 20:57:09.000000 mov-cli-4.2.8/LICENSE
--rw-rw-rw-   0        0        0     7435 2024-04-01 04:21:29.015893 mov-cli-4.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     4720 2024-03-31 20:57:09.000000 mov-cli-4.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:28.971783 mov-cli-4.2.8/mov_cli/
--rw-rw-rw-   0        0        0      137 2024-04-01 04:16:45.000000 mov-cli-4.2.8/mov_cli/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:28.998413 mov-cli-4.2.8/mov_cli/cli/
--rw-rw-rw-   0        0        0       17 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/cli/__init__.py
--rw-rw-rw-   0        0        0     4992 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/cli/__main__.py
--rw-rw-rw-   0        0        0      479 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/cli/auto_select.py
--rw-rw-rw-   0        0        0     1799 2024-03-31 22:00:55.000000 mov-cli-4.2.8/mov_cli/cli/configuration.py
--rw-rw-rw-   0        0        0     2175 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/cli/episode.py
--rw-rw-rw-   0        0        0     3034 2024-04-01 04:06:26.000000 mov-cli-4.2.8/mov_cli/cli/play.py
--rw-rw-rw-   0        0        0     4330 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/cli/scraper.py
--rw-rw-rw-   0        0        0     1319 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/cli/search.py
--rw-rw-rw-   0        0        0     3563 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/cli/ui.py
--rw-rw-rw-   0        0        0     3518 2024-03-31 22:16:15.000000 mov-cli-4.2.8/mov_cli/cli/utils.py
--rw-rw-rw-   0        0        0     1417 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/cli/watch_options.py
--rw-rw-rw-   0        0        0     6753 2024-04-01 04:03:08.000000 mov-cli-4.2.8/mov_cli/config.py
--rw-rw-rw-   0        0        0      535 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/config.template.toml
--rw-rw-rw-   0        0        0     1078 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/download.py
--rw-rw-rw-   0        0        0      970 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/errors.py
--rw-rw-rw-   0        0        0     2868 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/http_client.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:28.999411 mov-cli-4.2.8/mov_cli/iterfzf/
--rw-rw-rw-   0        0        0     4269 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/iterfzf/__init__.py
--rw-rw-rw-   0        0        0      237 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:29.001933 mov-cli-4.2.8/mov_cli/media/
--rw-rw-rw-   0        0        0       45 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/media/__init__.py
--rw-rw-rw-   0        0        0     2346 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/media/media.py
--rw-rw-rw-   0        0        0     1781 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/media/metadata.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:29.006917 mov-cli-4.2.8/mov_cli/players/
--rw-rw-rw-   0        0        0       93 2024-04-01 02:35:43.000000 mov-cli-4.2.8/mov_cli/players/__init__.py
--rw-rw-rw-   0        0        0     1135 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/players/custom_player.py
--rw-rw-rw-   0        0        0     2222 2024-04-01 02:33:00.000000 mov-cli-4.2.8/mov_cli/players/mpv.py
--rw-rw-rw-   0        0        0      572 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/players/player.py
--rw-rw-rw-   0        0        0     2143 2024-03-31 22:13:40.000000 mov-cli-4.2.8/mov_cli/players/vlc.py
--rw-rw-rw-   0        0        0     1125 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/plugins.py
--rw-rw-rw-   0        0        0     1903 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/scraper.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:29.010907 mov-cli-4.2.8/mov_cli/utils/
--rw-rw-rw-   0        0        0       80 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/utils/__init__.py
--rw-rw-rw-   0        0        0      640 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/utils/episode_selector.py
--rw-rw-rw-   0        0        0      682 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/utils/platform.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:29.012902 mov-cli-4.2.8/mov_cli/utils/scraper/
--rw-rw-rw-   0        0        0       93 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/utils/scraper/__init__.py
--rw-rw-rw-   0        0        0      982 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/utils/scraper/fuzzy.py
--rw-rw-rw-   0        0        0     5683 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/utils/scraper/the_movie_db.py
--rw-rw-rw-   0        0        0      326 2024-03-31 20:57:09.000000 mov-cli-4.2.8/mov_cli/utils/version.py
-drwxrwxrwx   0        0        0        0 2024-04-01 04:21:29.013899 mov-cli-4.2.8/mov_cli.egg-info/
--rw-rw-rw-   0        0        0     7435 2024-04-01 04:21:28.000000 mov-cli-4.2.8/mov_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2024-04-01 04:21:28.000000 mov-cli-4.2.8/mov_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 04:21:28.000000 mov-cli-4.2.8/mov_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-01 04:21:28.000000 mov-cli-4.2.8/mov_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      218 2024-04-01 04:21:28.000000 mov-cli-4.2.8/mov_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-01 04:21:28.000000 mov-cli-4.2.8/mov_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1804 2024-03-31 20:57:09.000000 mov-cli-4.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 04:21:29.017887 mov-cli-4.2.8/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.737147 mov-cli-4.2.9/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.727147 mov-cli-4.2.9/.github/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.727147 mov-cli-4.2.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      185 2023-12-08 21:51:24.000000 mov-cli-4.2.9/.github/ISSUE_TEMPLATE/addprovider.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      925 2023-12-08 21:51:24.000000 mov-cli-4.2.9/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      319 2023-12-08 21:51:24.000000 mov-cli-4.2.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov-cli-4.2.9/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov-cli-4.2.9/.github/dependabot.yml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.727147 mov-cli-4.2.9/.github/workflows/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov-cli-4.2.9/.github/workflows/pypi.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov-cli-4.2.9/.github/workflows/ruff.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov-cli-4.2.9/.gitignore
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov-cli-4.2.9/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      291 2024-03-23 15:35:14.000000 mov-cli-4.2.9/Makefile
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     7269 2024-04-03 20:55:36.737147 mov-cli-4.2.9/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4612 2024-03-25 22:44:43.000000 mov-cli-4.2.9/README.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1841 2024-03-13 15:29:53.000000 mov-cli-4.2.9/disclaimer.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.730480 mov-cli-4.2.9/mov_cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      131 2024-04-03 20:28:42.000000 mov-cli-4.2.9/mov_cli/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.730480 mov-cli-4.2.9/mov_cli/cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov-cli-4.2.9/mov_cli/cli/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4860 2024-03-26 01:19:10.000000 mov-cli-4.2.9/mov_cli/cli/__main__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      457 2024-03-25 22:44:50.000000 mov-cli-4.2.9/mov_cli/cli/auto_select.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2150 2024-04-03 20:45:12.000000 mov-cli-4.2.9/mov_cli/cli/configuration.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2101 2024-03-25 22:44:50.000000 mov-cli-4.2.9/mov_cli/cli/episode.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2927 2024-04-03 20:27:45.000000 mov-cli-4.2.9/mov_cli/cli/play.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4201 2024-03-25 22:44:50.000000 mov-cli-4.2.9/mov_cli/cli/scraper.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1276 2024-03-26 17:57:30.000000 mov-cli-4.2.9/mov_cli/cli/search.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3460 2024-03-27 21:54:10.000000 mov-cli-4.2.9/mov_cli/cli/ui.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3417 2024-04-03 20:27:45.000000 mov-cli-4.2.9/mov_cli/cli/utils.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1357 2024-03-25 22:44:50.000000 mov-cli-4.2.9/mov_cli/cli/watch_options.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6551 2024-04-03 20:27:45.000000 mov-cli-4.2.9/mov_cli/config.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      514 2024-03-16 14:22:02.000000 mov-cli-4.2.9/mov_cli/config.template.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1038 2024-03-24 17:18:21.000000 mov-cli-4.2.9/mov_cli/download.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      942 2024-03-23 15:35:14.000000 mov-cli-4.2.9/mov_cli/errors.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2784 2024-04-03 20:53:58.000000 mov-cli-4.2.9/mov_cli/http_client.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.733813 mov-cli-4.2.9/mov_cli/iterfzf/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov-cli-4.2.9/mov_cli/iterfzf/LICENSE.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-03-27 21:58:28.000000 mov-cli-4.2.9/mov_cli/iterfzf/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov-cli-4.2.9/mov_cli/logger.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.733813 mov-cli-4.2.9/mov_cli/media/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       44 2023-12-08 21:51:24.000000 mov-cli-4.2.9/mov_cli/media/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2259 2024-03-27 22:06:47.000000 mov-cli-4.2.9/mov_cli/media/media.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1724 2024-03-21 11:42:05.000000 mov-cli-4.2.9/mov_cli/media/metadata.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.733813 mov-cli-4.2.9/mov_cli/players/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       89 2023-12-08 21:51:24.000000 mov-cli-4.2.9/mov_cli/players/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1100 2024-03-23 15:35:14.000000 mov-cli-4.2.9/mov_cli/players/custom_player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2147 2024-03-23 15:35:14.000000 mov-cli-4.2.9/mov_cli/players/mpv.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      551 2024-03-23 15:35:14.000000 mov-cli-4.2.9/mov_cli/players/player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2072 2024-04-03 20:27:45.000000 mov-cli-4.2.9/mov_cli/players/vlc.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1086 2024-03-25 22:44:50.000000 mov-cli-4.2.9/mov_cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1849 2024-03-25 22:44:50.000000 mov-cli-4.2.9/mov_cli/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.733813 mov-cli-4.2.9/mov_cli/utils/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov-cli-4.2.9/mov_cli/utils/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      620 2024-03-25 22:44:50.000000 mov-cli-4.2.9/mov_cli/utils/episode_selector.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      652 2024-03-13 15:29:53.000000 mov-cli-4.2.9/mov_cli/utils/platform.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.733813 mov-cli-4.2.9/mov_cli/utils/scraper/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       90 2024-03-04 00:54:59.000000 mov-cli-4.2.9/mov_cli/utils/scraper/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      940 2023-12-08 21:51:24.000000 mov-cli-4.2.9/mov_cli/utils/scraper/fuzzy.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5533 2024-03-22 14:36:19.000000 mov-cli-4.2.9/mov_cli/utils/scraper/the_movie_db.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      312 2023-12-08 21:51:24.000000 mov-cli-4.2.9/mov_cli/utils/version.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.733813 mov-cli-4.2.9/mov_cli.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     7269 2024-04-03 20:55:36.000000 mov-cli-4.2.9/mov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1435 2024-04-03 20:55:36.000000 mov-cli-4.2.9/mov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-03 20:55:36.000000 mov-cli-4.2.9/mov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-04-03 20:55:36.000000 mov-cli-4.2.9/mov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      218 2024-04-03 20:55:36.000000 mov-cli-4.2.9/mov_cli.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-04-03 20:55:36.000000 mov-cli-4.2.9/mov_cli.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1736 2024-03-30 22:00:17.000000 mov-cli-4.2.9/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-03-25 22:44:50.000000 mov-cli-4.2.9/ruff.toml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-03 20:55:36.733813 mov-cli-4.2.9/scripts/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov-cli-4.2.9/scripts/test_cli.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-03 20:55:36.737147 mov-cli-4.2.9/setup.cfg
```

### Comparing `mov-cli-4.2.8/PKG-INFO` & `mov-cli-4.2.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-Metadata-Version: 2.1
-Name: mov-cli
-Version: 4.2.8
-Summary: Watch everything from your terminal.
-Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
-License: MIT License
-        
-        Copyright (c) 2024 mov-cli
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: GitHub, https://github.com/mov-cli/mov-cli
-Project-URL: BugTracker, https://github.com/mov-cli/mov-cli/issues
-Keywords: movie-cli,mov_cli
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: httpx
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: toml
-Requires-Dist: devgoldyutils>=2.5.7
-Requires-Dist: typer[all]==0.10.0
-Requires-Dist: inquirer
-Requires-Dist: beautifulsoup4
-Requires-Dist: Unidecode
-Requires-Dist: thefuzz
-Requires-Dist: deprecation
-Requires-Dist: mov-cli-test>=1.1.0
-Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev"
-
-<a name="readme-top"></a>
-
-[![Stargazers][stars-shield]][stars-url]
-[![Pypi Version][pypi-shield]][pypi-url]
-[![Python Versions][python-shield]][pypi-url]
-[![Issues][issues-shield]][issues-url]
-[![MIT License][license-shield]][license-url]
-[![Discord][discord-shield]][discord-url]
-
-<div align="center">
-
-  <a href="https://github.com/mov-cli/mov-cli">
-    <img src="https://github.com/mov-cli/mov-cli/assets/132799819/a23bec13-881d-41b9-b596-b31c6698b89e" alt="Logo" width="250">
-  </a>
-
-  <sub>Watch everything from your terminal.</sub>
-  <br>
-  <br>
-  <a href="https://github.com/mov-cli/mov-cli/issues">Report Bug</a>
-  ·
-  <a href="https://github.com/mov-cli/mov-cli/issues">Request Feature</a>
-
-</div>
-
-<br>
-
-> [!Note]
-> v4 is constantly changing so be sure to keep the tool up to date and with that said I would advise not using it as a library yet.
-
-## Installation 🛠️
-
-> [!TIP]
-> For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
-
-### Prerequisites
-- **A supported platform:**
-  - Linux
-  - Windows
-  - Android (via [Termux](https://termux.dev/en/))
-  - iOS (via [iSH Shell](https://ish.app/))
-  - *MacOS* (**Not tested**)
-- **[python](https://www.python.org/downloads/)** (**required**, with pip)
-- **[lxml](https://pypi.org/project/lxml/)** (optional, ⚡ faster scraping)
-- **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**)
-- **[mpv](https://mpv.io/installation/)** (recommended & default media player)
-
-To get running these are all the prerequisites you'll need.
-
-With the prerequisites installed, mov-cli can be installed via the pip command on all platforms with Python version 3.8 or above.
-
-```sh
-pip install mov-cli -U
-```
-
-## Usage 🖱️
-mov-cli comes packaged with a CLI interface via the `mov-cli` command you can use in your respective terminal. 
-
-> [!NOTE]
-> You may notice mov-cli doesn't ship with any scrapers (or previously known as providers) by default, this is because v4 is plugin-based and scrapers are now part of plugins that must be chosen to be installed.
-> Find out how to do so at the [wiki](https://github.com/mov-cli/mov-cli/wiki#plugins).
-
-1. Install the scraper plugin of your choice. Visit this [wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a list of **third-party** mov-cli plugins.
-```sh
-mov-cli -e
-```
-Alternatively, you may also edit by manually opening the config file. See the [Wiki](https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction).  
-```toml
-[mov-cli.plugins]
-films = "package_name"
-```
-
-
-2. Scraper away!
-```sh
-mov-cli -s films spider man no way home
-```
-<img width="370px" src="https://github.com/mov-cli/mov-cli/assets/66202304/86189cab-b246-405e-a266-6c624bee2d36">
-
-> The above command should search for `spider man no way home` with the following scraper.
-
-## Contributing ✨
-Pull requests are welcome and *appreciated*. For major changes, please open an issue first to discuss what you would like to change.
-
-<a href = "https://github.com/mov-cli/mov-cli/graphs/contributors">
-  <img src = "https://contrib.rocks/image?repo=mov-cli/mov-cli"/>
-</a>
-
-## Inspiration 🌟
-Inspired by [ani-cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/animdl)
-
-
-<!-- MARKDOWN LINKS & IMAGES -->
-<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-cli.svg?style=for-the-badge
-[contributors-url]: https://github.com/mov-cli/mov-cli/graphs/contributors
-[forks-shield]: https://img.shields.io/github/forks/mov-cli/mov-cli.svg?style=for-the-badge
-[forks-url]: https://github.com/mov-cli/mov-cli/network/members
-[stars-shield]: https://img.shields.io/github/stars/mov-cli/mov-cli?style=flat
-[stars-url]: https://github.com/mov-cli/mov-cli/stargazers
-[pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
-[pypi-url]: https://pypi.org/project/mov-cli/
-[python-shield]: https://img.shields.io/pypi/pyversions/mov-cli?style=flat
-[issues-shield]: https://img.shields.io/github/issues/mov-cli/mov-cli?style=flat
-[issues-url]: https://github.com/mov-cli/mov-cli/issues
-[license-shield]: https://img.shields.io/github/license/mov-cli/mov-cli?style=flat
-[license-url]: ./LICENSE
-[discord-shield]: https://img.shields.io/badge/Discord-7289da?logo=discord&logoColor=white
-[discord-url]: https://discord.gg/BMzC7ePsBV
+Metadata-Version: 2.1
+Name: mov-cli
+Version: 4.2.9
+Summary: Watch everything from your terminal.
+Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
+License: MIT License
+        
+        Copyright (c) 2024 mov-cli
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: GitHub, https://github.com/mov-cli/mov-cli
+Project-URL: BugTracker, https://github.com/mov-cli/mov-cli/issues
+Keywords: movie-cli,mov_cli
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: httpx
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: toml
+Requires-Dist: devgoldyutils>=2.5.7
+Requires-Dist: typer[all]==0.10.0
+Requires-Dist: inquirer
+Requires-Dist: beautifulsoup4
+Requires-Dist: Unidecode
+Requires-Dist: thefuzz
+Requires-Dist: deprecation
+Requires-Dist: mov-cli-test>=1.1.0
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev"
+
+<a name="readme-top"></a>
+
+[![Stargazers][stars-shield]][stars-url]
+[![Pypi Version][pypi-shield]][pypi-url]
+[![Python Versions][python-shield]][pypi-url]
+[![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
+[![Discord][discord-shield]][discord-url]
+
+<div align="center">
+
+  <a href="https://github.com/mov-cli/mov-cli">
+    <img src="https://github.com/mov-cli/mov-cli/assets/132799819/a23bec13-881d-41b9-b596-b31c6698b89e" alt="Logo" width="250">
+  </a>
+
+  <sub>Watch everything from your terminal.</sub>
+  <br>
+  <br>
+  <a href="https://github.com/mov-cli/mov-cli/issues">Report Bug</a>
+  ·
+  <a href="https://github.com/mov-cli/mov-cli/issues">Request Feature</a>
+
+</div>
+
+<br>
+
+> [!Note]
+> v4 is constantly changing so be sure to keep the tool up to date and with that said I would advise not using it as a library yet.
+
+## Installation 🛠️
+
+> [!TIP]
+> For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
+
+### Prerequisites
+- **A supported platform:**
+  - Linux
+  - Windows
+  - Android (via [Termux](https://termux.dev/en/))
+  - iOS (via [iSH Shell](https://ish.app/))
+  - *MacOS* (**Not tested**)
+- **[python](https://www.python.org/downloads/)** (**required**, with pip)
+- **[lxml](https://pypi.org/project/lxml/)** (optional, ⚡ faster scraping)
+- **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**)
+- **[mpv](https://mpv.io/installation/)** (recommended & default media player)
+
+To get running these are all the prerequisites you'll need.
+
+With the prerequisites installed, mov-cli can be installed via the pip command on all platforms with Python version 3.8 or above.
+
+```sh
+pip install mov-cli -U
+```
+
+## Usage 🖱️
+mov-cli comes packaged with a CLI interface via the `mov-cli` command you can use in your respective terminal. 
+
+> [!NOTE]
+> You may notice mov-cli doesn't ship with any scrapers (or previously known as providers) by default, this is because v4 is plugin-based and scrapers are now part of plugins that must be chosen to be installed.
+> Find out how to do so at the [wiki](https://github.com/mov-cli/mov-cli/wiki#plugins).
+
+1. Install the scraper plugin of your choice. Visit this [wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a list of **third-party** mov-cli plugins.
+```sh
+mov-cli -e
+```
+Alternatively, you may also edit by manually opening the config file. See the [Wiki](https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction).  
+```toml
+[mov-cli.plugins]
+films = "package_name"
+```
+
+
+2. Scraper away!
+```sh
+mov-cli -s films spider man no way home
+```
+<img width="370px" src="https://github.com/mov-cli/mov-cli/assets/66202304/86189cab-b246-405e-a266-6c624bee2d36">
+
+> The above command should search for `spider man no way home` with the following scraper.
+
+## Contributing ✨
+Pull requests are welcome and *appreciated*. For major changes, please open an issue first to discuss what you would like to change.
+
+<a href = "https://github.com/mov-cli/mov-cli/graphs/contributors">
+  <img src = "https://contrib.rocks/image?repo=mov-cli/mov-cli"/>
+</a>
+
+## Inspiration 🌟
+Inspired by [ani-cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/animdl)
+
+
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+[contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-cli.svg?style=for-the-badge
+[contributors-url]: https://github.com/mov-cli/mov-cli/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/mov-cli/mov-cli.svg?style=for-the-badge
+[forks-url]: https://github.com/mov-cli/mov-cli/network/members
+[stars-shield]: https://img.shields.io/github/stars/mov-cli/mov-cli?style=flat
+[stars-url]: https://github.com/mov-cli/mov-cli/stargazers
+[pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
+[pypi-url]: https://pypi.org/project/mov-cli/
+[python-shield]: https://img.shields.io/pypi/pyversions/mov-cli?style=flat
+[issues-shield]: https://img.shields.io/github/issues/mov-cli/mov-cli?style=flat
+[issues-url]: https://github.com/mov-cli/mov-cli/issues
+[license-shield]: https://img.shields.io/github/license/mov-cli/mov-cli?style=flat
+[license-url]: ./LICENSE
+[discord-shield]: https://img.shields.io/badge/Discord-7289da?logo=discord&logoColor=white
+[discord-url]: https://discord.gg/BMzC7ePsBV
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.2.8 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.2.9 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.lol>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

### Comparing `mov-cli-4.2.8/README.md` & `mov-cli-4.2.9/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-<a name="readme-top"></a>
-
-[![Stargazers][stars-shield]][stars-url]
-[![Pypi Version][pypi-shield]][pypi-url]
-[![Python Versions][python-shield]][pypi-url]
-[![Issues][issues-shield]][issues-url]
-[![MIT License][license-shield]][license-url]
-[![Discord][discord-shield]][discord-url]
-
-<div align="center">
-
-  <a href="https://github.com/mov-cli/mov-cli">
-    <img src="https://github.com/mov-cli/mov-cli/assets/132799819/a23bec13-881d-41b9-b596-b31c6698b89e" alt="Logo" width="250">
-  </a>
-
-  <sub>Watch everything from your terminal.</sub>
-  <br>
-  <br>
-  <a href="https://github.com/mov-cli/mov-cli/issues">Report Bug</a>
-  ·
-  <a href="https://github.com/mov-cli/mov-cli/issues">Request Feature</a>
-
-</div>
-
-<br>
-
-> [!Note]
-> v4 is constantly changing so be sure to keep the tool up to date and with that said I would advise not using it as a library yet.
-
-## Installation 🛠️
-
-> [!TIP]
-> For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
-
-### Prerequisites
-- **A supported platform:**
-  - Linux
-  - Windows
-  - Android (via [Termux](https://termux.dev/en/))
-  - iOS (via [iSH Shell](https://ish.app/))
-  - *MacOS* (**Not tested**)
-- **[python](https://www.python.org/downloads/)** (**required**, with pip)
-- **[lxml](https://pypi.org/project/lxml/)** (optional, ⚡ faster scraping)
-- **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**)
-- **[mpv](https://mpv.io/installation/)** (recommended & default media player)
-
-To get running these are all the prerequisites you'll need.
-
-With the prerequisites installed, mov-cli can be installed via the pip command on all platforms with Python version 3.8 or above.
-
-```sh
-pip install mov-cli -U
-```
-
-## Usage 🖱️
-mov-cli comes packaged with a CLI interface via the `mov-cli` command you can use in your respective terminal. 
-
-> [!NOTE]
-> You may notice mov-cli doesn't ship with any scrapers (or previously known as providers) by default, this is because v4 is plugin-based and scrapers are now part of plugins that must be chosen to be installed.
-> Find out how to do so at the [wiki](https://github.com/mov-cli/mov-cli/wiki#plugins).
-
-1. Install the scraper plugin of your choice. Visit this [wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a list of **third-party** mov-cli plugins.
-```sh
-mov-cli -e
-```
-Alternatively, you may also edit by manually opening the config file. See the [Wiki](https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction).  
-```toml
-[mov-cli.plugins]
-films = "package_name"
-```
-
-
-2. Scraper away!
-```sh
-mov-cli -s films spider man no way home
-```
-<img width="370px" src="https://github.com/mov-cli/mov-cli/assets/66202304/86189cab-b246-405e-a266-6c624bee2d36">
-
-> The above command should search for `spider man no way home` with the following scraper.
-
-## Contributing ✨
-Pull requests are welcome and *appreciated*. For major changes, please open an issue first to discuss what you would like to change.
-
-<a href = "https://github.com/mov-cli/mov-cli/graphs/contributors">
-  <img src = "https://contrib.rocks/image?repo=mov-cli/mov-cli"/>
-</a>
-
-## Inspiration 🌟
-Inspired by [ani-cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/animdl)
-
-
-<!-- MARKDOWN LINKS & IMAGES -->
-<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-cli.svg?style=for-the-badge
-[contributors-url]: https://github.com/mov-cli/mov-cli/graphs/contributors
-[forks-shield]: https://img.shields.io/github/forks/mov-cli/mov-cli.svg?style=for-the-badge
-[forks-url]: https://github.com/mov-cli/mov-cli/network/members
-[stars-shield]: https://img.shields.io/github/stars/mov-cli/mov-cli?style=flat
-[stars-url]: https://github.com/mov-cli/mov-cli/stargazers
-[pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
-[pypi-url]: https://pypi.org/project/mov-cli/
-[python-shield]: https://img.shields.io/pypi/pyversions/mov-cli?style=flat
-[issues-shield]: https://img.shields.io/github/issues/mov-cli/mov-cli?style=flat
-[issues-url]: https://github.com/mov-cli/mov-cli/issues
-[license-shield]: https://img.shields.io/github/license/mov-cli/mov-cli?style=flat
-[license-url]: ./LICENSE
-[discord-shield]: https://img.shields.io/badge/Discord-7289da?logo=discord&logoColor=white
-[discord-url]: https://discord.gg/BMzC7ePsBV
+<a name="readme-top"></a>
+
+[![Stargazers][stars-shield]][stars-url]
+[![Pypi Version][pypi-shield]][pypi-url]
+[![Python Versions][python-shield]][pypi-url]
+[![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
+[![Discord][discord-shield]][discord-url]
+
+<div align="center">
+
+  <a href="https://github.com/mov-cli/mov-cli">
+    <img src="https://github.com/mov-cli/mov-cli/assets/132799819/a23bec13-881d-41b9-b596-b31c6698b89e" alt="Logo" width="250">
+  </a>
+
+  <sub>Watch everything from your terminal.</sub>
+  <br>
+  <br>
+  <a href="https://github.com/mov-cli/mov-cli/issues">Report Bug</a>
+  ·
+  <a href="https://github.com/mov-cli/mov-cli/issues">Request Feature</a>
+
+</div>
+
+<br>
+
+> [!Note]
+> v4 is constantly changing so be sure to keep the tool up to date and with that said I would advise not using it as a library yet.
+
+## Installation 🛠️
+
+> [!TIP]
+> For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
+
+### Prerequisites
+- **A supported platform:**
+  - Linux
+  - Windows
+  - Android (via [Termux](https://termux.dev/en/))
+  - iOS (via [iSH Shell](https://ish.app/))
+  - *MacOS* (**Not tested**)
+- **[python](https://www.python.org/downloads/)** (**required**, with pip)
+- **[lxml](https://pypi.org/project/lxml/)** (optional, ⚡ faster scraping)
+- **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**)
+- **[mpv](https://mpv.io/installation/)** (recommended & default media player)
+
+To get running these are all the prerequisites you'll need.
+
+With the prerequisites installed, mov-cli can be installed via the pip command on all platforms with Python version 3.8 or above.
+
+```sh
+pip install mov-cli -U
+```
+
+## Usage 🖱️
+mov-cli comes packaged with a CLI interface via the `mov-cli` command you can use in your respective terminal. 
+
+> [!NOTE]
+> You may notice mov-cli doesn't ship with any scrapers (or previously known as providers) by default, this is because v4 is plugin-based and scrapers are now part of plugins that must be chosen to be installed.
+> Find out how to do so at the [wiki](https://github.com/mov-cli/mov-cli/wiki#plugins).
+
+1. Install the scraper plugin of your choice. Visit this [wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a list of **third-party** mov-cli plugins.
+```sh
+mov-cli -e
+```
+Alternatively, you may also edit by manually opening the config file. See the [Wiki](https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction).  
+```toml
+[mov-cli.plugins]
+films = "package_name"
+```
+
+
+2. Scraper away!
+```sh
+mov-cli -s films spider man no way home
+```
+<img width="370px" src="https://github.com/mov-cli/mov-cli/assets/66202304/86189cab-b246-405e-a266-6c624bee2d36">
+
+> The above command should search for `spider man no way home` with the following scraper.
+
+## Contributing ✨
+Pull requests are welcome and *appreciated*. For major changes, please open an issue first to discuss what you would like to change.
+
+<a href = "https://github.com/mov-cli/mov-cli/graphs/contributors">
+  <img src = "https://contrib.rocks/image?repo=mov-cli/mov-cli"/>
+</a>
+
+## Inspiration 🌟
+Inspired by [ani-cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/animdl)
+
+
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+[contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-cli.svg?style=for-the-badge
+[contributors-url]: https://github.com/mov-cli/mov-cli/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/mov-cli/mov-cli.svg?style=for-the-badge
+[forks-url]: https://github.com/mov-cli/mov-cli/network/members
+[stars-shield]: https://img.shields.io/github/stars/mov-cli/mov-cli?style=flat
+[stars-url]: https://github.com/mov-cli/mov-cli/stargazers
+[pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
+[pypi-url]: https://pypi.org/project/mov-cli/
+[python-shield]: https://img.shields.io/pypi/pyversions/mov-cli?style=flat
+[issues-shield]: https://img.shields.io/github/issues/mov-cli/mov-cli?style=flat
+[issues-url]: https://github.com/mov-cli/mov-cli/issues
+[license-shield]: https://img.shields.io/github/license/mov-cli/mov-cli?style=flat
+[license-url]: ./LICENSE
+[discord-shield]: https://img.shields.io/badge/Discord-7289da?logo=discord&logoColor=white
+[discord-url]: https://discord.gg/BMzC7ePsBV
```

### Comparing `mov-cli-4.2.8/mov_cli/cli/__main__.py` & `mov-cli-4.2.9/mov_cli/cli/__main__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-from __future__ import annotations
-from typing import List, Optional, TYPE_CHECKING
-
-if TYPE_CHECKING:
-    ...
-
-import typer
-import logging
-from devgoldyutils import Colours
-
-from .play import play
-from .search import search
-from .episode import handle_episode
-from .scraper import select_scraper, use_scraper, scrape
-from .configuration import open_config_file, set_cli_config
-from .utils import welcome_msg, steal_scraper_args
-
-from ..config import Config
-from ..download import Download
-from ..logger import mov_cli_logger
-from ..http_client import HTTPClient
-
-__all__ = ("mov_cli",)
-
-uwu_app = typer.Typer(pretty_exceptions_enable = False) # NOTE: goldy has an uwu complex.
-
-def mov_cli(
-    query: Optional[List[str]] = typer.Argument(None, help = "A film, tv show or anime you would like to Query."), 
-    debug: Optional[bool] = typer.Option(None, help = "Enable extra logging details. Useful for bug reporting."), 
-    player: Optional[str] = typer.Option(None, "--player", "-p", help = "Player you would like to stream with. E.g. mpv, vlc"), 
-    scraper: Optional[str] = typer.Option(None, "--scraper", "-s", help = "Scraper you would like to scrape with. E.g. remote_stream, sflix"), 
-    fzf: Optional[bool] = typer.Option(None, help = "Toggle fzf on/off for all user selection prompts."), 
-    episode: Optional[str] = typer.Option(None, "--episode", "-ep", help = "Episode and season you wanna scrape. E.g. {episode}:{season} like -> 26:3"), 
-    auto_select: Optional[int] = typer.Option(None, "--choice", "-c", help = "Auto select the search results. E.g. Setting it to 1 with query 'nyan cat' will pick " \
-        "the first nyan cat video to show up in search results."
-    ), 
-
-    version: bool = typer.Option(False, "--version", help = "Display what version mov-cli is currently on."), 
-    edit: bool = typer.Option(False, "--edit", "-e", help = "Opens the mov-cli config with your respective editor."), 
-    download: bool = typer.Option(False, "--download", "-d", help = "Downloads the media instead of playing.")
-):
-    config = Config()
-
-    config = set_cli_config(
-        config,
-        debug = debug,
-        player = player,
-        scraper = scraper,
-        fzf = fzf
-    )
-
-    if config.debug:
-        mov_cli_logger.setLevel(logging.DEBUG)
-
-    print(
-        welcome_msg(True if query is None else False, version)
-    )
-
-    mov_cli_logger.debug(f"Config -> {config.data}")
-
-    if edit is True:
-        open_config_file(config)
-        return None
-
-    if query is not None:
-        scrape_args = steal_scraper_args(query) 
-        # This allows passing arguments to scrapers like this: 
-        # https://github.com/mov-cli/mov-cli-youtube/commit/b538d82745a743cd74a02530d6a3d476cd60b808#diff-4e5b064838aa74a5375265f4dfbd94024b655ee24a191290aacd3673abed921a
-
-        query: str = " ".join(query)
-
-        http_client = HTTPClient(config)
-
-        selected_scraper = select_scraper(config.plugins, config.fzf_enabled, config.default_scraper)
-
-        if selected_scraper is None:
-            mov_cli_logger.error(
-                "You must choose a scraper to scrape with! " \
-                    "You can set a default scraper with the default key in config.toml."
-            )
-            return False
-
-        chosen_scraper = use_scraper(selected_scraper, config, http_client)
-
-        choice = search(query, auto_select, chosen_scraper, config.fzf_enabled)
-
-        if choice is None:
-            mov_cli_logger.error("There was no results or you didn't select anything.")
-            return False
-
-        chosen_episode = handle_episode(
-            episode_string = episode, 
-            scraper = chosen_scraper, 
-            choice = choice, 
-            fzf_enabled = config.fzf_enabled
-        )
-
-        if chosen_episode is None:
-            mov_cli_logger.error("You didn't select a season/episode.")
-            return False
-
-        media = scrape(choice, chosen_episode, chosen_scraper, **scrape_args)
-
-        if download:
-            dl = Download(config)
-            mov_cli_logger.debug(f"Downloading from this url -> '{media.url}'")
-
-            popen = dl.download(media)
-            popen.wait()
-
-        else:
-            option = play(media, choice, chosen_scraper, chosen_episode, config, scrape_args)
-
-            if option == "search":
-                query = input(Colours.BLUE.apply("  Enter Query: "))
-
-                mov_cli(
-                    query = [query], 
-                    debug = debug, 
-                    player = player, 
-                    scraper = scraper, 
-                    fzf = fzf,
-                    episode = None,
-                    auto_select = None,
-
-                    version = False,
-                    edit = False,
-                    download = False
-                )
-
-def app():
-    uwu_app.command()(mov_cli)
+from __future__ import annotations
+from typing import List, Optional, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    ...
+
+import typer
+import logging
+from devgoldyutils import Colours
+
+from .play import play
+from .search import search
+from .episode import handle_episode
+from .scraper import select_scraper, use_scraper, scrape
+from .configuration import open_config_file, set_cli_config
+from .utils import welcome_msg, steal_scraper_args
+
+from ..config import Config
+from ..download import Download
+from ..logger import mov_cli_logger
+from ..http_client import HTTPClient
+
+__all__ = ("mov_cli",)
+
+uwu_app = typer.Typer(pretty_exceptions_enable = False) # NOTE: goldy has an uwu complex.
+
+def mov_cli(
+    query: Optional[List[str]] = typer.Argument(None, help = "A film, tv show or anime you would like to Query."), 
+    debug: Optional[bool] = typer.Option(None, help = "Enable extra logging details. Useful for bug reporting."), 
+    player: Optional[str] = typer.Option(None, "--player", "-p", help = "Player you would like to stream with. E.g. mpv, vlc"), 
+    scraper: Optional[str] = typer.Option(None, "--scraper", "-s", help = "Scraper you would like to scrape with. E.g. remote_stream, sflix"), 
+    fzf: Optional[bool] = typer.Option(None, help = "Toggle fzf on/off for all user selection prompts."), 
+    episode: Optional[str] = typer.Option(None, "--episode", "-ep", help = "Episode and season you wanna scrape. E.g. {episode}:{season} like -> 26:3"), 
+    auto_select: Optional[int] = typer.Option(None, "--choice", "-c", help = "Auto select the search results. E.g. Setting it to 1 with query 'nyan cat' will pick " \
+        "the first nyan cat video to show up in search results."
+    ), 
+
+    version: bool = typer.Option(False, "--version", help = "Display what version mov-cli is currently on."), 
+    edit: bool = typer.Option(False, "--edit", "-e", help = "Opens the mov-cli config with your respective editor."), 
+    download: bool = typer.Option(False, "--download", "-d", help = "Downloads the media instead of playing.")
+):
+    config = Config()
+
+    config = set_cli_config(
+        config,
+        debug = debug,
+        player = player,
+        scraper = scraper,
+        fzf = fzf
+    )
+
+    if config.debug:
+        mov_cli_logger.setLevel(logging.DEBUG)
+
+    print(
+        welcome_msg(True if query is None else False, version)
+    )
+
+    mov_cli_logger.debug(f"Config -> {config.data}")
+
+    if edit is True:
+        open_config_file(config)
+        return None
+
+    if query is not None:
+        scrape_args = steal_scraper_args(query) 
+        # This allows passing arguments to scrapers like this: 
+        # https://github.com/mov-cli/mov-cli-youtube/commit/b538d82745a743cd74a02530d6a3d476cd60b808#diff-4e5b064838aa74a5375265f4dfbd94024b655ee24a191290aacd3673abed921a
+
+        query: str = " ".join(query)
+
+        http_client = HTTPClient(config)
+
+        selected_scraper = select_scraper(config.plugins, config.fzf_enabled, config.default_scraper)
+
+        if selected_scraper is None:
+            mov_cli_logger.error(
+                "You must choose a scraper to scrape with! " \
+                    "You can set a default scraper with the default key in config.toml."
+            )
+            return False
+
+        chosen_scraper = use_scraper(selected_scraper, config, http_client)
+
+        choice = search(query, auto_select, chosen_scraper, config.fzf_enabled)
+
+        if choice is None:
+            mov_cli_logger.error("There was no results or you didn't select anything.")
+            return False
+
+        chosen_episode = handle_episode(
+            episode_string = episode, 
+            scraper = chosen_scraper, 
+            choice = choice, 
+            fzf_enabled = config.fzf_enabled
+        )
+
+        if chosen_episode is None:
+            mov_cli_logger.error("You didn't select a season/episode.")
+            return False
+
+        media = scrape(choice, chosen_episode, chosen_scraper, **scrape_args)
+
+        if download:
+            dl = Download(config)
+            mov_cli_logger.debug(f"Downloading from this url -> '{media.url}'")
+
+            popen = dl.download(media)
+            popen.wait()
+
+        else:
+            option = play(media, choice, chosen_scraper, chosen_episode, config, scrape_args)
+
+            if option == "search":
+                query = input(Colours.BLUE.apply("  Enter Query: "))
+
+                mov_cli(
+                    query = [query], 
+                    debug = debug, 
+                    player = player, 
+                    scraper = scraper, 
+                    fzf = fzf,
+                    episode = None,
+                    auto_select = None,
+
+                    version = False,
+                    edit = False,
+                    download = False
+                )
+
+def app():
+    uwu_app.command()(mov_cli)
     uwu_app() # Wait whaaaaa.
```

### Comparing `mov-cli-4.2.8/mov_cli/cli/episode.py` & `mov-cli-4.2.9/mov_cli/cli/episode.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing import Optional
-    from ..media import Metadata
-    from ..scraper import Scraper
-
-from devgoldyutils import Colours
-
-from .ui import prompt
-
-from ..media import MetadataType
-from ..utils import EpisodeSelector
-from ..logger import mov_cli_logger
-
-__all__ = (
-    "handle_episode", 
-)
-
-def handle_episode(episode_string: Optional[str], scraper: Scraper, choice: Metadata, fzf_enabled: bool) -> Optional[EpisodeSelector]:
-    if choice.type == MetadataType.MOVIE:
-        return EpisodeSelector()
-
-    if episode_string is None:
-        mov_cli_logger.info(f"Scrapping episodes for '{Colours.CLAY.apply(choice.title)}'...")
-        metadata_episodes = scraper.scrape_episodes(choice)
-
-        if metadata_episodes.get(None) == 1:
-            return EpisodeSelector()
-
-        season = prompt(
-            "Select Season", 
-            choices = [season for season in metadata_episodes], 
-            display = lambda x: f"Season {x}", 
-            fzf_enabled = fzf_enabled
-        )
-
-        if season is None:
-            return None
-
-        episode = prompt(
-            "Select Episode", 
-            choices = [episode for episode in range(1, metadata_episodes[season] + 1)], 
-            display = lambda x: f"Episode {x}",
-            fzf_enabled = fzf_enabled
-        )
-
-        if episode is None:
-            return None
-
-        return EpisodeSelector(episode, season)
-
-    try:
-        episode_season = episode_string.split(":")
-
-        episode = 1
-        season = 1
-
-        if len(episode_season) == 1 or episode_season[1] == "":
-            episode = int(episode_season[0])
-
-        elif len(episode_season) == 2:
-            episode = int(episode_season[0])
-            season = int(episode_season[1])
-
-    except ValueError as e:
-        mov_cli_logger.error(
-            "Incorrect episode format! This is how it's done --> '5:1' (5 being episode and 1 being season)\n" \
-                f"Error: {e}"
-        )
-
-        return None
-
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Optional
+    from ..media import Metadata
+    from ..scraper import Scraper
+
+from devgoldyutils import Colours
+
+from .ui import prompt
+
+from ..media import MetadataType
+from ..utils import EpisodeSelector
+from ..logger import mov_cli_logger
+
+__all__ = (
+    "handle_episode", 
+)
+
+def handle_episode(episode_string: Optional[str], scraper: Scraper, choice: Metadata, fzf_enabled: bool) -> Optional[EpisodeSelector]:
+    if choice.type == MetadataType.MOVIE:
+        return EpisodeSelector()
+
+    if episode_string is None:
+        mov_cli_logger.info(f"Scrapping episodes for '{Colours.CLAY.apply(choice.title)}'...")
+        metadata_episodes = scraper.scrape_episodes(choice)
+
+        if metadata_episodes.get(None) == 1:
+            return EpisodeSelector()
+
+        season = prompt(
+            "Select Season", 
+            choices = [season for season in metadata_episodes], 
+            display = lambda x: f"Season {x}", 
+            fzf_enabled = fzf_enabled
+        )
+
+        if season is None:
+            return None
+
+        episode = prompt(
+            "Select Episode", 
+            choices = [episode for episode in range(1, metadata_episodes[season] + 1)], 
+            display = lambda x: f"Episode {x}",
+            fzf_enabled = fzf_enabled
+        )
+
+        if episode is None:
+            return None
+
+        return EpisodeSelector(episode, season)
+
+    try:
+        episode_season = episode_string.split(":")
+
+        episode = 1
+        season = 1
+
+        if len(episode_season) == 1 or episode_season[1] == "":
+            episode = int(episode_season[0])
+
+        elif len(episode_season) == 2:
+            episode = int(episode_season[0])
+            season = int(episode_season[1])
+
+    except ValueError as e:
+        mov_cli_logger.error(
+            "Incorrect episode format! This is how it's done --> '5:1' (5 being episode and 1 being season)\n" \
+                f"Error: {e}"
+        )
+
+        return None
+
     return EpisodeSelector(episode, season)
```

### Comparing `mov-cli-4.2.8/mov_cli/cli/search.py` & `mov-cli-4.2.9/mov_cli/cli/search.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing import Optional
-
-    from ..media import Metadata
-    from ..scraper import Scraper
-
-from devgoldyutils import Colours
-
-from .ui import prompt
-from .auto_select import auto_select_choice
-from .utils import handle_internal_plugin_error
-
-from ..media import MetadataType
-from ..logger import mov_cli_logger
-
-__all__ = (
-    "search", 
-)
-
-def search(query: str, auto_select: Optional[int], scraper: Scraper, fzf_enabled: bool) -> Optional[Metadata]:
-    choice = None
-
-    mov_cli_logger.info(f"Searching for '{Colours.ORANGE.apply(query)}'...")
-
-    try:
-        search_results = scraper.search(query)
-    except Exception as e:
-        handle_internal_plugin_error(e)
-
-    if auto_select is not None:
-        choice = auto_select_choice((choice for choice in search_results), auto_select)
-    else:
-        choice = prompt(
-            "Choose Result", 
-            choices = (choice for choice in search_results), 
-            display = lambda x: f"{Colours.CLAY if x.type == MetadataType.MOVIE else Colours.BLUE}{x.title}" \
-                f"{Colours.RESET} ({x.year if x.year is not None else 'N/A'})", 
-            fzf_enabled = fzf_enabled
-        )
-
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Optional
+
+    from ..media import Metadata
+    from ..scraper import Scraper
+
+from devgoldyutils import Colours
+
+from .ui import prompt
+from .auto_select import auto_select_choice
+from .utils import handle_internal_plugin_error
+
+from ..media import MetadataType
+from ..logger import mov_cli_logger
+
+__all__ = (
+    "search", 
+)
+
+def search(query: str, auto_select: Optional[int], scraper: Scraper, fzf_enabled: bool) -> Optional[Metadata]:
+    choice = None
+
+    mov_cli_logger.info(f"Searching for '{Colours.ORANGE.apply(query)}'...")
+
+    try:
+        search_results = scraper.search(query)
+    except Exception as e:
+        handle_internal_plugin_error(e)
+
+    if auto_select is not None:
+        choice = auto_select_choice((choice for choice in search_results), auto_select)
+    else:
+        choice = prompt(
+            "Choose Result", 
+            choices = (choice for choice in search_results), 
+            display = lambda x: f"{Colours.CLAY if x.type == MetadataType.MOVIE else Colours.BLUE}{x.title}" \
+                f"{Colours.RESET} ({x.year if x.year is not None else 'N/A'})", 
+            fzf_enabled = fzf_enabled
+        )
+
     return choice
```

### Comparing `mov-cli-4.2.8/mov_cli/cli/utils.py` & `mov-cli-4.2.9/mov_cli/cli/utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,102 +1,102 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing import Literal, Tuple, List, Dict, NoReturn
-
-import random
-import getpass
-from datetime import datetime
-from devgoldyutils import Colours
-
-from ..logger import mov_cli_logger
-from .. import __version__ as mov_cli_version
-from ..utils import  what_platform, update_available
-
-__all__ = (
-    "greetings", 
-    "welcome_msg", 
-    "steal_scraper_args",
-    "handle_internal_plugin_error"
-)
-
-def greetings() -> Tuple[Literal["Good Morning", "Good Afternoon", "Good Evening", "Good Night"], str]:
-    now = datetime.now()
-    user_name = random.choice(
-        ("buddy", "comrade", "co-worker", "human", "companion", "specimen")
-    )
-
-    p = now.strftime("%p")
-    i = int(now.strftime("%I"))
-
-    try:
-        user_name = user_name if what_platform() in ["Android", "iOS"] else getpass.getuser()
-    except Exception as e:  # NOTE: Apparently an exception is raised but they don't tell us what exception :(
-        mov_cli_logger.debug(
-            "getpass couldn't get the user name so a random one is being returned. "
-            f"\nError >> {e}"
-        )
-
-    greeting = None
-
-    if p == "AM":
-        if i <= 6 or i == 12:
-            greeting = "Good Night"
-        else:
-            greeting = "Good Morning"
-    else:
-        if i <= 5:
-            greeting = "Good Afternoon"
-        elif i > 5 and i <= 8:
-            greeting = "Good Evening"
-        elif i > 8:
-            greeting = "Good Night"
-
-    return greeting, user_name
-
-# This function below is inspired by animdl: https://github.com/justfoolingaround/animdl
-def welcome_msg(display_hint: bool = False, display_version: bool = False) -> str:
-    """Returns cli welcome message."""
-    now = datetime.now()
-    adjective = random.choice(
-        ("gorgeous", "wonderful", "beautiful", "magnificent")
-    )
-
-    greeting, user_name = greetings()
-
-    text = f"\n{greeting}, {Colours.ORANGE.apply(user_name)}."
-    text += now.strftime(
-        f"\n    It's {Colours.BLUE}%I:%M %p {Colours.RESET}on a {Colours.PURPLE}{adjective} {Colours.PINK_GREY}%A! {Colours.RESET}"
-    )
-
-    if display_hint is True and display_version is False:
-        text += f"\n\n- Hint: {Colours.CLAY}mov-cli {Colours.PINK_GREY}-s films {Colours.ORANGE}mr.robot{Colours.RESET}" \
-            f"\n- Hint: {Colours.CLAY}mov-cli {Colours.PINK_GREY}-s anime {Colours.ORANGE}chuunibyou demo take on me{Colours.RESET}"
-
-    if display_version is True:
-        text += f"\n\n{Colours.CLAY}-> {Colours.RESET}Version: {Colours.BLUE}{mov_cli_version}{Colours.RESET}"
-
-    if update_available():
-        text += f"\n\n {Colours.PURPLE}ツ {Colours.ORANGE}An update is available! --> {Colours.RESET}pip install mov-cli -U"
-
-    return text + "\n"
-
-def steal_scraper_args(query: List[str]) -> Dict[str, bool]:
-    scrape_arguments = [x for x in query if "--" in x]
-
-    mov_cli_logger.debug(f"Scraper args picked up on --> {scrape_arguments}")
-
-    for scrape_arg in scrape_arguments:
-        query.remove(scrape_arg)
-
-    return dict(
-        [(x.replace("--", ""), True) for x in scrape_arguments]
-    )
-
-def handle_internal_plugin_error(e: Exception) -> NoReturn:
-    mov_cli_logger.critical(
-        "An error occurred inside a plugin. This is most likely nothing to do with mov-cli, " \
-            f"make sure your plugins are up to date! \nError: {e}"
-    )
-
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Literal, Tuple, List, Dict, NoReturn
+
+import random
+import getpass
+from datetime import datetime
+from devgoldyutils import Colours
+
+from ..logger import mov_cli_logger
+from .. import __version__ as mov_cli_version
+from ..utils import  what_platform, update_available
+
+__all__ = (
+    "greetings", 
+    "welcome_msg", 
+    "steal_scraper_args",
+    "handle_internal_plugin_error"
+)
+
+def greetings() -> Tuple[Literal["Good Morning", "Good Afternoon", "Good Evening", "Good Night"], str]:
+    now = datetime.now()
+    user_name = random.choice(
+        ("buddy", "comrade", "co-worker", "human", "companion", "specimen")
+    )
+
+    p = now.strftime("%p")
+    i = int(now.strftime("%I"))
+
+    try:
+        user_name = user_name if what_platform() in ["Android", "iOS"] else getpass.getuser()
+    except Exception as e:  # NOTE: Apparently an exception is raised but they don't tell us what exception :(
+        mov_cli_logger.debug(
+            "getpass couldn't get the user name so a random one is being returned. "
+            f"\nError >> {e}"
+        )
+
+    greeting = None
+
+    if p == "AM":
+        if i <= 6 or i == 12:
+            greeting = "Good Night"
+        else:
+            greeting = "Good Morning"
+    else:
+        if i <= 5:
+            greeting = "Good Afternoon"
+        elif i > 5 and i <= 8:
+            greeting = "Good Evening"
+        elif i > 8:
+            greeting = "Good Night"
+
+    return greeting, user_name
+
+# This function below is inspired by animdl: https://github.com/justfoolingaround/animdl
+def welcome_msg(display_hint: bool = False, display_version: bool = False) -> str:
+    """Returns cli welcome message."""
+    now = datetime.now()
+    adjective = random.choice(
+        ("gorgeous", "wonderful", "beautiful", "magnificent")
+    )
+
+    greeting, user_name = greetings()
+
+    text = f"\n{greeting}, {Colours.ORANGE.apply(user_name)}."
+    text += now.strftime(
+        f"\n    It's {Colours.BLUE}%I:%M %p {Colours.RESET}on a {Colours.PURPLE}{adjective} {Colours.PINK_GREY}%A! {Colours.RESET}"
+    )
+
+    if display_hint is True and display_version is False:
+        text += f"\n\n- Hint: {Colours.CLAY}mov-cli {Colours.PINK_GREY}-s films {Colours.ORANGE}mr.robot{Colours.RESET}" \
+            f"\n- Hint: {Colours.CLAY}mov-cli {Colours.PINK_GREY}-s anime {Colours.ORANGE}chuunibyou demo take on me{Colours.RESET}"
+
+    if display_version is True:
+        text += f"\n\n{Colours.CLAY}-> {Colours.RESET}Version: {Colours.BLUE}{mov_cli_version}{Colours.RESET}"
+
+    if update_available():
+        text += f"\n\n {Colours.PURPLE}ツ {Colours.ORANGE}An update is available! --> {Colours.RESET}pip install mov-cli -U"
+
+    return text + "\n"
+
+def steal_scraper_args(query: List[str]) -> Dict[str, bool]:
+    scrape_arguments = [x for x in query if "--" in x]
+
+    mov_cli_logger.debug(f"Scraper args picked up on --> {scrape_arguments}")
+
+    for scrape_arg in scrape_arguments:
+        query.remove(scrape_arg)
+
+    return dict(
+        [(x.replace("--", ""), True) for x in scrape_arguments]
+    )
+
+def handle_internal_plugin_error(e: Exception) -> NoReturn:
+    mov_cli_logger.critical(
+        "An error occurred inside a plugin. This is most likely nothing to do with mov-cli, " \
+            f"make sure your plugins are up to date! \nError: {e}"
+    )
+
     raise e
```

### Comparing `mov-cli-4.2.8/mov_cli/config.py` & `mov-cli-4.2.9/mov_cli/config.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING, TypedDict, final
-
-if TYPE_CHECKING:
-    from .players import Player
-    from typing import Dict, Union, Literal, Any, Optional, Type
-
-    JSON_VALUES = Union[str, bool, int, dict]
-    SUPPORTED_PARSERS = Literal["lxml", "html.parser"]
-
-import os
-import toml
-from pathlib import Path
-from importlib.util import find_spec
-from devgoldyutils import LoggerAdapter
-
-from . import players, utils
-from .logger import mov_cli_logger
-
-__all__ = ("Config",)
-
-@final
-class ConfigUIData(TypedDict):
-    fzf: bool
-
-@final
-class ConfigHTTPData(TypedDict):
-    headers: Dict[str, str]
-
-@final
-class ConfigDownloadsData(TypedDict):
-    save_path: str
-
-@final
-class ScrapersData(TypedDict):
-    default: str
-
-@final
-class ConfigData(TypedDict):
-    version: int
-    debug: bool
-    player: str
-    parser: SUPPORTED_PARSERS
-    ui: ConfigUIData
-    http: ConfigHTTPData
-    downloads: ConfigDownloadsData
-    scrapers: ScrapersData
-    plugins: Dict[str, str]
-
-logger = LoggerAdapter(mov_cli_logger, prefix = "Config")
-
-class Config():
-    """Class that wraps the mov-cli configuration file. Mostly used under the CLI interface."""
-    def __init__(self, override_config: ConfigData = None, config_path: Path = None) -> None:
-        self.config_path = config_path
-
-        self.data: ConfigData = {}
-
-        if override_config is None:
-            self.config_path = self.__get_config_file()
-
-            try:
-                self.data = toml.load(self.config_path).get("mov-cli", {})
-            except toml.decoder.TomlDecodeError as e:
-                logger.critical(
-                    "Failed to read config.toml! Please check you haven't made any mistakes in the config." \
-                        f"All values will fallback to default. \nError: {e}"
-                )
-
-        else:
-            self.data = override_config
-
-    @property
-    def version(self) -> int:
-        return self.data.get("version", 1)
-
-    @property
-    def player(self) -> Type[Player]:
-        """Returns the player class that was configured in the config. Defaults to MPV."""
-        value = self.data.get("player", "mpv")
-
-        platform = utils.what_platform()
-
-        if value.lower() == "mpv":
-            return players.MPV(platform)
-        elif value.lower() == "vlc":
-            return players.VLC(platform)
-
-        return players.CustomPlayer(value)
-
-    @property
-    def plugins(self) -> Dict[str, str]:
-        return self.data.get("plugins", {"test": "mov-cli-test"})
-
-    @property
-    def editor(self) -> Optional[str]:
-        """Returns the editor that should be opened while editing."""
-        return self.data.get("editor")
-
-    @property
-    def default_scraper(self) -> Optional[str]:
-        """Returns the scraper that should be used to scrape by default."""
-        return self.data.get("scrapers", {}).get("default", None)
-
-    @property
-    def fzf_enabled(self) -> bool:
-        """Returns whether fzf is allowed to be used."""
-        return self.data.get("ui", {}).get("fzf", True)
-
-    @property
-    def parser(self) -> SUPPORTED_PARSERS | Any:
-        """Returns the parser type configured by the user else it just returns the default."""
-        default_parser = "lxml" if find_spec("lxml") else "html.parser"
-        return self.data.get("parser", default_parser)
-
-    @property
-    def download_location(self) -> str:
-        """Returns download location. Defaults to OS's download location."""
-        return self.data.get("downloads", {}).get("save_path", os.getcwd())
-
-    @property
-    def debug(self) -> bool:
-        """Returns whether debug should be enabled or not."""
-        return self.data.get("debug", False)
-
-    @property
-    def proxy(self) -> dict | None:
-        """Returns proxy data. Defaults to None"""
-        proxy_config = self.data.get("proxy")
-
-        if proxy_config is not None:
-            proxy = None
-
-            username = proxy_config.get("username")
-            password = proxy_config.get("password")
-
-            scheme = proxy_config.get("scheme")
-            ip = proxy_config.get("ip")
-            port = proxy_config.get("port")
-
-            if username and password:
-                proxy = f"{scheme}://{username}:{password}@{ip}:{port}"
-            else:
-                proxy = f"{scheme}://{ip}:{port}"
-
-            return {"all://": proxy}
-        else:
-            return None
-
-    @property
-    def http_headers(self) -> dict:
-        """Returns http headers."""
-        default_headers = {
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/117.0",
-            "Accept-Language": "en-US,en;q=0.5",
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
-        }
-
-        return self.data.get("http", {}).get("headers", default_headers)
-
-    def __get_config_file(self) -> Path:
-        """Function that returns the path to the config file with multi platform support."""
-        platform = utils.what_platform()
-
-        appdata_dir = Path("./mov-cli-temp")
-
-        if platform == "Windows":
-            user_profile = Path(os.getenv("USERPROFILE"))
-            appdata_dir = user_profile.joinpath("AppData", "Local")
-
-        elif platform == "Darwin": # NOTE: Path maybe incorrect
-            user_profile = Path.home()
-            appdata_dir = user_profile.joinpath("Library", "Application Support")
-
-        elif platform == "iOS":
-            user_profile = Path(os.getenv("HOME"))
-            appdata_dir = user_profile.joinpath("Library")
-
-            appdata_dir.mkdir(exist_ok = True)
-
-        elif platform == "Linux" or platform == "Android":
-            user_profile = Path(os.getenv("HOME"))
-            appdata_dir = user_profile.joinpath(".config")
- 
-            appdata_dir.mkdir(exist_ok = True) # on android the .config file may not exist.
-
-        config_path = appdata_dir.joinpath("mov-cli", "config.toml")
-        config_path.parent.mkdir(exist_ok = True)
-
-        if not config_path.exists():
-            logger.debug("The 'config.toml' file doesn't exist so we're creating it...")
-            config_file = open(config_path, "w")
-
-            template_config_path = f"{Path(os.path.split(__file__)[0])}{os.sep}config.template.toml"
-
-            with open(template_config_path, "r") as config_template:
-                config_file.write(config_template.read())
-
-            config_file.close()
-            logger.info(f"Config created at '{config_path}'.")
-
-        return config_path
+from __future__ import annotations
+from typing import TYPE_CHECKING, TypedDict, final
+
+if TYPE_CHECKING:
+    from .players import Player
+    from typing import Dict, Union, Literal, Any, Optional, Type
+
+    JSON_VALUES = Union[str, bool, int, dict]
+    SUPPORTED_PARSERS = Literal["lxml", "html.parser"]
+
+import os
+import toml
+from pathlib import Path
+from importlib.util import find_spec
+from devgoldyutils import LoggerAdapter
+
+from . import players, utils
+from .logger import mov_cli_logger
+
+__all__ = ("Config",)
+
+@final
+class ConfigUIData(TypedDict):
+    fzf: bool
+
+@final
+class ConfigHTTPData(TypedDict):
+    headers: Dict[str, str]
+
+@final
+class ConfigDownloadsData(TypedDict):
+    save_path: str
+
+@final
+class ScrapersData(TypedDict):
+    default: str
+
+@final
+class ConfigData(TypedDict):
+    version: int
+    debug: bool
+    player: str
+    parser: SUPPORTED_PARSERS
+    ui: ConfigUIData
+    http: ConfigHTTPData
+    downloads: ConfigDownloadsData
+    scrapers: ScrapersData
+    plugins: Dict[str, str]
+
+logger = LoggerAdapter(mov_cli_logger, prefix = "Config")
+
+class Config():
+    """Class that wraps the mov-cli configuration file. Mostly used under the CLI interface."""
+    def __init__(self, override_config: ConfigData = None, config_path: Path = None) -> None:
+        self.config_path = config_path
+
+        self.data: ConfigData = {}
+
+        if override_config is None:
+            self.config_path = self.__get_config_file()
+
+            try:
+                self.data = toml.load(self.config_path).get("mov-cli", {})
+            except toml.decoder.TomlDecodeError as e:
+                logger.critical(
+                    "Failed to read config.toml! Please check you haven't made any mistakes in the config." \
+                        f"All values will fallback to default. \nError: {e}"
+                )
+
+        else:
+            self.data = override_config
+
+    @property
+    def version(self) -> int:
+        return self.data.get("version", 1)
+
+    @property
+    def player(self) -> Type[Player]:
+        """Returns the player class that was configured in the config. Defaults to MPV."""
+        value = self.data.get("player", "mpv")
+
+        platform = utils.what_platform()
+
+        if value.lower() == "mpv":
+            return players.MPV(platform)
+        elif value.lower() == "vlc":
+            return players.VLC(platform)
+
+        return players.CustomPlayer(value)
+
+    @property
+    def plugins(self) -> Dict[str, str]:
+        return self.data.get("plugins", {"test": "mov-cli-test"})
+
+    @property
+    def editor(self) -> Optional[str]:
+        """Returns the editor that should be opened while editing."""
+        return self.data.get("editor")
+
+    @property
+    def default_scraper(self) -> Optional[str]:
+        """Returns the scraper that should be used to scrape by default."""
+        return self.data.get("scrapers", {}).get("default", None)
+
+    @property
+    def fzf_enabled(self) -> bool:
+        """Returns whether fzf is allowed to be used."""
+        return self.data.get("ui", {}).get("fzf", True)
+
+    @property
+    def parser(self) -> SUPPORTED_PARSERS | Any:
+        """Returns the parser type configured by the user else it just returns the default."""
+        default_parser = "lxml" if find_spec("lxml") else "html.parser"
+        return self.data.get("parser", default_parser)
+
+    @property
+    def download_location(self) -> str:
+        """Returns download location. Defaults to OS's download location."""
+        return self.data.get("downloads", {}).get("save_path", os.getcwd())
+
+    @property
+    def debug(self) -> bool:
+        """Returns whether debug should be enabled or not."""
+        return self.data.get("debug", False)
+
+    @property
+    def proxy(self) -> dict | None:
+        """Returns proxy data. Defaults to None"""
+        proxy_config = self.data.get("proxy")
+
+        if proxy_config is not None:
+            proxy = None
+
+            username = proxy_config.get("username")
+            password = proxy_config.get("password")
+
+            scheme = proxy_config.get("scheme")
+            ip = proxy_config.get("ip")
+            port = proxy_config.get("port")
+
+            if username and password:
+                proxy = f"{scheme}://{username}:{password}@{ip}:{port}"
+            else:
+                proxy = f"{scheme}://{ip}:{port}"
+
+            return {"all://": proxy}
+        else:
+            return None
+
+    @property
+    def http_headers(self) -> dict:
+        """Returns http headers."""
+        default_headers = {
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/117.0",
+            "Accept-Language": "en-US,en;q=0.5",
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
+        }
+
+        return self.data.get("http", {}).get("headers", default_headers)
+
+    def __get_config_file(self) -> Path:
+        """Function that returns the path to the config file with multi platform support."""
+        platform = utils.what_platform()
+
+        appdata_dir = Path("./mov-cli-temp")
+
+        if platform == "Windows":
+            user_profile = Path(os.getenv("USERPROFILE"))
+            appdata_dir = user_profile.joinpath("AppData", "Local")
+
+        elif platform == "Darwin": # NOTE: Path maybe incorrect
+            user_profile = Path.home()
+            appdata_dir = user_profile.joinpath("Library", "Application Support")
+
+        elif platform == "iOS":
+            user_profile = Path(os.getenv("HOME"))
+            appdata_dir = user_profile.joinpath("Library")
+
+            appdata_dir.mkdir(exist_ok = True)
+
+        elif platform == "Linux" or platform == "Android":
+            user_profile = Path(os.getenv("HOME"))
+            appdata_dir = user_profile.joinpath(".config")
+ 
+            appdata_dir.mkdir(exist_ok = True) # on android the .config file may not exist.
+
+        config_path = appdata_dir.joinpath("mov-cli", "config.toml")
+        config_path.parent.mkdir(exist_ok = True)
+
+        if not config_path.exists():
+            logger.debug("The 'config.toml' file doesn't exist so we're creating it...")
+            config_file = open(config_path, "w")
+
+            template_config_path = f"{Path(os.path.split(__file__)[0])}{os.sep}config.template.toml"
+
+            with open(template_config_path, "r") as config_template:
+                config_file.write(config_template.read())
+
+            config_file.close()
+            logger.info(f"Config created at '{config_path}'.")
+
+        return config_path
```

### Comparing `mov-cli-4.2.8/mov_cli/download.py` & `mov-cli-4.2.9/mov_cli/download.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-import subprocess
-import unicodedata
-import os
-
-__all__ = ("Download",)
-
-if TYPE_CHECKING:
-    from .config import Config
-    from .media import Series, Movie
-
-class Download():
-    def __init__(self, config: Config) -> None:
-        self.config = config
-
-    def download(self, media: Series | Movie, subtitles: str = None) -> subprocess.Popen:
-        title = unicodedata.normalize('NFKD', media.display_name).encode('ascii', 'ignore').decode('ascii') # normalize title
-        
-        file = os.path.join(self.config.download_location, title + ".mp4")
-
-        args = [
-            "ffmpeg",
-            "-n",
-            "-thread_queue_size",
-            "4096",
-            "-headers",
-            f"Referer: {media.referrer}",
-            "-i",
-            media.url,
-            "-c",
-            "copy",
-        ]
-
-        if subtitles:
-            args.extend(["-vf", f"subtitle={subtitles}"])
-
-        args.append(file)
-
-        return subprocess.Popen(args)
+from __future__ import annotations
+from typing import TYPE_CHECKING
+import subprocess
+import unicodedata
+import os
+
+__all__ = ("Download",)
+
+if TYPE_CHECKING:
+    from .config import Config
+    from .media import Series, Movie
+
+class Download():
+    def __init__(self, config: Config) -> None:
+        self.config = config
+
+    def download(self, media: Series | Movie, subtitles: str = None) -> subprocess.Popen:
+        title = unicodedata.normalize('NFKD', media.display_name).encode('ascii', 'ignore').decode('ascii') # normalize title
+        
+        file = os.path.join(self.config.download_location, title + ".mp4")
+
+        args = [
+            "ffmpeg",
+            "-n",
+            "-thread_queue_size",
+            "4096",
+            "-headers",
+            f"Referer: {media.referrer}",
+            "-i",
+            media.url,
+            "-c",
+            "copy",
+        ]
+
+        if subtitles:
+            args.extend(["-vf", f"subtitle={subtitles}"])
+
+        args.append(file)
+
+        return subprocess.Popen(args)
```

### Comparing `mov-cli-4.2.8/mov_cli/errors.py` & `mov-cli-4.2.9/mov_cli/errors.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    import logging
-    from .players import Player
-
-from devgoldyutils import Colours
-from .logger import mov_cli_logger
-
-class MovCliException(Exception):
-    """Raises whenever there's a known error in mov-cli."""
-    def __init__(self, message: str, logger: logging.Logger = None):
-        message = Colours.RED.apply_to_string(message)
-
-        if logger is None:
-            logger = mov_cli_logger
-
-        logger.critical(message)
-        super().__init__(message)
-
-# NOTE: I might remove this. ~ Goldy
-class PlayerNotFound(MovCliException):
-    """Raised when player is not found."""
-    def __init__(self, player: Player) -> None:
-        super().__init__(
-            f"The player '{player.__class__.__name__}' was not found. Are you sure you have it installed? " \
-            "Are you sure the environment variable is set correctly?"
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    import logging
+    from .players import Player
+
+from devgoldyutils import Colours
+from .logger import mov_cli_logger
+
+class MovCliException(Exception):
+    """Raises whenever there's a known error in mov-cli."""
+    def __init__(self, message: str, logger: logging.Logger = None):
+        message = Colours.RED.apply_to_string(message)
+
+        if logger is None:
+            logger = mov_cli_logger
+
+        logger.critical(message)
+        super().__init__(message)
+
+# NOTE: I might remove this. ~ Goldy
+class PlayerNotFound(MovCliException):
+    """Raised when player is not found."""
+    def __init__(self, player: Player) -> None:
+        super().__init__(
+            f"The player '{player.__class__.__name__}' was not found. Are you sure you have it installed? " \
+            "Are you sure the environment variable is set correctly?"
         )
```

### Comparing `mov-cli-4.2.8/mov_cli/http_client.py` & `mov-cli-4.2.9/mov_cli/http_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from httpx import Response
-    from .config import Config
-
-import httpx
-from devgoldyutils import LoggerAdapter, Colours
-
-from . import errors
-from .logger import mov_cli_logger
-
-__all__ = ("HTTPClient",)
-
-class SiteMaybeBlocked(errors.MovCliException):
-    """Raises there's a connection error during a get request."""
-    def __init__(self, url: str, error: httpx.ConnectError) -> None:
-        super().__init__(
-            f"A connection error occurred while making a GET request to '{url}'.\n" \
-            "There's most likely nothing wrong with mov-cli. Your ISP's DNS could be blocking this site or perhaps the site is down. " \
-            f"{Colours.GREEN}SOLUTION: Use a VPN or switch DNS!{Colours.RED}\n" \
-            f"Actual Error >> {error}"
-        )
-
-class HTTPClient():
-    def __init__(self, config: Config) -> None:
-        """A base class for building scrapers from."""
-        self.config = config
-        self.logger = LoggerAdapter(mov_cli_logger, prefix = self.__class__.__name__)
-
-        self.__httpx_client = httpx.Client(
-            timeout = 15.0,
-            cookies = None
-        )
-
-        super().__init__()
-
-    def get(
-        self, 
-        url: str, 
-        headers: dict = {}, 
-        include_default_headers: bool = True, 
-        redirect: bool = False, 
-        **kwargs
-    ) -> Response:
-        """Performs a GET request and returns httpx.Response."""
-        self.logger.debug(Colours.GREEN.apply("GET") + f" -> {url}")
-
-        if include_default_headers is True:
-            headers.update({"Referer": url})
-            headers.update(self.config.http_headers)
-
-        try:
-            response = self.__httpx_client.get(
-                url, 
-                headers = headers, 
-                follow_redirects = redirect, 
-                **kwargs
-            )
-
-            if response.is_error:
-                self.logger.error(
-                    f"GET Request to {response.url} failed! ({response})"
-                )
-
-            return response
-
-        except httpx.ConnectError as e:
-            if "[SSL: CERTIFICATE_VERIFY_FAILED]" in str(e):
-                raise SiteMaybeBlocked(url, e)
-
-            raise e
-
-    def post(self, url: str, data: dict = None, json: dict = None, **kwargs) -> Response: 
-        """Performs a POST request and returns httpx.Response."""
-        self.logger.debug(Colours.ORANGE.apply("POST") + f": {url}")
-
-        self.__httpx_client.headers["Referer"] = url
-
-        return self.__httpx_client.post(
-            url, data = data, json = json, **kwargs
-        )
-
-    def set_cookies(self, cookies: dict) -> None:
-        """Sets cookies."""
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from httpx import Response
+    from .config import Config
+
+import httpx
+from devgoldyutils import LoggerAdapter, Colours
+
+from . import errors
+from .logger import mov_cli_logger
+
+__all__ = ("HTTPClient",)
+
+class SiteMaybeBlocked(errors.MovCliException):
+    """Raises there's a connection error during a get request."""
+    def __init__(self, url: str, error: httpx.ConnectError) -> None:
+        super().__init__(
+            f"A connection error occurred while making a GET request to '{url}'.\n" \
+            "There's most likely nothing wrong with mov-cli. Your ISP's DNS could be blocking this site or perhaps the site is down. " \
+            f"{Colours.GREEN}SOLUTION: Use a VPN or switch DNS!{Colours.RED}\n" \
+            f"Actual Error >> {error}"
+        )
+
+class HTTPClient():
+    def __init__(self, config: Config) -> None:
+        """A base class for building scrapers from."""
+        self.config = config
+        self.logger = LoggerAdapter(mov_cli_logger, prefix = self.__class__.__name__)
+
+        self.__httpx_client = httpx.Client(
+            timeout = 15.0,
+            cookies = None
+        )
+
+        super().__init__()
+
+    def get(
+        self, 
+        url: str, 
+        headers: dict = {}, 
+        include_default_headers: bool = True, 
+        redirect: bool = False, 
+        **kwargs
+    ) -> Response:
+        """Performs a GET request and returns httpx.Response."""
+        self.logger.debug(Colours.GREEN.apply("GET") + f" -> {url}")
+
+        if include_default_headers is True:
+            headers.update({"Referer": url})
+            headers.update(self.config.http_headers)
+
+        try:
+            response = self.__httpx_client.get(
+                url, 
+                headers = headers, 
+                follow_redirects = redirect, 
+                **kwargs
+            )
+
+            if response.is_error:
+                self.logger.debug(
+                    f"GET Request to '{response.url}' failed! ({response})"
+                )
+
+            return response
+
+        except httpx.ConnectError as e:
+            if "[SSL: CERTIFICATE_VERIFY_FAILED]" in str(e):
+                raise SiteMaybeBlocked(url, e)
+
+            raise e
+
+    def post(self, url: str, data: dict = None, json: dict = None, **kwargs) -> Response: 
+        """Performs a POST request and returns httpx.Response."""
+        self.logger.debug(Colours.ORANGE.apply("POST") + f": {url}")
+
+        self.__httpx_client.headers["Referer"] = url
+
+        return self.__httpx_client.post(
+            url, data = data, json = json, **kwargs
+        )
+
+    def set_cookies(self, cookies: dict) -> None:
+        """Sets cookies."""
         self.__httpx_client.cookies = cookies
```

### Comparing `mov-cli-4.2.8/mov_cli/iterfzf/__init__.py` & `mov-cli-4.2.9/mov_cli/iterfzf/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-"""
-Ported over from [goldy's fork](https://github.com/THEGOLDENPRO/iterfzf/) of [iterfzf](https://github.com/dahlia/iterfzf) 
-as of [issue #238](https://github.com/mov-cli/mov-cli/issues/238).
-
-Source code changes can be seen [here](https://github.com/THEGOLDENPRO/iterfzf/commits/main/).
-"""
-
-from __future__ import print_function, annotations
-from typing import TYPE_CHECKING
-
-import sys
-import errno
-import subprocess
-from os import fspath, PathLike
-
-if TYPE_CHECKING:
-    from typing import AnyStr, Iterable, Literal, Optional, Tuple, TypeVar
-
-    T = TypeVar("T")
-
-__all__ = (
-    '__fzf_version__', 
-    '__version__', 
-    'BUNDLED_EXECUTABLE', 
-    'iterfzf'
-)
-
-__fzf_version__ = '0.42.0'
-__version__ = '1.0.' + __fzf_version__
-
-POSIX_EXECUTABLE_NAME: Literal['fzf'] = 'fzf'
-WINDOWS_EXECUTABLE_NAME: Literal['fzf.exe'] = 'fzf.exe'
-EXECUTABLE_NAME: Literal['fzf', 'fzf.exe'] = \
-    WINDOWS_EXECUTABLE_NAME \
-    if sys.platform == 'win32' \
-    else POSIX_EXECUTABLE_NAME
-
-
-def iterfzf(
-    iterable: Iterable[Tuple[AnyStr, T]],
-    *,
-    # Search mode:
-    extended: bool = True,
-    exact: bool = False,
-    case_sensitive: bool = None,
-    # Interface:
-    multi: bool = False,
-    mouse: bool = True,
-    print_query: bool = False,
-    # Layout:
-    prompt: str = '> ',
-    ansi: bool = False,
-    preview: Optional[str] = None,
-    # Misc:
-    query: str = '',
-    encoding: Optional[str] = None,
-    executable: PathLike = EXECUTABLE_NAME
-):
-    cmd = [fspath(executable), '--no-sort', '--prompt=' + prompt]
-    if not extended:
-        cmd.append('--no-extended')
-    if case_sensitive is not None:
-        cmd.append('+i' if case_sensitive else '-i')
-    if exact:
-        cmd.append('--exact')
-    if multi:
-        cmd.append('--multi')
-    if not mouse:
-        cmd.append('--no-mouse')
-    if print_query:
-        cmd.append('--print-query')
-    if query:
-        cmd.append('--query=' + query)
-    if preview:
-        cmd.append('--preview=' + preview)
-    if ansi:
-        cmd.append('--ansi')
-    encoding = encoding or sys.getdefaultencoding()
-    proc = None
-    stdin = None
-    byte = None
-    lf = u'\n'
-    cr = u'\r'
-    for line in iterable:
-        line = line[0]
-
-        if byte is None:
-            byte = isinstance(line, bytes)
-            if byte:
-                lf = b'\n'
-                cr = b'\r'
-        elif isinstance(line, bytes) is not byte:
-            raise ValueError(
-                'element values must be all byte strings or all '
-                'unicode strings, not mixed of them: ' + repr(line)
-            )
-        if lf in line or cr in line:
-            raise ValueError(
-                r"element values must not contain CR({1!r})/"
-                r"LF({2!r}): {0!r}".format(line, cr, lf)
-            )
-        if proc is None:
-            proc = subprocess.Popen(
-                cmd,
-                stdin=subprocess.PIPE,
-                stdout=subprocess.PIPE,
-                stderr=None
-            )
-            stdin = proc.stdin
-        if not byte:
-            line = line.encode(encoding)
-        try:
-            stdin.write(line + b'\n')
-            stdin.flush()
-        except IOError as e:
-            if e.errno != errno.EPIPE and errno.EPIPE != 32:
-                raise
-            break
-    if proc is None or proc.wait() not in [0, 1]:
-        if print_query:
-            return None, None
-        else:
-            return None
-    try:
-        stdin.close()
-    except IOError as e:
-        if e.errno != errno.EPIPE and errno.EPIPE != 32:
-            raise
-    stdout = proc.stdout
-    decode = (lambda b: b) if byte else (lambda t: t.decode(encoding))
-    output = [decode(ln.strip(b'\r\n\0')) for ln in iter(stdout.readline, b'')]
-    if print_query:
-        try:
-            if multi:
-                return output[0], output[1:]
-            else:
-                return output[0], output[1]
-        except IndexError:
-            return output[0], None
-    else:
-        if multi:
-            return output
-        else:
-            try:
-                return output[0]
-            except IndexError:
+"""
+Ported over from [goldy's fork](https://github.com/THEGOLDENPRO/iterfzf/) of [iterfzf](https://github.com/dahlia/iterfzf) 
+as of [issue #238](https://github.com/mov-cli/mov-cli/issues/238).
+
+Source code changes can be seen [here](https://github.com/THEGOLDENPRO/iterfzf/commits/main/).
+"""
+
+from __future__ import print_function, annotations
+from typing import TYPE_CHECKING
+
+import sys
+import errno
+import subprocess
+from os import fspath, PathLike
+
+if TYPE_CHECKING:
+    from typing import AnyStr, Iterable, Literal, Optional, Tuple, TypeVar
+
+    T = TypeVar("T")
+
+__all__ = (
+    '__fzf_version__', 
+    '__version__', 
+    'BUNDLED_EXECUTABLE', 
+    'iterfzf'
+)
+
+__fzf_version__ = '0.42.0'
+__version__ = '1.0.' + __fzf_version__
+
+POSIX_EXECUTABLE_NAME: Literal['fzf'] = 'fzf'
+WINDOWS_EXECUTABLE_NAME: Literal['fzf.exe'] = 'fzf.exe'
+EXECUTABLE_NAME: Literal['fzf', 'fzf.exe'] = \
+    WINDOWS_EXECUTABLE_NAME \
+    if sys.platform == 'win32' \
+    else POSIX_EXECUTABLE_NAME
+
+
+def iterfzf(
+    iterable: Iterable[Tuple[AnyStr, T]],
+    *,
+    # Search mode:
+    extended: bool = True,
+    exact: bool = False,
+    case_sensitive: bool = None,
+    # Interface:
+    multi: bool = False,
+    mouse: bool = True,
+    print_query: bool = False,
+    # Layout:
+    prompt: str = '> ',
+    ansi: bool = False,
+    preview: Optional[str] = None,
+    # Misc:
+    query: str = '',
+    encoding: Optional[str] = None,
+    executable: PathLike = EXECUTABLE_NAME
+):
+    cmd = [fspath(executable), '--no-sort', '--prompt=' + prompt]
+    if not extended:
+        cmd.append('--no-extended')
+    if case_sensitive is not None:
+        cmd.append('+i' if case_sensitive else '-i')
+    if exact:
+        cmd.append('--exact')
+    if multi:
+        cmd.append('--multi')
+    if not mouse:
+        cmd.append('--no-mouse')
+    if print_query:
+        cmd.append('--print-query')
+    if query:
+        cmd.append('--query=' + query)
+    if preview:
+        cmd.append('--preview=' + preview)
+    if ansi:
+        cmd.append('--ansi')
+    encoding = encoding or sys.getdefaultencoding()
+    proc = None
+    stdin = None
+    byte = None
+    lf = u'\n'
+    cr = u'\r'
+    for line in iterable:
+        line = line[0]
+
+        if byte is None:
+            byte = isinstance(line, bytes)
+            if byte:
+                lf = b'\n'
+                cr = b'\r'
+        elif isinstance(line, bytes) is not byte:
+            raise ValueError(
+                'element values must be all byte strings or all '
+                'unicode strings, not mixed of them: ' + repr(line)
+            )
+        if lf in line or cr in line:
+            raise ValueError(
+                r"element values must not contain CR({1!r})/"
+                r"LF({2!r}): {0!r}".format(line, cr, lf)
+            )
+        if proc is None:
+            proc = subprocess.Popen(
+                cmd,
+                stdin=subprocess.PIPE,
+                stdout=subprocess.PIPE,
+                stderr=None
+            )
+            stdin = proc.stdin
+        if not byte:
+            line = line.encode(encoding)
+        try:
+            stdin.write(line + b'\n')
+            stdin.flush()
+        except IOError as e:
+            if e.errno != errno.EPIPE and errno.EPIPE != 32:
+                raise
+            break
+    if proc is None or proc.wait() not in [0, 1]:
+        if print_query:
+            return None, None
+        else:
+            return None
+    try:
+        stdin.close()
+    except IOError as e:
+        if e.errno != errno.EPIPE and errno.EPIPE != 32:
+            raise
+    stdout = proc.stdout
+    decode = (lambda b: b) if byte else (lambda t: t.decode(encoding))
+    output = [decode(ln.strip(b'\r\n\0')) for ln in iter(stdout.readline, b'')]
+    if print_query:
+        try:
+            if multi:
+                return output[0], output[1:]
+            else:
+                return output[0], output[1]
+        except IndexError:
+            return output[0], None
+    else:
+        if multi:
+            return output
+        else:
+            try:
+                return output[0]
+            except IndexError:
                 return None
```

### Comparing `mov-cli-4.2.8/mov_cli/media/media.py` & `mov-cli-4.2.9/mov_cli/media/media.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing import Optional
-    from ..utils import EpisodeSelector
-
-from abc import abstractmethod
-
-__all__ = (
-    "Media", 
-    "Series", 
-    "Movie"
-)
-
-class Media():
-    """Represents any piece of media in mov-cli that can be streamed or downloaded."""
-    def __init__(self, url: str, title: str, referrer: Optional[str]) -> None:
-        self.url = url
-        """The stream-able url."""
-        self.title = title
-        """A title to represent this stream-able media."""
-        self.referrer = referrer
-        """The required referrer for streaming the media content."""
-
-    @property
-    @abstractmethod
-    def display_name(self) -> str:
-        """The title that should be displayed by the player."""
-        ...
-
-class Series(Media):
-    """Represents a TV Show. E.g an Anime or Cartoon."""
-    def __init__(
-        self, 
-        url: str, 
-        title: str, 
-        episode: EpisodeSelector, 
-        referrer: Optional[str] = None, 
-        subtitles: Optional[dict] = None
-    ) -> None:
-        self.episode = episode
-        """The episode and season of this series."""
-        self.subtitles = subtitles
-
-        super().__init__(
-            url, title, referrer
-        )
-
-    @property
-    def display_name(self) -> str:
-        return f"{self.title} - S{self.episode.season} EP{self.episode.episode}"
-
-class Movie(Media):
-    """Represents a Film/Movie."""
-    def __init__(
-        self, 
-        url: str,
-        title: str,
-        referrer: Optional[str] = None,
-        year: Optional[str] = None,
-        subtitles: Optional[dict] = None
-    ) -> None:
-        self.year = year
-        """The year this film was released."""
-        self.subtitles = subtitles
-
-        super().__init__(
-            url, title, referrer
-        )
-
-    @property
-    def display_name(self) -> str:
-        return f"{self.title} ({self.year})"
-
-
-# class LiveTV(Media):
-#     """Represents media that is live, like a tv channel or a live stream."""
-#     def __init__(
-#         self, 
-#         url: str, 
-#         title: str, 
-#         referrer: str, 
-#     ) -> None:
-
-#         super().__init__(
-#             url, title, referrer
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Optional
+    from ..utils import EpisodeSelector
+
+from abc import abstractmethod
+
+__all__ = (
+    "Media", 
+    "Series", 
+    "Movie"
+)
+
+class Media():
+    """Represents any piece of media in mov-cli that can be streamed or downloaded."""
+    def __init__(self, url: str, title: str, referrer: Optional[str]) -> None:
+        self.url = url
+        """The stream-able url."""
+        self.title = title
+        """A title to represent this stream-able media."""
+        self.referrer = referrer
+        """The required referrer for streaming the media content."""
+
+    @property
+    @abstractmethod
+    def display_name(self) -> str:
+        """The title that should be displayed by the player."""
+        ...
+
+class Series(Media):
+    """Represents a TV Show. E.g an Anime or Cartoon."""
+    def __init__(
+        self, 
+        url: str, 
+        title: str, 
+        episode: EpisodeSelector, 
+        referrer: Optional[str] = None, 
+        subtitles: Optional[dict] = None
+    ) -> None:
+        self.episode = episode
+        """The episode and season of this series."""
+        self.subtitles = subtitles
+
+        super().__init__(
+            url, title, referrer
+        )
+
+    @property
+    def display_name(self) -> str:
+        return f"{self.title} - S{self.episode.season} EP{self.episode.episode}"
+
+class Movie(Media):
+    """Represents a Film/Movie."""
+    def __init__(
+        self, 
+        url: str,
+        title: str,
+        referrer: Optional[str] = None,
+        year: Optional[str] = None,
+        subtitles: Optional[dict] = None
+    ) -> None:
+        self.year = year
+        """The year this film was released."""
+        self.subtitles = subtitles
+
+        super().__init__(
+            url, title, referrer
+        )
+
+    @property
+    def display_name(self) -> str:
+        return f"{self.title} ({self.year})"
+
+
+# class LiveTV(Media):
+#     """Represents media that is live, like a tv channel or a live stream."""
+#     def __init__(
+#         self, 
+#         url: str, 
+#         title: str, 
+#         referrer: str, 
+#     ) -> None:
+
+#         super().__init__(
+#             url, title, referrer
 #         )
```

### Comparing `mov-cli-4.2.8/mov_cli/media/metadata.py` & `mov-cli-4.2.9/mov_cli/media/metadata.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing import List, Callable, Optional, Tuple
-
-from enum import Enum
-from dataclasses import dataclass, field
-
-__all__ = ("MetadataType", "Metadata", "ExtraMetadata", "AiringType")
-
-class MetadataType(Enum):
-    SERIES = 0
-    """Media with multiple seasons and episodes."""
-    MOVIE = 1
-    """Media with no seasons and episodes. Like a film or short animation."""
-    LIVE = 2
-    """Media that is live, like a tv channel or a live stream."""
-
-class AiringType(Enum):
-    DONE = 0
-    ONGOING = 1
-    PRODUCTION = 2
-    RELEASED = 3
-    CANCELED = 4
-
-@dataclass
-class Metadata:
-    """Search results from the providers."""
-    id: str
-    title: str
-    """Title of the Series, Film or TV Station."""
-    type: MetadataType
-    """The type of metadata. Is it a Series, Film or LIVE TV Station?"""
-    year: Optional[str] = field(default = None)
-    """Year the Series or Film was released."""
-
-    extra_func: Callable[[], Optional[ExtraMetadata]] = field(default = lambda: None)
-    """Callback that returns extra metadata."""
-
-    def get_extra(self) -> Optional[ExtraMetadata]:
-        """Returns extra metadata."""
-        return self.extra_func()
-
-@dataclass
-class ExtraMetadata():
-    """More in-depth metadata about media."""
-    description: Optional[str]
-    """Description of Series, Film or TV Station."""
-    image_url: Optional[str]
-    """Url to high res image cover of Series, Film or TV Station."""
-
-    alternate_titles: List[str] | Tuple[str, str]
-
-    cast: List[str] | None = field(default = None)
-    genres: List[str] | None = field(default = None)
-
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import List, Callable, Optional, Tuple
+
+from enum import Enum
+from dataclasses import dataclass, field
+
+__all__ = ("MetadataType", "Metadata", "ExtraMetadata", "AiringType")
+
+class MetadataType(Enum):
+    SERIES = 0
+    """Media with multiple seasons and episodes."""
+    MOVIE = 1
+    """Media with no seasons and episodes. Like a film or short animation."""
+    LIVE = 2
+    """Media that is live, like a tv channel or a live stream."""
+
+class AiringType(Enum):
+    DONE = 0
+    ONGOING = 1
+    PRODUCTION = 2
+    RELEASED = 3
+    CANCELED = 4
+
+@dataclass
+class Metadata:
+    """Search results from the providers."""
+    id: str
+    title: str
+    """Title of the Series, Film or TV Station."""
+    type: MetadataType
+    """The type of metadata. Is it a Series, Film or LIVE TV Station?"""
+    year: Optional[str] = field(default = None)
+    """Year the Series or Film was released."""
+
+    extra_func: Callable[[], Optional[ExtraMetadata]] = field(default = lambda: None)
+    """Callback that returns extra metadata."""
+
+    def get_extra(self) -> Optional[ExtraMetadata]:
+        """Returns extra metadata."""
+        return self.extra_func()
+
+@dataclass
+class ExtraMetadata():
+    """More in-depth metadata about media."""
+    description: Optional[str]
+    """Description of Series, Film or TV Station."""
+    image_url: Optional[str]
+    """Url to high res image cover of Series, Film or TV Station."""
+
+    alternate_titles: List[str] | Tuple[str, str]
+
+    cast: List[str] | None = field(default = None)
+    genres: List[str] | None = field(default = None)
+
     airing: AiringType | None = field(default = None)
```

### Comparing `mov-cli-4.2.8/mov_cli/players/custom_player.py` & `mov-cli-4.2.9/mov_cli/players/custom_player.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from ..media import Media
-
-import subprocess
-from devgoldyutils import Colours, LoggerAdapter
-
-from .. import errors
-from ..logger import mov_cli_logger
-from .player import Player
-
-__all__ = ("CustomPlayer",)
-
-logger = LoggerAdapter(mov_cli_logger, prefix = Colours.GREY.apply("CustomPlayer"))
-
-class CustomPlayer(Player):
-    """
-    This player is invoked if you set a player that is not supported by mov-cli in the config, allowing users to invoke their own players.
-    """
-    def __init__(self, player_command: str, **kwargs) -> None:
-        self.player_command = player_command
-
-        super().__init__(**kwargs)
-
-    def play(self, media: Media) -> subprocess.Popen:
-        """Plays this media in a custom player."""
-        logger.info(f"Launching your custom media player '{self.player_command}'...")
-
-        try:
-            return subprocess.Popen(
-                [self.player_command, media.url]
-            )
-        except ModuleNotFoundError:
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from ..media import Media
+
+import subprocess
+from devgoldyutils import Colours, LoggerAdapter
+
+from .. import errors
+from ..logger import mov_cli_logger
+from .player import Player
+
+__all__ = ("CustomPlayer",)
+
+logger = LoggerAdapter(mov_cli_logger, prefix = Colours.GREY.apply("CustomPlayer"))
+
+class CustomPlayer(Player):
+    """
+    This player is invoked if you set a player that is not supported by mov-cli in the config, allowing users to invoke their own players.
+    """
+    def __init__(self, player_command: str, **kwargs) -> None:
+        self.player_command = player_command
+
+        super().__init__(**kwargs)
+
+    def play(self, media: Media) -> subprocess.Popen:
+        """Plays this media in a custom player."""
+        logger.info(f"Launching your custom media player '{self.player_command}'...")
+
+        try:
+            return subprocess.Popen(
+                [self.player_command, media.url]
+            )
+        except ModuleNotFoundError:
             raise errors.PlayerNotFound(self)
```

### Comparing `mov-cli-4.2.8/mov_cli/players/player.py` & `mov-cli-4.2.9/mov_cli/players/player.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing import Optional
-
-    from ..media import Media
-
-import subprocess
-from abc import ABC, abstractmethod
-
-__all__ = ("Player",)
-
-class Player(ABC):
-    """A base class for all players in mov-cli."""
-    def __init__(self, **kwargs) -> None:
-        super().__init__()
-
-    @abstractmethod
-    def play(self, media: Media) -> Optional[subprocess.Popen]:
-        """Method to be overridden with code to play media in that specific player."""
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Optional
+
+    from ..media import Media
+
+import subprocess
+from abc import ABC, abstractmethod
+
+__all__ = ("Player",)
+
+class Player(ABC):
+    """A base class for all players in mov-cli."""
+    def __init__(self, **kwargs) -> None:
+        super().__init__()
+
+    @abstractmethod
+    def play(self, media: Media) -> Optional[subprocess.Popen]:
+        """Method to be overridden with code to play media in that specific player."""
         ...
```

### Comparing `mov-cli-4.2.8/mov_cli/plugins.py` & `mov-cli-4.2.9/mov_cli/plugins.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-"""
-Module containing mov-cli plugin related stuff.
-"""
-from __future__ import annotations
-from typing import TYPE_CHECKING, TypedDict
-
-if TYPE_CHECKING:
-    from typing import Optional, Dict, Literal
-
-    from .scraper import Scraper
-
-import importlib
-from devgoldyutils import LoggerAdapter
-
-from .logger import mov_cli_logger
-
-__all__ = (
-    "load_plugin", 
-    "PluginHookData"
-)
-
-logger = LoggerAdapter(mov_cli_logger, prefix = "Plugins")
-
-class PluginHookData(TypedDict):
-    version: int
-    scrapers: Dict[str, Scraper] | Dict[Literal["DEFAULT"], Scraper]
-
-def load_plugin(module_name: str) -> Optional[PluginHookData]:
-    try:
-        plugin_module = importlib.import_module(module_name.replace("-", "_"))
-    except ModuleNotFoundError as e:
-        logger.error(f"Failed to import a plugin from the module '{module_name}'! Error --> {e}")
-        return None
-
-    plugin_data = getattr(plugin_module, "plugin", None)
-
-    if plugin_data is None:
-        logger.warning(f"Failed to load the plugin '{module_name}'! It doesn't contain a plugin hook!")
-
+"""
+Module containing mov-cli plugin related stuff.
+"""
+from __future__ import annotations
+from typing import TYPE_CHECKING, TypedDict
+
+if TYPE_CHECKING:
+    from typing import Optional, Dict, Literal
+
+    from .scraper import Scraper
+
+import importlib
+from devgoldyutils import LoggerAdapter
+
+from .logger import mov_cli_logger
+
+__all__ = (
+    "load_plugin", 
+    "PluginHookData"
+)
+
+logger = LoggerAdapter(mov_cli_logger, prefix = "Plugins")
+
+class PluginHookData(TypedDict):
+    version: int
+    scrapers: Dict[str, Scraper] | Dict[Literal["DEFAULT"], Scraper]
+
+def load_plugin(module_name: str) -> Optional[PluginHookData]:
+    try:
+        plugin_module = importlib.import_module(module_name.replace("-", "_"))
+    except ModuleNotFoundError as e:
+        logger.error(f"Failed to import a plugin from the module '{module_name}'! Error --> {e}")
+        return None
+
+    plugin_data = getattr(plugin_module, "plugin", None)
+
+    if plugin_data is None:
+        logger.warning(f"Failed to load the plugin '{module_name}'! It doesn't contain a plugin hook!")
+
     return plugin_data
```

### Comparing `mov-cli-4.2.8/mov_cli/scraper.py` & `mov-cli-4.2.9/mov_cli/scraper.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing import Dict, Literal, Optional, Iterable
-    from .config import Config
-    from .http_client import HTTPClient
-    from .media import Metadata, Series, Movie
-    from .utils import EpisodeSelector
-
-from bs4 import BeautifulSoup
-from abc import ABC, abstractmethod
-from devgoldyutils import LoggerAdapter
-
-from . import errors
-from .logger import mov_cli_logger
-
-__all__ = ("Scraper", "MediaNotFound")
-
-class Scraper(ABC):
-    def __init__(self, config: Config, http_client: HTTPClient) -> None:
-        """A base class for building scrapers from."""
-        self.config = config
-        self.http_client = http_client
-        self.logger = LoggerAdapter(mov_cli_logger, prefix = self.__class__.__name__)
-
-        super().__init__()
-
-    def soup(self, html: str) -> BeautifulSoup:
-        return BeautifulSoup(html, self.config.parser)
-
-    @abstractmethod
-    def search(self, query: str, limit: int = 20) -> Iterable[Metadata]:
-        ...
-
-    @abstractmethod
-    def scrape(self, metadata: Metadata, episode: Optional[EpisodeSelector] = None, **kwargs) -> Series | Movie:
-        """
-        Where your searching and scraping for the media should be performed done. 
-        Should return an instance of Media.
-        """
-        ...
-
-    @abstractmethod
-    def scrape_episodes(self, metadata: Metadata, **kwargs) -> Dict[int, int] | Dict[None, Literal[1]]:
-        """Returns episode count for each season in that Movie/Series."""
-        ...
-
-class MediaNotFound(errors.MovCliException):
-    """Raises when a scraper fails to find a show/movie/tv-station."""
-    def __init__(self, message, scraper: Scraper) -> None:
-        super().__init__(
-            f"Failed to find media: {message}",
-            logger = scraper.logger
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Dict, Literal, Optional, Iterable
+    from .config import Config
+    from .http_client import HTTPClient
+    from .media import Metadata, Series, Movie
+    from .utils import EpisodeSelector
+
+from bs4 import BeautifulSoup
+from abc import ABC, abstractmethod
+from devgoldyutils import LoggerAdapter
+
+from . import errors
+from .logger import mov_cli_logger
+
+__all__ = ("Scraper", "MediaNotFound")
+
+class Scraper(ABC):
+    def __init__(self, config: Config, http_client: HTTPClient) -> None:
+        """A base class for building scrapers from."""
+        self.config = config
+        self.http_client = http_client
+        self.logger = LoggerAdapter(mov_cli_logger, prefix = self.__class__.__name__)
+
+        super().__init__()
+
+    def soup(self, html: str) -> BeautifulSoup:
+        return BeautifulSoup(html, self.config.parser)
+
+    @abstractmethod
+    def search(self, query: str, limit: int = 20) -> Iterable[Metadata]:
+        ...
+
+    @abstractmethod
+    def scrape(self, metadata: Metadata, episode: Optional[EpisodeSelector] = None, **kwargs) -> Series | Movie:
+        """
+        Where your searching and scraping for the media should be performed done. 
+        Should return an instance of Media.
+        """
+        ...
+
+    @abstractmethod
+    def scrape_episodes(self, metadata: Metadata, **kwargs) -> Dict[int, int] | Dict[None, Literal[1]]:
+        """Returns episode count for each season in that Movie/Series."""
+        ...
+
+class MediaNotFound(errors.MovCliException):
+    """Raises when a scraper fails to find a show/movie/tv-station."""
+    def __init__(self, message, scraper: Scraper) -> None:
+        super().__init__(
+            f"Failed to find media: {message}",
+            logger = scraper.logger
         )
```

### Comparing `mov-cli-4.2.8/mov_cli/utils/platform.py` & `mov-cli-4.2.9/mov_cli/utils/platform.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing import Literal
-
-    SUPPORTED_PLATFORMS = Literal["Windows", "Linux", "Android", "Darwin", "iOS"]
-
-import sys
-import platform
-
-__all__ = ("what_platform",)
-
-def what_platform() -> SUPPORTED_PLATFORMS:
-    """
-    Returns what platform/OS this device is running on.
-
-    E.g. Windows, Linux, Android, Darwin, iOS
-    """
-    os = platform.system()
-
-    if os == "Linux":
-        if hasattr(sys, "getandroidapilevel"):
-            return "Android"
-        elif "-ish" in platform.platform():
-            return "iOS"
-
-        return os
-
-    return os
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Literal
+
+    SUPPORTED_PLATFORMS = Literal["Windows", "Linux", "Android", "Darwin", "iOS"]
+
+import sys
+import platform
+
+__all__ = ("what_platform",)
+
+def what_platform() -> SUPPORTED_PLATFORMS:
+    """
+    Returns what platform/OS this device is running on.
+
+    E.g. Windows, Linux, Android, Darwin, iOS
+    """
+    os = platform.system()
+
+    if os == "Linux":
+        if hasattr(sys, "getandroidapilevel"):
+            return "Android"
+        elif "-ish" in platform.platform():
+            return "iOS"
+
+        return os
+
+    return os
```

### Comparing `mov-cli-4.2.8/mov_cli.egg-info/PKG-INFO` & `mov-cli-4.2.9/mov_cli.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-Metadata-Version: 2.1
-Name: mov-cli
-Version: 4.2.8
-Summary: Watch everything from your terminal.
-Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
-License: MIT License
-        
-        Copyright (c) 2024 mov-cli
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: GitHub, https://github.com/mov-cli/mov-cli
-Project-URL: BugTracker, https://github.com/mov-cli/mov-cli/issues
-Keywords: movie-cli,mov_cli
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: httpx
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: toml
-Requires-Dist: devgoldyutils>=2.5.7
-Requires-Dist: typer[all]==0.10.0
-Requires-Dist: inquirer
-Requires-Dist: beautifulsoup4
-Requires-Dist: Unidecode
-Requires-Dist: thefuzz
-Requires-Dist: deprecation
-Requires-Dist: mov-cli-test>=1.1.0
-Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev"
-
-<a name="readme-top"></a>
-
-[![Stargazers][stars-shield]][stars-url]
-[![Pypi Version][pypi-shield]][pypi-url]
-[![Python Versions][python-shield]][pypi-url]
-[![Issues][issues-shield]][issues-url]
-[![MIT License][license-shield]][license-url]
-[![Discord][discord-shield]][discord-url]
-
-<div align="center">
-
-  <a href="https://github.com/mov-cli/mov-cli">
-    <img src="https://github.com/mov-cli/mov-cli/assets/132799819/a23bec13-881d-41b9-b596-b31c6698b89e" alt="Logo" width="250">
-  </a>
-
-  <sub>Watch everything from your terminal.</sub>
-  <br>
-  <br>
-  <a href="https://github.com/mov-cli/mov-cli/issues">Report Bug</a>
-  ·
-  <a href="https://github.com/mov-cli/mov-cli/issues">Request Feature</a>
-
-</div>
-
-<br>
-
-> [!Note]
-> v4 is constantly changing so be sure to keep the tool up to date and with that said I would advise not using it as a library yet.
-
-## Installation 🛠️
-
-> [!TIP]
-> For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
-
-### Prerequisites
-- **A supported platform:**
-  - Linux
-  - Windows
-  - Android (via [Termux](https://termux.dev/en/))
-  - iOS (via [iSH Shell](https://ish.app/))
-  - *MacOS* (**Not tested**)
-- **[python](https://www.python.org/downloads/)** (**required**, with pip)
-- **[lxml](https://pypi.org/project/lxml/)** (optional, ⚡ faster scraping)
-- **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**)
-- **[mpv](https://mpv.io/installation/)** (recommended & default media player)
-
-To get running these are all the prerequisites you'll need.
-
-With the prerequisites installed, mov-cli can be installed via the pip command on all platforms with Python version 3.8 or above.
-
-```sh
-pip install mov-cli -U
-```
-
-## Usage 🖱️
-mov-cli comes packaged with a CLI interface via the `mov-cli` command you can use in your respective terminal. 
-
-> [!NOTE]
-> You may notice mov-cli doesn't ship with any scrapers (or previously known as providers) by default, this is because v4 is plugin-based and scrapers are now part of plugins that must be chosen to be installed.
-> Find out how to do so at the [wiki](https://github.com/mov-cli/mov-cli/wiki#plugins).
-
-1. Install the scraper plugin of your choice. Visit this [wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a list of **third-party** mov-cli plugins.
-```sh
-mov-cli -e
-```
-Alternatively, you may also edit by manually opening the config file. See the [Wiki](https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction).  
-```toml
-[mov-cli.plugins]
-films = "package_name"
-```
-
-
-2. Scraper away!
-```sh
-mov-cli -s films spider man no way home
-```
-<img width="370px" src="https://github.com/mov-cli/mov-cli/assets/66202304/86189cab-b246-405e-a266-6c624bee2d36">
-
-> The above command should search for `spider man no way home` with the following scraper.
-
-## Contributing ✨
-Pull requests are welcome and *appreciated*. For major changes, please open an issue first to discuss what you would like to change.
-
-<a href = "https://github.com/mov-cli/mov-cli/graphs/contributors">
-  <img src = "https://contrib.rocks/image?repo=mov-cli/mov-cli"/>
-</a>
-
-## Inspiration 🌟
-Inspired by [ani-cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/animdl)
-
-
-<!-- MARKDOWN LINKS & IMAGES -->
-<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
-[contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-cli.svg?style=for-the-badge
-[contributors-url]: https://github.com/mov-cli/mov-cli/graphs/contributors
-[forks-shield]: https://img.shields.io/github/forks/mov-cli/mov-cli.svg?style=for-the-badge
-[forks-url]: https://github.com/mov-cli/mov-cli/network/members
-[stars-shield]: https://img.shields.io/github/stars/mov-cli/mov-cli?style=flat
-[stars-url]: https://github.com/mov-cli/mov-cli/stargazers
-[pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
-[pypi-url]: https://pypi.org/project/mov-cli/
-[python-shield]: https://img.shields.io/pypi/pyversions/mov-cli?style=flat
-[issues-shield]: https://img.shields.io/github/issues/mov-cli/mov-cli?style=flat
-[issues-url]: https://github.com/mov-cli/mov-cli/issues
-[license-shield]: https://img.shields.io/github/license/mov-cli/mov-cli?style=flat
-[license-url]: ./LICENSE
-[discord-shield]: https://img.shields.io/badge/Discord-7289da?logo=discord&logoColor=white
-[discord-url]: https://discord.gg/BMzC7ePsBV
+Metadata-Version: 2.1
+Name: mov-cli
+Version: 4.2.9
+Summary: Watch everything from your terminal.
+Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.lol>, Goldy <goldy@devgoldy.xyz>
+License: MIT License
+        
+        Copyright (c) 2024 mov-cli
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: GitHub, https://github.com/mov-cli/mov-cli
+Project-URL: BugTracker, https://github.com/mov-cli/mov-cli/issues
+Keywords: movie-cli,mov_cli
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: httpx
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: toml
+Requires-Dist: devgoldyutils>=2.5.7
+Requires-Dist: typer[all]==0.10.0
+Requires-Dist: inquirer
+Requires-Dist: beautifulsoup4
+Requires-Dist: Unidecode
+Requires-Dist: thefuzz
+Requires-Dist: deprecation
+Requires-Dist: mov-cli-test>=1.1.0
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: devgoldyutils[pprint]>=2.5.7; extra == "dev"
+
+<a name="readme-top"></a>
+
+[![Stargazers][stars-shield]][stars-url]
+[![Pypi Version][pypi-shield]][pypi-url]
+[![Python Versions][python-shield]][pypi-url]
+[![Issues][issues-shield]][issues-url]
+[![MIT License][license-shield]][license-url]
+[![Discord][discord-shield]][discord-url]
+
+<div align="center">
+
+  <a href="https://github.com/mov-cli/mov-cli">
+    <img src="https://github.com/mov-cli/mov-cli/assets/132799819/a23bec13-881d-41b9-b596-b31c6698b89e" alt="Logo" width="250">
+  </a>
+
+  <sub>Watch everything from your terminal.</sub>
+  <br>
+  <br>
+  <a href="https://github.com/mov-cli/mov-cli/issues">Report Bug</a>
+  ·
+  <a href="https://github.com/mov-cli/mov-cli/issues">Request Feature</a>
+
+</div>
+
+<br>
+
+> [!Note]
+> v4 is constantly changing so be sure to keep the tool up to date and with that said I would advise not using it as a library yet.
+
+## Installation 🛠️
+
+> [!TIP]
+> For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
+
+### Prerequisites
+- **A supported platform:**
+  - Linux
+  - Windows
+  - Android (via [Termux](https://termux.dev/en/))
+  - iOS (via [iSH Shell](https://ish.app/))
+  - *MacOS* (**Not tested**)
+- **[python](https://www.python.org/downloads/)** (**required**, with pip)
+- **[lxml](https://pypi.org/project/lxml/)** (optional, ⚡ faster scraping)
+- **[fzf](https://github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**)
+- **[mpv](https://mpv.io/installation/)** (recommended & default media player)
+
+To get running these are all the prerequisites you'll need.
+
+With the prerequisites installed, mov-cli can be installed via the pip command on all platforms with Python version 3.8 or above.
+
+```sh
+pip install mov-cli -U
+```
+
+## Usage 🖱️
+mov-cli comes packaged with a CLI interface via the `mov-cli` command you can use in your respective terminal. 
+
+> [!NOTE]
+> You may notice mov-cli doesn't ship with any scrapers (or previously known as providers) by default, this is because v4 is plugin-based and scrapers are now part of plugins that must be chosen to be installed.
+> Find out how to do so at the [wiki](https://github.com/mov-cli/mov-cli/wiki#plugins).
+
+1. Install the scraper plugin of your choice. Visit this [wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a list of **third-party** mov-cli plugins.
+```sh
+mov-cli -e
+```
+Alternatively, you may also edit by manually opening the config file. See the [Wiki](https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction).  
+```toml
+[mov-cli.plugins]
+films = "package_name"
+```
+
+
+2. Scraper away!
+```sh
+mov-cli -s films spider man no way home
+```
+<img width="370px" src="https://github.com/mov-cli/mov-cli/assets/66202304/86189cab-b246-405e-a266-6c624bee2d36">
+
+> The above command should search for `spider man no way home` with the following scraper.
+
+## Contributing ✨
+Pull requests are welcome and *appreciated*. For major changes, please open an issue first to discuss what you would like to change.
+
+<a href = "https://github.com/mov-cli/mov-cli/graphs/contributors">
+  <img src = "https://contrib.rocks/image?repo=mov-cli/mov-cli"/>
+</a>
+
+## Inspiration 🌟
+Inspired by [ani-cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/animdl)
+
+
+<!-- MARKDOWN LINKS & IMAGES -->
+<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
+[contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-cli.svg?style=for-the-badge
+[contributors-url]: https://github.com/mov-cli/mov-cli/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/mov-cli/mov-cli.svg?style=for-the-badge
+[forks-url]: https://github.com/mov-cli/mov-cli/network/members
+[stars-shield]: https://img.shields.io/github/stars/mov-cli/mov-cli?style=flat
+[stars-url]: https://github.com/mov-cli/mov-cli/stargazers
+[pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
+[pypi-url]: https://pypi.org/project/mov-cli/
+[python-shield]: https://img.shields.io/pypi/pyversions/mov-cli?style=flat
+[issues-shield]: https://img.shields.io/github/issues/mov-cli/mov-cli?style=flat
+[issues-url]: https://github.com/mov-cli/mov-cli/issues
+[license-shield]: https://img.shields.io/github/license/mov-cli/mov-cli?style=flat
+[license-url]: ./LICENSE
+[discord-shield]: https://img.shields.io/badge/Discord-7289da?logo=discord&logoColor=white
+[discord-url]: https://discord.gg/BMzC7ePsBV
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.2.8 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.2.9 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.lol>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
```

