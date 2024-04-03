# Comparing `tmp/cardano-clusterlib-0.6.0a8.tar.gz` & `tmp/cardano-clusterlib-0.6.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardano-clusterlib-0.6.0a8.tar", last modified: Thu Dec 14 17:23:24 2023, max compression
+gzip compressed data, was "cardano-clusterlib-0.6.0a9.tar", last modified: Fri Dec 15 14:15:58 2023, max compression
```

## Comparing `cardano-clusterlib-0.6.0a8.tar` & `cardano-clusterlib-0.6.0a9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-14 17:23:24.007962 cardano-clusterlib-0.6.0a8/
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-14 17:23:24.002962 cardano-clusterlib-0.6.0a8/.github/
--rw-r--r--   0 martink   (1000) martink   (1000)      214 2023-06-22 11:16:14.000000 cardano-clusterlib-0.6.0a8/.github/dependabot.yml
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-14 17:23:24.003962 cardano-clusterlib-0.6.0a8/.github/workflows/
--rw-r--r--   0 martink   (1000) martink   (1000)     1669 2023-09-26 14:20:33.000000 cardano-clusterlib-0.6.0a8/.github/workflows/codeql.yml
--rw-r--r--   0 martink   (1000) martink   (1000)      353 2023-09-26 14:20:33.000000 cardano-clusterlib-0.6.0a8/.github/workflows/repo_lint.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)      948 2021-12-16 16:01:16.000000 cardano-clusterlib-0.6.0a8/.gitignore
--rw-r--r--   0 martink   (1000) martink   (1000)      698 2022-09-23 12:55:52.000000 cardano-clusterlib-0.6.0a8/.markdownlint.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     1224 2023-11-22 11:00:28.000000 cardano-clusterlib-0.6.0a8/.pre-commit-config.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     2523 2022-06-03 10:16:54.000000 cardano-clusterlib-0.6.0a8/.pylintrc
--rw-r--r--   0 martink   (1000) martink   (1000)      318 2021-03-11 15:25:52.000000 cardano-clusterlib-0.6.0a8/.readthedocs.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     3267 2023-03-16 13:20:33.000000 cardano-clusterlib-0.6.0a8/CODE-OF-CONDUCT.md
--rw-r--r--   0 martink   (1000) martink   (1000)    11360 2023-03-16 13:20:33.000000 cardano-clusterlib-0.6.0a8/LICENSE
--rw-r--r--   0 martink   (1000) martink   (1000)     1297 2023-06-22 11:53:24.000000 cardano-clusterlib-0.6.0a8/Makefile
--rw-r--r--   0 martink   (1000) martink   (1000)     8221 2023-12-14 17:23:24.007962 cardano-clusterlib-0.6.0a8/PKG-INFO
--rw-r--r--   0 martink   (1000) martink   (1000)     7170 2023-03-16 13:15:07.000000 cardano-clusterlib-0.6.0a8/README.md
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-14 17:23:24.005962 cardano-clusterlib-0.6.0a8/cardano_clusterlib/
--rw-r--r--   0 martink   (1000) martink   (1000)      174 2023-06-27 09:41:48.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/__init__.py
--rw-r--r--   0 martink   (1000) martink   (1000)     8099 2023-06-27 12:02:33.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/address_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     3176 2023-12-14 16:57:58.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/clusterlib.py
--rw-r--r--   0 martink   (1000) martink   (1000)     8412 2023-11-15 13:41:11.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/clusterlib_helpers.py
--rw-r--r--   0 martink   (1000) martink   (1000)    17489 2023-11-15 13:41:11.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/clusterlib_klass.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1554 2023-12-14 13:09:15.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/consts.py
--rw-r--r--   0 martink   (1000) martink   (1000)    20750 2023-12-14 16:57:58.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/conway_gov_action_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     6578 2023-11-15 13:41:11.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/conway_gov_committee_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     8108 2023-12-13 15:53:41.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/conway_gov_drep_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     2834 2023-11-15 13:41:11.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/conway_gov_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     4021 2023-11-22 14:13:21.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/conway_gov_query_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     8835 2023-12-14 16:46:47.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/conway_gov_vote_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1110 2023-06-27 12:02:33.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/coverage.py
--rw-r--r--   0 martink   (1000) martink   (1000)       36 2023-06-27 09:41:48.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/exceptions.py
--rw-r--r--   0 martink   (1000) martink   (1000)     4259 2023-06-27 12:02:33.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/genesis_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     7358 2023-08-08 07:08:33.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/governance_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1721 2023-12-14 16:46:47.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/helpers.py
--rw-r--r--   0 martink   (1000) martink   (1000)     2790 2023-06-27 12:02:33.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/key_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     5992 2023-06-27 12:02:33.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/node_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)        0 2021-03-10 16:56:29.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/py.typed
--rw-r--r--   0 martink   (1000) martink   (1000)    18967 2023-11-29 16:51:04.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/query_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    17215 2023-11-20 17:01:54.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/stake_address_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    13206 2023-12-13 15:53:41.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/stake_pool_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    12028 2023-12-14 16:57:58.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/structs.py
--rw-r--r--   0 martink   (1000) martink   (1000)    64140 2023-11-15 13:41:11.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/transaction_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    45288 2023-11-15 13:41:11.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/txtools.py
--rw-r--r--   0 martink   (1000) martink   (1000)      522 2023-12-03 17:40:31.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib/types.py
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-14 17:23:24.007962 cardano-clusterlib-0.6.0a8/cardano_clusterlib.egg-info/
--rw-r--r--   0 martink   (1000) martink   (1000)     8221 2023-12-14 17:23:23.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib.egg-info/PKG-INFO
--rw-r--r--   0 martink   (1000) martink   (1000)     1661 2023-12-14 17:23:23.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib.egg-info/SOURCES.txt
--rw-r--r--   0 martink   (1000) martink   (1000)        1 2023-12-14 17:23:23.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib.egg-info/dependency_links.txt
--rw-r--r--   0 martink   (1000) martink   (1000)        1 2021-03-10 16:00:20.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib.egg-info/not-zip-safe
--rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-12-14 17:23:23.000000 cardano-clusterlib-0.6.0a8/cardano_clusterlib.egg-info/top_level.txt
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-14 17:23:24.006962 cardano-clusterlib-0.6.0a8/docs/
--rw-r--r--   0 martink   (1000) martink   (1000)      740 2021-03-23 15:49:32.000000 cardano-clusterlib-0.6.0a8/docs/Makefile
--rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-09-23 12:55:52.000000 cardano-clusterlib-0.6.0a8/docs/requirements.txt
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-14 17:23:24.006962 cardano-clusterlib-0.6.0a8/docs/source/
--rw-r--r--   0 martink   (1000) martink   (1000)     3694 2022-10-21 06:56:49.000000 cardano-clusterlib-0.6.0a8/docs/source/cardano_clusterlib.rst
--rw-r--r--   0 martink   (1000) martink   (1000)     4112 2023-04-17 08:42:14.000000 cardano-clusterlib-0.6.0a8/docs/source/conf.py
--rw-r--r--   0 martink   (1000) martink   (1000)      491 2021-03-11 13:53:31.000000 cardano-clusterlib-0.6.0a8/docs/source/index.rst
--rw-r--r--   0 martink   (1000) martink   (1000)       95 2021-03-11 13:52:06.000000 cardano-clusterlib-0.6.0a8/docs/source/modules.rst
--rw-r--r--   0 martink   (1000) martink   (1000)       31 2021-03-11 13:53:55.000000 cardano-clusterlib-0.6.0a8/docs/source/readme.rst
--rw-r--r--   0 martink   (1000) martink   (1000)      236 2021-03-10 15:33:40.000000 cardano-clusterlib-0.6.0a8/mypy.ini
--rw-r--r--   0 martink   (1000) martink   (1000)     1531 2023-06-22 11:53:24.000000 cardano-clusterlib-0.6.0a8/pyproject.toml
--rw-r--r--   0 martink   (1000) martink   (1000)       59 2023-01-19 14:58:18.000000 cardano-clusterlib-0.6.0a8/requirements-dev.txt
--rw-r--r--   0 martink   (1000) martink   (1000)      352 2023-12-14 17:23:24.007962 cardano-clusterlib-0.6.0a8/setup.cfg
--rw-r--r--   0 martink   (1000) martink   (1000)      202 2023-05-03 11:49:49.000000 cardano-clusterlib-0.6.0a8/setup.py
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-14 17:23:24.006962 cardano-clusterlib-0.6.0a8/upgrading/
--rw-r--r--   0 martink   (1000) martink   (1000)     7363 2022-10-21 06:56:49.000000 cardano-clusterlib-0.6.0a8/upgrading/refactor_to_0_4_0rc1.sed
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-15 14:15:58.619849 cardano-clusterlib-0.6.0a9/
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-15 14:15:58.615849 cardano-clusterlib-0.6.0a9/.github/
+-rw-r--r--   0 martink   (1000) martink   (1000)      214 2023-06-22 11:16:14.000000 cardano-clusterlib-0.6.0a9/.github/dependabot.yml
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-15 14:15:58.615849 cardano-clusterlib-0.6.0a9/.github/workflows/
+-rw-r--r--   0 martink   (1000) martink   (1000)     1669 2023-09-26 14:20:33.000000 cardano-clusterlib-0.6.0a9/.github/workflows/codeql.yml
+-rw-r--r--   0 martink   (1000) martink   (1000)      353 2023-09-26 14:20:33.000000 cardano-clusterlib-0.6.0a9/.github/workflows/repo_lint.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)      948 2021-12-16 16:01:16.000000 cardano-clusterlib-0.6.0a9/.gitignore
+-rw-r--r--   0 martink   (1000) martink   (1000)      698 2022-09-23 12:55:52.000000 cardano-clusterlib-0.6.0a9/.markdownlint.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     1224 2023-11-22 11:00:28.000000 cardano-clusterlib-0.6.0a9/.pre-commit-config.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     2523 2022-06-03 10:16:54.000000 cardano-clusterlib-0.6.0a9/.pylintrc
+-rw-r--r--   0 martink   (1000) martink   (1000)      318 2021-03-11 15:25:52.000000 cardano-clusterlib-0.6.0a9/.readthedocs.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     3267 2023-03-16 13:20:33.000000 cardano-clusterlib-0.6.0a9/CODE-OF-CONDUCT.md
+-rw-r--r--   0 martink   (1000) martink   (1000)    11360 2023-03-16 13:20:33.000000 cardano-clusterlib-0.6.0a9/LICENSE
+-rw-r--r--   0 martink   (1000) martink   (1000)     1297 2023-06-22 11:53:24.000000 cardano-clusterlib-0.6.0a9/Makefile
+-rw-r--r--   0 martink   (1000) martink   (1000)     8221 2023-12-15 14:15:58.619849 cardano-clusterlib-0.6.0a9/PKG-INFO
+-rw-r--r--   0 martink   (1000) martink   (1000)     7170 2023-03-16 13:15:07.000000 cardano-clusterlib-0.6.0a9/README.md
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-15 14:15:58.617849 cardano-clusterlib-0.6.0a9/cardano_clusterlib/
+-rw-r--r--   0 martink   (1000) martink   (1000)      174 2023-06-27 09:41:48.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/__init__.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     8099 2023-06-27 12:02:33.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/address_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     3176 2023-12-14 16:57:58.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/clusterlib.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     8464 2023-12-15 14:14:59.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/clusterlib_helpers.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    17489 2023-11-15 13:41:11.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/clusterlib_klass.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1554 2023-12-14 13:09:15.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/consts.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    20750 2023-12-14 16:57:58.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/conway_gov_action_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     6578 2023-11-15 13:41:11.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/conway_gov_committee_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     8108 2023-12-13 15:53:41.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/conway_gov_drep_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     2834 2023-11-15 13:41:11.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/conway_gov_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     4021 2023-11-22 14:13:21.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/conway_gov_query_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     8835 2023-12-14 16:46:47.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/conway_gov_vote_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1110 2023-06-27 12:02:33.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/coverage.py
+-rw-r--r--   0 martink   (1000) martink   (1000)       36 2023-06-27 09:41:48.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/exceptions.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     4259 2023-06-27 12:02:33.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/genesis_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     7358 2023-08-08 07:08:33.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/governance_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1721 2023-12-14 16:46:47.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/helpers.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     2790 2023-06-27 12:02:33.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/key_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     5992 2023-06-27 12:02:33.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/node_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)        0 2021-03-10 16:56:29.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/py.typed
+-rw-r--r--   0 martink   (1000) martink   (1000)    18967 2023-11-29 16:51:04.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/query_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    17215 2023-11-20 17:01:54.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/stake_address_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    13206 2023-12-13 15:53:41.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/stake_pool_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    12862 2023-12-15 14:14:59.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/structs.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    64140 2023-11-15 13:41:11.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/transaction_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    45352 2023-12-15 14:14:59.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/txtools.py
+-rw-r--r--   0 martink   (1000) martink   (1000)      522 2023-12-03 17:40:31.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib/types.py
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-15 14:15:58.619849 cardano-clusterlib-0.6.0a9/cardano_clusterlib.egg-info/
+-rw-r--r--   0 martink   (1000) martink   (1000)     8221 2023-12-15 14:15:58.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib.egg-info/PKG-INFO
+-rw-r--r--   0 martink   (1000) martink   (1000)     1661 2023-12-15 14:15:58.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib.egg-info/SOURCES.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)        1 2023-12-15 14:15:58.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib.egg-info/dependency_links.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)        1 2021-03-10 16:00:20.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib.egg-info/not-zip-safe
+-rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-12-15 14:15:58.000000 cardano-clusterlib-0.6.0a9/cardano_clusterlib.egg-info/top_level.txt
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-15 14:15:58.618849 cardano-clusterlib-0.6.0a9/docs/
+-rw-r--r--   0 martink   (1000) martink   (1000)      740 2021-03-23 15:49:32.000000 cardano-clusterlib-0.6.0a9/docs/Makefile
+-rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-09-23 12:55:52.000000 cardano-clusterlib-0.6.0a9/docs/requirements.txt
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-15 14:15:58.618849 cardano-clusterlib-0.6.0a9/docs/source/
+-rw-r--r--   0 martink   (1000) martink   (1000)     3694 2022-10-21 06:56:49.000000 cardano-clusterlib-0.6.0a9/docs/source/cardano_clusterlib.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)     4112 2023-04-17 08:42:14.000000 cardano-clusterlib-0.6.0a9/docs/source/conf.py
+-rw-r--r--   0 martink   (1000) martink   (1000)      491 2021-03-11 13:53:31.000000 cardano-clusterlib-0.6.0a9/docs/source/index.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)       95 2021-03-11 13:52:06.000000 cardano-clusterlib-0.6.0a9/docs/source/modules.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)       31 2021-03-11 13:53:55.000000 cardano-clusterlib-0.6.0a9/docs/source/readme.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)      236 2021-03-10 15:33:40.000000 cardano-clusterlib-0.6.0a9/mypy.ini
+-rw-r--r--   0 martink   (1000) martink   (1000)     1531 2023-06-22 11:53:24.000000 cardano-clusterlib-0.6.0a9/pyproject.toml
+-rw-r--r--   0 martink   (1000) martink   (1000)       59 2023-01-19 14:58:18.000000 cardano-clusterlib-0.6.0a9/requirements-dev.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)      352 2023-12-15 14:15:58.619849 cardano-clusterlib-0.6.0a9/setup.cfg
+-rw-r--r--   0 martink   (1000) martink   (1000)      202 2023-05-03 11:49:49.000000 cardano-clusterlib-0.6.0a9/setup.py
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-12-15 14:15:58.618849 cardano-clusterlib-0.6.0a9/upgrading/
+-rw-r--r--   0 martink   (1000) martink   (1000)     7363 2022-10-21 06:56:49.000000 cardano-clusterlib-0.6.0a9/upgrading/refactor_to_0_4_0rc1.sed
```

### Comparing `cardano-clusterlib-0.6.0a8/.github/workflows/codeql.yml` & `cardano-clusterlib-0.6.0a9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/.gitignore` & `cardano-clusterlib-0.6.0a9/.gitignore`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/.markdownlint.yaml` & `cardano-clusterlib-0.6.0a9/.markdownlint.yaml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/.pre-commit-config.yaml` & `cardano-clusterlib-0.6.0a9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/.pylintrc` & `cardano-clusterlib-0.6.0a9/.pylintrc`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/CODE-OF-CONDUCT.md` & `cardano-clusterlib-0.6.0a9/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/LICENSE` & `cardano-clusterlib-0.6.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/Makefile` & `cardano-clusterlib-0.6.0a9/Makefile`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/PKG-INFO` & `cardano-clusterlib-0.6.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.6.0a8
+Version: 0.6.0a9
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
 Author-email: Martin Kourim <martin.kourim@iohk.io>
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/input-output-hk/cardano-clusterlib-py
```

### Comparing `cardano-clusterlib-0.6.0a8/README.md` & `cardano-clusterlib-0.6.0a9/README.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/address_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/address_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/clusterlib.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/clusterlib.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/clusterlib_helpers.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/clusterlib_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helper functions for `ClusterLib`."""
+import dataclasses
 import datetime
 import json
 import logging
 import pathlib as pl
 import re
 import time
 import typing as tp
@@ -11,15 +12,16 @@
 from cardano_clusterlib import types as itp
 
 LOGGER = logging.getLogger(__name__)
 
 SPECIAL_ARG_CHARS_RE = re.compile("[^A-Za-z0-9/._-]")
 
 
-class EpochInfo(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class EpochInfo:
     epoch: int
     first_slot: int
     last_slot: int
 
 
 def _find_genesis_json(clusterlib_obj: "itp.ClusterLib") -> pl.Path:
     """Find Shelley genesis JSON file in state dir."""
```

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/clusterlib_klass.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/clusterlib_klass.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/consts.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/consts.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/conway_gov_action_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/conway_gov_action_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/conway_gov_committee_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/conway_gov_committee_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/conway_gov_drep_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/conway_gov_drep_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/conway_gov_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/conway_gov_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/conway_gov_query_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/conway_gov_query_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/conway_gov_vote_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/conway_gov_vote_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/coverage.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/coverage.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/genesis_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/genesis_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/governance_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/governance_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/helpers.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/key_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/key_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/node_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/node_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/query_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/query_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/stake_address_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/stake_address_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/stake_pool_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/stake_pool_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/structs.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/structs.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,61 +3,68 @@
 import pathlib as pl
 import typing as tp
 
 from cardano_clusterlib import consts
 from cardano_clusterlib import types as itp
 
 
-class CLIOut(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True)
+class CLIOut:
     stdout: bytes
     stderr: bytes
 
 
-class KeyPair(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class KeyPair:
     vkey_file: pl.Path
     skey_file: pl.Path
 
 
-class ColdKeyPair(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class ColdKeyPair:
     vkey_file: pl.Path
     skey_file: pl.Path
     counter_file: pl.Path
 
 
-class AddressRecord(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class AddressRecord:
     address: str
     vkey_file: pl.Path
     skey_file: pl.Path
 
 
-class StakeAddrInfo(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class StakeAddrInfo:
     address: str
     delegation: str
     reward_account_balance: int
     delegation_deposit: int
     vote_delegation: str
 
     def __bool__(self) -> bool:
         return bool(self.address)
 
 
-class UTXOData(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class UTXOData:
     utxo_hash: str
     utxo_ix: int
     amount: int
     address: str
     coin: str = consts.DEFAULT_COIN
     decoded_coin: str = ""
     datum_hash: str = ""
     inline_datum_hash: str = ""
     inline_datum: tp.Optional[tp.Union[str, dict]] = None
     reference_script: tp.Optional[dict] = None
 
 
-class TxOut(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class TxOut:
     address: str
     amount: int
     coin: str = consts.DEFAULT_COIN
     datum_hash: str = ""
     datum_hash_file: itp.FileType = ""
     datum_hash_cbor_file: itp.FileType = ""
     datum_hash_value: str = ""
@@ -72,15 +79,16 @@
 
 # list of `TxOut`s, empty list, or empty tuple
 OptionalTxOuts = tp.Union[tp.List[TxOut], tp.Tuple[()]]
 # list of `UTXOData`s, empty list, or empty tuple
 OptionalUTXOData = tp.Union[tp.List[UTXOData], tp.Tuple[()]]  # pylint: disable=invalid-name
 
 
-class ScriptTxIn(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class ScriptTxIn:
     """Data structure for Tx inputs that are combined with scripts (simple or Plutus)."""
 
     txins: tp.List[UTXOData]
     script_file: itp.FileType = ""
     reference_txin: tp.Optional[UTXOData] = None
     reference_type: str = ""
     # values below needed only when working with Plutus
@@ -91,29 +99,31 @@
     datum_value: str = ""
     inline_datum_present: bool = False
     redeemer_file: itp.FileType = ""
     redeemer_cbor_file: itp.FileType = ""
     redeemer_value: str = ""
 
 
-class ScriptWithdrawal(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class ScriptWithdrawal:
     """Data structure for withdrawals that are combined with Plutus scripts."""
 
     txout: TxOut
     script_file: itp.FileType = ""
     reference_txin: tp.Optional[UTXOData] = None
     reference_type: str = ""
     collaterals: OptionalUTXOData = ()
     execution_units: tp.Optional[tp.Tuple[int, int]] = None
     redeemer_file: itp.FileType = ""
     redeemer_cbor_file: itp.FileType = ""
     redeemer_value: str = ""
 
 
-class ComplexCert(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class ComplexCert:
     """Data structure for certificates with optional data for Plutus scripts.
 
     If used for one certificate, it needs to be used for all the other certificates in a given
     transaction (instead of `TxFiles.certificate_files`). Otherwise, order of certificates
     cannot be guaranteed.
     """
 
@@ -124,15 +134,16 @@
     collaterals: OptionalUTXOData = ()
     execution_units: tp.Optional[tp.Tuple[int, int]] = None
     redeemer_file: itp.FileType = ""
     redeemer_cbor_file: itp.FileType = ""
     redeemer_value: str = ""
 
 
-class Mint(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class Mint:
     txouts: tp.List[TxOut]
     script_file: itp.FileType = ""
     reference_txin: tp.Optional[UTXOData] = None
     reference_type: str = ""
     policyid: str = ""
     # values below needed only when working with Plutus
     collaterals: OptionalUTXOData = ()
@@ -148,43 +159,47 @@
 OptionalScriptCerts = tp.Union[tp.List[ComplexCert], tp.Tuple[()]]
 # list of `ScriptWithdrawal`s, empty list, or empty tuple
 OptionalScriptWithdrawals = tp.Union[tp.List[ScriptWithdrawal], tp.Tuple[()]]
 # list of `Mint`s, empty list, or empty tuple
 OptionalMint = tp.Union[tp.List[Mint], tp.Tuple[()]]
 
 
-class TxFiles(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class TxFiles:
     certificate_files: itp.OptionalFiles = ()
     proposal_files: itp.OptionalFiles = ()
     metadata_json_files: itp.OptionalFiles = ()
     metadata_cbor_files: itp.OptionalFiles = ()
     signing_key_files: itp.OptionalFiles = ()
     auxiliary_script_files: itp.OptionalFiles = ()
     vote_files: itp.OptionalFiles = ()
     metadata_json_detailed_schema: bool = False
 
 
-class PoolUser(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class PoolUser:
     payment: AddressRecord
     stake: AddressRecord
 
 
-class PoolData(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class PoolData:
     pool_name: str
     pool_pledge: int
     pool_cost: int
     pool_margin: float
     pool_metadata_url: str = ""
     pool_metadata_hash: str = ""
     pool_relay_dns: str = ""
     pool_relay_ipv4: str = ""
     pool_relay_port: int = 0
 
 
-class TxRawOutput(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class TxRawOutput:
     txins: tp.List[UTXOData]  # UTXOs used as inputs
     txouts: tp.List[TxOut]  # Tx outputs
     txouts_count: int  # Final number of tx outputs after adding change address and joining outputs
     tx_files: TxFiles  # Files needed for transaction building (certificates, signing keys, etc.)
     out_file: pl.Path  # Output file path for the transaction body
     fee: int  # Tx fee
     build_args: tp.List[str]  # Arguments that were passed to `cardano-cli transaction build*`
@@ -203,64 +218,71 @@
     script_valid: bool = True  # Whether the plutus script is valid
     required_signers: itp.OptionalFiles = ()  # Signing keys required for the transaction
     # Hashes of signing keys that are required for the transaction
     required_signer_hashes: tp.Union[tp.List[str], tp.Tuple[()]] = ()
     combined_reference_txins: OptionalUTXOData = ()  # All reference tx inputs
 
 
-class PoolCreationOutput(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class PoolCreationOutput:
     stake_pool_id: str
     vrf_key_pair: KeyPair
     cold_key_pair: ColdKeyPair
     pool_reg_cert_file: pl.Path
     pool_data: PoolData
     pool_owners: tp.List[PoolUser]
     tx_raw_output: TxRawOutput
     kes_key_pair: tp.Optional[KeyPair] = None
 
 
-class GenesisKeys(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class GenesisKeys:
     genesis_utxo_vkey: pl.Path
     genesis_utxo_skey: pl.Path
     genesis_vkeys: tp.List[pl.Path]
     delegate_skeys: tp.List[pl.Path]
 
 
-class PoolParamsTop(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class PoolParamsTop:
     pool_params: dict
     future_pool_params: dict
     retiring: tp.Optional[int]
 
 
-class AddressInfo(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class AddressInfo:
     address: str
     era: str
     encoding: str
     type: str
     base16: str
 
 
-class Value(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class Value:
     value: int
     coin: str
 
 
-class LeadershipSchedule(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class LeadershipSchedule:
     slot_no: int
     utc_time: datetime.datetime
 
 
-class DataForBuild(tp.NamedTuple):
+@dataclasses.dataclass(frozen=True, order=True)
+class DataForBuild:
     txins: tp.List[UTXOData]
     txouts: tp.List[TxOut]
     withdrawals: OptionalTxOuts
     script_withdrawals: OptionalScriptWithdrawals
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclasses.dataclass(frozen=True, order=True)
 class CCMember:
     epoch: int
     cold_vkey: str = ""
     cold_vkey_file: itp.FileType = ""
     cold_vkey_hash: str = ""
     cold_skey: str = ""
     cold_skey_file: itp.FileType = ""
@@ -269,93 +291,93 @@
     hot_vkey_file: itp.FileType = ""
     hot_vkey_hash: str = ""
     hot_skey: str = ""
     hot_skey_file: itp.FileType = ""
     hot_skey_hash: str = ""
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclasses.dataclass(frozen=True, order=True)
 class VoteCC:
     action_txid: str
     action_ix: int
     vote: consts.Votes
     vote_file: pl.Path
     cc_hot_vkey: str = ""
     cc_hot_vkey_file: tp.Optional[pl.Path] = None
     cc_hot_key_hash: str = ""
     anchor_url: str = ""
     anchor_data_hash: str = ""
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclasses.dataclass(frozen=True, order=True)
 class VoteDrep:
     action_txid: str
     action_ix: int
     vote: consts.Votes
     vote_file: pl.Path
     drep_vkey: str = ""
     drep_vkey_file: tp.Optional[pl.Path] = None
     drep_key_hash: str = ""
     anchor_url: str = ""
     anchor_data_hash: str = ""
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclasses.dataclass(frozen=True, order=True)
 class VoteSPO:
     action_txid: str
     action_ix: int
     vote: consts.Votes
     vote_file: pl.Path
     stake_pool_vkey: str = ""
     cold_vkey_file: tp.Optional[pl.Path] = None
     stake_pool_id: str = ""
     anchor_url: str = ""
     anchor_data_hash: str = ""
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclasses.dataclass(frozen=True, order=True)
 class ActionConstitution:
     action_file: pl.Path
     deposit_amt: int
     anchor_url: str
     anchor_data_hash: str
     constitution_url: str
     constitution_hash: str
     deposit_return_stake_vkey: str = ""
     deposit_return_stake_vkey_file: tp.Optional[pl.Path] = None
     deposit_return_stake_key_hash: str = ""
     prev_action_txid: str = ""
     prev_action_ix: int = -1
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclasses.dataclass(frozen=True, order=True)
 class ActionInfo:
     action_file: pl.Path
     deposit_amt: int
     anchor_url: str
     anchor_data_hash: str
     deposit_return_stake_vkey: str = ""
     deposit_return_stake_vkey_file: tp.Optional[pl.Path] = None
     deposit_return_stake_key_hash: str = ""
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclasses.dataclass(frozen=True, order=True)
 class ActionNoConfidence:
     action_file: pl.Path
     deposit_amt: int
     anchor_url: str
     anchor_data_hash: str
     prev_action_txid: str
     prev_action_ix: int
     deposit_return_stake_vkey: str = ""
     deposit_return_stake_vkey_file: tp.Optional[pl.Path] = None
     deposit_return_stake_key_hash: str = ""
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclasses.dataclass(frozen=True, order=True)
 class ActionUpdateCommittee:
     action_file: pl.Path
     deposit_amt: int
     anchor_url: str
     anchor_data_hash: str
     quorum: str
     add_cc_members: tp.List[CCMember] = dataclasses.field(default_factory=list)
@@ -363,29 +385,29 @@
     prev_action_txid: str = ""
     prev_action_ix: int = -1
     deposit_return_stake_vkey: str = ""
     deposit_return_stake_vkey_file: tp.Optional[pl.Path] = None
     deposit_return_stake_key_hash: str = ""
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclasses.dataclass(frozen=True, order=True)
 class ActionPParamsUpdate:
     action_file: pl.Path
     deposit_amt: int
     anchor_url: str
     anchor_data_hash: str
     cli_args: itp.UnpackableSequence
     prev_action_txid: str = ""
     prev_action_ix: int = -1
     deposit_return_stake_vkey: str = ""
     deposit_return_stake_vkey_file: tp.Optional[pl.Path] = None
     deposit_return_stake_key_hash: str = ""
 
 
-@dataclasses.dataclass(frozen=True)
+@dataclasses.dataclass(frozen=True, order=True)
 class ActionTreasuryWithdrawal:
     action_file: pl.Path
     transfer_amt: int
     deposit_amt: int
     anchor_url: str
     anchor_data_hash: str
     funds_receiving_stake_vkey: str = ""
```

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/transaction_group.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/transaction_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/txtools.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/txtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Tools used by `ClusterLib` for constructing transactions."""
 import base64
 import contextlib
+import dataclasses
 import functools
 import itertools
 import logging
 import typing as tp
 
 from cardano_clusterlib import consts
 from cardano_clusterlib import exceptions
@@ -249,16 +250,16 @@
 
     Return simple withdrawals, script withdrawals, combination of all withdrawals Tx outputs.
     """
     withdrawals = withdrawals and _resolve_withdrawals(
         clusterlib_obj=clusterlib_obj, withdrawals=withdrawals
     )
     script_withdrawals = [
-        s._replace(
-            txout=_resolve_withdrawals(clusterlib_obj=clusterlib_obj, withdrawals=[s.txout])[0]
+        dataclasses.replace(
+            s, txout=_resolve_withdrawals(clusterlib_obj=clusterlib_obj, withdrawals=[s.txout])[0]
         )
         for s in script_withdrawals
     ]
     withdrawals_txouts = [*withdrawals, *[s.txout for s in script_withdrawals]]
     return withdrawals, script_withdrawals, withdrawals_txouts
 
 
@@ -406,15 +407,15 @@
             if ar.coin in txouts_by_coin:
                 txouts_by_coin[ar.coin][1].append(ar.amount)
             else:
                 txouts_by_coin[ar.coin] = (ar, [ar.amount])
         # The tuple for each coin is `("one of the original TxOuts", "list of amounts")`.
         # All the `TxOut` values except of amount are the same in this loop, so we can
         # take the original `TxOut` and replace `amount` with sum of all amounts.
-        sum_txouts = [r[0]._replace(amount=sum(r[1])) for r in txouts_by_coin.values()]
+        sum_txouts = [dataclasses.replace(r[0], amount=sum(r[1])) for r in txouts_by_coin.values()]
 
         joined_txouts.append(sum_txouts)
 
     return joined_txouts
 
 
 def _join_txouts(
@@ -651,19 +652,20 @@
 
     # combine txins and make sure we have enough funds to satisfy all txouts
     combined_txins = [
         *txins,
         *script_txins_records,
     ]
     mint_txouts = list(itertools.chain.from_iterable(m.txouts for m in mint))
-    combined_tx_files = tx_files._replace(
+    combined_tx_files = dataclasses.replace(
+        tx_files,
         certificate_files=[
             *tx_files.certificate_files,
             *[c.certificate_file for c in complex_certs],
-        ]
+        ],
     )
     txins_copy, txouts_copy = _get_tx_ins_outs(
         clusterlib_obj=clusterlib_obj,
         src_address=src_address,
         tx_files=combined_tx_files,
         txins=combined_txins,
         txouts=txouts,
```

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib/types.py` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib/types.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib.egg-info/PKG-INFO` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.6.0a8
+Version: 0.6.0a9
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
 Author-email: Martin Kourim <martin.kourim@iohk.io>
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
 License: Apache License 2.0
 Project-URL: homepage, https://github.com/input-output-hk/cardano-clusterlib-py
```

### Comparing `cardano-clusterlib-0.6.0a8/cardano_clusterlib.egg-info/SOURCES.txt` & `cardano-clusterlib-0.6.0a9/cardano_clusterlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/docs/Makefile` & `cardano-clusterlib-0.6.0a9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/docs/source/cardano_clusterlib.rst` & `cardano-clusterlib-0.6.0a9/docs/source/cardano_clusterlib.rst`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/docs/source/conf.py` & `cardano-clusterlib-0.6.0a9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/pyproject.toml` & `cardano-clusterlib-0.6.0a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.6.0a8/upgrading/refactor_to_0_4_0rc1.sed` & `cardano-clusterlib-0.6.0a9/upgrading/refactor_to_0_4_0rc1.sed`

 * *Files identical despite different names*

