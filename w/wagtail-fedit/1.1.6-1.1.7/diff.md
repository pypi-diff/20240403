# Comparing `tmp/wagtail_fedit-1.1.6.tar.gz` & `tmp/wagtail_fedit-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.1.6.tar", last modified: Wed Apr  3 14:33:38 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.1.7.tar", last modified: Wed Apr  3 15:44:23 2024, max compression
```

## Comparing `wagtail_fedit-1.1.6.tar` & `wagtail_fedit-1.1.7.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.431957 wagtail_fedit-1.1.6/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5493 2024-04-03 14:33:38.431957 wagtail_fedit-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.1.6/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-03 14:33:38.442994 wagtail_fedit-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.339974 wagtail_fedit-1.1.6/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.340978 wagtail_fedit-1.1.6/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.342973 wagtail_fedit-1.1.6/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.342973 wagtail_fedit-1.1.6/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.347054 wagtail_fedit-1.1.6/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.6/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.355447 wagtail_fedit-1.1.6/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.6/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.6/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.6/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.378448 wagtail_fedit-1.1.6/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.1.6/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.1.6/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.1.6/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.1.6/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.379447 wagtail_fedit-1.1.6/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.6/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.380447 wagtail_fedit-1.1.6/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.6/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.6/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.329653 wagtail_fedit-1.1.6/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.331164 wagtail_fedit-1.1.6/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.382447 wagtail_fedit-1.1.6/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.1.6/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.1.6/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.1.6/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.384446 wagtail_fedit-1.1.6/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    10561 2024-04-02 19:44:50.000000 wagtail_fedit-1.1.6/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.331164 wagtail_fedit-1.1.6/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.332176 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.386586 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.388596 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.395776 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
--rw-rw-rw-   0        0        0     1959 2024-04-02 19:17:17.000000 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.398940 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      834 2024-04-03 13:43:07.000000 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-02 20:15:18.000000 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
--rw-rw-rw-   0        0        0      845 2024-04-02 20:15:27.000000 wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.413946 wagtail_fedit-1.1.6/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.1.6/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.415946 wagtail_fedit-1.1.6/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.6/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16682 2024-04-03 13:00:40.000000 wagtail_fedit-1.1.6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    14091 2024-04-03 14:31:01.000000 wagtail_fedit-1.1.6/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.417950 wagtail_fedit-1.1.6/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.1.6/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.1.6/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0       63 2024-04-02 18:34:47.000000 wagtail_fedit-1.1.6/wagtail_fedit/tests.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.1.6/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.1.6/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     3806 2024-04-02 18:36:29.000000 wagtail_fedit-1.1.6/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.423628 wagtail_fedit-1.1.6/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.1.6/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8659 2024-04-03 12:33:35.000000 wagtail_fedit-1.1.6/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.1.6/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     9478 2024-04-03 12:33:35.000000 wagtail_fedit-1.1.6/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.429942 wagtail_fedit-1.1.6/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      106 2024-04-02 18:12:22.000000 wagtail_fedit-1.1.6/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.1.6/wagtail_fedit/wagtail_hooks/editorjs.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.1.6/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.1.6/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.1.6/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.1.6/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:33:38.429942 wagtail_fedit-1.1.6/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     5493 2024-04-03 14:33:38.000000 wagtail_fedit-1.1.6/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2670 2024-04-03 14:33:38.000000 wagtail_fedit-1.1.6/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 14:33:38.000000 wagtail_fedit-1.1.6/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-03 14:33:38.000000 wagtail_fedit-1.1.6/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-03 14:33:38.000000 wagtail_fedit-1.1.6/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.875994 wagtail_fedit-1.1.7/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5493 2024-04-03 15:44:23.874990 wagtail_fedit-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.1.7/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-03 15:44:23.892080 wagtail_fedit-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.496192 wagtail_fedit-1.1.7/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.500859 wagtail_fedit-1.1.7/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.504785 wagtail_fedit-1.1.7/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.508289 wagtail_fedit-1.1.7/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.521850 wagtail_fedit-1.1.7/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.7/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.637916 wagtail_fedit-1.1.7/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.7/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.7/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.7/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.695999 wagtail_fedit-1.1.7/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.1.7/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.1.7/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.1.7/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      625 2024-04-03 15:41:06.000000 wagtail_fedit-1.1.7/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.698527 wagtail_fedit-1.1.7/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.7/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.700528 wagtail_fedit-1.1.7/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.7/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.7/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.463061 wagtail_fedit-1.1.7/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.464044 wagtail_fedit-1.1.7/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.706528 wagtail_fedit-1.1.7/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.1.7/wagtail_fedit/static/wagtail_fedit/css/admin.css
+-rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.1.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.1.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.709659 wagtail_fedit-1.1.7/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    10561 2024-04-02 19:44:50.000000 wagtail_fedit-1.1.7/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.466023 wagtail_fedit-1.1.7/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.472828 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.714657 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.719091 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.734853 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
+-rw-rw-rw-   0        0        0     1959 2024-04-02 19:17:17.000000 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.743968 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      834 2024-04-03 13:43:07.000000 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0     1023 2024-04-02 20:15:18.000000 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+-rw-rw-rw-   0        0        0      845 2024-04-02 20:15:27.000000 wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.766048 wagtail_fedit-1.1.7/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.1.7/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.773602 wagtail_fedit-1.1.7/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.7/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16682 2024-04-03 13:00:40.000000 wagtail_fedit-1.1.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13707 2024-04-03 15:30:16.000000 wagtail_fedit-1.1.7/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.795684 wagtail_fedit-1.1.7/wagtail_fedit/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.1.7/wagtail_fedit/tests/__init__.py
+-rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.1.7/wagtail_fedit/tests/test_blocks.py
+-rw-rw-rw-   0        0        0       63 2024-04-02 18:34:47.000000 wagtail_fedit-1.1.7/wagtail_fedit/tests.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.1.7/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.1.7/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0     5448 2024-04-03 15:43:33.000000 wagtail_fedit-1.1.7/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.820334 wagtail_fedit-1.1.7/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.1.7/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8659 2024-04-03 12:33:35.000000 wagtail_fedit-1.1.7/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.1.7/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     9046 2024-04-03 15:44:02.000000 wagtail_fedit-1.1.7/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.869997 wagtail_fedit-1.1.7/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      132 2024-04-03 15:22:27.000000 wagtail_fedit-1.1.7/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.1.7/wagtail_fedit/wagtail_hooks/editorjs.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.1.7/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.1.7/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.1.7/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.1.7/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.1.7/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:44:23.871992 wagtail_fedit-1.1.7/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     5493 2024-04-03 15:44:22.000000 wagtail_fedit-1.1.7/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2711 2024-04-03 15:44:23.000000 wagtail_fedit-1.1.7/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 15:44:22.000000 wagtail_fedit-1.1.7/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-03 15:44:22.000000 wagtail_fedit-1.1.7/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-03 15:44:22.000000 wagtail_fedit-1.1.7/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.1.6/LICENSE` & `wagtail_fedit-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/PKG-INFO` & `wagtail_fedit-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.1.6
+Version: 1.1.7
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.6 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.7 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.1.6/README.md` & `wagtail_fedit-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/setup.cfg` & `wagtail_fedit-1.1.7/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 312e  ..version = 1.1.
-00000030: 360d 0a64 6573 6372 6970 7469 6f6e 203d  6..description =
+00000030: 370d 0a64 6573 6372 6970 7469 6f6e 203d  7..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.1.6/tests/testapp/manage.py` & `wagtail_fedit-1.1.7/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.1.7/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.1.7/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.1.7/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.1.7/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.1.7/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.1.7/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.1.7/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.1.7/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.1.7/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.1.7/wagtail_fedit/templatetags/fedit.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,22 @@
 
 import warnings
 
 from ..toolbar import (
     FeditBlockEditButton,
     FeditFieldEditButton,
 )
-from ..utils import FEDIT_PREVIEW_VAR
+from ..utils import FEDIT_PREVIEW_VAR, get_field_content
 from ..hooks import (
     CONSTRUCT_BLOCK_TOOLBAR,
     CONSTRUCT_FIELD_TOOLBAR,
 )
 
 
 register = library.Library()
-
 url_value_signer = signing.TimestampSigner()
 
 
 WARNING_FIELD_NAME_NOT_AVAILABLE = "Field name is not available in the context for block {block.name}."
 WARNING_MODEL_INSTANCE_NOT_AVAILABLE = "Model instance is not available in the context for block {block.name}."
 
 
@@ -308,31 +307,22 @@
     if not all([field_name, model]):
         raise ValueError("Field name, and model are required")
 
     extra = {}
     for key, value in kwargs.items():
         extra[key] = value
 
-        
     request = context.get("request")
-    if not content:
-        if hasattr(model, f"render_fedit_{field_name}"):
-            content = getattr(model, f"render_fedit_{field_name}")(request)
-        else:
-            content = getattr(model, field_name)
-
-    context["wagtail_fedit_field_name"] = field_name
-    context["wagtail_fedit_instance"] = model
-
-    if hasattr(context, "flatten"):
-        context = context.flatten()
-
-    if hasattr(content, "render_as_block"):
-        context.update(kwargs)
-        content = content.render_as_block(context)
+    content = get_field_content(
+        request,
+        model,
+        field_name,
+        context,
+        content=content,
+    )
 
     if request:
         if (
             not request.user.is_authenticated\
             or not request.user.has_perm("wagtailadmin.access_admin")\
             or not request.user.has_perm(f"{model._meta.app_label}.change_{model._meta.model_name}")\
             or not getattr(request, FEDIT_PREVIEW_VAR, False)
```

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.1.7/wagtail_fedit/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.1.7/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/urls.py` & `wagtail_fedit-1.1.7/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.1.7/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.1.7/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.1.7/wagtail_fedit/views/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from ..forms import (
     blocks as block_forms,
     fields as field_forms,
 )
 from ..utils import (
     FeditPermissionCheck,
     use_related_form,
+    get_field_content,
 )
 
 
 
 @method_decorator(xframe_options_sameorigin, name="dispatch")
 class EditFieldView(FeditPermissionCheck, WagtailAdminTemplateMixin, View):
     template_name = "wagtail_fedit/editor/field_iframe.html"
@@ -200,24 +201,20 @@
                 title=self.get_header_title(),
                 uuid=uid,
                 data=data,
                 content_changed=True,
                 **extra_log_kwargs,
             )
 
-            # Check for a rendering method if it exists
-            if hasattr(self.original_instance, f"render_fedit_{self.field_name}"):
-                content = getattr(self.original_instance, f"render_fedit_{self.field_name}")(self.request, context=context)
-            else:
-                content = getattr(self.original_instance, self.field_name)
-
-            # The content might be a streamblock etc, we can render it as a block
-            # if isinstance(content, (blocks.BoundBlock, blocks.StructValue)):
-            if hasattr(content, "render_as_block"):
-                content = content.render_as_block(context)
+            content = get_field_content(
+                request,
+                self.original_instance,
+                self.meta_field,
+                context
+            )
 
             # Render the frame HTML
             html = render_editable_field(
                 self.request, content,
                 self.field_name, self.original_instance,
                 context=context,
             )
```

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.1.7/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.1.7/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.1.7/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.1.6
+Version: 1.1.7
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.6 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.7 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.1.6/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.1.7/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,9 +61,10 @@
 wagtail_fedit/views/blocks.py
 wagtail_fedit/views/editable.py
 wagtail_fedit/views/fields.py
 wagtail_fedit/wagtail_hooks/__init__.py
 wagtail_fedit/wagtail_hooks/editorjs.py
 wagtail_fedit/wagtail_hooks/excluded_relations.py
 wagtail_fedit/wagtail_hooks/log_actions.py
+wagtail_fedit/wagtail_hooks/renderers.py
 wagtail_fedit/wagtail_hooks/urls.py
 wagtail_fedit/wagtail_hooks/userbar.py
```

