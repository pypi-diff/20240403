# Comparing `tmp/pg-activity-3.5.0.tar.gz` & `tmp/pg-activity-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg-activity-3.5.0.tar", last modified: Fri Mar  1 13:42:19 2024, max compression
+gzip compressed data, was "pg-activity-3.5.1.tar", last modified: Wed Apr  3 12:46:58 2024, max compression
```

## Comparing `pg-activity-3.5.0.tar` & `pg-activity-3.5.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:42:19.528888 pg-activity-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-01 13:42:08.000000 pg-activity-3.5.0/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-01 13:42:08.000000 pg-activity-3.5.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-01 13:42:08.000000 pg-activity-3.5.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-01 13:42:08.000000 pg-activity-3.5.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-01 13:42:08.000000 pg-activity-3.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-03-01 13:42:08.000000 pg-activity-3.5.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-03-01 13:42:08.000000 pg-activity-3.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-01 13:42:08.000000 pg-activity-3.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-01 13:42:08.000000 pg-activity-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17563 2024-03-01 13:42:19.528888 pg-activity-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15298 2024-03-01 13:42:08.000000 pg-activity-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-01 13:42:08.000000 pg-activity-3.5.0/RELEASE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:42:19.508888 pg-activity-3.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:42:19.512888 pg-activity-3.5.0/docs/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)    28659 2024-03-01 13:42:08.000000 pg-activity-3.5.0/docs/imgs/logo-horizontal.png
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-03-01 13:42:08.000000 pg-activity-3.5.0/docs/imgs/logo-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-03-01 13:42:08.000000 pg-activity-3.5.0/docs/imgs/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   337072 2024-03-01 13:42:08.000000 pg-activity-3.5.0/docs/imgs/screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:42:19.512888 pg-activity-3.5.0/docs/man/
--rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-03-01 13:42:08.000000 pg-activity-3.5.0/docs/man/build-man.sh
--rw-r--r--   0 runner    (1001) docker     (127)    27818 2024-03-01 13:42:08.000000 pg-activity-3.5.0/docs/man/pg_activity.1
--rw-r--r--   0 runner    (1001) docker     (127)    13881 2024-03-01 13:42:08.000000 pg-activity-3.5.0/docs/man/pg_activity.pod
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-01 13:42:08.000000 pg-activity-3.5.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:42:19.524888 pg-activity-3.5.0/pg_activity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17563 2024-03-01 13:42:19.000000 pg-activity-3.5.0/pg_activity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-01 13:42:19.000000 pg-activity-3.5.0/pg_activity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 13:42:19.000000 pg-activity-3.5.0/pg_activity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-01 13:42:19.000000 pg-activity-3.5.0/pg_activity.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-01 13:42:19.000000 pg-activity-3.5.0/pg_activity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-01 13:42:19.000000 pg-activity-3.5.0/pg_activity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:42:19.516888 pg-activity-3.5.0/pgactivity/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/activities.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11654 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19961 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/pg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:42:19.516888 pg-activity-3.5.0/pgactivity/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/profiles/minimal.conf
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/profiles/narrow.conf
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/profiles/wide.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:42:19.524888 pg-activity-3.5.0/pgactivity/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/disable_log_min_duration_sample.sql
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/disable_log_min_duration_statement.sql
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/do_pg_cancel_backend.sql
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/do_pg_terminate_backend.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_blocking_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_blocking_post_090200.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_blocking_post_090600.sql
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_data_directory.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_pg_activity_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_pg_activity_post_090200.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_pg_activity_post_090600.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_pg_activity_post_100000.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_pg_activity_post_110000.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_pg_activity_post_130000.sql
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_pga_inet_addresses.sql
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_replication_slots_post_140000.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_server_info_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_server_info_post_090100.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_server_info_post_090200.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_server_info_post_090400.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_server_info_post_090600.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_server_info_post_100000.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_server_info_post_110000.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_temporary_files_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_temporary_files_post_090100.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_temporary_files_post_090500.sql
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_temporary_files_post_120000.sql
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_version.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_waiting_oldest.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_waiting_post_090200.sql
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_wal_receivers_post_090600.sql
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/get_wal_senders_post_090100.sql
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/queries/reset_statement_timeout.sql
--rw-r--r--   0 runner    (1001) docker     (127)    31356 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19050 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pgactivity/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-01 13:42:08.000000 pg-activity-3.5.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 13:42:19.528888 pg-activity-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 13:42:08.000000 pg-activity-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:42:19.524888 pg-activity-3.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-03-01 13:42:08.000000 pg-activity-3.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 13:42:19.524888 pg-activity-3.5.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    62239 2024-03-01 13:42:08.000000 pg-activity-3.5.0/tests/data/local-processes-input.json
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-03-01 13:42:08.000000 pg-activity-3.5.0/tests/test_activities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-03-01 13:42:08.000000 pg-activity-3.5.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-03-01 13:42:08.000000 pg-activity-3.5.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-01 13:42:08.000000 pg-activity-3.5.0/tests/test_scroll.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-01 13:42:08.000000 pg-activity-3.5.0/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    41106 2024-03-01 13:42:08.000000 pg-activity-3.5.0/tests/test_ui.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-01 13:42:08.000000 pg-activity-3.5.0/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    24432 2024-03-01 13:42:08.000000 pg-activity-3.5.0/tests/test_views.txt
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-01 13:42:08.000000 pg-activity-3.5.0/tests/test_widgets.txt
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-01 13:42:08.000000 pg-activity-3.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:46:58.611309 pg-activity-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 12:46:51.000000 pg-activity-3.5.1/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 12:46:51.000000 pg-activity-3.5.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 12:46:51.000000 pg-activity-3.5.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-03 12:46:51.000000 pg-activity-3.5.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-03 12:46:51.000000 pg-activity-3.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-03 12:46:51.000000 pg-activity-3.5.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-04-03 12:46:51.000000 pg-activity-3.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-03 12:46:51.000000 pg-activity-3.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-03 12:46:51.000000 pg-activity-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17563 2024-04-03 12:46:58.611309 pg-activity-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15298 2024-04-03 12:46:51.000000 pg-activity-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-03 12:46:51.000000 pg-activity-3.5.1/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:46:58.591309 pg-activity-3.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:46:58.595309 pg-activity-3.5.1/docs/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)    28659 2024-04-03 12:46:51.000000 pg-activity-3.5.1/docs/imgs/logo-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-03 12:46:51.000000 pg-activity-3.5.1/docs/imgs/logo-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-03 12:46:51.000000 pg-activity-3.5.1/docs/imgs/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   337072 2024-04-03 12:46:51.000000 pg-activity-3.5.1/docs/imgs/screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:46:58.595309 pg-activity-3.5.1/docs/man/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-04-03 12:46:51.000000 pg-activity-3.5.1/docs/man/build-man.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    27818 2024-04-03 12:46:51.000000 pg-activity-3.5.1/docs/man/pg_activity.1
+-rw-r--r--   0 runner    (1001) docker     (127)    13881 2024-04-03 12:46:51.000000 pg-activity-3.5.1/docs/man/pg_activity.pod
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 12:46:51.000000 pg-activity-3.5.1/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:46:58.607309 pg-activity-3.5.1/pg_activity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17563 2024-04-03 12:46:58.000000 pg-activity-3.5.1/pg_activity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-03 12:46:58.000000 pg-activity-3.5.1/pg_activity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:46:58.000000 pg-activity-3.5.1/pg_activity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 12:46:58.000000 pg-activity-3.5.1/pg_activity.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 12:46:58.000000 pg-activity-3.5.1/pg_activity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 12:46:58.000000 pg-activity-3.5.1/pg_activity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:46:58.599309 pg-activity-3.5.1/pgactivity/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11773 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/activities.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11654 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19961 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10266 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/pg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:46:58.599309 pg-activity-3.5.1/pgactivity/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/profiles/minimal.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/profiles/narrow.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/profiles/wide.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:46:58.607309 pg-activity-3.5.1/pgactivity/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/disable_log_min_duration_sample.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/disable_log_min_duration_statement.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/do_pg_cancel_backend.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/do_pg_terminate_backend.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_blocking_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_blocking_post_090200.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_blocking_post_090600.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_data_directory.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_pg_activity_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_pg_activity_post_090200.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_pg_activity_post_090600.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_pg_activity_post_100000.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_pg_activity_post_110000.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_pg_activity_post_130000.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_pga_inet_addresses.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_replication_slots_post_140000.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_server_info_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_server_info_post_090100.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_server_info_post_090200.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_server_info_post_090400.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_server_info_post_090600.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_server_info_post_100000.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_server_info_post_110000.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_temporary_files_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_temporary_files_post_090100.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_temporary_files_post_090500.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_temporary_files_post_120000.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_version.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_waiting_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_waiting_post_090200.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_wal_receivers_post_090600.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/get_wal_senders_post_090100.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/queries/reset_statement_timeout.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    31356 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19050 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pgactivity/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 12:46:51.000000 pg-activity-3.5.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:46:58.611309 pg-activity-3.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:46:51.000000 pg-activity-3.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:46:58.607309 pg-activity-3.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-03 12:46:51.000000 pg-activity-3.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:46:58.607309 pg-activity-3.5.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    62239 2024-04-03 12:46:51.000000 pg-activity-3.5.1/tests/data/local-processes-input.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-03 12:46:51.000000 pg-activity-3.5.1/tests/test_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-03 12:46:51.000000 pg-activity-3.5.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-03 12:46:51.000000 pg-activity-3.5.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-03 12:46:51.000000 pg-activity-3.5.1/tests/test_scroll.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-03 12:46:51.000000 pg-activity-3.5.1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41255 2024-04-03 12:46:51.000000 pg-activity-3.5.1/tests/test_ui.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-03 12:46:51.000000 pg-activity-3.5.1/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24432 2024-04-03 12:46:51.000000 pg-activity-3.5.1/tests/test_views.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-03 12:46:51.000000 pg-activity-3.5.1/tests/test_widgets.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-03 12:46:51.000000 pg-activity-3.5.1/tox.ini
```

### Comparing `pg-activity-3.5.0/.pre-commit-config.yaml` & `pg-activity-3.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/AUTHORS.md` & `pg-activity-3.5.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/CHANGELOG.md` & `pg-activity-3.5.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 # Change log
 
+## pg\_activity 3.5.1 - 2024-04-03
+
+### Fixed
+
+* Resolve a warning about usage of a deprecated Python `datetime` API from
+  Python 3.12.
+* Resolve setuptools warnings about packages 'pgactivity.profiles' and
+  'pgactivity.queries' being absent from `packages` configuration by getting
+  back to setuptools "automatic discovery" (#411).
+
+### Misc
+
+* Turn Python warnings into errors when running the test suite.
+
 ## pg\_activity 3.5.0 - 2024-03-01
 
 ### Added
 
 * The *rollback ratio* is now displayed in the "global" header (#385).
 * Make header's sections display configurable through the `[header]` section of
   the configuration file.
```

### Comparing `pg-activity-3.5.0/LICENSE.txt` & `pg-activity-3.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/PKG-INFO` & `pg-activity-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-activity
-Version: 3.5.0
+Version: 3.5.1
 Summary: Command line tool for PostgreSQL server activity monitoring.
 Author-email: Julien Tachoires <julmon@gmail.com>, Benoit Lobréau <benoit.lobreau@dalibo.com>, Denis Laxalde <denis.laxalde@dalibo.com>, Dalibo <contact@dalibo.com>
 Maintainer-email: Denis Laxalde <denis.laxalde@dalibo.com>, Benoit Lobréau <benoit.lobreau@dalibo.com>
 License: PostgreSQL
 Project-URL: Bug Tracker, https://github.com/dalibo/pg_activity/issues/
 Project-URL: Changelog, https://github.com/dalibo/pg_activity/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/dalibo/pg_activity
```

### Comparing `pg-activity-3.5.0/README.md` & `pg-activity-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/RELEASE.md` & `pg-activity-3.5.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/docs/imgs/logo-horizontal.png` & `pg-activity-3.5.1/docs/imgs/logo-horizontal.png`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/docs/imgs/logo-horizontal.svg` & `pg-activity-3.5.1/docs/imgs/logo-horizontal.svg`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/docs/imgs/logo.svg` & `pg-activity-3.5.1/docs/imgs/logo.svg`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/docs/imgs/screenshot.png` & `pg-activity-3.5.1/docs/imgs/screenshot.png`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/docs/man/pg_activity.1` & `pg-activity-3.5.1/docs/man/pg_activity.1`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 .    ds ae ae
 .    ds Ae AE
 .\}
 .rm #[ #] #H #V #F C
 .\" ========================================================================
 .\"
 .IX Title "PG_ACTIVITY 1"
-.TH PG_ACTIVITY 1 "2024-03-01" "pg_activity 3.5.0" "Command line tool for PostgreSQL server activity monitoring."
+.TH PG_ACTIVITY 1 "2024-04-03" "pg_activity 3.5.1" "Command line tool for PostgreSQL server activity monitoring."
 .\" For nroff, turn off justification.  Always turn off hyphenation; it makes
 .\" way too many mistakes in technical documents.
 .if n .ad l
 .nh
 .SH "NAME"
 pg_activity \- Realtime PostgreSQL database server monitoring tool
 .SH "SYNOPSIS"
```

### Comparing `pg-activity-3.5.0/docs/man/pg_activity.pod` & `pg-activity-3.5.1/docs/man/pg_activity.pod`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pg_activity.egg-info/PKG-INFO` & `pg-activity-3.5.1/pg_activity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-activity
-Version: 3.5.0
+Version: 3.5.1
 Summary: Command line tool for PostgreSQL server activity monitoring.
 Author-email: Julien Tachoires <julmon@gmail.com>, Benoit Lobréau <benoit.lobreau@dalibo.com>, Denis Laxalde <denis.laxalde@dalibo.com>, Dalibo <contact@dalibo.com>
 Maintainer-email: Denis Laxalde <denis.laxalde@dalibo.com>, Benoit Lobréau <benoit.lobreau@dalibo.com>
 License: PostgreSQL
 Project-URL: Bug Tracker, https://github.com/dalibo/pg_activity/issues/
 Project-URL: Changelog, https://github.com/dalibo/pg_activity/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/dalibo/pg_activity
```

### Comparing `pg-activity-3.5.0/pg_activity.egg-info/SOURCES.txt` & `pg-activity-3.5.1/pg_activity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/activities.py` & `pg-activity-3.5.1/pgactivity/activities.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/cli.py` & `pg-activity-3.5.1/pgactivity/cli.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/colors.py` & `pg-activity-3.5.1/pgactivity/colors.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/compat.py` & `pg-activity-3.5.1/pgactivity/compat.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/config.py` & `pg-activity-3.5.1/pgactivity/config.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/data.py` & `pg-activity-3.5.1/pgactivity/data.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/handlers.py` & `pg-activity-3.5.1/pgactivity/handlers.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/keys.py` & `pg-activity-3.5.1/pgactivity/keys.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/pg.py` & `pg-activity-3.5.1/pgactivity/pg.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_blocking_oldest.sql` & `pg-activity-3.5.1/pgactivity/queries/get_blocking_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_blocking_post_090200.sql` & `pg-activity-3.5.1/pgactivity/queries/get_blocking_post_090200.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_blocking_post_090600.sql` & `pg-activity-3.5.1/pgactivity/queries/get_blocking_post_090600.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_pg_activity_oldest.sql` & `pg-activity-3.5.1/pgactivity/queries/get_pg_activity_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_pg_activity_post_090200.sql` & `pg-activity-3.5.1/pgactivity/queries/get_pg_activity_post_090200.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_pg_activity_post_090600.sql` & `pg-activity-3.5.1/pgactivity/queries/get_pg_activity_post_090600.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_pg_activity_post_100000.sql` & `pg-activity-3.5.1/pgactivity/queries/get_pg_activity_post_100000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_pg_activity_post_110000.sql` & `pg-activity-3.5.1/pgactivity/queries/get_pg_activity_post_110000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_pg_activity_post_130000.sql` & `pg-activity-3.5.1/pgactivity/queries/get_pg_activity_post_130000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_server_info_oldest.sql` & `pg-activity-3.5.1/pgactivity/queries/get_server_info_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_server_info_post_090100.sql` & `pg-activity-3.5.1/pgactivity/queries/get_server_info_post_090100.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_server_info_post_090200.sql` & `pg-activity-3.5.1/pgactivity/queries/get_server_info_post_090200.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_server_info_post_090400.sql` & `pg-activity-3.5.1/pgactivity/queries/get_server_info_post_090400.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_server_info_post_090600.sql` & `pg-activity-3.5.1/pgactivity/queries/get_server_info_post_090600.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_server_info_post_100000.sql` & `pg-activity-3.5.1/pgactivity/queries/get_server_info_post_100000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_server_info_post_110000.sql` & `pg-activity-3.5.1/pgactivity/queries/get_server_info_post_110000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_temporary_files_oldest.sql` & `pg-activity-3.5.1/pgactivity/queries/get_temporary_files_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_temporary_files_post_090100.sql` & `pg-activity-3.5.1/pgactivity/queries/get_temporary_files_post_090100.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_temporary_files_post_090500.sql` & `pg-activity-3.5.1/pgactivity/queries/get_temporary_files_post_090500.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_waiting_oldest.sql` & `pg-activity-3.5.1/pgactivity/queries/get_waiting_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/queries/get_waiting_post_090200.sql` & `pg-activity-3.5.1/pgactivity/queries/get_waiting_post_090200.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/types.py` & `pg-activity-3.5.1/pgactivity/types.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/ui.py` & `pg-activity-3.5.1/pgactivity/ui.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/utils.py` & `pg-activity-3.5.1/pgactivity/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import functools
 import re
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from typing import IO, Any, Iterable, Mapping
 
 import attr
 import humanize
 
 naturalsize = functools.partial(humanize.naturalsize, gnu=True, format="%.2f")
 try:
@@ -276,15 +276,15 @@
 
     def yn_na(value: bool | None) -> str:
         if value is None:
             return "N/A"
         return yn(value)
 
     for p in procs:
-        dt = datetime.utcnow().strftime("%Y-%m-%dT%H:%m:%SZ")
+        dt = datetime.now(timezone.utc).strftime("%Y-%m-%dT%H:%m:%SZ")
         pid = p.get("pid", "N/A")
         database = p.get("database", "N/A") or ""
         appname = p.get("application_name", "N/A")
         user = p.get("user", "N/A")
         client = p.get("client", "N/A")
         cpu = p.get("cpu", "N/A")
         mem = p.get("mem", "N/A")
```

### Comparing `pg-activity-3.5.0/pgactivity/views.py` & `pg-activity-3.5.1/pgactivity/views.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pgactivity/widgets.py` & `pg-activity-3.5.1/pgactivity/widgets.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/pyproject.toml` & `pg-activity-3.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -80,17 +80,14 @@
 Changelog = "https://github.com/dalibo/pg_activity/blob/master/CHANGELOG.md"
 Homepage = "https://github.com/dalibo/pg_activity"
 "Source code" = "https://github.com/dalibo/pg_activity/"
 
 [tool.setuptools.dynamic]
 version = { attr = "pgactivity.__version__" }
 
-[tool.setuptools]
-packages = ["pgactivity"]
-
 [tool.black]
 line-length = 88
 include = '\.pyi?$'
 exclude = '''
 (
   /(
       \.eggs
```

### Comparing `pg-activity-3.5.0/tests/conftest.py` & `pg-activity-3.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/tests/data/local-processes-input.json` & `pg-activity-3.5.1/tests/data/local-processes-input.json`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/tests/test_activities.py` & `pg-activity-3.5.1/tests/test_activities.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/tests/test_config.py` & `pg-activity-3.5.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/tests/test_data.py` & `pg-activity-3.5.1/tests/test_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,36 +7,34 @@
 import pytest
 from psycopg.errors import WrongObjectType
 
 from pgactivity import types
 from pgactivity.data import Data
 
 
-def wait_for_data(fct, msg: str, timeout: int = 2):
+def retry(fct, msg: str, timeout: int = 2):
     count = int(timeout / 0.1)
     for _ in range(count):
         time.sleep(0.1)
-        data = fct()
-
-        if not data:
-            continue
-        break
-    else:
-        raise AssertionError(msg)
-    return data
+        value = fct()
+        if value:
+            return value
+    pytest.fail(msg)
 
 
 @pytest.fixture
 def data(postgresql):
-    return Data.pg_connect(
+    obj = Data.pg_connect(
         host=postgresql.info.host,
         port=postgresql.info.port,
         database=postgresql.info.dbname,
         user=postgresql.info.user,
     )
+    yield obj
+    obj.pg_conn.close()
 
 
 def test_pg_is_local(postgresql, data):
     assert data.pg_is_local()
 
 
 def test_pg_is_local_access(postgresql, data):
@@ -61,17 +59,15 @@
 
 def test_blocking_waiting(postgresql, data, execute):
     postgresql.execute("CREATE TABLE t AS (SELECT 'init'::text s)")
     postgresql.commit()
     execute("UPDATE t SET s = 'blocking'")
     execute("UPDATE t SET s = 'waiting 1'", commit=True)
     execute("UPDATE t SET s = 'waiting 2'", commit=True)
-    blocking = wait_for_data(
-        data.pg_get_blocking, msg="could not fetch blocking queries"
-    )
+    blocking = retry(data.pg_get_blocking, msg="could not fetch blocking queries")
     waiting = data.pg_get_waiting()
     assert len(blocking) == 2
     assert len(waiting) == 2
     assert "blocking" in blocking[0].query
     assert "waiting 1" in waiting[0].query and "waiting 2" in waiting[1].query
     if postgresql.info.server_version >= 100000:
         assert blocking[0].wait == "ClientRead"
@@ -81,17 +77,15 @@
 
 
 def test_pg_get_blocking_virtualxid(postgresql, data, execute):
     postgresql.execute("CREATE TABLE t AS (SELECT 'init'::text s)")
     postgresql.commit()
     execute("UPDATE t SET s = 'blocking'")
     execute("CREATE INDEX CONCURRENTLY ON t(s)", autocommit=True)
-    (blocking,) = wait_for_data(
-        data.pg_get_blocking, msg="could not fetch blocking queries"
-    )
+    (blocking,) = retry(data.pg_get_blocking, msg="could not fetch blocking queries")
     (waiting,) = data.pg_get_waiting()
     assert "blocking" in blocking.query
     assert "CREATE INDEX CONCURRENTLY ON t(s)" in waiting.query
     assert str(blocking.type) == "virtualxid"
 
 
 def test_cancel_backend(postgresql, data):
@@ -100,15 +94,15 @@
     assert data.pg_cancel_backend(running.pid)
 
 
 def test_terminate_backend(postgresql, data):
     postgresql.execute("SELECT pg_sleep(1)")
     (running,) = data.pg_get_activities()
     assert data.pg_terminate_backend(running.pid)
-    assert not data.pg_get_activities()
+    retry(lambda: not data.pg_get_activities(), msg="some processes are still active")
 
 
 def test_encoding(postgresql, data, execute):
     """Test for issue #149, #332."""
     conninfo = postgresql.info.dsn
     # plateform specific locales (Centos, Ubuntu)
     encodings = ["fr_FR.latin1", "fr_FR.88591", "fr_FR.8859-1"]
@@ -129,34 +123,37 @@
 
     with psycopg.connect(conninfo, dbname="latin1") as conn:
         conn.execute("CREATE TABLE tbl AS (SELECT 'initilialized éléphant' s)")
         conn.commit()
 
     execute("UPDATE tbl SET s = 'blocking éléphant'", dbname="latin1")
     execute("UPDATE tbl SET s = 'waiting éléphant'", dbname="latin1", commit=True)
-    running = wait_for_data(data.pg_get_activities, msg="could not fetch activities")
+    running = retry(data.pg_get_activities, msg="could not fetch activities")
     assert "blocking éléphant" in running[0].query
-    (waiting,) = wait_for_data(data.pg_get_waiting, "no waiting process")
+    (waiting,) = retry(data.pg_get_waiting, "no waiting process")
     assert waiting.query and "waiting éléphant" in waiting.query
     (blocking,) = data.pg_get_blocking()
     assert blocking.query and "blocking éléphant" in blocking.query
 
 
 @pytest.mark.parametrize("encoding", ["utf-8", "latin1", "sql_ascii"])
 def test_client_encoding(postgresql, encoding: str) -> None:
     data = Data.pg_connect(
         host=postgresql.info.host,
         port=postgresql.info.port,
         database=postgresql.info.dbname,
         user=postgresql.info.user,
         dsn=f"client_encoding={encoding}",
     )
-    assert data.pg_version.startswith(
-        f"PostgreSQL {str(postgresql.info.server_version)[:2]}"
-    )
+    try:
+        assert data.pg_version.startswith(
+            f"PostgreSQL {str(postgresql.info.server_version)[:2]}"
+        )
+    finally:
+        data.pg_conn.close()
 
 
 @pytest.mark.parametrize(
     "pyenc, pgenc, locale",
     [
         ("utf8", "UTF8", None),
         ("ascii", "SQL_ASCII", None),
@@ -180,17 +177,17 @@
     assert running.encoding == pgenc
     assert running.database == dbname
 
 
 def test_filters_dbname(data, execute):
     data_filtered = attr.evolve(data, filters=types.Filters(dbname="temp"))
     execute("SELECT pg_sleep(2)", dbname="template1", autocommit=True)
-    nbconn = wait_for_data(
+    nbconn = retry(
         data.pg_get_server_information,
         msg="could not get active connections for filtered DBNAME",
     )
-    nbconn_filtered = wait_for_data(
+    nbconn_filtered = retry(
         data_filtered.pg_get_server_information,
         msg="could not get active connections for filtered DBNAME",
     )
     assert nbconn.active_connections == 2
     assert nbconn_filtered.active_connections == 1
```

### Comparing `pg-activity-3.5.0/tests/test_scroll.txt` & `pg-activity-3.5.1/tests/test_scroll.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/tests/test_ui.txt` & `pg-activity-3.5.1/tests/test_ui.txt`

 * *Files 0% similar despite different names*

```diff
@@ -53,40 +53,40 @@
 >>> options = argparse.Namespace(**defaults)
 
 >>> os.environ["LINES"] = "26"
 >>> term = blessed.Terminal(force_styling=None)
 >>> term.width, term.height
 (80, 26)
 
->>> host = types.Host(
-...     "test",
-...     postgres.info.user,
-...     postgres.info.host,
-...     postgres.info.port,
-...     postgres.info.dbname,
-... )
->>> dataobj = data.Data.pg_connect(
-...     host=postgres.info.host,
-...     port=postgres.info.port,
-...     user=postgres.info.user,
-...     database=postgres.info.dbname,
-...     min_duration=options.minduration,
-... )
-
 >>> def mkconfig(value):
 ...     return config.Configuration(
 ...         **{k: config.UISection(**v) for k, v in value.items()}
 ... )
 >>> CONFIG = mkconfig({"database": {"width": 9}, "client": {"width": 12}})
 
 >>> def run_ui(options, keys, config=CONFIG, expected_timeouts=None,
 ...            render_header=True, render_footer=False,
 ...            width=200):
 ...     """Wrapper to ui.main() with a fake term.inkey()."""
 ...
+...     host = types.Host(
+...         "test",
+...         postgres.info.user,
+...         postgres.info.host,
+...         postgres.info.port,
+...         postgres.info.dbname,
+...     )
+...     dataobj = data.Data.pg_connect(
+...         host=postgres.info.host,
+...         port=postgres.info.port,
+...         user=postgres.info.user,
+...         database=postgres.info.dbname,
+...         min_duration=options.minduration,
+...     )
+...
 ...     call_args_list = []
 ...
 ...     def inkey(*, timeout):
 ...         call_args_list.append(timeout)
 ...         key = keys.pop(0)
 ...         if isinstance(key, dict):
 ...             ks = Keystroke(**key)
@@ -94,17 +94,20 @@
 ...             ks = Keystroke(key)
 ...         if render_footer:
 ...             print()
 ...         print(term.center(f" sending key '{ks}' ", fillchar="-", width=width))
 ...         return ks
 ...
 ...     with patch.object(term, "inkey", new=inkey):
-...         ui.main(term, config, dataobj, host, options,
-...                 render_header=render_header, render_footer=render_footer,
-...                 width=width, wait_on_actions=1)
+...         try:
+...             ui.main(term, config, dataobj, host, options,
+...                     render_header=render_header, render_footer=render_footer,
+...                     width=width, wait_on_actions=1)
+...         finally:
+...             dataobj.pg_conn.close()
 ...
 ...     if expected_timeouts is not None:
 ...         assert call_args_list == expected_timeouts
 
 Force local mode and mock server and system info
 
 >>> pg_is_local_access = patch("pgactivity.data.Data.pg_is_local_access", return_value=True)
```

### Comparing `pg-activity-3.5.0/tests/test_views.py` & `pg-activity-3.5.1/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/tests/test_views.txt` & `pg-activity-3.5.1/tests/test_views.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/tests/test_widgets.txt` & `pg-activity-3.5.1/tests/test_widgets.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.5.0/tox.ini` & `pg-activity-3.5.1/tox.ini`

 * *Files identical despite different names*

