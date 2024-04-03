# Comparing `tmp/artd_price_list-1.0.2.tar.gz` & `tmp/artd_price_list-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd_price_list-1.0.2.tar", last modified: Fri Mar 22 02:41:33 2024, max compression
+gzip compressed data, was "artd_price_list-1.0.3.tar", last modified: Wed Apr  3 17:35:13 2024, max compression
```

## Comparing `artd_price_list-1.0.2.tar` & `artd_price_list-1.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:41:33.916849 artd_price_list-1.0.2/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1495 2024-03-01 15:54:55.000000 artd_price_list-1.0.2/LICENSE
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      144 2024-03-04 15:56:17.000000 artd_price_list-1.0.2/MANIFEST.in
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1909 2024-03-22 02:41:33.916849 artd_price_list-1.0.2/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      804 2024-03-04 12:11:08.000000 artd_price_list-1.0.2/README.rst
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:41:33.916849 artd_price_list-1.0.2/artd_packages/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:54:55.000000 artd_price_list-1.0.2/artd_packages/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:54:55.000000 artd_price_list-1.0.2/artd_packages/asgi.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3651 2024-03-10 02:48:36.000000 artd_price_list-1.0.2/artd_packages/settings.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      831 2024-03-10 02:45:39.000000 artd_price_list-1.0.2/artd_packages/urls.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:54:55.000000 artd_price_list-1.0.2/artd_packages/wsgi.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:41:33.916849 artd_price_list-1.0.2/artd_price_list/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:54:55.000000 artd_price_list-1.0.2/artd_price_list/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3523 2024-03-10 03:54:25.000000 artd_price_list-1.0.2/artd_price_list/admin.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      255 2024-03-04 12:10:44.000000 artd_price_list-1.0.2/artd_price_list/apps.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1084 2024-03-10 04:33:32.000000 artd_price_list-1.0.2/artd_price_list/forms.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:41:33.916849 artd_price_list-1.0.2/artd_price_list/locale/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:41:33.916849 artd_price_list-1.0.2/artd_price_list/locale/en/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:41:33.916849 artd_price_list-1.0.2/artd_price_list/locale/en/LC_MESSAGES/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2810 2024-03-10 03:58:08.000000 artd_price_list-1.0.2/artd_price_list/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:41:33.916849 artd_price_list-1.0.2/artd_price_list/locale/es/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:41:33.916849 artd_price_list-1.0.2/artd_price_list/locale/es/LC_MESSAGES/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3273 2024-03-10 03:58:08.000000 artd_price_list-1.0.2/artd_price_list/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:41:33.916849 artd_price_list-1.0.2/artd_price_list/migrations/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     6891 2024-03-01 15:54:55.000000 artd_price_list-1.0.2/artd_price_list/migrations/0001_initial.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1367 2024-03-01 15:54:55.000000 artd_price_list-1.0.2/artd_price_list/migrations/0002_pricelist_external_id_pricelist_source_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1922 2024-03-10 03:57:58.000000 artd_price_list-1.0.2/artd_price_list/migrations/0003_alter_pricelist_partner_alter_pricelist_product_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:54:55.000000 artd_price_list-1.0.2/artd_price_list/migrations/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3651 2024-03-10 03:57:11.000000 artd_price_list-1.0.2/artd_price_list/models.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       60 2024-03-01 15:54:55.000000 artd_price_list-1.0.2/artd_price_list/tests.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:41:33.916849 artd_price_list-1.0.2/artd_price_list/utils/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:54:55.000000 artd_price_list-1.0.2/artd_price_list/utils/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1801 2024-03-01 15:54:55.000000 artd_price_list-1.0.2/artd_price_list/utils/generators.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       63 2024-03-01 15:54:55.000000 artd_price_list-1.0.2/artd_price_list/views.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:41:33.916849 artd_price_list-1.0.2/artd_price_list.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1909 2024-03-22 02:41:33.000000 artd_price_list-1.0.2/artd_price_list.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      962 2024-03-22 02:41:33.000000 artd_price_list-1.0.2/artd_price_list.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-03-22 02:41:33.000000 artd_price_list-1.0.2/artd_price_list.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      137 2024-03-22 02:41:33.000000 artd_price_list-1.0.2/artd_price_list.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       30 2024-03-22 02:41:33.000000 artd_price_list-1.0.2/artd_price_list.egg-info/top_level.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1185 2024-03-22 02:41:33.916849 artd_price_list-1.0.2/setup.cfg
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-03-01 15:54:55.000000 artd_price_list-1.0.2/setup.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:35:13.715740 artd_price_list-1.0.3/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1495 2024-03-01 15:54:55.000000 artd_price_list-1.0.3/LICENSE
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      144 2024-03-04 15:56:17.000000 artd_price_list-1.0.3/MANIFEST.in
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1909 2024-04-03 17:35:13.715740 artd_price_list-1.0.3/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      804 2024-03-04 12:11:08.000000 artd_price_list-1.0.3/README.rst
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:35:13.705740 artd_price_list-1.0.3/artd_packages/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:54:55.000000 artd_price_list-1.0.3/artd_packages/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:54:55.000000 artd_price_list-1.0.3/artd_packages/asgi.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3651 2024-03-10 02:48:36.000000 artd_price_list-1.0.3/artd_packages/settings.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      831 2024-03-10 02:45:39.000000 artd_price_list-1.0.3/artd_packages/urls.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      403 2024-03-01 15:54:55.000000 artd_price_list-1.0.3/artd_packages/wsgi.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:35:13.705740 artd_price_list-1.0.3/artd_price_list/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:54:55.000000 artd_price_list-1.0.3/artd_price_list/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3523 2024-03-10 03:54:25.000000 artd_price_list-1.0.3/artd_price_list/admin.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      255 2024-03-04 12:10:44.000000 artd_price_list-1.0.3/artd_price_list/apps.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1084 2024-03-10 04:33:32.000000 artd_price_list-1.0.3/artd_price_list/forms.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:35:13.705740 artd_price_list-1.0.3/artd_price_list/locale/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:35:13.705740 artd_price_list-1.0.3/artd_price_list/locale/en/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:35:13.705740 artd_price_list-1.0.3/artd_price_list/locale/en/LC_MESSAGES/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2810 2024-03-10 03:58:08.000000 artd_price_list-1.0.3/artd_price_list/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:35:13.705740 artd_price_list-1.0.3/artd_price_list/locale/es/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:35:13.715740 artd_price_list-1.0.3/artd_price_list/locale/es/LC_MESSAGES/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3273 2024-03-10 03:58:08.000000 artd_price_list-1.0.3/artd_price_list/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:35:13.715740 artd_price_list-1.0.3/artd_price_list/migrations/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     6891 2024-03-01 15:54:55.000000 artd_price_list-1.0.3/artd_price_list/migrations/0001_initial.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1367 2024-03-01 15:54:55.000000 artd_price_list-1.0.3/artd_price_list/migrations/0002_pricelist_external_id_pricelist_source_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1922 2024-03-10 03:57:58.000000 artd_price_list-1.0.3/artd_price_list/migrations/0003_alter_pricelist_partner_alter_pricelist_product_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:54:55.000000 artd_price_list-1.0.3/artd_price_list/migrations/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3651 2024-03-10 03:57:11.000000 artd_price_list-1.0.3/artd_price_list/models.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       60 2024-03-01 15:54:55.000000 artd_price_list-1.0.3/artd_price_list/tests.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:35:13.715740 artd_price_list-1.0.3/artd_price_list/utils/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-01 15:54:55.000000 artd_price_list-1.0.3/artd_price_list/utils/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1801 2024-03-01 15:54:55.000000 artd_price_list-1.0.3/artd_price_list/utils/generators.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       63 2024-03-01 15:54:55.000000 artd_price_list-1.0.3/artd_price_list/views.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:35:13.705740 artd_price_list-1.0.3/artd_price_list.egg-info/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1909 2024-04-03 17:35:13.000000 artd_price_list-1.0.3/artd_price_list.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      962 2024-04-03 17:35:13.000000 artd_price_list-1.0.3/artd_price_list.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-04-03 17:35:13.000000 artd_price_list-1.0.3/artd_price_list.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      137 2024-04-03 17:35:13.000000 artd_price_list-1.0.3/artd_price_list.egg-info/requires.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       30 2024-04-03 17:35:13.000000 artd_price_list-1.0.3/artd_price_list.egg-info/top_level.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1185 2024-04-03 17:35:13.715740 artd_price_list-1.0.3/setup.cfg
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-03-01 15:54:55.000000 artd_price_list-1.0.3/setup.py
```

### Comparing `artd_price_list-1.0.2/LICENSE` & `artd_price_list-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `artd_price_list-1.0.2/PKG-INFO` & `artd_price_list-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd_price_list
-Version: 1.0.2
+Version: 1.0.3
 Summary: ArtD Price List.
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola
 Author-email: jonathan@artd.com.co
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `artd_price_list-1.0.2/README.rst` & `artd_price_list-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `artd_price_list-1.0.2/artd_packages/settings.py` & `artd_price_list-1.0.3/artd_packages/settings.py`

 * *Files identical despite different names*

### Comparing `artd_price_list-1.0.2/artd_packages/urls.py` & `artd_price_list-1.0.3/artd_packages/urls.py`

 * *Files identical despite different names*

### Comparing `artd_price_list-1.0.2/artd_price_list/admin.py` & `artd_price_list-1.0.3/artd_price_list/admin.py`

 * *Files identical despite different names*

### Comparing `artd_price_list-1.0.2/artd_price_list/forms.py` & `artd_price_list-1.0.3/artd_price_list/forms.py`

 * *Files identical despite different names*

### Comparing `artd_price_list-1.0.2/artd_price_list/locale/en/LC_MESSAGES/django.po` & `artd_price_list-1.0.3/artd_price_list/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `artd_price_list-1.0.2/artd_price_list/locale/es/LC_MESSAGES/django.po` & `artd_price_list-1.0.3/artd_price_list/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `artd_price_list-1.0.2/artd_price_list/migrations/0001_initial.py` & `artd_price_list-1.0.3/artd_price_list/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd_price_list-1.0.2/artd_price_list/migrations/0002_pricelist_external_id_pricelist_source_and_more.py` & `artd_price_list-1.0.3/artd_price_list/migrations/0002_pricelist_external_id_pricelist_source_and_more.py`

 * *Files identical despite different names*

### Comparing `artd_price_list-1.0.2/artd_price_list/migrations/0003_alter_pricelist_partner_alter_pricelist_product_and_more.py` & `artd_price_list-1.0.3/artd_price_list/migrations/0003_alter_pricelist_partner_alter_pricelist_product_and_more.py`

 * *Files identical despite different names*

### Comparing `artd_price_list-1.0.2/artd_price_list/models.py` & `artd_price_list-1.0.3/artd_price_list/models.py`

 * *Files identical despite different names*

### Comparing `artd_price_list-1.0.2/artd_price_list/utils/generators.py` & `artd_price_list-1.0.3/artd_price_list/utils/generators.py`

 * *Files identical despite different names*

### Comparing `artd_price_list-1.0.2/artd_price_list.egg-info/PKG-INFO` & `artd_price_list-1.0.3/artd_price_list.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-price-list
-Version: 1.0.2
+Version: 1.0.3
 Summary: ArtD Price List.
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola
 Author-email: jonathan@artd.com.co
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `artd_price_list-1.0.2/artd_price_list.egg-info/SOURCES.txt` & `artd_price_list-1.0.3/artd_price_list.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artd_price_list-1.0.2/setup.cfg` & `artd_price_list-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = artd_price_list
-version = 1.0.2
+version = 1.0.3
 long_description_content_type = text/markdown
 description = ArtD Price List.
 long_description = file: README.rst
 url = https://www.artd.com.co/
 author = Jonathan Urzola
 author_email = jonathan@artd.com.co
 license = BSD-3-Clause
@@ -33,13 +33,13 @@
 install_requires = 
 	Django>=4.2.10
 	django-admin==2.0.2
 	django-json-widget==1.1.1
 	pillow==10.2.0
 	artd-location==1.0.2
 	artd-partner==1.0.1
-	artd-product==1.0.5
+	artd-product==1.0.6
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

