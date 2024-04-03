# Comparing `tmp/fflogsapi-2.0.2.tar.gz` & `tmp/fflogsapi-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fflogsapi-2.0.2.tar", last modified: Wed Feb 14 00:08:59 2024, max compression
+gzip compressed data, was "fflogsapi-2.1.0.tar", last modified: Wed Apr  3 19:56:27 2024, max compression
```

## Comparing `fflogsapi-2.0.2.tar` & `fflogsapi-2.1.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:08:59.185806 fflogsapi-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-02-14 00:08:59.185806 fflogsapi-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:08:59.173806 fflogsapi-2.0.2/fflogsapi/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:08:59.177806 fflogsapi-2.0.2/fflogsapi/characters/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/characters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/characters/character.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/characters/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/characters/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:08:59.177806 fflogsapi-2.0.2/fflogsapi/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/data/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/data/page.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/data/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:08:59.177806 fflogsapi-2.0.2/fflogsapi/game/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/game/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/game/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/game/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:08:59.177806 fflogsapi-2.0.2/fflogsapi/guilds/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/guilds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/guilds/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/guilds/guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/guilds/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/guilds/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:08:59.177806 fflogsapi-2.0.2/fflogsapi/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:08:59.177806 fflogsapi-2.0.2/fflogsapi/prograce/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/prograce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/prograce/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/prograce/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:08:59.181806 fflogsapi-2.0.2/fflogsapi/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/reports/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/reports/fight.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/reports/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/reports/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/reports/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:08:59.181806 fflogsapi-2.0.2/fflogsapi/user/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/user/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/user/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/user_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:08:59.181806 fflogsapi-2.0.2/fflogsapi/util/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/util/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/util/gql_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/util/indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:08:59.185806 fflogsapi-2.0.2/fflogsapi/world/
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/world/client_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/world/encounter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/world/expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/world/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/world/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/world/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/world/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/fflogsapi/world/zone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 00:08:59.185806 fflogsapi-2.0.2/fflogsapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-02-14 00:08:59.000000 fflogsapi-2.0.2/fflogsapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-02-14 00:08:59.000000 fflogsapi-2.0.2/fflogsapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 00:08:59.000000 fflogsapi-2.0.2/fflogsapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-14 00:08:59.000000 fflogsapi-2.0.2/fflogsapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-14 00:08:59.000000 fflogsapi-2.0.2/fflogsapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-14 00:08:50.000000 fflogsapi-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 00:08:59.185806 fflogsapi-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.175485 fflogsapi-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-03 19:56:27.175485 fflogsapi-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.163485 fflogsapi-2.1.0/fflogsapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.167485 fflogsapi-2.1.0/fflogsapi/characters/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/characters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/characters/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/characters/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/characters/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11896 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.167485 fflogsapi-2.1.0/fflogsapi/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/data/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/data/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/data/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.167485 fflogsapi-2.1.0/fflogsapi/game/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/game/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/game/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/game/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.167485 fflogsapi-2.1.0/fflogsapi/guilds/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/guilds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/guilds/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/guilds/guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/guilds/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/guilds/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.167485 fflogsapi-2.1.0/fflogsapi/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.167485 fflogsapi-2.1.0/fflogsapi/prograce/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/prograce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/prograce/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/prograce/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.171485 fflogsapi-2.1.0/fflogsapi/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/reports/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20408 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/reports/fight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/reports/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/reports/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/reports/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.171485 fflogsapi-2.1.0/fflogsapi/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/user/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/user/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/user_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.171485 fflogsapi-2.1.0/fflogsapi/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/util/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/util/gql_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/util/indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.171485 fflogsapi-2.1.0/fflogsapi/world/
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/client_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/encounter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/fflogsapi/world/zone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:56:27.171485 fflogsapi-2.1.0/fflogsapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-03 19:56:27.000000 fflogsapi-2.1.0/fflogsapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-03 19:56:27.000000 fflogsapi-2.1.0/fflogsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:56:27.000000 fflogsapi-2.1.0/fflogsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-03 19:56:27.000000 fflogsapi-2.1.0/fflogsapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 19:56:27.000000 fflogsapi-2.1.0/fflogsapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-03 19:56:20.000000 fflogsapi-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:56:27.175485 fflogsapi-2.1.0/setup.cfg
```

### Comparing `fflogsapi-2.0.2/LICENSE` & `fflogsapi-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/PKG-INFO` & `fflogsapi-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fflogsapi
-Version: 2.0.2
+Version: 2.1.0
 Summary: Python client for the FF Logs v2 API
 Author-email: Markus Wang Halvorsen <mwh@halvorsenfamilien.com>
 Project-URL: Repository, https://github.com/halworsen/fflogsapi
 Keywords: api,client,ffxiv,fflogs,lazy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,15 +12,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gql~=3.4.0
 Requires-Dist: oauthlib~=3.2.2
 Requires-Dist: requests_oauthlib~=1.3.1
 Requires-Dist: requests_toolbelt~=0.10.1
-Requires-Dist: cryptography~=39.0.1
+Requires-Dist: cryptography~=42.0.5
 Requires-Dist: urllib3~=1.26.14
 Provides-Extra: dev
 Requires-Dist: flake8==6.0.0; extra == "dev"
 Requires-Dist: autopep8==2.0.1; extra == "dev"
 Requires-Dist: isort==5.12.0; extra == "dev"
 Requires-Dist: removestar==1.3.1; extra == "dev"
 Requires-Dist: sphinx==7.2.5; extra == "dev"
```

### Comparing `fflogsapi-2.0.2/README.md` & `fflogsapi-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/__init__.py` & `fflogsapi-2.1.0/fflogsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/characters/character.py` & `fflogsapi-2.1.0/fflogsapi/characters/character.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/characters/client_extensions.py` & `fflogsapi-2.1.0/fflogsapi/characters/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/client.py` & `fflogsapi-2.1.0/fflogsapi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 '''
 The client implementation that allows communication with the FF Logs API.
 '''
 
 import os
 import pickle
+import tempfile
 from copy import deepcopy
 from functools import wraps
 from time import time
 from typing import Any
+from warnings import warn
 
 from gql import Client as GQLClient
 from gql import gql
 from gql.transport.requests import RequestsHTTPTransport
 from oauthlib.oauth2 import BackendApplicationClient, WebApplicationClient
 from requests.auth import HTTPBasicAuth
 from requests_oauthlib import OAuth2Session
@@ -123,17 +125,25 @@
         self.oauth_session = OAuth2Session(client=oauth_client)
         self.token = {}
         self.mode = mode
 
         self._query_cache = {}
         self.cache_expiry = cache_expiry
         self.cache_queries = enable_caching
-        self.cache_dir = cache_directory
         self.ignore_cache_expiry = ignore_cache_expiry
 
+        # deprecation warning for cache_directory use
+        if cache_directory != './fflogs-querycache':
+            warn('Custom cache directories are deprecated in favor of system temp dirs.'
+                 ' Consider removing usage of cache_directory when instantiating FFLogsClient.',
+                 category=FutureWarning)
+        else:
+            # future behavior
+            self.cache_dir = os.path.join(tempfile.gettempdir(), 'fflogsapi')
+
         if enable_caching:
             if not os.path.exists(self.cache_dir):
                 os.makedirs(self.cache_dir)
 
             cache_path = ''
             if cache_override:
                 cache_path = cache_override
```

### Comparing `fflogsapi-2.0.2/fflogsapi/constants.py` & `fflogsapi-2.1.0/fflogsapi/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,11 +31,13 @@
     REMOVE_BUFF = 'removebuff'
     REMOVE_BUFF_STACK = 'removebuffstack'
     APPLY_DEBUFF = 'applydebuff'
     REFRESH_DEBUFF = 'refreshdebuff'
     REMOVE_DEBUFF = 'removedebuff'
     LB_UPDATE = 'limitbreakupdate'
     ENCOUNTER_END = 'encounterend'
+    TARGETABILITY_UPDATE = 'targetabilityupdate'
+    HEAD_MARKER = 'headmarker'
 
 
 # FF Logs uses millisecond precision in its timestamps
 TIMESTAMP_PRECISION = 1e-3
```

### Comparing `fflogsapi-2.0.2/fflogsapi/data/__init__.py` & `fflogsapi-2.1.0/fflogsapi/data/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 '''
 Dataclasses and such.
 '''
 
 from .dataclasses import (FFAbility, FFGameZone, FFGrandCompany, FFItem, FFJob, FFLogsActor,
                           FFLogsAllStarsRanking, FFLogsArchivalData, FFLogsAttendanceReport,
                           FFLogsEncounterRankings, FFLogsFightRank, FFLogsGuildZoneRankings,
-                          FFLogsNPCData, FFLogsPartition, FFLogsPlayerDetails, FFLogsRank,
-                          FFLogsReportAbility, FFLogsReportCharacterRanking,
+                          FFLogsNPCData, FFLogsPartition, FFLogsPhase, FFLogsPlayerDetails,
+                          FFLogsRank, FFLogsReportAbility, FFLogsReportCharacterRanking,
                           FFLogsReportComboRanking, FFLogsReportRanking, FFLogsReportTag,
                           FFLogsZoneEncounterRanking, FFLogsZoneRanking, FFMap,)
 
 __all__ = [
     # dataclasses.py
     'FFLogsAllStarsRanking',
     'FFLogsFightRank',
@@ -32,8 +32,9 @@
     'FFLogsActor',
     'FFLogsReportAbility',
     'FFLogsArchivalData',
     'FFLogsPlayerDetails',
     'FFLogsNPCData',
     'FFGameZone',
     'FFLogsPartition',
+    'FFLogsPhase',
 ]
```

### Comparing `fflogsapi-2.0.2/fflogsapi/data/dataclasses.py` & `fflogsapi-2.1.0/fflogsapi/data/dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,7 +378,22 @@
     '''
     A partition within a zone.
     '''
     id: int
     name: str
     compact_name: str
     default: bool
+
+
+@dataclass
+class FFLogsPhase:
+    '''
+    Phase information for an encounter
+
+    The encounter is not part of this dataclass because it can
+    be queried from the fight from which this information was gotten
+    '''
+    id: int
+    name: str
+    intermission: bool
+    separates_wipes: bool
+    ''' Does this visually distinguish wipes in the FF Logs report UI? '''
```

### Comparing `fflogsapi-2.0.2/fflogsapi/data/page.py` & `fflogsapi-2.1.0/fflogsapi/data/page.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/game/__init__.py` & `fflogsapi-2.1.0/fflogsapi/game/__init__.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/game/client_extensions.py` & `fflogsapi-2.1.0/fflogsapi/game/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/game/pages.py` & `fflogsapi-2.1.0/fflogsapi/game/pages.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/game/queries.py` & `fflogsapi-2.1.0/fflogsapi/game/queries.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/guilds/client_extensions.py` & `fflogsapi-2.1.0/fflogsapi/guilds/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/guilds/guild.py` & `fflogsapi-2.1.0/fflogsapi/guilds/guild.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/guilds/pages.py` & `fflogsapi-2.1.0/fflogsapi/guilds/pages.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/guilds/queries.py` & `fflogsapi-2.1.0/fflogsapi/guilds/queries.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/prograce/client_extensions.py` & `fflogsapi-2.1.0/fflogsapi/prograce/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/reports/client_extensions.py` & `fflogsapi-2.1.0/fflogsapi/reports/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/reports/fight.py` & `fflogsapi-2.1.0/fflogsapi/reports/fight.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from typing import TYPE_CHECKING, Any, Optional
+from typing import TYPE_CHECKING, Any, Optional, Union
+from warnings import warn
 
 from ..characters.character import FFLogsCharacter
-from ..data import (FFGameZone, FFLogsNPCData, FFLogsPlayerDetails, FFLogsReportCharacterRanking,
-                    FFLogsReportComboRanking, FFLogsReportRanking, FFMap,)
+from ..data import (FFGameZone, FFLogsNPCData, FFLogsPhase, FFLogsPlayerDetails,
+                    FFLogsReportCharacterRanking, FFLogsReportComboRanking, FFLogsReportRanking,
+                    FFMap,)
 from ..util.decorators import fetch_data
 from ..util.filters import construct_filter_string
 from ..util.indexing import itindex
 from ..world.encounter import FFLogsEncounter
 from .queries import Q_FIGHT_DATA
 
 if TYPE_CHECKING:
@@ -109,22 +111,14 @@
     def fight_percentage(self) -> float:
         '''
         Returns:
             The minimum percentage of the entire fight that was reached
         '''
         return self._data['fightPercentage']
 
-    @fetch_data('lastPhase')
-    def last_phase(self) -> int:
-        '''
-        Returns:
-            The last phase the fight was in when it ended
-        '''
-        return self._data['lastPhase']
-
     @fetch_data('lastPhaseAsAbsoluteIndex')
     def last_phase_absolute(self) -> int:
         '''
         Returns:
             The last phase the fight was in when it ended,
             counting from 0 and including intermissions
         '''
@@ -229,29 +223,29 @@
         if 'endTime' not in filters:
             filters['endTime'] = fight_end
         elif filters['endTime'] > fight_end:
             raise ValueError('Cannot retrieve fight events after the fight has ended!')
 
         return construct_filter_string(filters), filters
 
-    def events(self, filters: dict[str, Any] = {}) -> dict[Any, Any]:
+    def events(self, filters: dict[str, Any] = {}) -> list[dict[str, Any]]:
         '''
         Retrieves the events of the fight.
 
         If start/end time is not specified in filters, the default is the start/end of the fight.
 
         This data isn't considered frozen by FF Logs and may therefore change without notice.
 
         For a full list of valid filters see the API documentation:
         https://www.fflogs.com/v2-api-docs/warcraft/report.doc.html
 
         Args:
             filters: Filters to use when retrieving event log data.
         Returns:
-            A dictionary of all events in the fight or None if the fight has zero duration
+            A filtered list of all events in the fight or None if the fight has zero duration
         '''
         if self.duration() == 0:
             return None
 
         filter_string, filters = self._prepare_data_filters(filters.copy())
 
         # used for pagination
@@ -260,17 +254,15 @@
         result = self.report._query_data(f'events({filter_string}) {{ data, nextPageTimestamp }}')
         fight_events = result['events']['data']
 
         # Check if there are more pages to this fight.
         # If so, retrieve all of them and merge the data.
         next_page = result['events']['nextPageTimestamp']
         while next_page and next_page < desired_end:
-            time_range = filters['endTime'] - filters['startTime']
             filters['startTime'] = next_page
-            filters['endTime'] = min(next_page + time_range, desired_end)
 
             filter_string = construct_filter_string(filters)
             result = self.report._query_data(
                 f'events({filter_string}) {{ data, nextPageTimestamp }}'
             )
             events = result['events']['data']
             fight_events += events
@@ -525,7 +517,56 @@
         Get a list of all the maps involved in this fight.
 
         Returns:
             All maps involved in the fight.
         '''
         maps = self._query_data('maps{ id }')['maps']
         return [self._client.map(id=map['id']) for map in maps]
+
+    @fetch_data('encounterID')
+    def phases(self) -> list[FFLogsPhase]:
+        '''
+        Get a list of phases in this fight.
+
+        Returns:
+            A list of phases
+        '''
+        # Awkward implementation, the API exposes phase info on the report
+        # But we want to expose it at the fight level, so we have to communicate
+        # backwards with the parent report for this information
+        if 'phases' not in self._data:
+            assert (self.report is not None)
+            encounter_id = self._data['encounterID']
+            self._data['phases'] = self.report._query_phases()[encounter_id]
+        return self._data['phases']
+
+    @fetch_data('lastPhase', 'lastPhaseAsAbsoluteIndex')
+    def last_phase(
+        self,
+        ignore_intermissions: bool = True,
+        as_dataclass: bool = False
+    ) -> Union[int, FFLogsPhase]:
+        '''
+        Get the phase the fight was in when the fight ended.
+
+        Args:
+            ignore_intermissions: When True, the last non-intermission phase is returned
+            as_dataclass: Return the last phase as a FFLogsPhase dataclass.
+                          This will become standard in the future.
+        Returns:
+            The last phase the fight was in when it ended
+        '''
+        last_phase = self._data['lastPhase']
+        if as_dataclass:
+            if not ignore_intermissions:
+                last_phase = self._data['lastPhaseAsAbsoluteIndex'] + 1
+            for phase in self.phases():
+                if phase.id == last_phase:
+                    last_phase = phase
+                    break
+        else:
+            warn(
+                'integer returns from FFLogsFight.last_phase are deprecated. '
+                'Pass as_dataclass=True to get the new dataclass return instead.',
+                category=FutureWarning,
+            )
+        return last_phase
```

### Comparing `fflogsapi-2.0.2/fflogsapi/reports/pages.py` & `fflogsapi-2.1.0/fflogsapi/reports/pages.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/reports/queries.py` & `fflogsapi-2.1.0/fflogsapi/reports/queries.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,36 +29,52 @@
                 {innerQuery}
             }}
         }}
     }}
 }}
 '''
 
+# Report-internal query for the report's log version
 IQ_REPORT_LOG_VERSION = '''
 masterData {
     logVersion
 }
 '''
 
+# Report-internal query for the actor data contained in the report
 IQ_REPORT_ACTORS = '''
 masterData {
     actors {
         gameID
         id
         name
         server
         petOwner
         subType
         type
     }
 }
 '''
 
+# Report-internal query for all abilities seen in the report
 IQ_REPORT_ABILITIES = '''
 masterData {
     abilities {
         gameID
         name
         type
     }
 }
 '''
+
+# Report-internal query for phase information contained in the report
+IQ_REPORT_PHASES = '''
+phases {
+    encounterID
+    separatesWipes
+    phases {
+        id
+        isIntermission
+        name
+    }
+}
+'''
```

### Comparing `fflogsapi-2.0.2/fflogsapi/reports/report.py` & `fflogsapi-2.1.0/fflogsapi/reports/report.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import TYPE_CHECKING, Iterator, Optional
 
 from ..characters.character import FFLogsCharacter
-from ..data import FFLogsActor, FFLogsArchivalData, FFLogsReportAbility, FFLogsReportTag
+from ..data import (FFLogsActor, FFLogsArchivalData, FFLogsPhase, FFLogsReportAbility,
+                    FFLogsReportTag,)
 from ..user.user import FFLogsUser
 from ..util.decorators import fetch_data
 from ..util.indexing import itindex
 from ..world.region import FFLogsRegion
 from ..world.zone import FFLogsZone
 from .fight import FFLogsFight
-from .queries import IQ_REPORT_ABILITIES, IQ_REPORT_ACTORS, IQ_REPORT_LOG_VERSION, Q_REPORT_DATA
+from .queries import (IQ_REPORT_ABILITIES, IQ_REPORT_ACTORS, IQ_REPORT_LOG_VERSION,
+                      IQ_REPORT_PHASES, Q_REPORT_DATA,)
 
 if TYPE_CHECKING:
     from ..client import FFLogsClient
     from ..guilds.guild import FFLogsGuild
 
 
 class FFLogsReport:
@@ -32,23 +34,49 @@
         self._client = client
 
     def __iter__(self) -> Iterator:
         return iter(self.fights())
 
     def _query_data(self, query: str, ignore_cache: bool = False) -> None:
         '''
+        INTERNAL
         Query for a specific piece of information from a report.
         '''
         result = self._client.q(Q_REPORT_DATA.format(
             reportCode=self.code,
             innerQuery=query
         ), ignore_cache=ignore_cache)
 
         return itindex(result, self.DATA_INDICES)
 
+    def _query_phases(self) -> dict[int, list[FFLogsPhase]]:
+        '''
+        INTERNAL
+        Query for all phase data exposed by this report
+
+        Returns:
+            A dictionary mapping encounter IDs in the report to a list of phases for that encounter
+        '''
+        if 'phases' not in self._data:
+            all_phases: dict[int, list[FFLogsPhase]] = {}
+            encounter_phases = self._query_data(IQ_REPORT_PHASES)['phases']
+            for encounter in encounter_phases:
+                separates_wipes = encounter['separatesWipes']
+                all_phases[encounter['encounterID']] = []
+                for phase in encounter['phases']:
+                    phase = FFLogsPhase(
+                        id=phase['id'],
+                        name=phase['name'],
+                        intermission=phase['isIntermission'],
+                        separates_wipes=separates_wipes,
+                    )
+                    all_phases[encounter['encounterID']].append(phase)
+            self._data['phases'] = all_phases
+        return self._data['phases']
+
     def actors(self) -> list[FFLogsActor]:
         '''
         Returns:
             A list of all actors in the report
         '''
         if 'masterActors' not in self._data:
             actors = self._query_data(IQ_REPORT_ACTORS)['masterData']['actors']
```

### Comparing `fflogsapi-2.0.2/fflogsapi/user/client_extensions.py` & `fflogsapi-2.1.0/fflogsapi/user/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/user/user.py` & `fflogsapi-2.1.0/fflogsapi/user/user.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/user_auth.py` & `fflogsapi-2.1.0/fflogsapi/user_auth.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/util/decorators.py` & `fflogsapi-2.1.0/fflogsapi/util/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-def fetch_data(key):
+from functools import wraps
+
+
+def fetch_data(*keys):
     '''
     Decorator that queries and stores the given `key` in a class's `_data` dictionary.
 
     The class must have a `_data` dictionary field and a `_query_data` function which
     queries for the data specified by the `key`. The class must also have a `DATA_INDICES` field
     which is a list describing how to index into the relevant data.
 
     Args:
         `key`: The key to query and store.
     '''
     def decorator(func):
+        @wraps(func)
         def ensured(*args, **kwargs):
             self = args[0]
-            if key not in self._data:
-                result = self._query_data(key)
-                self._data[key] = result[key]
+            for key in keys:
+                if key not in self._data:
+                    result = self._query_data(key)
+                    self._data[key] = result[key]
             return func(*args, **kwargs)
         return ensured
     return decorator
```

### Comparing `fflogsapi-2.0.2/fflogsapi/util/filters.py` & `fflogsapi-2.1.0/fflogsapi/util/filters.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,17 @@
     Returns:
         A filter string usable in GQL queries.
     '''
     prepped_filters = []
     for key, f in filters.items():
         filter = ''
         if type(f) is str:
+            # escape quotes
+            f = f.replace('"', '\\"')
+            f = f.replace('\'', '\\"')
             filter = f'{key}: "{f}"'
         elif type(f) is bool:
             # bool type must be lowercase
             filter = f'{key}: {str(f).lower()}'
         else:
             filter = f'{key}: {f}'
         prepped_filters.append(filter)
```

### Comparing `fflogsapi-2.0.2/fflogsapi/world/__init__.py` & `fflogsapi-2.1.0/fflogsapi/world/__init__.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/world/client_extensions.py` & `fflogsapi-2.1.0/fflogsapi/world/client_extensions.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/world/encounter.py` & `fflogsapi-2.1.0/fflogsapi/world/encounter.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/world/expansion.py` & `fflogsapi-2.1.0/fflogsapi/world/expansion.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/world/pages.py` & `fflogsapi-2.1.0/fflogsapi/world/pages.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/world/queries.py` & `fflogsapi-2.1.0/fflogsapi/world/queries.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/world/region.py` & `fflogsapi-2.1.0/fflogsapi/world/region.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/world/server.py` & `fflogsapi-2.1.0/fflogsapi/world/server.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi/world/zone.py` & `fflogsapi-2.1.0/fflogsapi/world/zone.py`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/fflogsapi.egg-info/PKG-INFO` & `fflogsapi-2.1.0/fflogsapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fflogsapi
-Version: 2.0.2
+Version: 2.1.0
 Summary: Python client for the FF Logs v2 API
 Author-email: Markus Wang Halvorsen <mwh@halvorsenfamilien.com>
 Project-URL: Repository, https://github.com/halworsen/fflogsapi
 Keywords: api,client,ffxiv,fflogs,lazy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,15 +12,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gql~=3.4.0
 Requires-Dist: oauthlib~=3.2.2
 Requires-Dist: requests_oauthlib~=1.3.1
 Requires-Dist: requests_toolbelt~=0.10.1
-Requires-Dist: cryptography~=39.0.1
+Requires-Dist: cryptography~=42.0.5
 Requires-Dist: urllib3~=1.26.14
 Provides-Extra: dev
 Requires-Dist: flake8==6.0.0; extra == "dev"
 Requires-Dist: autopep8==2.0.1; extra == "dev"
 Requires-Dist: isort==5.12.0; extra == "dev"
 Requires-Dist: removestar==1.3.1; extra == "dev"
 Requires-Dist: sphinx==7.2.5; extra == "dev"
```

### Comparing `fflogsapi-2.0.2/fflogsapi.egg-info/SOURCES.txt` & `fflogsapi-2.1.0/fflogsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fflogsapi-2.0.2/pyproject.toml` & `fflogsapi-2.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'fflogsapi'
-version = '2.0.2'
+version = '2.1.0'
 description = 'Python client for the FF Logs v2 API'
 readme = 'README.md'
 authors = [
     { name = 'Markus Wang Halvorsen', email = 'mwh@halvorsenfamilien.com' },
 ]
 keywords = ['api', 'client', 'ffxiv', 'fflogs', 'lazy']
 classifiers = [
@@ -15,15 +15,15 @@
     'Topic :: Software Development :: Libraries',
 ]
 dependencies = [
     'gql~=3.4.0',
     'oauthlib~=3.2.2',
     'requests_oauthlib~=1.3.1',
     'requests_toolbelt~=0.10.1',
-    'cryptography~=39.0.1',
+    'cryptography~=42.0.5',
     'urllib3~=1.26.14',
 ]
 
 [project.optional-dependencies]
 dev = [
     'flake8==6.0.0',
     'autopep8==2.0.1',
```

