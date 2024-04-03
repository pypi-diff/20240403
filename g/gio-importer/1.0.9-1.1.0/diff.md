# Comparing `tmp/gio_importer-1.0.9.tar.gz` & `tmp/gio_importer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gio_importer-1.0.9.tar", last modified: Tue Apr  2 06:29:17 2024, max compression
+gzip compressed data, was "gio_importer-1.1.0.tar", last modified: Wed Apr  3 08:07:08 2024, max compression
```

## Comparing `gio_importer-1.0.9.tar` & `gio_importer-1.1.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:29:17.988166 gio_importer-1.0.9/
--rw-r--r--   0 chengcheng   (501) staff       (20)     1061 2024-03-22 01:45:40.000000 gio_importer-1.0.9/LICENSE
--rw-r--r--   0 chengcheng   (501) staff       (20)       71 2024-03-22 01:45:40.000000 gio_importer-1.0.9/MANIFEST.in
--rw-r--r--   0 chengcheng   (501) staff       (20)    12101 2024-04-02 06:29:17.987775 gio_importer-1.0.9/PKG-INFO
--rw-r--r--   0 chengcheng   (501) staff       (20)      792 2024-03-22 01:45:40.000000 gio_importer-1.0.9/README.md
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:29:17.957695 gio_importer-1.0.9/gio_importer.egg-info/
--rw-r--r--   0 chengcheng   (501) staff       (20)    12101 2024-04-02 06:29:17.000000 gio_importer-1.0.9/gio_importer.egg-info/PKG-INFO
--rw-r--r--   0 chengcheng   (501) staff       (20)     1381 2024-04-02 06:29:17.000000 gio_importer-1.0.9/gio_importer.egg-info/SOURCES.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)        1 2024-04-02 06:29:17.000000 gio_importer-1.0.9/gio_importer.egg-info/dependency_links.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)      197 2024-04-02 06:29:17.000000 gio_importer-1.0.9/gio_importer.egg-info/entry_points.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)       84 2024-04-02 06:29:17.000000 gio_importer-1.0.9/gio_importer.egg-info/requires.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)       10 2024-04-02 06:29:17.000000 gio_importer-1.0.9/gio_importer.egg-info/top_level.txt
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:29:17.966590 gio_importer-1.0.9/importers/
--rw-r--r--   0 chengcheng   (501) staff       (20)    11711 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/README.md
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/__init__.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:29:17.967462 gio_importer-1.0.9/importers/clear_data/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/clear_data/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2820 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/clear_data/clear_data.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     1714 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/clear_user.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:29:17.969583 gio_importer-1.0.9/importers/common/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/common/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     5581 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/common/common_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2507 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/common/config_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2602 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/common/http_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      955 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/common/log_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      771 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/conf.cfg
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:29:17.976994 gio_importer-1.0.9/importers/data_import/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/data_import/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    21814 2024-03-22 02:06:04.000000 gio_importer-1.0.9/importers/data_import/data_ads.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    21731 2024-03-22 02:06:54.000000 gio_importer-1.0.9/importers/data_import/data_events.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    11148 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/data_import/data_format_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    17799 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/data_import/data_item_variable.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     6455 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/data_import/data_model.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    15382 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/data_import/data_user_variable.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     6943 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/data_importer.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:29:17.981337 gio_importer-1.0.9/importers/db_import/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/db_import/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2717 2024-03-22 02:07:32.000000 gio_importer-1.0.9/importers/db_import/database_import.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    14364 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/db_import/hive_import.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    14467 2024-03-22 02:11:11.000000 gio_importer-1.0.9/importers/db_import/mysql_import.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:29:17.984404 gio_importer-1.0.9/importers/example/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/example/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     5144 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/format_importer.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      472 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/log_conf.yaml
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:29:17.986456 gio_importer-1.0.9/importers/meta/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/meta/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    10656 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/meta/check_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     8398 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/meta/data_center.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    21399 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/meta/meta_create.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     4862 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/meta_importer.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:29:17.987325 gio_importer-1.0.9/importers/saas_export/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/saas_export/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     3303 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/saas_export/saas_meta.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     1179 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/saas_export.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      232 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/setup.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     1372 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/trigger_job.py
--rw-r--r--   0 chengcheng   (501) staff       (20)       95 2024-03-22 01:45:40.000000 gio_importer-1.0.9/importers/zk.py
--rw-r--r--   0 chengcheng   (501) staff       (20)       38 2024-04-02 06:29:17.988238 gio_importer-1.0.9/setup.cfg
--rw-r--r--   0 chengcheng   (501) staff       (20)     1251 2024-04-02 06:29:00.000000 gio_importer-1.0.9/setup.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:07:08.237298 gio_importer-1.1.0/
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1061 2024-04-03 08:02:43.000000 gio_importer-1.1.0/LICENSE
+-rw-r--r--   0 chengcheng   (501) staff       (20)       71 2024-04-03 08:02:43.000000 gio_importer-1.1.0/MANIFEST.in
+-rw-r--r--   0 chengcheng   (501) staff       (20)    12295 2024-04-03 08:07:08.236946 gio_importer-1.1.0/PKG-INFO
+-rw-r--r--   0 chengcheng   (501) staff       (20)      792 2024-04-03 08:02:43.000000 gio_importer-1.1.0/README.md
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:07:08.211344 gio_importer-1.1.0/gio_importer.egg-info/
+-rw-r--r--   0 chengcheng   (501) staff       (20)    12295 2024-04-03 08:07:08.000000 gio_importer-1.1.0/gio_importer.egg-info/PKG-INFO
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1381 2024-04-03 08:07:08.000000 gio_importer-1.1.0/gio_importer.egg-info/SOURCES.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)        1 2024-04-03 08:07:08.000000 gio_importer-1.1.0/gio_importer.egg-info/dependency_links.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)      196 2024-04-03 08:07:08.000000 gio_importer-1.1.0/gio_importer.egg-info/entry_points.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)       84 2024-04-03 08:07:08.000000 gio_importer-1.1.0/gio_importer.egg-info/requires.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)       10 2024-04-03 08:07:08.000000 gio_importer-1.1.0/gio_importer.egg-info/top_level.txt
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:07:08.221875 gio_importer-1.1.0/importers/
+-rw-r--r--   0 chengcheng   (501) staff       (20)    11711 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/README.md
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/__init__.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:07:08.223198 gio_importer-1.1.0/importers/clear_data/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/clear_data/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2820 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/clear_data/clear_data.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1714 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/clear_user.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:07:08.227524 gio_importer-1.1.0/importers/common/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/common/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     5581 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/common/common_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2620 2024-04-03 08:06:02.000000 gio_importer-1.1.0/importers/common/config_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2602 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/common/http_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)      955 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/common/log_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)      771 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/conf.cfg
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:07:08.231783 gio_importer-1.1.0/importers/data_import/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/data_import/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    21814 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/data_import/data_ads.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    21731 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/data_import/data_events.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    11251 2024-04-03 08:06:02.000000 gio_importer-1.1.0/importers/data_import/data_format_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    17799 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/data_import/data_item_variable.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     6455 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/data_import/data_model.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    15382 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/data_import/data_user_variable.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     6943 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/data_importer.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:07:08.233642 gio_importer-1.1.0/importers/db_import/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/db_import/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2717 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/db_import/database_import.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    14364 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/db_import/hive_import.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    14467 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/db_import/mysql_import.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:07:08.234122 gio_importer-1.1.0/importers/example/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/example/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     5144 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/format_importer.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)      472 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/log_conf.yaml
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:07:08.235664 gio_importer-1.1.0/importers/meta/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/meta/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    10656 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/meta/check_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     8398 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/meta/data_center.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    21399 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/meta/meta_create.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     4862 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/meta_importer.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:07:08.236491 gio_importer-1.1.0/importers/saas_export/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/saas_export/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     3303 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/saas_export/saas_meta.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1179 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/saas_export.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)      232 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/setup.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1372 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/trigger_job.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)       95 2024-04-03 08:02:43.000000 gio_importer-1.1.0/importers/zk.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)       38 2024-04-03 08:07:08.237351 gio_importer-1.1.0/setup.cfg
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1251 2024-04-03 08:06:33.000000 gio_importer-1.1.0/setup.py
```

### Comparing `gio_importer-1.0.9/LICENSE` & `gio_importer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/PKG-INFO` & `gio_importer-1.1.0/importers/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: gio_importer
-Version: 1.0.9
-Summary: GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具
-Home-page: UNKNOWN
-Author: gio
-Author-email: dev-growing@startdt.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # GrowingIO Importer
 
 GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具。
 
 ## 入门
 
 有关GrowingIO Importer请访问[GrowingIO官方文档](https://docs.growingio.com/op/developer-manual/toolbox/ )获取帮助。
@@ -404,9 +390,8 @@
     }
 
     clear_user.do_user(params)
 
 |参数|参数说明|
 |----|----|
 |-m|必填参数. 批量添加待删除用户-clear_users_meta|
-|-users|必填参数. 添加待删除用户,多个用户以逗号(,)分隔|
-
+|-users|必填参数. 添加待删除用户,多个用户以逗号(,)分隔|
```

### Comparing `gio_importer-1.0.9/README.md` & `gio_importer-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/gio_importer.egg-info/PKG-INFO` & `gio_importer-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 Metadata-Version: 2.1
-Name: gio-importer
-Version: 1.0.9
+Name: gio_importer
+Version: 1.1.0
 Summary: GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具
-Home-page: UNKNOWN
 Author: gio
 Author-email: dev-growing@startdt.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pip
+Requires-Dist: numpy
+Requires-Dist: requests
+Requires-Dist: pandas
+Requires-Dist: curlify
+Requires-Dist: PyYAML
+Requires-Dist: psycopg2-binary
+Requires-Dist: pymysql
+Requires-Dist: pyhive
+Requires-Dist: thrift
+Requires-Dist: sasl
 
 # GrowingIO Importer
 
 GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具。
 
 ## 入门
 
@@ -405,8 +413,7 @@
 
     clear_user.do_user(params)
 
 |参数|参数说明|
 |----|----|
 |-m|必填参数. 批量添加待删除用户-clear_users_meta|
 |-users|必填参数. 添加待删除用户,多个用户以逗号(,)分隔|
-
```

### Comparing `gio_importer-1.0.9/gio_importer.egg-info/SOURCES.txt` & `gio_importer-1.1.0/gio_importer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/README.md` & `gio_importer-1.1.0/gio_importer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: gio-importer
+Version: 1.1.0
+Summary: GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具
+Author: gio
+Author-email: dev-growing@startdt.com
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pip
+Requires-Dist: numpy
+Requires-Dist: requests
+Requires-Dist: pandas
+Requires-Dist: curlify
+Requires-Dist: PyYAML
+Requires-Dist: psycopg2-binary
+Requires-Dist: pymysql
+Requires-Dist: pyhive
+Requires-Dist: thrift
+Requires-Dist: sasl
+
 # GrowingIO Importer
 
 GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具。
 
 ## 入门
 
 有关GrowingIO Importer请访问[GrowingIO官方文档](https://docs.growingio.com/op/developer-manual/toolbox/ )获取帮助。
@@ -390,8 +412,8 @@
     }
 
     clear_user.do_user(params)
 
 |参数|参数说明|
 |----|----|
 |-m|必填参数. 批量添加待删除用户-clear_users_meta|
-|-users|必填参数. 添加待删除用户,多个用户以逗号(,)分隔|
+|-users|必填参数. 添加待删除用户,多个用户以逗号(,)分隔|
```

### Comparing `gio_importer-1.0.9/importers/clear_data/clear_data.py` & `gio_importer-1.1.0/importers/clear_data/clear_data.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/clear_user.py` & `gio_importer-1.1.0/importers/clear_user.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/common/common_util.py` & `gio_importer-1.1.0/importers/common/common_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/common/config_util.py` & `gio_importer-1.1.0/importers/common/config_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 
 class ApiConfig:
     """A ApiConfig Class"""
     oauth2_uri = config['API']['oauth2_uri']
     token = config['API']['token']
     project_id = config['API']['project_id']
 
+    @classmethod
+    def update_token(cls, new_token):
+        """Update token"""
+        cls.token = new_token
+
 
 class SSLConfig:
     """SSL证书校验"""
     verify = config['SSL']['verify']
 
 
 class BaseConfig:
```

### Comparing `gio_importer-1.0.9/importers/common/http_util.py` & `gio_importer-1.1.0/importers/common/http_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/common/log_util.py` & `gio_importer-1.1.0/importers/common/log_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/conf.cfg` & `gio_importer-1.1.0/importers/conf.cfg`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/data_import/data_ads.py` & `gio_importer-1.1.0/importers/data_import/data_ads.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/data_import/data_events.py` & `gio_importer-1.1.0/importers/data_import/data_events.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/data_import/data_format_util.py` & `gio_importer-1.1.0/importers/data_import/data_format_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import ftplib
 import json
 import csv
 import time
 
 from importers.common.common_util import time_format
-from importers.common.config_util import FTPConfig, BaseConfig
+from importers.common.config_util import FTPConfig, BaseConfig, ApiConfig
 
 from collections import Counter
 
 from importers.common.log_util import logger, my_logger
 from importers.data_import.data_model import DataEvent
 
 
@@ -311,7 +311,12 @@
     total_lines = 0
     for path in paths:
         with open(path, 'r') as file:
             lines = sum(1 for line in file)
         total_lines += lines
 
     return total_lines
+
+
+def portal_token(new_token):
+    """更新 token"""
+    ApiConfig.update_token(new_token)
```

### Comparing `gio_importer-1.0.9/importers/data_import/data_item_variable.py` & `gio_importer-1.1.0/importers/data_import/data_item_variable.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/data_import/data_model.py` & `gio_importer-1.1.0/importers/data_import/data_model.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/data_import/data_user_variable.py` & `gio_importer-1.1.0/importers/data_import/data_user_variable.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/data_importer.py` & `gio_importer-1.1.0/importers/data_importer.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/db_import/database_import.py` & `gio_importer-1.1.0/importers/db_import/database_import.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/db_import/hive_import.py` & `gio_importer-1.1.0/importers/db_import/hive_import.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/db_import/mysql_import.py` & `gio_importer-1.1.0/importers/db_import/mysql_import.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/format_importer.py` & `gio_importer-1.1.0/importers/format_importer.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/meta/check_util.py` & `gio_importer-1.1.0/importers/meta/check_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/meta/data_center.py` & `gio_importer-1.1.0/importers/meta/data_center.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/meta/meta_create.py` & `gio_importer-1.1.0/importers/meta/meta_create.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/meta_importer.py` & `gio_importer-1.1.0/importers/meta_importer.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/saas_export/saas_meta.py` & `gio_importer-1.1.0/importers/saas_export/saas_meta.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/saas_export.py` & `gio_importer-1.1.0/importers/saas_export.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/importers/trigger_job.py` & `gio_importer-1.1.0/importers/trigger_job.py`

 * *Files identical despite different names*

### Comparing `gio_importer-1.0.9/setup.py` & `gio_importer-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     'pyhive',
     'thrift',
     'sasl'
 ]
 
 setup(
     name='gio_importer',
-    version='1.0.9',
+    version='1.1.0',
     description='GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='gio',
     author_email='dev-growing@startdt.com',
     packages=find_packages(include=["importers*"]),
     include_package_data=True,
```

