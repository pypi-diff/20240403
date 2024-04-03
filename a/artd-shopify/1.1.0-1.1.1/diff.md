# Comparing `tmp/artd-shopify-1.1.0.tar.gz` & `tmp/artd-shopify-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd-shopify-1.1.0.tar", last modified: Wed Mar 27 07:15:56 2024, max compression
+gzip compressed data, was "artd-shopify-1.1.1.tar", last modified: Wed Apr  3 17:48:05 2024, max compression
```

## Comparing `artd-shopify-1.1.0.tar` & `artd-shopify-1.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-27 07:15:56.714533 artd-shopify-1.1.0/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1495 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/LICENSE
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      138 2024-03-06 17:20:48.000000 artd-shopify-1.1.0/MANIFEST.in
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2286 2024-03-27 07:15:56.714533 artd-shopify-1.1.0/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1187 2024-03-06 21:00:51.000000 artd-shopify-1.1.0/README.rst
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-27 07:15:56.714533 artd-shopify-1.1.0/artd_package/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_package/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      401 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_package/asgi.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3949 2024-03-10 19:25:04.000000 artd-shopify-1.1.0/artd_package/settings.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1132 2024-03-10 19:25:44.000000 artd-shopify-1.1.0/artd_package/urls.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      401 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_package/wsgi.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-27 07:15:56.714533 artd-shopify-1.1.0/artd_shopify/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_shopify/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     8624 2024-03-27 02:17:47.000000 artd-shopify-1.1.0/artd_shopify/admin.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      247 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_shopify/apps.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      952 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_shopify/forms.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-27 07:15:56.704533 artd-shopify-1.1.0/artd_shopify/locale/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-27 07:15:56.704533 artd-shopify-1.1.0/artd_shopify/locale/en/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-27 07:15:56.714533 artd-shopify-1.1.0/artd_shopify/locale/en/LC_MESSAGES/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      425 2024-03-06 17:19:26.000000 artd-shopify-1.1.0/artd_shopify/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5183 2024-03-06 17:12:25.000000 artd-shopify-1.1.0/artd_shopify/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-27 07:15:56.704533 artd-shopify-1.1.0/artd_shopify/locale/es/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-27 07:15:56.714533 artd-shopify-1.1.0/artd_shopify/locale/es/LC_MESSAGES/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3810 2024-03-06 17:19:26.000000 artd-shopify-1.1.0/artd_shopify/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     6341 2024-03-06 17:19:18.000000 artd-shopify-1.1.0/artd_shopify/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-27 07:15:56.714533 artd-shopify-1.1.0/artd_shopify/management/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_shopify/management/__init__.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-27 07:15:56.714533 artd-shopify-1.1.0/artd_shopify/management/commands/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_shopify/management/commands/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      950 2024-03-27 02:30:26.000000 artd-shopify-1.1.0/artd_shopify/management/commands/convert_tags_to_categories.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1060 2024-03-26 23:12:43.000000 artd-shopify-1.1.0/artd_shopify/management/commands/import_shopify_product.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      920 2024-03-27 02:30:23.000000 artd-shopify-1.1.0/artd_shopify/management/commands/import_shopify_tags.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      929 2024-03-27 07:04:40.000000 artd-shopify-1.1.0/artd_shopify/management/commands/update_categories_for_all_products.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-27 07:15:56.714533 artd-shopify-1.1.0/artd_shopify/migrations/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    21297 2024-03-06 13:52:49.000000 artd-shopify-1.1.0/artd_shopify/migrations/0001_initial.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3028 2024-03-26 22:56:24.000000 artd-shopify-1.1.0/artd_shopify/migrations/0002_shopifytag.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2523 2024-03-27 01:47:25.000000 artd-shopify-1.1.0/artd_shopify/migrations/0003_shopifyroottag.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      979 2024-03-27 01:54:45.000000 artd-shopify-1.1.0/artd_shopify/migrations/0004_rename_partner_shopifyroottag_artd_partner_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    19937 2024-03-27 02:15:09.000000 artd-shopify-1.1.0/artd_shopify/migrations/0005_remove_shopifyroottag_category_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_shopify/migrations/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    10833 2024-03-27 02:15:01.000000 artd-shopify-1.1.0/artd_shopify/models.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       60 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_shopify/tests.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-27 07:15:56.714533 artd-shopify-1.1.0/artd_shopify/utils/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_shopify/utils/__init__.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-27 07:15:56.714533 artd-shopify-1.1.0/artd_shopify/utils/graphql/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_shopify/utils/graphql/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      499 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_shopify/utils/graphql/queries.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    22857 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_shopify/utils/shopify.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    36360 2024-03-27 06:59:35.000000 artd-shopify-1.1.0/artd_shopify/utils/shopify_graphql.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      254 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/artd_shopify/views.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-27 07:15:56.714533 artd-shopify-1.1.0/artd_shopify.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2286 2024-03-27 07:15:56.000000 artd-shopify-1.1.0/artd_shopify.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1506 2024-03-27 07:15:56.000000 artd-shopify-1.1.0/artd_shopify.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-03-27 07:15:56.000000 artd-shopify-1.1.0/artd_shopify.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      155 2024-03-27 07:15:56.000000 artd-shopify-1.1.0/artd_shopify.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       26 2024-03-27 07:15:56.000000 artd-shopify-1.1.0/artd_shopify.egg-info/top_level.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1198 2024-03-27 07:15:56.714533 artd-shopify-1.1.0/setup.cfg
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-03-06 13:48:57.000000 artd-shopify-1.1.0/setup.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:48:05.865475 artd-shopify-1.1.1/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1495 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/LICENSE
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      138 2024-03-06 17:20:48.000000 artd-shopify-1.1.1/MANIFEST.in
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2286 2024-04-03 17:48:05.865475 artd-shopify-1.1.1/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1187 2024-03-06 21:00:51.000000 artd-shopify-1.1.1/README.rst
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:48:05.855475 artd-shopify-1.1.1/artd_package/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_package/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      401 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_package/asgi.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3949 2024-03-10 19:25:04.000000 artd-shopify-1.1.1/artd_package/settings.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1132 2024-03-10 19:25:44.000000 artd-shopify-1.1.1/artd_package/urls.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      401 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_package/wsgi.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:48:05.855475 artd-shopify-1.1.1/artd_shopify/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_shopify/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     8624 2024-03-27 02:17:47.000000 artd-shopify-1.1.1/artd_shopify/admin.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      247 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_shopify/apps.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      952 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_shopify/forms.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:48:05.855475 artd-shopify-1.1.1/artd_shopify/locale/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:48:05.855475 artd-shopify-1.1.1/artd_shopify/locale/en/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:48:05.855475 artd-shopify-1.1.1/artd_shopify/locale/en/LC_MESSAGES/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      425 2024-03-06 17:19:26.000000 artd-shopify-1.1.1/artd_shopify/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5183 2024-03-06 17:12:25.000000 artd-shopify-1.1.1/artd_shopify/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:48:05.855475 artd-shopify-1.1.1/artd_shopify/locale/es/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:48:05.855475 artd-shopify-1.1.1/artd_shopify/locale/es/LC_MESSAGES/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3810 2024-03-06 17:19:26.000000 artd-shopify-1.1.1/artd_shopify/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     6341 2024-03-06 17:19:18.000000 artd-shopify-1.1.1/artd_shopify/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:48:05.855475 artd-shopify-1.1.1/artd_shopify/management/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_shopify/management/__init__.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:48:05.865475 artd-shopify-1.1.1/artd_shopify/management/commands/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_shopify/management/commands/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      950 2024-03-27 02:30:26.000000 artd-shopify-1.1.1/artd_shopify/management/commands/convert_tags_to_categories.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1059 2024-04-03 17:45:52.000000 artd-shopify-1.1.1/artd_shopify/management/commands/import_shopify_product.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      920 2024-03-27 02:30:23.000000 artd-shopify-1.1.1/artd_shopify/management/commands/import_shopify_tags.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      929 2024-03-27 07:04:40.000000 artd-shopify-1.1.1/artd_shopify/management/commands/update_categories_for_all_products.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:48:05.865475 artd-shopify-1.1.1/artd_shopify/migrations/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    21297 2024-03-06 13:52:49.000000 artd-shopify-1.1.1/artd_shopify/migrations/0001_initial.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3028 2024-03-26 22:56:24.000000 artd-shopify-1.1.1/artd_shopify/migrations/0002_shopifytag.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2523 2024-03-27 01:47:25.000000 artd-shopify-1.1.1/artd_shopify/migrations/0003_shopifyroottag.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      979 2024-03-27 01:54:45.000000 artd-shopify-1.1.1/artd_shopify/migrations/0004_rename_partner_shopifyroottag_artd_partner_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    19937 2024-03-27 02:15:09.000000 artd-shopify-1.1.1/artd_shopify/migrations/0005_remove_shopifyroottag_category_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_shopify/migrations/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    10833 2024-03-27 02:15:01.000000 artd-shopify-1.1.1/artd_shopify/models.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       60 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_shopify/tests.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:48:05.865475 artd-shopify-1.1.1/artd_shopify/utils/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_shopify/utils/__init__.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:48:05.865475 artd-shopify-1.1.1/artd_shopify/utils/graphql/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_shopify/utils/graphql/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      499 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_shopify/utils/graphql/queries.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    22857 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_shopify/utils/shopify.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    36360 2024-03-27 06:59:35.000000 artd-shopify-1.1.1/artd_shopify/utils/shopify_graphql.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      254 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/artd_shopify/views.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:48:05.855475 artd-shopify-1.1.1/artd_shopify.egg-info/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2286 2024-04-03 17:48:05.000000 artd-shopify-1.1.1/artd_shopify.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1506 2024-04-03 17:48:05.000000 artd-shopify-1.1.1/artd_shopify.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-04-03 17:48:05.000000 artd-shopify-1.1.1/artd_shopify.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      155 2024-04-03 17:48:05.000000 artd-shopify-1.1.1/artd_shopify.egg-info/requires.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       26 2024-04-03 17:48:05.000000 artd-shopify-1.1.1/artd_shopify.egg-info/top_level.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1198 2024-04-03 17:48:05.865475 artd-shopify-1.1.1/setup.cfg
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-03-06 13:48:57.000000 artd-shopify-1.1.1/setup.py
```

### Comparing `artd-shopify-1.1.0/LICENSE` & `artd-shopify-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/PKG-INFO` & `artd-shopify-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-shopify
-Version: 1.1.0
+Version: 1.1.1
 Summary: ArtD Shopify.
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola
 Author-email: jonathan@artd.com.co
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `artd-shopify-1.1.0/README.rst` & `artd-shopify-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_package/settings.py` & `artd-shopify-1.1.1/artd_package/settings.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_package/urls.py` & `artd-shopify-1.1.1/artd_package/urls.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/admin.py` & `artd-shopify-1.1.1/artd_shopify/admin.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/forms.py` & `artd-shopify-1.1.1/artd_shopify/forms.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/locale/en/LC_MESSAGES/django.po` & `artd-shopify-1.1.1/artd_shopify/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/locale/es/LC_MESSAGES/django.mo` & `artd-shopify-1.1.1/artd_shopify/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/locale/es/LC_MESSAGES/django.po` & `artd-shopify-1.1.1/artd_shopify/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/management/commands/convert_tags_to_categories.py` & `artd-shopify-1.1.1/artd_shopify/management/commands/convert_tags_to_categories.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/management/commands/import_shopify_product.py` & `artd-shopify-1.1.1/artd_shopify/management/commands/import_shopify_product.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
         # Define aquí los parámetros del comando
         parser.add_argument("partner_slug", type=str, help="Partner slug")
 
     def handle(self, *args, **kwargs):
         partner_slug = kwargs["partner_slug"]
         print(partner_slug)
         try:
-
             partner = Partner.objects.filter(
                 partner_slug=partner_slug,
             ).first()
             print(partner)
             sgq = ShopifyGraphQl(partner)
             sgq.store_products_from_shopify()
             sgq.store_categories()
```

### Comparing `artd-shopify-1.1.0/artd_shopify/management/commands/import_shopify_tags.py` & `artd-shopify-1.1.1/artd_shopify/management/commands/import_shopify_tags.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/management/commands/update_categories_for_all_products.py` & `artd-shopify-1.1.1/artd_shopify/management/commands/update_categories_for_all_products.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/migrations/0001_initial.py` & `artd-shopify-1.1.1/artd_shopify/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/migrations/0002_shopifytag.py` & `artd-shopify-1.1.1/artd_shopify/migrations/0002_shopifytag.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/migrations/0003_shopifyroottag.py` & `artd-shopify-1.1.1/artd_shopify/migrations/0003_shopifyroottag.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/migrations/0004_rename_partner_shopifyroottag_artd_partner_and_more.py` & `artd-shopify-1.1.1/artd_shopify/migrations/0004_rename_partner_shopifyroottag_artd_partner_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/migrations/0005_remove_shopifyroottag_category_and_more.py` & `artd-shopify-1.1.1/artd_shopify/migrations/0005_remove_shopifyroottag_category_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/models.py` & `artd-shopify-1.1.1/artd_shopify/models.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/utils/shopify.py` & `artd-shopify-1.1.1/artd_shopify/utils/shopify.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify/utils/shopify_graphql.py` & `artd-shopify-1.1.1/artd_shopify/utils/shopify_graphql.py`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/artd_shopify.egg-info/PKG-INFO` & `artd-shopify-1.1.1/artd_shopify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-shopify
-Version: 1.1.0
+Version: 1.1.1
 Summary: ArtD Shopify.
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola
 Author-email: jonathan@artd.com.co
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `artd-shopify-1.1.0/artd_shopify.egg-info/SOURCES.txt` & `artd-shopify-1.1.1/artd_shopify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artd-shopify-1.1.0/setup.cfg` & `artd-shopify-1.1.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = artd-shopify
-version = 1.1.0
+version = 1.1.1
 long_description_content_type = text/markdown
 description = ArtD Shopify.
 long_description = file: README.rst
 url = https://www.artd.com.co/
 author = Jonathan Urzola
 author_email = jonathan@artd.com.co
 license = BSD-3-Clause
@@ -32,15 +32,15 @@
 packages = find:
 install_requires = 
 	Django>=4.2
 	django-json-widget==1.1.1
 	pillow==10.2.0
 	artd-location==1.0.2
 	artd-partner==1.0.1
-	artd-product==1.0.5
-	artd_price_list==1.0.2
-	artd-stock==1.0.2
+	artd-product==1.0.6
+	artd_price_list==1.0.3
+	artd-stock==1.0.3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

