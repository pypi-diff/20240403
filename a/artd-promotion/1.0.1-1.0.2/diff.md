# Comparing `tmp/artd_promotion-1.0.1.tar.gz` & `tmp/artd_promotion-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd_promotion-1.0.1.tar", last modified: Fri Mar 22 02:46:45 2024, max compression
+gzip compressed data, was "artd_promotion-1.0.2.tar", last modified: Wed Apr  3 17:37:38 2024, max compression
```

## Comparing `artd_promotion-1.0.1.tar` & `artd_promotion-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:46:45.416809 artd_promotion-1.0.1/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1495 2024-03-04 12:30:15.000000 artd_promotion-1.0.1/LICENSE
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      142 2024-03-04 16:13:27.000000 artd_promotion-1.0.1/MANIFEST.in
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1876 2024-03-22 02:46:45.416809 artd_promotion-1.0.1/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      773 2024-03-10 04:21:53.000000 artd_promotion-1.0.1/README.rst
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:46:45.416809 artd_promotion-1.0.1/artd/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-04 12:19:42.000000 artd_promotion-1.0.1/artd/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      385 2024-03-04 12:19:42.000000 artd_promotion-1.0.1/artd/asgi.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3645 2024-03-10 04:11:55.000000 artd_promotion-1.0.1/artd/settings.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      822 2024-03-10 04:20:26.000000 artd_promotion-1.0.1/artd/urls.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      385 2024-03-04 12:19:42.000000 artd_promotion-1.0.1/artd/wsgi.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:46:45.416809 artd_promotion-1.0.1/artd_promotion/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-04 12:22:25.000000 artd_promotion-1.0.1/artd_promotion/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     4386 2024-03-10 05:19:34.000000 artd_promotion-1.0.1/artd_promotion/admin.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      253 2024-03-04 12:23:44.000000 artd_promotion-1.0.1/artd_promotion/apps.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1673 2024-03-10 04:41:16.000000 artd_promotion-1.0.1/artd_promotion/forms.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:46:45.416809 artd_promotion-1.0.1/artd_promotion/locale/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:46:45.416809 artd_promotion-1.0.1/artd_promotion/locale/en/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:46:45.416809 artd_promotion-1.0.1/artd_promotion/locale/en/LC_MESSAGES/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     4188 2024-03-10 05:21:01.000000 artd_promotion-1.0.1/artd_promotion/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:46:45.416809 artd_promotion-1.0.1/artd_promotion/locale/es/
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:46:45.416809 artd_promotion-1.0.1/artd_promotion/locale/es/LC_MESSAGES/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5748 2024-03-10 05:27:02.000000 artd_promotion-1.0.1/artd_promotion/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:46:45.416809 artd_promotion-1.0.1/artd_promotion/migrations/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5229 2024-03-04 12:23:11.000000 artd_promotion-1.0.1/artd_promotion/migrations/0001_initial.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1365 2024-03-04 12:23:11.000000 artd_promotion-1.0.1/artd_promotion/migrations/0002_promotionrule_created_at_promotionrule_status_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1925 2024-03-04 12:23:11.000000 artd_promotion-1.0.1/artd_promotion/migrations/0003_alter_coupon_options_alter_promotionrule_options_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1447 2024-03-04 12:23:11.000000 artd_promotion-1.0.1/artd_promotion/migrations/0004_coupon_external_id_coupon_source_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1355 2024-03-04 16:22:25.000000 artd_promotion-1.0.1/artd_promotion/migrations/0005_alter_promotionrule_categories_and_more.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-04 12:23:11.000000 artd_promotion-1.0.1/artd_promotion/migrations/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3104 2024-03-10 04:39:31.000000 artd_promotion-1.0.1/artd_promotion/models.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-03-22 02:46:45.416809 artd_promotion-1.0.1/artd_promotion.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1876 2024-03-22 02:46:45.000000 artd_promotion-1.0.1/artd_promotion.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      939 2024-03-22 02:46:45.000000 artd_promotion-1.0.1/artd_promotion.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-03-22 02:46:45.000000 artd_promotion-1.0.1/artd_promotion.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      158 2024-03-22 02:46:45.000000 artd_promotion-1.0.1/artd_promotion.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       20 2024-03-22 02:46:45.000000 artd_promotion-1.0.1/artd_promotion.egg-info/top_level.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1205 2024-03-22 02:46:45.416809 artd_promotion-1.0.1/setup.cfg
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-03-04 12:53:23.000000 artd_promotion-1.0.1/setup.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:37:38.805692 artd_promotion-1.0.2/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1495 2024-03-04 12:30:15.000000 artd_promotion-1.0.2/LICENSE
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      142 2024-03-04 16:13:27.000000 artd_promotion-1.0.2/MANIFEST.in
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1876 2024-04-03 17:37:38.805692 artd_promotion-1.0.2/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      773 2024-03-10 04:21:53.000000 artd_promotion-1.0.2/README.rst
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:37:38.805692 artd_promotion-1.0.2/artd/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-04 12:19:42.000000 artd_promotion-1.0.2/artd/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      385 2024-03-04 12:19:42.000000 artd_promotion-1.0.2/artd/asgi.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3645 2024-03-10 04:11:55.000000 artd_promotion-1.0.2/artd/settings.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      822 2024-03-10 04:20:26.000000 artd_promotion-1.0.2/artd/urls.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      385 2024-03-04 12:19:42.000000 artd_promotion-1.0.2/artd/wsgi.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:37:38.805692 artd_promotion-1.0.2/artd_promotion/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-04 12:22:25.000000 artd_promotion-1.0.2/artd_promotion/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     4386 2024-03-10 05:19:34.000000 artd_promotion-1.0.2/artd_promotion/admin.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      253 2024-03-04 12:23:44.000000 artd_promotion-1.0.2/artd_promotion/apps.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1673 2024-03-10 04:41:16.000000 artd_promotion-1.0.2/artd_promotion/forms.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:37:38.805692 artd_promotion-1.0.2/artd_promotion/locale/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:37:38.795692 artd_promotion-1.0.2/artd_promotion/locale/en/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:37:38.805692 artd_promotion-1.0.2/artd_promotion/locale/en/LC_MESSAGES/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     4188 2024-03-10 05:21:01.000000 artd_promotion-1.0.2/artd_promotion/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:37:38.805692 artd_promotion-1.0.2/artd_promotion/locale/es/
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:37:38.805692 artd_promotion-1.0.2/artd_promotion/locale/es/LC_MESSAGES/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5748 2024-03-10 05:27:02.000000 artd_promotion-1.0.2/artd_promotion/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:37:38.805692 artd_promotion-1.0.2/artd_promotion/migrations/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     5229 2024-03-04 12:23:11.000000 artd_promotion-1.0.2/artd_promotion/migrations/0001_initial.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1365 2024-03-04 12:23:11.000000 artd_promotion-1.0.2/artd_promotion/migrations/0002_promotionrule_created_at_promotionrule_status_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1925 2024-03-04 12:23:11.000000 artd_promotion-1.0.2/artd_promotion/migrations/0003_alter_coupon_options_alter_promotionrule_options_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1447 2024-03-04 12:23:11.000000 artd_promotion-1.0.2/artd_promotion/migrations/0004_coupon_external_id_coupon_source_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1355 2024-03-04 16:22:25.000000 artd_promotion-1.0.2/artd_promotion/migrations/0005_alter_promotionrule_categories_and_more.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        0 2024-03-04 12:23:11.000000 artd_promotion-1.0.2/artd_promotion/migrations/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     3104 2024-03-10 04:39:31.000000 artd_promotion-1.0.2/artd_promotion/models.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2024-04-03 17:37:38.805692 artd_promotion-1.0.2/artd_promotion.egg-info/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1876 2024-04-03 17:37:38.000000 artd_promotion-1.0.2/artd_promotion.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      939 2024-04-03 17:37:38.000000 artd_promotion-1.0.2/artd_promotion.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2024-04-03 17:37:38.000000 artd_promotion-1.0.2/artd_promotion.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      158 2024-04-03 17:37:38.000000 artd_promotion-1.0.2/artd_promotion.egg-info/requires.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       20 2024-04-03 17:37:38.000000 artd_promotion-1.0.2/artd_promotion.egg-info/top_level.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1205 2024-04-03 17:37:38.805692 artd_promotion-1.0.2/setup.cfg
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2024-03-04 12:53:23.000000 artd_promotion-1.0.2/setup.py
```

### Comparing `artd_promotion-1.0.1/LICENSE` & `artd_promotion-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/PKG-INFO` & `artd_promotion-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd_promotion
-Version: 1.0.1
+Version: 1.0.2
 Summary: ArtD Promotion.
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola
 Author-email: jonathan@artd.com.co
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `artd_promotion-1.0.1/README.rst` & `artd_promotion-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/artd/settings.py` & `artd_promotion-1.0.2/artd/settings.py`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/artd/urls.py` & `artd_promotion-1.0.2/artd/urls.py`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/artd_promotion/admin.py` & `artd_promotion-1.0.2/artd_promotion/admin.py`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/artd_promotion/forms.py` & `artd_promotion-1.0.2/artd_promotion/forms.py`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/artd_promotion/locale/en/LC_MESSAGES/django.po` & `artd_promotion-1.0.2/artd_promotion/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/artd_promotion/locale/es/LC_MESSAGES/django.po` & `artd_promotion-1.0.2/artd_promotion/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/artd_promotion/migrations/0001_initial.py` & `artd_promotion-1.0.2/artd_promotion/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/artd_promotion/migrations/0002_promotionrule_created_at_promotionrule_status_and_more.py` & `artd_promotion-1.0.2/artd_promotion/migrations/0002_promotionrule_created_at_promotionrule_status_and_more.py`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/artd_promotion/migrations/0003_alter_coupon_options_alter_promotionrule_options_and_more.py` & `artd_promotion-1.0.2/artd_promotion/migrations/0003_alter_coupon_options_alter_promotionrule_options_and_more.py`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/artd_promotion/migrations/0004_coupon_external_id_coupon_source_and_more.py` & `artd_promotion-1.0.2/artd_promotion/migrations/0004_coupon_external_id_coupon_source_and_more.py`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/artd_promotion/migrations/0005_alter_promotionrule_categories_and_more.py` & `artd_promotion-1.0.2/artd_promotion/migrations/0005_alter_promotionrule_categories_and_more.py`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/artd_promotion/models.py` & `artd_promotion-1.0.2/artd_promotion/models.py`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/artd_promotion.egg-info/PKG-INFO` & `artd_promotion-1.0.2/artd_promotion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-promotion
-Version: 1.0.1
+Version: 1.0.2
 Summary: ArtD Promotion.
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola
 Author-email: jonathan@artd.com.co
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `artd_promotion-1.0.1/artd_promotion.egg-info/SOURCES.txt` & `artd_promotion-1.0.2/artd_promotion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artd_promotion-1.0.1/setup.cfg` & `artd_promotion-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = artd_promotion
-version = 1.0.1
+version = 1.0.2
 long_description_content_type = text/markdown
 description = ArtD Promotion.
 long_description = file: README.rst
 url = https://www.artd.com.co/
 author = Jonathan Urzola
 author_email = jonathan@artd.com.co
 license = BSD-3-Clause
@@ -34,13 +34,13 @@
 	Django>=4.2.10
 	django-admin==2.0.2
 	django-json-widget==1.1.1
 	pillow==10.2.0
 	artd-location==1.0.2
 	artd-partner==1.0.1
 	artd-customer==1.0.1
-	artd-product==1.0.5
+	artd-product==1.0.6
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

