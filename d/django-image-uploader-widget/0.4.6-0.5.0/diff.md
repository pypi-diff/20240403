# Comparing `tmp/django-image-uploader-widget-0.4.6.tar.gz` & `tmp/django-image-uploader-widget-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-image-uploader-widget-0.4.6.tar", last modified: Fri Mar 29 16:58:09 2024, max compression
+gzip compressed data, was "django-image-uploader-widget-0.5.0.tar", last modified: Wed Apr  3 11:48:48 2024, max compression
```

## Comparing `django-image-uploader-widget-0.4.6.tar` & `django-image-uploader-widget-0.5.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.716506 django-image-uploader-widget-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-03-29 16:58:09.716506 django-image-uploader-widget-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.712506 django-image-uploader-widget-0.4.6/django_image_uploader_widget.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-03-29 16:58:09.000000 django-image-uploader-widget-0.4.6/django_image_uploader_widget.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-29 16:58:09.000000 django-image-uploader-widget-0.4.6/django_image_uploader_widget.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:58:09.000000 django-image-uploader-widget-0.4.6/django_image_uploader_widget.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:58:09.000000 django-image-uploader-widget-0.4.6/django_image_uploader_widget.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-29 16:58:09.000000 django-image-uploader-widget-0.4.6/django_image_uploader_widget.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-29 16:58:09.000000 django-image-uploader-widget-0.4.6/django_image_uploader_widget.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.708506 django-image-uploader-widget-0.4.6/image_uploader_widget/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.704506 django-image-uploader-widget-0.4.6/image_uploader_widget/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.704506 django-image-uploader-widget-0.4.6/image_uploader_widget/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.708506 django-image-uploader-widget-0.4.6/image_uploader_widget/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.704506 django-image-uploader-widget-0.4.6/image_uploader_widget/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.712506 django-image-uploader-widget-0.4.6/image_uploader_widget/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.704506 django-image-uploader-widget-0.4.6/image_uploader_widget/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.712506 django-image-uploader-widget-0.4.6/image_uploader_widget/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.712506 django-image-uploader-widget-0.4.6/image_uploader_widget/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/postgres/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/postgres/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/postgres/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.704506 django-image-uploader-widget-0.4.6/image_uploader_widget/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.708506 django-image-uploader-widget-0.4.6/image_uploader_widget/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.712506 django-image-uploader-widget-0.4.6/image_uploader_widget/static/admin/css/
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/static/admin/css/image-uploader-inline.css
--rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/static/admin/css/image-uploader-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.712506 django-image-uploader-widget-0.4.6/image_uploader_widget/static/admin/js/
--rw-r--r--   0 runner    (1001) docker     (127)    20595 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/static/admin/js/image-uploader-inline.js
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/static/admin/js/image-uploader-modal.js
--rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/static/admin/js/image-uploader-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.708506 django-image-uploader-widget-0.4.6/image_uploader_widget/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.708506 django-image-uploader-widget-0.4.6/image_uploader_widget/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.712506 django-image-uploader-widget-0.4.6/image_uploader_widget/templates/admin/edit_inline/
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/templates/admin/edit_inline/image_uploader.html
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/templates/admin/edit_inline/ordered_image_uploader.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.712506 django-image-uploader-widget-0.4.6/image_uploader_widget/templates/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/templates/admin/widgets/image_uploader_widget.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.708506 django-image-uploader-widget-0.4.6/image_uploader_widget/templates/postgres/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:58:09.712506 django-image-uploader-widget-0.4.6/image_uploader_widget/templates/postgres/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/templates/postgres/widgets/image_array.html
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/image_uploader_widget/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-29 16:58:04.000000 django-image-uploader-widget-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 16:58:09.716506 django-image-uploader-widget-0.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.929618 django-image-uploader-widget-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-04-03 11:48:48.929618 django-image-uploader-widget-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.929618 django-image-uploader-widget-0.5.0/django_image_uploader_widget.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-04-03 11:48:48.000000 django-image-uploader-widget-0.5.0/django_image_uploader_widget.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-03 11:48:48.000000 django-image-uploader-widget-0.5.0/django_image_uploader_widget.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:48:48.000000 django-image-uploader-widget-0.5.0/django_image_uploader_widget.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:48:48.000000 django-image-uploader-widget-0.5.0/django_image_uploader_widget.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 11:48:48.000000 django-image-uploader-widget-0.5.0/django_image_uploader_widget.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 11:48:48.000000 django-image-uploader-widget-0.5.0/django_image_uploader_widget.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.925618 django-image-uploader-widget-0.5.0/image_uploader_widget/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.921618 django-image-uploader-widget-0.5.0/image_uploader_widget/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.921618 django-image-uploader-widget-0.5.0/image_uploader_widget/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.925618 django-image-uploader-widget-0.5.0/image_uploader_widget/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.921618 django-image-uploader-widget-0.5.0/image_uploader_widget/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.925618 django-image-uploader-widget-0.5.0/image_uploader_widget/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.921618 django-image-uploader-widget-0.5.0/image_uploader_widget/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.925618 django-image-uploader-widget-0.5.0/image_uploader_widget/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.925618 django-image-uploader-widget-0.5.0/image_uploader_widget/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/postgres/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/postgres/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/postgres/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.921618 django-image-uploader-widget-0.5.0/image_uploader_widget/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.921618 django-image-uploader-widget-0.5.0/image_uploader_widget/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.925618 django-image-uploader-widget-0.5.0/image_uploader_widget/static/admin/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/static/admin/css/image-uploader-inline.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8111 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/static/admin/css/image-uploader-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.925618 django-image-uploader-widget-0.5.0/image_uploader_widget/static/admin/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    20595 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/static/admin/js/image-uploader-inline.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/static/admin/js/image-uploader-modal.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/static/admin/js/image-uploader-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.921618 django-image-uploader-widget-0.5.0/image_uploader_widget/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.921618 django-image-uploader-widget-0.5.0/image_uploader_widget/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.925618 django-image-uploader-widget-0.5.0/image_uploader_widget/templates/admin/edit_inline/
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/templates/admin/edit_inline/image_uploader.html
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/templates/admin/edit_inline/ordered_image_uploader.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.925618 django-image-uploader-widget-0.5.0/image_uploader_widget/templates/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/templates/admin/widgets/image_uploader_widget.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.921618 django-image-uploader-widget-0.5.0/image_uploader_widget/templates/postgres/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:48:48.929618 django-image-uploader-widget-0.5.0/image_uploader_widget/templates/postgres/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/templates/postgres/widgets/image_array.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/image_uploader_widget/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-03 11:48:44.000000 django-image-uploader-widget-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:48:48.929618 django-image-uploader-widget-0.5.0/setup.cfg
```

### Comparing `django-image-uploader-widget-0.4.6/LICENSE` & `django-image-uploader-widget-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/django_image_uploader_widget.egg-info/SOURCES.txt` & `django-image-uploader-widget-0.5.0/django_image_uploader_widget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/admin.py` & `django-image-uploader-widget-0.5.0/image_uploader_widget/admin.py`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/locale/es/LC_MESSAGES/django.mo` & `django-image-uploader-widget-0.5.0/image_uploader_widget/locale/es/LC_MESSAGES/django.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,15 +1,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: image_uploader_widget\n"
 "Report-Msgid-Bugs-To: \n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: es\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Add image"
 msgstr "Añadir imagen"
 
 msgid "Drop your image here or click to select one..."
 msgstr "Suelta tu imagen aquí o haz clic para seleccionar una..."
@@ -18,7 +18,10 @@
 msgstr "Suelta tu imagen aquí..."
 
 msgid "Drop your images here or click to select..."
 msgstr "Suelte sus imágenes aquí o haga clic para seleccionar..."
 
 msgid "Drop your images here..."
 msgstr "Suelte sus imagenes aquí..."
+
+msgid "Item %(name)s in the array did not validate:"
+msgstr "El elemento %(nth)s del arreglo no se pudo validar:"
```

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.mo` & `django-image-uploader-widget-0.5.0/image_uploader_widget/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,15 +1,15 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: image_uploader_widget\n"
 "Report-Msgid-Bugs-To: \n"
+"Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: pt_BR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "Add image"
 msgstr "Adicionar Imagem"
 
 msgid "Drop your image here or click to select one..."
 msgstr "Solte sua imagem aqui ou clique para selecionar uma..."
@@ -18,7 +18,10 @@
 msgstr "Solte sua imagem aqui..."
 
 msgid "Drop your images here or click to select..."
 msgstr "Solte suas imagens aqui ou clique para selecionar..."
 
 msgid "Drop your images here..."
 msgstr "Solte suas imagens aqui..."
+
+msgid "Item %(name)s in the array did not validate:"
+msgstr "O item %(name)s na matriz não validou:"
```

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/postgres/fields.py` & `django-image-uploader-widget-0.5.0/image_uploader_widget/postgres/fields.py`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/postgres/forms.py` & `django-image-uploader-widget-0.5.0/image_uploader_widget/postgres/forms.py`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/postgres/widget.py` & `django-image-uploader-widget-0.5.0/image_uploader_widget/postgres/widget.py`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/static/admin/css/image-uploader-inline.css` & `django-image-uploader-widget-0.5.0/image_uploader_widget/static/admin/css/image-uploader-inline.css`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/static/admin/css/image-uploader-widget.css` & `django-image-uploader-widget-0.5.0/image_uploader_widget/static/admin/css/image-uploader-widget.css`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/static/admin/js/image-uploader-inline.js` & `django-image-uploader-widget-0.5.0/image_uploader_widget/static/admin/js/image-uploader-inline.js`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/static/admin/js/image-uploader-modal.js` & `django-image-uploader-widget-0.5.0/image_uploader_widget/static/admin/js/image-uploader-modal.js`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/static/admin/js/image-uploader-widget.js` & `django-image-uploader-widget-0.5.0/image_uploader_widget/static/admin/js/image-uploader-widget.js`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/templates/admin/edit_inline/image_uploader.html` & `django-image-uploader-widget-0.5.0/image_uploader_widget/templates/admin/edit_inline/image_uploader.html`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/templates/admin/widgets/image_uploader_widget.html` & `django-image-uploader-widget-0.5.0/image_uploader_widget/templates/admin/widgets/image_uploader_widget.html`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/templates/postgres/widgets/image_array.html` & `django-image-uploader-widget-0.5.0/image_uploader_widget/templates/postgres/widgets/image_array.html`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/image_uploader_widget/widgets.py` & `django-image-uploader-widget-0.5.0/image_uploader_widget/widgets.py`

 * *Files identical despite different names*

### Comparing `django-image-uploader-widget-0.4.6/pyproject.toml` & `django-image-uploader-widget-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 requires-python = ">= 3.8"
 name = 'django-image-uploader-widget'
-version = '0.4.6'
+version = '0.5.0'
 description='Simple Image Uploader Widget for Django-Admin'
 dependencies = [
   'django>=3.2',
   'Pillow',
 ]
 authors = [{name = "Eduardo Oliveira", email = "eduardo_y05@outlook.com"}]
 maintainers = [{name = "Eduardo Oliveira", email = "eduardo_y05@outlook.com"}]
@@ -26,15 +26,16 @@
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
   'Programming Language :: Python :: 3.12',
 ]
 
 [project.optional-dependencies]
 dev = ["black", "isort", "pre-commit"]
-test = ["playwright"]
+test = ["playwright", "tiny-match-snapshot"]
+docs = ["mkdocs", "mkdocs-material", "mkdocs-glightbox", "mkdocs-awesome-pages-plugin"]
 
 [project.urls]
 homepage = "https://github.com/inventare/django-image-uploader-widget"
 documentation = "https://inventare.github.io/django-image-uploader-widget/"
 
 [build-system]
 requires = ["setuptools", "build"]
```

