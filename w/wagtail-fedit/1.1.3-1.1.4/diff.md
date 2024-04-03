# Comparing `tmp/wagtail_fedit-1.1.3.tar.gz` & `tmp/wagtail_fedit-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.1.3.tar", last modified: Wed Apr  3 13:02:39 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.1.4.tar", last modified: Wed Apr  3 13:09:01 2024, max compression
```

## Comparing `wagtail_fedit-1.1.3.tar` & `wagtail_fedit-1.1.4.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.512817 wagtail_fedit-1.1.3/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5493 2024-04-03 13:02:39.512817 wagtail_fedit-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.1.3/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-03 13:02:39.523156 wagtail_fedit-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.338351 wagtail_fedit-1.1.3/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.340321 wagtail_fedit-1.1.3/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.341325 wagtail_fedit-1.1.3/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.341325 wagtail_fedit-1.1.3/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.346138 wagtail_fedit-1.1.3/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.361471 wagtail_fedit-1.1.3/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.3/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.3/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.3/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.399508 wagtail_fedit-1.1.3/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.1.3/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.1.3/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.1.3/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.1.3/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.400509 wagtail_fedit-1.1.3/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.3/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.400509 wagtail_fedit-1.1.3/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.3/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.328518 wagtail_fedit-1.1.3/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.328518 wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.405815 wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.425205 wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    10561 2024-04-02 19:44:50.000000 wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.329519 wagtail_fedit-1.1.3/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.330813 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.427588 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.429658 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.436208 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
--rw-rw-rw-   0        0        0     1959 2024-04-02 19:17:17.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.439589 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-02 20:15:18.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
--rw-rw-rw-   0        0        0      845 2024-04-02 20:15:27.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.451779 wagtail_fedit-1.1.3/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.1.3/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.454218 wagtail_fedit-1.1.3/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16682 2024-04-03 13:00:40.000000 wagtail_fedit-1.1.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13617 2024-04-03 13:00:38.000000 wagtail_fedit-1.1.3/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.469113 wagtail_fedit-1.1.3/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.1.3/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.1.3/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0       63 2024-04-02 18:34:47.000000 wagtail_fedit-1.1.3/wagtail_fedit/tests.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.1.3/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.1.3/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     3806 2024-04-02 18:36:29.000000 wagtail_fedit-1.1.3/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.497437 wagtail_fedit-1.1.3/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.1.3/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8659 2024-04-03 12:33:35.000000 wagtail_fedit-1.1.3/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.1.3/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     9478 2024-04-03 12:33:35.000000 wagtail_fedit-1.1.3/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.510799 wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      106 2024-04-02 18:12:22.000000 wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/editorjs.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.511805 wagtail_fedit-1.1.3/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     5493 2024-04-03 13:02:39.000000 wagtail_fedit-1.1.3/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2670 2024-04-03 13:02:39.000000 wagtail_fedit-1.1.3/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 13:02:39.000000 wagtail_fedit-1.1.3/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-03 13:02:39.000000 wagtail_fedit-1.1.3/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-03 13:02:39.000000 wagtail_fedit-1.1.3/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:01.071979 wagtail_fedit-1.1.4/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5493 2024-04-03 13:09:01.071979 wagtail_fedit-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.1.4/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-03 13:09:01.085746 wagtail_fedit-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.914133 wagtail_fedit-1.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.916426 wagtail_fedit-1.1.4/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.919441 wagtail_fedit-1.1.4/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.920950 wagtail_fedit-1.1.4/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.932449 wagtail_fedit-1.1.4/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.4/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.949906 wagtail_fedit-1.1.4/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.4/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.4/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.4/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.970763 wagtail_fedit-1.1.4/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.1.4/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.1.4/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.1.4/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.1.4/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.973760 wagtail_fedit-1.1.4/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.4/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.975764 wagtail_fedit-1.1.4/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.4/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.4/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.891959 wagtail_fedit-1.1.4/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.894213 wagtail_fedit-1.1.4/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.982758 wagtail_fedit-1.1.4/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.1.4/wagtail_fedit/static/wagtail_fedit/css/admin.css
+-rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.1.4/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.1.4/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.985760 wagtail_fedit-1.1.4/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    10561 2024-04-02 19:44:50.000000 wagtail_fedit-1.1.4/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.896216 wagtail_fedit-1.1.4/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.899211 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.990759 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:00.995761 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:01.009777 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
+-rw-rw-rw-   0        0        0     1959 2024-04-02 19:17:17.000000 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:01.015780 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0     1023 2024-04-02 20:15:18.000000 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+-rw-rw-rw-   0        0        0      845 2024-04-02 20:15:27.000000 wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:01.033698 wagtail_fedit-1.1.4/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.1.4/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:01.039248 wagtail_fedit-1.1.4/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.4/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16682 2024-04-03 13:00:40.000000 wagtail_fedit-1.1.4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13615 2024-04-03 13:08:46.000000 wagtail_fedit-1.1.4/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:01.042239 wagtail_fedit-1.1.4/wagtail_fedit/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.1.4/wagtail_fedit/tests/__init__.py
+-rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.1.4/wagtail_fedit/tests/test_blocks.py
+-rw-rw-rw-   0        0        0       63 2024-04-02 18:34:47.000000 wagtail_fedit-1.1.4/wagtail_fedit/tests.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.1.4/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.1.4/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0     3806 2024-04-02 18:36:29.000000 wagtail_fedit-1.1.4/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:01.051256 wagtail_fedit-1.1.4/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.1.4/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8659 2024-04-03 12:33:35.000000 wagtail_fedit-1.1.4/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.1.4/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     9478 2024-04-03 12:33:35.000000 wagtail_fedit-1.1.4/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:01.066447 wagtail_fedit-1.1.4/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      106 2024-04-02 18:12:22.000000 wagtail_fedit-1.1.4/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.1.4/wagtail_fedit/wagtail_hooks/editorjs.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.1.4/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.1.4/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.1.4/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.1.4/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:09:01.069977 wagtail_fedit-1.1.4/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     5493 2024-04-03 13:09:00.000000 wagtail_fedit-1.1.4/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2670 2024-04-03 13:09:00.000000 wagtail_fedit-1.1.4/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 13:09:00.000000 wagtail_fedit-1.1.4/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-03 13:09:00.000000 wagtail_fedit-1.1.4/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-03 13:09:00.000000 wagtail_fedit-1.1.4/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.1.3/LICENSE` & `wagtail_fedit-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/PKG-INFO` & `wagtail_fedit-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.1.3
+Version: 1.1.4
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.3 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.4 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.1.3/README.md` & `wagtail_fedit-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/setup.cfg` & `wagtail_fedit-1.1.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 312e  ..version = 1.1.
-00000030: 330d 0a64 6573 6372 6970 7469 6f6e 203d  3..description =
+00000030: 340d 0a64 6573 6372 6970 7469 6f6e 203d  4..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.1.3/tests/testapp/manage.py` & `wagtail_fedit-1.1.4/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.1.4/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.1.4/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.1.4/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.1.4/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.1.4/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.1.4/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.1.4/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.1.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.1.4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.1.4/wagtail_fedit/templatetags/fedit.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,18 @@
 
         if not block_id and "block_id" not in context and not block:
             raise ValueError("Block ID is required")
         
         if not model and "wagtail_fedit_instance" not in context:
             raise ValueError("Model instance is required")
         
+        # `wagtail_fedit_instance` is provided after the form is saved.
+        # This allows us to easily use the same instance across multiple views.
+        # Model will only be provided initially when the block is rendered.
+        model = model or context["wagtail_fedit_instance"]
         context["wagtail_fedit_field_name"] = field_name
         context["wagtail_fedit_instance"] = model
         
         # Render the block or nodelist
         # This allows us to use the block as a block tag or as a simple tag.
         if block:
             try:
@@ -105,19 +109,14 @@
         if not block_id and "block_id" in context:
             block_id = context["block_id"]
         elif not block_id and block and hasattr(block, "id"):
             block_id = block.id
         elif not block_id:
             raise ValueError("Block ID is required")
 
-        # `wagtail_fedit_instance` is provided after the form is saved.
-        # This allows us to easily use the same instance across multiple views.
-        # Model will only be provided initially when the block is rendered.
-        model = model or context["wagtail_fedit_instance"]
-
         # Check if the user has permission to edit the block.
         request = context.get("request")
         if request:
             if (
                 not request.user.is_authenticated\
                 or not request.user.has_perm("wagtailadmin.access_admin")\
                 or not request.user.has_perm(f"{model._meta.app_label}.change_{model._meta.model_name}")
```

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.1.4/wagtail_fedit/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.1.4/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/urls.py` & `wagtail_fedit-1.1.4/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/utils.py` & `wagtail_fedit-1.1.4/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.1.4/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.1.4/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.1.4/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.1.4/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.1.4/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.1.4/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.1.3
+Version: 1.1.4
 Summary: An application made for the Django Web Framework.
 Home-page: https://github.com/Nigel2392/wagtail_fedit
 Author: Nigel
 Author-email: nigel@goodadvice.it
 License: GPL-3.0-only
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.3 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.4 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.1.3/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.1.4/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*
