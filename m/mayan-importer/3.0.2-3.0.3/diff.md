# Comparing `tmp/mayan-importer-3.0.2.tar.gz` & `tmp/mayan-importer-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayan-importer-3.0.2.tar", last modified: Tue Apr  2 11:02:58 2024, max compression
+gzip compressed data, was "mayan-importer-3.0.3.tar", last modified: Wed Apr  3 13:18:53 2024, max compression
```

## Comparing `mayan-importer-3.0.2.tar` & `mayan-importer-3.0.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-02 11:02:58.714255 mayan-importer-3.0.2/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6341 2024-04-01 10:00:26.000000 mayan-importer-3.0.2/HISTORY.rst
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-3.0.2/LICENSE
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-3.0.2/MANIFEST.in
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9233 2024-04-02 11:02:58.714255 mayan-importer-3.0.2/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-3.0.2/README.rst
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-02 11:02:58.700255 mayan-importer-3.0.2/importer/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-3.0.2/importer/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      405 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/admin.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4643 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/api_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7455 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/apps.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7145 2024-04-01 11:57:21.000000 mayan-importer-3.0.2/importer/classes.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      145 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/dependencies.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1729 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/events.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       93 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/exceptions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      997 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/forms.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1366 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8712 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/importers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5779 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/links.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      904 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/literals.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-02 11:02:58.709255 mayan-importer-3.0.2/importer/migrations/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-3.0.2/importer/migrations/0001_initial.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-3.0.2/importer/migrations/0002_auto_20200908_0458.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-3.0.2/importer/migrations/0003_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/migrations/0004_auto_20200908_0853.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/migrations/0005_importsetup_state.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/migrations/0006_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/migrations/0007_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/migrations/0008_auto_20200924_0903.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/migrations/0009_importsetupaction.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      289 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/migrations/0010_remove_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/migrations/0011_auto_20201004_0042.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/migrations/0012_importsetupitem_documents.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/migrations/0013_auto_20201225_0155.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/migrations/0014_auto_20201227_0610.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/migrations/0015_auto_20220901_0932.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/migrations/0016_importsetup_item_time_buffer.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      239 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/migrations/0017_delete_importsetuplog.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1064 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/migrations/0018_auto_20240401_0808.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1326 2024-04-02 11:02:22.000000 mayan-importer-3.0.2/importer/migrations/0019_auto_20240402_1101.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-3.0.2/importer/migrations/__init__.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-02 11:02:58.710255 mayan-importer-3.0.2/importer/models/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      134 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/models/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4220 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/models/import_setup_item_model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2882 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/models/import_setup_item_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5737 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/models/import_setup_model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2470 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/models/import_setup_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1386 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/permissions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1197 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/queues.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3473 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/serializers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2794 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/tasks.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-02 11:02:58.712255 mayan-importer-3.0.2/importer/tests/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/tests/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1559 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/tests/importers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      408 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/tests/literals.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8729 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/tests/mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8233 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/tests/test_import_setup_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7881 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/tests/test_import_setup_item_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    12253 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/tests/test_import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6425 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/tests/test_import_setup_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5600 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/urls.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-02 11:02:58.713255 mayan-importer-3.0.2/importer/views/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-3.0.2/importer/views/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    16658 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/views/import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4343 2024-04-01 10:00:47.000000 mayan-importer-3.0.2/importer/views/import_setup_views.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-02 11:02:58.714255 mayan-importer-3.0.2/mayan_importer.egg-info/
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9233 2024-04-02 11:02:58.000000 mayan-importer-3.0.2/mayan_importer.egg-info/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2195 2024-04-02 11:02:58.000000 mayan-importer-3.0.2/mayan_importer.egg-info/SOURCES.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-04-02 11:02:58.000000 mayan-importer-3.0.2/mayan_importer.egg-info/dependency_links.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-04-02 11:02:58.000000 mayan-importer-3.0.2/mayan_importer.egg-info/not-zip-safe
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       16 2024-04-02 11:02:58.000000 mayan-importer-3.0.2/mayan_importer.egg-info/requires.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2024-04-02 11:02:58.000000 mayan-importer-3.0.2/mayan_importer.egg-info/top_level.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2024-04-02 11:02:58.715255 mayan-importer-3.0.2/setup.cfg
--rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3038 2024-04-02 11:02:38.000000 mayan-importer-3.0.2/setup.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-03 13:18:53.983857 mayan-importer-3.0.3/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6341 2024-04-01 10:00:26.000000 mayan-importer-3.0.3/HISTORY.rst
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/LICENSE
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/MANIFEST.in
+-rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9233 2024-04-03 13:18:53.983857 mayan-importer-3.0.3/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/README.rst
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-03 13:18:53.969857 mayan-importer-3.0.3/importer/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/importer/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      405 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/admin.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4643 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/api_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7455 2024-04-03 06:48:45.000000 mayan-importer-3.0.3/importer/apps.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7145 2024-04-01 11:57:21.000000 mayan-importer-3.0.3/importer/classes.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      145 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/dependencies.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1729 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/events.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       93 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/exceptions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      997 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/forms.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1366 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8712 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/importers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5779 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      904 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/literals.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-03 13:18:53.976857 mayan-importer-3.0.3/importer/migrations/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/importer/migrations/0001_initial.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/importer/migrations/0002_auto_20200908_0458.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/importer/migrations/0003_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0004_auto_20200908_0853.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0005_importsetup_state.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0006_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0007_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0008_auto_20200924_0903.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0009_importsetupaction.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      289 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0010_remove_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0011_auto_20201004_0042.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0012_importsetupitem_documents.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0013_auto_20201225_0155.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0014_auto_20201227_0610.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0015_auto_20220901_0932.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/migrations/0016_importsetup_item_time_buffer.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      239 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/migrations/0017_delete_importsetuplog.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1064 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/migrations/0018_auto_20240401_0808.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1326 2024-04-02 11:02:22.000000 mayan-importer-3.0.3/importer/migrations/0019_auto_20240402_1101.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-3.0.3/importer/migrations/__init__.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-03 13:18:53.977857 mayan-importer-3.0.3/importer/models/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      134 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/models/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4220 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/models/import_setup_item_model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2882 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/models/import_setup_item_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5737 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/models/import_setup_model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2470 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/models/import_setup_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1386 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/permissions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1197 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/queues.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3473 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/serializers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2794 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tasks.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-03 13:18:53.980857 mayan-importer-3.0.3/importer/tests/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tests/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1559 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tests/importers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      408 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tests/literals.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8729 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tests/mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8233 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/tests/test_import_setup_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7881 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tests/test_import_setup_item_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    12253 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tests/test_import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6425 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/tests/test_import_setup_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5600 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/urls.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-03 13:18:53.981857 mayan-importer-3.0.3/importer/views/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-3.0.3/importer/views/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    16658 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/views/import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4343 2024-04-01 10:00:47.000000 mayan-importer-3.0.3/importer/views/import_setup_views.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-03 13:18:53.982857 mayan-importer-3.0.3/mayan_importer.egg-info/
+-rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9233 2024-04-03 13:18:53.000000 mayan-importer-3.0.3/mayan_importer.egg-info/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2195 2024-04-03 13:18:53.000000 mayan-importer-3.0.3/mayan_importer.egg-info/SOURCES.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-04-03 13:18:53.000000 mayan-importer-3.0.3/mayan_importer.egg-info/dependency_links.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-04-03 13:18:53.000000 mayan-importer-3.0.3/mayan_importer.egg-info/not-zip-safe
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       16 2024-04-03 13:18:53.000000 mayan-importer-3.0.3/mayan_importer.egg-info/requires.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2024-04-03 13:18:53.000000 mayan-importer-3.0.3/mayan_importer.egg-info/top_level.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2024-04-03 13:18:53.983857 mayan-importer-3.0.3/setup.cfg
+-rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3038 2024-04-03 13:18:25.000000 mayan-importer-3.0.3/setup.py
```

### Comparing `mayan-importer-3.0.2/HISTORY.rst` & `mayan-importer-3.0.3/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/LICENSE` & `mayan-importer-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/PKG-INFO` & `mayan-importer-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 3.0.2
+Version: 3.0.3
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mayan-importer-3.0.2/README.rst` & `mayan-importer-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/api_views.py` & `mayan-importer-3.0.3/importer/api_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/apps.py` & `mayan-importer-3.0.3/importer/apps.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,21 +196,21 @@
         )
 
         # Import setup item
 
         menu_list_facet.bind_links(
             links=(
                 link_import_setup_item_document_list,
-                link_import_setup_item_edit
             ), sources=(ImportSetupItem,)
         )
         menu_multi_item.bind_links(
             links=(
                 link_import_setup_item_multiple_delete,
                 link_import_setup_item_multiple_process
             ), sources=(ImportSetupItem,)
         )
         menu_object.bind_links(
             links=(
-                link_import_setup_item_delete, link_import_setup_item_process,
+                link_import_setup_item_delete, link_import_setup_item_edit,
+                link_import_setup_item_process
             ), sources=(ImportSetupItem,)
         )
```

### Comparing `mayan-importer-3.0.2/importer/classes.py` & `mayan-importer-3.0.3/importer/classes.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/events.py` & `mayan-importer-3.0.3/importer/events.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/forms.py` & `mayan-importer-3.0.3/importer/forms.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/icons.py` & `mayan-importer-3.0.3/importer/icons.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/importers.py` & `mayan-importer-3.0.3/importer/importers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/links.py` & `mayan-importer-3.0.3/importer/links.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/literals.py` & `mayan-importer-3.0.3/importer/literals.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/migrations/0001_initial.py` & `mayan-importer-3.0.3/importer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/migrations/0002_auto_20200908_0458.py` & `mayan-importer-3.0.3/importer/migrations/0002_auto_20200908_0458.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/migrations/0003_importsetup_metadata_map.py` & `mayan-importer-3.0.3/importer/migrations/0003_importsetup_metadata_map.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/migrations/0004_auto_20200908_0853.py` & `mayan-importer-3.0.3/importer/migrations/0004_auto_20200908_0853.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/migrations/0005_importsetup_state.py` & `mayan-importer-3.0.3/importer/migrations/0005_importsetup_state.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/migrations/0008_auto_20200924_0903.py` & `mayan-importer-3.0.3/importer/migrations/0008_auto_20200924_0903.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/migrations/0009_importsetupaction.py` & `mayan-importer-3.0.3/importer/migrations/0009_importsetupaction.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/migrations/0011_auto_20201004_0042.py` & `mayan-importer-3.0.3/importer/migrations/0011_auto_20201004_0042.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/migrations/0012_importsetupitem_documents.py` & `mayan-importer-3.0.3/importer/migrations/0012_importsetupitem_documents.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/migrations/0013_auto_20201225_0155.py` & `mayan-importer-3.0.3/importer/migrations/0013_auto_20201225_0155.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/migrations/0015_auto_20220901_0932.py` & `mayan-importer-3.0.3/importer/migrations/0015_auto_20220901_0932.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/migrations/0016_importsetup_item_time_buffer.py` & `mayan-importer-3.0.3/importer/migrations/0016_importsetup_item_time_buffer.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/migrations/0018_auto_20240401_0808.py` & `mayan-importer-3.0.3/importer/migrations/0018_auto_20240401_0808.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/migrations/0019_auto_20240402_1101.py` & `mayan-importer-3.0.3/importer/migrations/0019_auto_20240402_1101.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/models/import_setup_item_model_mixins.py` & `mayan-importer-3.0.3/importer/models/import_setup_item_model_mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/models/import_setup_item_models.py` & `mayan-importer-3.0.3/importer/models/import_setup_item_models.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/models/import_setup_model_mixins.py` & `mayan-importer-3.0.3/importer/models/import_setup_model_mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/models/import_setup_models.py` & `mayan-importer-3.0.3/importer/models/import_setup_models.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/permissions.py` & `mayan-importer-3.0.3/importer/permissions.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/queues.py` & `mayan-importer-3.0.3/importer/queues.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/serializers.py` & `mayan-importer-3.0.3/importer/serializers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/tasks.py` & `mayan-importer-3.0.3/importer/tasks.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/tests/importers.py` & `mayan-importer-3.0.3/importer/tests/importers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/tests/mixins.py` & `mayan-importer-3.0.3/importer/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/tests/test_import_setup_api.py` & `mayan-importer-3.0.3/importer/tests/test_import_setup_api.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/tests/test_import_setup_item_api.py` & `mayan-importer-3.0.3/importer/tests/test_import_setup_item_api.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/tests/test_import_setup_item_views.py` & `mayan-importer-3.0.3/importer/tests/test_import_setup_item_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/tests/test_import_setup_views.py` & `mayan-importer-3.0.3/importer/tests/test_import_setup_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/urls.py` & `mayan-importer-3.0.3/importer/urls.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/views/import_setup_item_views.py` & `mayan-importer-3.0.3/importer/views/import_setup_item_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/importer/views/import_setup_views.py` & `mayan-importer-3.0.3/importer/views/import_setup_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/mayan_importer.egg-info/PKG-INFO` & `mayan-importer-3.0.3/mayan_importer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 3.0.2
+Version: 3.0.3
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mayan-importer-3.0.2/mayan_importer.egg-info/SOURCES.txt` & `mayan-importer-3.0.3/mayan_importer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0.2/setup.py` & `mayan-importer-3.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,10 +94,10 @@
     license='Apache 2.0',
     long_description=readme + '\n\n' + history,
     name=PACKAGE_NAME,
     packages=find_packages(PACKAGE_DIR),
     platforms=['any'],
     python_requires='!=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*',
     url='https://gitlab.com/mayan-edms/importer',
-    version='3.0.2',
+    version='3.0.3',
     zip_safe=False,
 )
```

