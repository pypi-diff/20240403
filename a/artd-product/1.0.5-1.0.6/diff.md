# Comparing `tmp/artd-product-1.0.5.tar.gz` & `tmp/artd-product-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd-product-1.0.5.tar", last modified: Fri Mar 22 02:38:10 2024, max compression
+gzip compressed data, was "artd-product-1.0.6.tar", last modified: Wed Apr  3 17:32:48 2024, max compression
```

## Comparing `artd-product-1.0.5.tar` & `artd-product-1.0.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:38:10.006876 artd-product-1.0.5/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1495 2024-03-01 15:51:40.000000 artd-product-1.0.5/LICENSE
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      139 2024-03-04 15:35:35.000000 artd-product-1.0.5/MANIFEST.in
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1922 2024-03-22 02:38:10.006876 artd-product-1.0.5/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      823 2024-03-10 02:47:38.000000 artd-product-1.0.5/README.rst
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:38:10.006876 artd-product-1.0.5/artd_packages/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_packages/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_packages/asgi.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3627 2024-03-10 02:44:22.000000 artd-product-1.0.5/artd_packages/settings.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      831 2024-03-09 17:59:54.000000 artd-product-1.0.5/artd_packages/urls.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_packages/wsgi.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:38:10.006876 artd-product-1.0.5/artd_product/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    13932 2024-03-10 05:15:33.000000 artd-product-1.0.5/artd_product/admin.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      247 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/apps.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:38:10.006876 artd-product-1.0.5/artd_product/data/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/data/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       59 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/data/taxes.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:38:09.996876 artd-product-1.0.5/artd_product/locale/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:38:09.996876 artd-product-1.0.5/artd_product/locale/en/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:38:10.006876 artd-product-1.0.5/artd_product/locale/en/LC_MESSAGES/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    12265 2024-03-10 02:58:21.000000 artd-product-1.0.5/artd_product/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:38:10.006876 artd-product-1.0.5/artd_product/locale/es/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:38:10.006876 artd-product-1.0.5/artd_product/locale/es/LC_MESSAGES/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    14893 2024-03-10 03:06:17.000000 artd-product-1.0.5/artd_product/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:38:10.006876 artd-product-1.0.5/artd_product/management/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/management/__init__.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:38:10.006876 artd-product-1.0.5/artd_product/management/commands/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/management/commands/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      446 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/management/commands/create_taxes.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:38:10.006876 artd-product-1.0.5/artd_product/migrations/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    26224 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/migrations/0001_initial.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     7170 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/migrations/0002_brand_external_id_brand_json_data_brand_source_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      737 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/migrations/0003_alter_product_brand.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      602 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/migrations/0004_groupedproduct_variations.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      601 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/migrations/0005_product_variations.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1321 2024-03-04 06:08:47.000000 artd-product-1.0.5/artd_product/migrations/0006_alter_category_banner_image_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5701 2024-03-06 15:15:02.000000 artd-product-1.0.5/artd_product/migrations/0007_alter_brand_created_at_alter_brand_updated_at_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      758 2024-03-06 15:19:13.000000 artd-product-1.0.5/artd_product/migrations/0008_remove_productimage_alt_alter_productimage_image.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      790 2024-03-06 15:57:25.000000 artd-product-1.0.5/artd_product/migrations/0009_product_partner.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      764 2024-03-06 16:00:02.000000 artd-product-1.0.5/artd_product/migrations/0010_groupedproduct_partner.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      967 2024-03-09 02:12:48.000000 artd-product-1.0.5/artd_product/migrations/0011_category_secondary_mini_image_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      642 2024-03-09 18:17:51.000000 artd-product-1.0.5/artd_product/migrations/0012_rootcategory_secondary_mini_image.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      413 2024-03-09 18:28:17.000000 artd-product-1.0.5/artd_product/migrations/0013_rename_secondary_mini_image_category_secondary_mini_image.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/migrations/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    15177 2024-03-10 02:58:10.000000 artd-product-1.0.5/artd_product/models.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       60 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/tests.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:38:10.006876 artd-product-1.0.5/artd_product/utils/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/utils/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2784 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/utils/product_util.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       63 2024-03-01 15:51:40.000000 artd-product-1.0.5/artd_product/views.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:38:10.006876 artd-product-1.0.5/artd_product.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1922 2024-03-22 02:38:09.000000 artd-product-1.0.5/artd_product.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1716 2024-03-22 02:38:09.000000 artd-product-1.0.5/artd_product.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-03-22 02:38:09.000000 artd-product-1.0.5/artd_product.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      151 2024-03-22 02:38:09.000000 artd-product-1.0.5/artd_product.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       27 2024-03-22 02:38:09.000000 artd-product-1.0.5/artd_product.egg-info/top_level.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1193 2024-03-22 02:38:10.006876 artd-product-1.0.5/setup.cfg
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-03-01 15:51:40.000000 artd-product-1.0.5/setup.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:32:48.555789 artd-product-1.0.6/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1495 2024-03-01 15:51:40.000000 artd-product-1.0.6/LICENSE
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      139 2024-03-04 15:35:35.000000 artd-product-1.0.6/MANIFEST.in
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1922 2024-04-03 17:32:48.555789 artd-product-1.0.6/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      823 2024-03-10 02:47:38.000000 artd-product-1.0.6/README.rst
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:32:48.545789 artd-product-1.0.6/artd_packages/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_packages/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_packages/asgi.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3627 2024-03-10 02:44:22.000000 artd-product-1.0.6/artd_packages/settings.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      831 2024-03-09 17:59:54.000000 artd-product-1.0.6/artd_packages/urls.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_packages/wsgi.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:32:48.545789 artd-product-1.0.6/artd_product/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    14129 2024-04-03 17:31:59.000000 artd-product-1.0.6/artd_product/admin.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      247 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/apps.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:32:48.545789 artd-product-1.0.6/artd_product/data/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/data/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       59 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/data/taxes.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:32:48.545789 artd-product-1.0.6/artd_product/locale/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:32:48.545789 artd-product-1.0.6/artd_product/locale/en/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:32:48.545789 artd-product-1.0.6/artd_product/locale/en/LC_MESSAGES/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    12265 2024-03-10 02:58:21.000000 artd-product-1.0.6/artd_product/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:32:48.545789 artd-product-1.0.6/artd_product/locale/es/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:32:48.555789 artd-product-1.0.6/artd_product/locale/es/LC_MESSAGES/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    14893 2024-03-10 03:06:17.000000 artd-product-1.0.6/artd_product/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:32:48.555789 artd-product-1.0.6/artd_product/management/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/management/__init__.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:32:48.555789 artd-product-1.0.6/artd_product/management/commands/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/management/commands/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      446 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/management/commands/create_taxes.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:32:48.555789 artd-product-1.0.6/artd_product/migrations/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    26224 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/migrations/0001_initial.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     7170 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/migrations/0002_brand_external_id_brand_json_data_brand_source_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      737 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/migrations/0003_alter_product_brand.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      602 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/migrations/0004_groupedproduct_variations.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      601 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/migrations/0005_product_variations.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1321 2024-03-04 06:08:47.000000 artd-product-1.0.6/artd_product/migrations/0006_alter_category_banner_image_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5701 2024-03-06 15:15:02.000000 artd-product-1.0.6/artd_product/migrations/0007_alter_brand_created_at_alter_brand_updated_at_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      758 2024-03-06 15:19:13.000000 artd-product-1.0.6/artd_product/migrations/0008_remove_productimage_alt_alter_productimage_image.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      790 2024-03-06 15:57:25.000000 artd-product-1.0.6/artd_product/migrations/0009_product_partner.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      764 2024-03-06 16:00:02.000000 artd-product-1.0.6/artd_product/migrations/0010_groupedproduct_partner.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      967 2024-03-09 02:12:48.000000 artd-product-1.0.6/artd_product/migrations/0011_category_secondary_mini_image_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      642 2024-03-09 18:17:51.000000 artd-product-1.0.6/artd_product/migrations/0012_rootcategory_secondary_mini_image.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      413 2024-03-09 18:28:17.000000 artd-product-1.0.6/artd_product/migrations/0013_rename_secondary_mini_image_category_secondary_mini_image.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/migrations/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    15651 2024-04-03 17:04:55.000000 artd-product-1.0.6/artd_product/models.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       60 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/tests.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:32:48.555789 artd-product-1.0.6/artd_product/utils/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/utils/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2784 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/utils/product_util.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       63 2024-03-01 15:51:40.000000 artd-product-1.0.6/artd_product/views.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:32:48.545789 artd-product-1.0.6/artd_product.egg-info/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1922 2024-04-03 17:32:48.000000 artd-product-1.0.6/artd_product.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1716 2024-04-03 17:32:48.000000 artd-product-1.0.6/artd_product.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-04-03 17:32:48.000000 artd-product-1.0.6/artd_product.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      151 2024-04-03 17:32:48.000000 artd-product-1.0.6/artd_product.egg-info/requires.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       27 2024-04-03 17:32:48.000000 artd-product-1.0.6/artd_product.egg-info/top_level.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1193 2024-04-03 17:32:48.555789 artd-product-1.0.6/setup.cfg
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-03-01 15:51:40.000000 artd-product-1.0.6/setup.py
```

### Comparing `artd-product-1.0.5/LICENSE` & `artd-product-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/PKG-INFO` & `artd-product-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-product
-Version: 1.0.5
+Version: 1.0.6
 Summary: ArtD Product.
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola
 Author-email: jonathan@artd.com.co
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `artd-product-1.0.5/README.rst` & `artd-product-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_packages/settings.py` & `artd-product-1.0.6/artd_packages/settings.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_packages/urls.py` & `artd-product-1.0.6/artd_packages/urls.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/admin.py` & `artd-product-1.0.6/artd_product/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,21 +252,23 @@
 
 @admin.register(Category)
 class CategoryAdmin(admin.ModelAdmin):
     list_display = (
         "name",
         "id",
         "partner",
+        "root_category",
         "parent",
         "status",
     )
     list_filter = ("status",)
     search_fields = (
         "name",
         "parent__name",
+        "root_category__name",
         "status",
         "url_key",
         "meta_title",
         "meta_description",
         "meta_keywords",
     )
     readonly_fields = [
@@ -344,31 +346,36 @@
     }
 
 
 @admin.register(Product)
 class ProductAdmin(admin.ModelAdmin):
     list_display = (
         "name",
+        "grouped_product_name",
         "sku",
+        "grouped_product_sku",
         "brand",
         "status",
     )
     list_filter = (
         "name",
         "brand",
         "status",
     )
     search_fields = (
         "name",
         "brand__name",
         "status",
+        "sku",
         "url_key",
         "meta_title",
         "meta_description",
         "meta_keywords",
+        "groupedproduct__name",
+        "groupedproduct__sku",
     )
     readonly_fields = [
         "created_at",
         "updated_at",
     ]
 
     fieldsets = (
```

### Comparing `artd-product-1.0.5/artd_product/locale/en/LC_MESSAGES/django.po` & `artd-product-1.0.6/artd_product/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/locale/es/LC_MESSAGES/django.po` & `artd-product-1.0.6/artd_product/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/migrations/0001_initial.py` & `artd-product-1.0.6/artd_product/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/migrations/0002_brand_external_id_brand_json_data_brand_source_and_more.py` & `artd-product-1.0.6/artd_product/migrations/0002_brand_external_id_brand_json_data_brand_source_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/migrations/0003_alter_product_brand.py` & `artd-product-1.0.6/artd_product/migrations/0003_alter_product_brand.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/migrations/0004_groupedproduct_variations.py` & `artd-product-1.0.6/artd_product/migrations/0004_groupedproduct_variations.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/migrations/0005_product_variations.py` & `artd-product-1.0.6/artd_product/migrations/0005_product_variations.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/migrations/0006_alter_category_banner_image_and_more.py` & `artd-product-1.0.6/artd_product/migrations/0006_alter_category_banner_image_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/migrations/0007_alter_brand_created_at_alter_brand_updated_at_and_more.py` & `artd-product-1.0.6/artd_product/migrations/0007_alter_brand_created_at_alter_brand_updated_at_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/migrations/0008_remove_productimage_alt_alter_productimage_image.py` & `artd-product-1.0.6/artd_product/migrations/0008_remove_productimage_alt_alter_productimage_image.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/migrations/0009_product_partner.py` & `artd-product-1.0.6/artd_product/migrations/0009_product_partner.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/migrations/0010_groupedproduct_partner.py` & `artd-product-1.0.6/artd_product/migrations/0010_groupedproduct_partner.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/migrations/0011_category_secondary_mini_image_and_more.py` & `artd-product-1.0.6/artd_product/migrations/0011_category_secondary_mini_image_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/migrations/0012_rootcategory_secondary_mini_image.py` & `artd-product-1.0.6/artd_product/migrations/0012_rootcategory_secondary_mini_image.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product/models.py` & `artd-product-1.0.6/artd_product/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -472,14 +472,29 @@
         _("Variations"),
         help_text=_("Enter the variations of the grouped product"),
         null=True,
         blank=True,
         default=dict,
     )
 
+    @property
+    def grouped_product_name(self):
+        grouped_product: GroupedProduct = self.groupedproduct_set.last()
+        return grouped_product.name
+
+    @property
+    def grouped_product_sku(self):
+        grouped_product: GroupedProduct = self.groupedproduct_set.last()
+        return grouped_product.sku
+
+    @property
+    def grouped_product_id(self):
+        grouped_product: GroupedProduct = self.groupedproduct_set.last()
+        return grouped_product.id
+
     class Meta:
         """Meta definition for Product."""
 
         verbose_name = _("Product")
         verbose_name_plural = _("Products")
 
     def __str__(self):
```

### Comparing `artd-product-1.0.5/artd_product/utils/product_util.py` & `artd-product-1.0.6/artd_product/utils/product_util.py`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/artd_product.egg-info/PKG-INFO` & `artd-product-1.0.6/artd_product.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-product
-Version: 1.0.5
+Version: 1.0.6
 Summary: ArtD Product.
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola
 Author-email: jonathan@artd.com.co
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `artd-product-1.0.5/artd_product.egg-info/SOURCES.txt` & `artd-product-1.0.6/artd_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artd-product-1.0.5/setup.cfg` & `artd-product-1.0.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = artd-product
-version = 1.0.5
+version = 1.0.6
 long_description_content_type = text/markdown
 description = ArtD Product.
 long_description = file: README.rst
 url = https://www.artd.com.co/
 author = Jonathan Urzola
 author_email = jonathan@artd.com.co
 license = BSD-3-Clause
```

