# Comparing `tmp/django-geo-spaas-2.5.2.dev0.tar.gz` & `tmp/django-geo-spaas-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-geo-spaas-2.5.2.dev0.tar", last modified: Wed Feb 15 09:15:58 2023, max compression
+gzip compressed data, was "django-geo-spaas-2.5.3.tar", last modified: Wed Apr  3 14:31:20 2024, max compression
```

## Comparing `django-geo-spaas-2.5.2.dev0.tar` & `django-geo-spaas-2.5.3.tar`

### file list

```diff
@@ -1,113 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3981 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/django_geo_spaas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      805 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/django_geo_spaas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3416 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/django_geo_spaas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/django_geo_spaas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/django_geo_spaas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/django_geo_spaas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/geospaas/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/static/base_viewer/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/static/base_viewer/js/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/static/base_viewer/js/base_viewer.js
--rw-r--r--   0 runner    (1001) docker     (122)     8163 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/static/base_viewer/js/leaflet.ajax.min.js
--rw-r--r--   0 runner    (1001) docker     (122)      987 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/static/base_viewer/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/templates/base_viewer/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/templates/base_viewer/ds_info.html
--rw-r--r--   0 runner    (1001) docker     (122)     2339 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/templates/base_viewer/elements.html
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/templates/base_viewer/page_structure.html
--rw-r--r--   0 runner    (1001) docker     (122)    13856 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      273 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2964 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      512 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:57.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/management/commands/count.py
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     6164 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0002_auto_20160705_1331.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0003_dataset_entry_id.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0004_populate_entry_id_values.py
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0005_remove_entry_id_null.py
--rw-r--r--   0 runner    (1001) docker     (122)     1590 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0006_auto_20190130_1442.py
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0007_auto_20190626_1313.py
--rw-r--r--   0 runner    (1001) docker     (122)     1964 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0008_auto_20200331_0806.py
--rw-r--r--   0 runner    (1001) docker     (122)      721 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0009_auto_20201012_0905.py
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0010_auto_20201019_1331.py
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0011_auto_20210525_1252.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8325 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/models.py
--rw-r--r--   0 runner    (1001) docker     (122)    14836 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/catalog/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/geospaas/export_DIF/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/export_DIF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/export_DIF/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/geospaas/export_DIF/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/export_DIF/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/export_DIF/models.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/export_DIF/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/export_DIF/views.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2356 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/management/commands/ingest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/management/commands/ingest_hyrax.py
--rw-r--r--   0 runner    (1001) docker     (122)     3564 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/management/commands/ingest_thredds_crawl.py
--rw-r--r--   0 runner    (1001) docker     (122)     7319 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/models.py
--rw-r--r--   0 runner    (1001) docker     (122)    19850 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/geospaas/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6072 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/utils/processing_base_command.py
--rw-r--r--   0 runner    (1001) docker     (122)     2509 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2249 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/management/commands/update_vocabularies.py
--rw-r--r--   0 runner    (1001) docker     (122)     9660 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     5598 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/migrations/0002_auto_20190101_1128.py
--rw-r--r--   0 runner    (1001) docker     (122)      410 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/migrations/0003_auto_20190829_0847.py
--rw-r--r--   0 runner    (1001) docker     (122)     2701 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/migrations/0004_auto_20200331_0806.py
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/migrations/0005_auto_20210528_1139.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8466 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/models.py
--rw-r--r--   0 runner    (1001) docker     (122)    22836 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/views.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:58.000000 django-geo-spaas-2.5.2.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3703 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-02-15 09:15:56.000000 django-geo-spaas-2.5.2.dev0/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.315545 django-geo-spaas-2.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-03 14:31:20.315545 django-geo-spaas-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.307546 django-geo-spaas-2.5.3/django_geo_spaas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-03 14:31:20.000000 django-geo-spaas-2.5.3/django_geo_spaas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-03 14:31:20.000000 django-geo-spaas-2.5.3/django_geo_spaas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:31:20.000000 django-geo-spaas-2.5.3/django_geo_spaas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:31:20.000000 django-geo-spaas-2.5.3/django_geo_spaas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 14:31:20.000000 django-geo-spaas-2.5.3/django_geo_spaas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 14:31:20.000000 django-geo-spaas-2.5.3/django_geo_spaas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.307546 django-geo-spaas-2.5.3/geospaas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.307546 django-geo-spaas-2.5.3/geospaas/base_viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/base_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/base_viewer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/base_viewer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.303545 django-geo-spaas-2.5.3/geospaas/base_viewer/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.307546 django-geo-spaas-2.5.3/geospaas/base_viewer/static/base_viewer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.307546 django-geo-spaas-2.5.3/geospaas/base_viewer/static/base_viewer/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/base_viewer/static/base_viewer/js/base_viewer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/base_viewer/static/base_viewer/js/leaflet.ajax.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/base_viewer/static/base_viewer/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.303545 django-geo-spaas-2.5.3/geospaas/base_viewer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.307546 django-geo-spaas-2.5.3/geospaas/base_viewer/templates/base_viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/base_viewer/templates/base_viewer/ds_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/base_viewer/templates/base_viewer/elements.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/base_viewer/templates/base_viewer/page_structure.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/base_viewer/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/base_viewer/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/base_viewer/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.307546 django-geo-spaas-2.5.3/geospaas/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.307546 django-geo-spaas-2.5.3/geospaas/catalog/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.307546 django-geo-spaas-2.5.3/geospaas/catalog/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/management/commands/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.311545 django-geo-spaas-2.5.3/geospaas/catalog/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/migrations/0002_auto_20160705_1331.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/migrations/0003_dataset_entry_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/migrations/0004_populate_entry_id_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/migrations/0005_remove_entry_id_null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/migrations/0006_auto_20190130_1442.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/migrations/0007_auto_20190626_1313.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/migrations/0008_auto_20200331_0806.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/migrations/0009_auto_20201012_0905.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/migrations/0010_auto_20201019_1331.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/migrations/0011_auto_20210525_1252.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14836 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/catalog/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.311545 django-geo-spaas-2.5.3/geospaas/export_DIF/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/export_DIF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/export_DIF/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.311545 django-geo-spaas-2.5.3/geospaas/export_DIF/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/export_DIF/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/export_DIF/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/export_DIF/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/export_DIF/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.311545 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.311545 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.311545 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/management/commands/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/management/commands/ingest_hyrax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/management/commands/ingest_thredds_crawl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.315545 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19850 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/nansat_ingestor/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.315545 django-geo-spaas-2.5.3/geospaas/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/utils/processing_base_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.315545 django-geo-spaas-2.5.3/geospaas/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.315545 django-geo-spaas-2.5.3/geospaas/vocabularies/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.315545 django-geo-spaas-2.5.3/geospaas/vocabularies/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/management/commands/update_vocabularies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.315545 django-geo-spaas-2.5.3/geospaas/vocabularies/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/migrations/0002_auto_20190101_1128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/migrations/0003_auto_20190829_0847.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/migrations/0004_auto_20200331_0806.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/migrations/0005_auto_20210528_1139.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22836 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/geospaas/vocabularies/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:31:20.315545 django-geo-spaas-2.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:20.315545 django-geo-spaas-2.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 14:31:19.000000 django-geo-spaas-2.5.3/tests/urls.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-geo-spaas-2.5.2.dev0/django_geo_spaas.egg-info/SOURCES.txt` & `django-geo-spaas-2.5.3/django_geo_spaas.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 django_geo_spaas.egg-info/PKG-INFO
 django_geo_spaas.egg-info/SOURCES.txt
 django_geo_spaas.egg-info/dependency_links.txt
 django_geo_spaas.egg-info/not-zip-safe
+django_geo_spaas.egg-info/requires.txt
 django_geo_spaas.egg-info/top_level.txt
 geospaas/__init__.py
 geospaas/admin.py
 geospaas/models.py
 geospaas/tests.py
 geospaas/urls.py
 geospaas/base_viewer/__init__.py
```

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/forms.py` & `django-geo-spaas-2.5.3/geospaas/base_viewer/forms.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/static/base_viewer/js/base_viewer.js` & `django-geo-spaas-2.5.3/geospaas/base_viewer/static/base_viewer/js/base_viewer.js`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/static/base_viewer/js/leaflet.ajax.min.js` & `django-geo-spaas-2.5.3/geospaas/base_viewer/static/base_viewer/js/leaflet.ajax.min.js`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/static/base_viewer/styles.css` & `django-geo-spaas-2.5.3/geospaas/base_viewer/static/base_viewer/styles.css`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/templates/base_viewer/ds_info.html` & `django-geo-spaas-2.5.3/geospaas/base_viewer/templates/base_viewer/ds_info.html`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/templates/base_viewer/elements.html` & `django-geo-spaas-2.5.3/geospaas/base_viewer/templates/base_viewer/elements.html`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/templates/base_viewer/page_structure.html` & `django-geo-spaas-2.5.3/geospaas/base_viewer/templates/base_viewer/page_structure.html`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/tests.py` & `django-geo-spaas-2.5.3/geospaas/base_viewer/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         all_tds = soup.find_all("tr", class_="dataset_row")
         self.assertEqual(len(all_tds), 2)
         self.assertIn('file://localhost/some/test/file1.ext', all_tds[0].text)
         self.assertIn('file://localhost/some/test/file2.ext', all_tds[1].text)
 
     def test_post_without_polygon_public_version(self):
         """shall not reveal the uri of fixtures' datasets (presumably confidential) in the specified
-         placement of datasets inside the resulted HTML in the case of a POST request without
+        placement of datasets inside the resulted HTML in the case of a POST request without
         any polygon from user """
         res = self.client.post('/tests/', {
             'time_coverage_start': timezone.datetime(2000, 12, 29),
             'time_coverage_end': timezone.datetime(2020, 1, 1),
             'source': 1})
         self.assertEqual(res.status_code, 200)
         soup = BeautifulSoup(str(res.content), features="lxml")
```

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/base_viewer/views.py` & `django-geo-spaas-2.5.3/geospaas/base_viewer/views.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/admin.py` & `django-geo-spaas-2.5.3/geospaas/catalog/admin.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/managers.py` & `django-geo-spaas-2.5.3/geospaas/catalog/managers.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0001_initial.py` & `django-geo-spaas-2.5.3/geospaas/catalog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0002_auto_20160705_1331.py` & `django-geo-spaas-2.5.3/geospaas/catalog/migrations/0002_auto_20160705_1331.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0003_dataset_entry_id.py` & `django-geo-spaas-2.5.3/geospaas/catalog/migrations/0003_dataset_entry_id.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0004_populate_entry_id_values.py` & `django-geo-spaas-2.5.3/geospaas/catalog/migrations/0004_populate_entry_id_values.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0005_remove_entry_id_null.py` & `django-geo-spaas-2.5.3/geospaas/catalog/migrations/0005_remove_entry_id_null.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0006_auto_20190130_1442.py` & `django-geo-spaas-2.5.3/geospaas/catalog/migrations/0006_auto_20190130_1442.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0007_auto_20190626_1313.py` & `django-geo-spaas-2.5.3/geospaas/catalog/migrations/0007_auto_20190626_1313.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0008_auto_20200331_0806.py` & `django-geo-spaas-2.5.3/geospaas/catalog/migrations/0008_auto_20200331_0806.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0009_auto_20201012_0905.py` & `django-geo-spaas-2.5.3/geospaas/catalog/migrations/0009_auto_20201012_0905.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0010_auto_20201019_1331.py` & `django-geo-spaas-2.5.3/geospaas/catalog/migrations/0010_auto_20201019_1331.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/migrations/0011_auto_20210525_1252.py` & `django-geo-spaas-2.5.3/geospaas/catalog/migrations/0011_auto_20210525_1252.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/models.py` & `django-geo-spaas-2.5.3/geospaas/catalog/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,32 +102,32 @@
 
     For a full description of the DIF format, see
     http://gcmd.nasa.gov/add/difguide/index.html and
     http://gcmd.nasa.gov/add/difguide/WRITEADIF.pdf
 
     Fields:
     -------
-    entry_id : TextField
+    :entry_id: TextField.
         A unique dataset ID. Only alphanumeric characters are allowed.
-    entry_title : CharField
-    parameters: ManyToManyField to Parameter
-    ISO_topic_category : ForeignKey to ISOTopicCategory
-    data_center : ForeignKey to DataCenter
-    summary : TextField
+    :entry_title: CharField
+    :parameters: ManyToManyField to Parameter
+    :ISO_topic_category: ForeignKey to ISOTopicCategory
+    :data_center: ForeignKey to DataCenter
+    :summary: TextField.
         In addition to some general information, the summary should also
         contain information about the project from/for which the data was
         collected/created
-    source : ForeignKey to Source
+    :source: ForeignKey to Source
         Contains information about the instrument and platform by which the
         data was collected
-    time_coverage_start : DateTimeField
-    time_coverage_end : DateTimeField
-    geographic_location : ForeignKey to GeographicLocation
-    gcmd_location : ForeignKey to vocabularies.models.Location
-    access_constraints : CharField
+    :time_coverage_start: DateTimeField
+    :time_coverage_end: DateTimeField
+    :geographic_location: ForeignKey to GeographicLocation
+    :gcmd_location: ForeignKey to vocabularies.models.Location
+    :access_constraints: CharField.
         Determines the access level of the Dataset: Limited, In-house, or Public
     '''
     ACCESS_LEVEL0 = 'accessLevel0'
     ACCESS_LEVEL1 = 'accessLevel1'
     ACCESS_LEVEL2 = 'accessLevel2'
     ACCESS_CHOICES = (
             (ACCESS_LEVEL0, _('Limited')),
```

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/catalog/tests.py` & `django-geo-spaas-2.5.3/geospaas/catalog/tests.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/management/commands/ingest.py` & `django-geo-spaas-2.5.3/geospaas/nansat_ingestor/management/commands/ingest.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/management/commands/ingest_hyrax.py` & `django-geo-spaas-2.5.3/geospaas/nansat_ingestor/management/commands/ingest_hyrax.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import time
 import re
-import urllib2
+import urllib.error
+import urllib.request
 
 from django.core.management.base import BaseCommand, CommandError
 
 from geospaas.nansat_ingestor.management.commands.ingest import Command as IngestCommand
 
 # extend Ingest
 class Command(IngestCommand):
@@ -20,27 +21,27 @@
         super(Command, self).handle(*nc_uris, **options)
 
 def find_netcdf_uris(uri0, sleep=1.0):
     uri0_base = os.path.split(uri0)[0]
     print('Search in ', uri0_base)
     # get HTML from the URL
     time.sleep(sleep)
-    response = urllib2.urlopen(uri0)
+    response = urllib.request.urlopen(uri0)
     html = response.read()
 
     # find all links to netDCF
     nc_uris = [os.path.join(uri0_base, uri.replace('href="', '').replace('.nc.dds', '.nc'))
             for uri in re.findall('href=.*nc\.dds', html)]
 
     # find all links to sub-pages
     uris = [os.path.join(uri0_base, uri.replace('href="', ''))
             for uri in re.findall('href=.*/contents.html', html)]
     # get links to netcDF also from sub-pages
     try:
         for uri in uris:
             nc_uris += find_netcdf_uris(uri)
-    except (urllib2.HTTPError, urllib2.URLError) as e:
+    except (urllib.error.HTTPError, urllib.error.URLError) as e:
         print('Server error %s'%e.message)
     # return all links to netCDF
     return nc_uris
```

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/management/commands/ingest_thredds_crawl.py` & `django-geo-spaas-2.5.3/geospaas/nansat_ingestor/management/commands/ingest_thredds_crawl.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/managers.py` & `django-geo-spaas-2.5.3/geospaas/nansat_ingestor/managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,28 +24,28 @@
                       uri_filter_args=None,
                       uri_service_name=FILE_SERVICE_NAME,
                       uri_service_type=LOCAL_FILE_SERVICE,
                       *args, **kwargs):
         """ Create dataset and corresponding metadata
 
         Parameters:
-        ----------
+        -----------
             uri : str
                   URI to file or stream openable by Nansat
             n_points : int
                   Number of border points (default is 10)
             uri_filter_args : dict
                 Extra DatasetURI filter arguments if several datasets can refer to the same URI
             uri_service_name : str
                 name of the service which is used  ('dapService', 'fileService', 'http' or 'wms')
             uri_service_type : str
                 type of the service which is used  ('OPENDAP', 'local', 'HTTPServer' or 'WMS')
 
         Returns:
-        -------
+        --------
             dataset and flag
         """
         if not uri_filter_args:
             uri_filter_args = {}
 
         # Validate uri - this should raise an exception if the uri doesn't point to a valid
         # file or stream
```

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/migrations/0001_initial.py` & `django-geo-spaas-2.5.3/geospaas/nansat_ingestor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/nansat_ingestor/tests.py` & `django-geo-spaas-2.5.3/geospaas/nansat_ingestor/tests.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/tests.py` & `django-geo-spaas-2.5.3/geospaas/tests.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/utils/processing_base_command.py` & `django-geo-spaas-2.5.3/geospaas/utils/processing_base_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,30 +14,33 @@
     try:
         return dt.strptime(s, "%Y-%m-%d")
     except:# ValueError:
         raise CommandError("Not a valid date: '{0}'.".format(s))
 
 
 class ProcessingBaseCommand(BaseCommand):
-    """ Base class for geospaas-based processing commands for initial filtering on space and time.
+    """Base class for geospaas-based processing commands for initial filtering on space and time.
 
     Usage
     -----
-    from geospaas.utils import ProcessingBaseCommand
-    class SomeProcessingCommand(ProcessingBaseCommand):
-        args = '<filename filename ...>'
-        help = 'Run classification of texture features'
-
-        def handle(self, *args, **options):
-            # find input datasets
-            inp_datasets = self.find_datasets(**options)
+    .. code:: python
 
-            # continue to filter inp_datasets
-            # continue to process inp_datasets
+        from geospaas.utils import ProcessingBaseCommand
+        class SomeProcessingCommand(ProcessingBaseCommand):
+            args = '<filename filename ...>'
+            help = 'Run classification of texture features'
+
+            def handle(self, *args, **options):
+                # find input datasets
+                inp_datasets = self.find_datasets(**options)
+
+                # continue to filter inp_datasets
+                # continue to process inp_datasets
     """
+
     def add_arguments(self, parser):
         parser.add_argument('--start',
                             action='store',
                             metavar='YYYY-MM-DD',
                             default='1900-01-01',
                             help='Start of time range',)
                             #type=valid_date) # such validation doesn't work with Django ...
@@ -76,27 +79,27 @@
         parser.add_argument('--limit',
                             action='store',
                             default=None,
                             type=int,
                             help='Number of found datasets to process')
 
     def geometry_from_options(self, extent=None, geojson=None, **kwargs):
-        """ Generate geometry to use in spatial search
+        """Generate geometry to use in spatial search
 
         If extent is not None, return Polygon generated as POLYGON(()) with min/max lon/lat
         If geojson is not None, return Polygon loaded from the GeoJSON file
         Otherwise, return None
 
         Parameters
         ----------
         extent : [float, float, float, float]
             Values of min_lon, max_lon, min_lat, max_lat
         geojson : str
             Filename with Polygon GeoJSON
-        **kwargs : dict
+        \*\*kwargs : dict
             other options from input arguments
 
         Returns
         -------
         geometry : geos.Polygon or None
         """
         polygon = None
```

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/utils/utils.py` & `django-geo-spaas-2.5.3/geospaas/utils/utils.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/management/commands/update_vocabularies.py` & `django-geo-spaas-2.5.3/geospaas/vocabularies/management/commands/update_vocabularies.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/managers.py` & `django-geo-spaas-2.5.3/geospaas/vocabularies/managers.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/migrations/0001_initial.py` & `django-geo-spaas-2.5.3/geospaas/vocabularies/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/migrations/0002_auto_20190101_1128.py` & `django-geo-spaas-2.5.3/geospaas/vocabularies/migrations/0002_auto_20190101_1128.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/migrations/0004_auto_20200331_0806.py` & `django-geo-spaas-2.5.3/geospaas/vocabularies/migrations/0004_auto_20200331_0806.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/models.py` & `django-geo-spaas-2.5.3/geospaas/vocabularies/models.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/geospaas/vocabularies/tests.py` & `django-geo-spaas-2.5.3/geospaas/vocabularies/tests.py`

 * *Files identical despite different names*

### Comparing `django-geo-spaas-2.5.2.dev0/setup.py` & `django-geo-spaas-2.5.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,23 @@
 # Copyright:    (c) NERSC
 # License:
 #-------------------------------------------------------------------------------
 import os
 import sys
 from setuptools import setup, find_packages
 
-install_requires = []
+install_requires = [
+    'django-forms-bootstrap',
+    'django-leaflet',
+    'django<4',
+    'gdal',
+    'nansat',
+    'netCDF4',
+    'pythesint',
+]
 
 setup(
     name='django-geo-spaas',
     version=os.getenv('DJANGO_GEO_SPAAS_RELEASE', '0.0.0dev'),
     description='Geo-Scientific Platform as a Service',
     zip_safe=False,
     author='Morten W. Hansen, Anton Korosov, Artem Moiseev, Jeong-Won Park, Adrien Perrin, A.Azamifard',
```

### Comparing `django-geo-spaas-2.5.2.dev0/tests/settings.py` & `django-geo-spaas-2.5.3/tests/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 DATABASES = {
     'default': {
         'ENGINE': 'django.contrib.gis.db.backends.spatialite',
         'NAME': os.path.join(BASE_DIR, 'geodjango.db'),
     }
 }
 
+DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
 
 # Password validation
 # https://docs.djangoproject.com/en/1.11/ref/settings/#auth-password-validators
 
 AUTH_PASSWORD_VALIDATORS = [
     {
         'NAME': 'django.contrib.auth.password_validation.UserAttributeSimilarityValidator',
```

