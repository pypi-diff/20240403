# Comparing `tmp/wagtail_fedit-1.1.1.tar.gz` & `tmp/wagtail_fedit-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.1.1.tar", last modified: Tue Apr  2 23:37:08 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.1.2.tar", last modified: Wed Apr  3 12:33:54 2024, max compression
```

## Comparing `wagtail_fedit-1.1.1.tar` & `wagtail_fedit-1.1.2.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.783286 wagtail_fedit-1.1.1/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5493 2024-04-02 23:37:08.783286 wagtail_fedit-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.1.1/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-02 23:37:08.793031 wagtail_fedit-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.355621 wagtail_fedit-1.1.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.357777 wagtail_fedit-1.1.1/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.358779 wagtail_fedit-1.1.1/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.359778 wagtail_fedit-1.1.1/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.362949 wagtail_fedit-1.1.1/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.1/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.430049 wagtail_fedit-1.1.1/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.1/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.1/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.1/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.483779 wagtail_fedit-1.1.1/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.1.1/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.1.1/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.1.1/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.1.1/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.484787 wagtail_fedit-1.1.1/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.1/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.485820 wagtail_fedit-1.1.1/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.1/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.1/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.348119 wagtail_fedit-1.1.1/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.348634 wagtail_fedit-1.1.1/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.510247 wagtail_fedit-1.1.1/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.1.1/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.1.1/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.1.1/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.524472 wagtail_fedit-1.1.1/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    10561 2024-04-02 19:44:50.000000 wagtail_fedit-1.1.1/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.349156 wagtail_fedit-1.1.1/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.350193 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.541366 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.557256 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.606704 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
--rw-rw-rw-   0        0        0     1959 2024-04-02 19:17:17.000000 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.638790 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-02 20:15:18.000000 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
--rw-rw-rw-   0        0        0      845 2024-04-02 20:15:27.000000 wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.654041 wagtail_fedit-1.1.1/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.1.1/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.656324 wagtail_fedit-1.1.1/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.1/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16610 2024-04-02 18:36:53.000000 wagtail_fedit-1.1.1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13337 2024-04-02 18:34:03.000000 wagtail_fedit-1.1.1/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.672338 wagtail_fedit-1.1.1/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.1.1/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.1.1/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0       63 2024-04-02 18:34:47.000000 wagtail_fedit-1.1.1/wagtail_fedit/tests.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.1.1/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.1.1/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     3806 2024-04-02 18:36:29.000000 wagtail_fedit-1.1.1/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.724088 wagtail_fedit-1.1.1/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.1.1/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8655 2024-04-02 23:20:23.000000 wagtail_fedit-1.1.1/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.1.1/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     9474 2024-04-02 20:03:35.000000 wagtail_fedit-1.1.1/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.781390 wagtail_fedit-1.1.1/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      106 2024-04-02 18:12:22.000000 wagtail_fedit-1.1.1/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.1.1/wagtail_fedit/wagtail_hooks/editorjs.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.1.1/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.1.1/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.1.1/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.1.1/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:37:08.782689 wagtail_fedit-1.1.1/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     5493 2024-04-02 23:37:08.000000 wagtail_fedit-1.1.1/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2670 2024-04-02 23:37:08.000000 wagtail_fedit-1.1.1/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 23:37:08.000000 wagtail_fedit-1.1.1/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-02 23:37:08.000000 wagtail_fedit-1.1.1/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-02 23:37:08.000000 wagtail_fedit-1.1.1/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.631238 wagtail_fedit-1.1.2/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5493 2024-04-03 12:33:54.631238 wagtail_fedit-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.1.2/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-03 12:33:54.643238 wagtail_fedit-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.495952 wagtail_fedit-1.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.498952 wagtail_fedit-1.1.2/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.501956 wagtail_fedit-1.1.2/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.503953 wagtail_fedit-1.1.2/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.510236 wagtail_fedit-1.1.2/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.522503 wagtail_fedit-1.1.2/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.2/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.2/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.2/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.553518 wagtail_fedit-1.1.2/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.1.2/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.1.2/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.1.2/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.1.2/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.554524 wagtail_fedit-1.1.2/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.2/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.556517 wagtail_fedit-1.1.2/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.2/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.477934 wagtail_fedit-1.1.2/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.478935 wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.561562 wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/css/admin.css
+-rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.563558 wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    10561 2024-04-02 19:44:50.000000 wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.479936 wagtail_fedit-1.1.2/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.482934 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.568159 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.573261 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.587381 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
+-rw-rw-rw-   0        0        0     1959 2024-04-02 19:17:17.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.594389 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0     1023 2024-04-02 20:15:18.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+-rw-rw-rw-   0        0        0      845 2024-04-02 20:15:27.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.599149 wagtail_fedit-1.1.2/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.1.2/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.604150 wagtail_fedit-1.1.2/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16610 2024-04-02 18:36:53.000000 wagtail_fedit-1.1.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13337 2024-04-02 18:34:03.000000 wagtail_fedit-1.1.2/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.608669 wagtail_fedit-1.1.2/wagtail_fedit/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.1.2/wagtail_fedit/tests/__init__.py
+-rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.1.2/wagtail_fedit/tests/test_blocks.py
+-rw-rw-rw-   0        0        0       63 2024-04-02 18:34:47.000000 wagtail_fedit-1.1.2/wagtail_fedit/tests.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.1.2/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.1.2/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0     3806 2024-04-02 18:36:29.000000 wagtail_fedit-1.1.2/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.616239 wagtail_fedit-1.1.2/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.1.2/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8659 2024-04-03 12:33:35.000000 wagtail_fedit-1.1.2/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.1.2/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     9478 2024-04-03 12:33:35.000000 wagtail_fedit-1.1.2/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.626234 wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      106 2024-04-02 18:12:22.000000 wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/editorjs.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.629233 wagtail_fedit-1.1.2/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     5493 2024-04-03 12:33:54.000000 wagtail_fedit-1.1.2/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2670 2024-04-03 12:33:54.000000 wagtail_fedit-1.1.2/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 12:33:54.000000 wagtail_fedit-1.1.2/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-03 12:33:54.000000 wagtail_fedit-1.1.2/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-03 12:33:54.000000 wagtail_fedit-1.1.2/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.1.1/LICENSE` & `wagtail_fedit-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/PKG-INFO` & `wagtail_fedit-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.1.1
+Version: 1.1.2
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.1 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.2 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.1.1/README.md` & `wagtail_fedit-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/setup.cfg` & `wagtail_fedit-1.1.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 312e  ..version = 1.1.
-00000030: 310d 0a64 6573 6372 6970 7469 6f6e 203d  1..description =
+00000030: 320d 0a64 6573 6372 6970 7469 6f6e 203d  2..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.1.1/tests/testapp/manage.py` & `wagtail_fedit-1.1.2/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.1.2/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.1.2/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.1.2/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.1.2/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.1.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.1.2/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.1.2/wagtail_fedit/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.1.2/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/urls.py` & `wagtail_fedit-1.1.2/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/utils.py` & `wagtail_fedit-1.1.2/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.1.2/wagtail_fedit/views/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 
         if not self.form_class:
             return HttpResponseBadRequest("Invalid block type")
 
         return super().dispatch(request, block_id, field_name, model_id, model_name, app_label)
 
-    def get_page_title(self):
+    def get_header_title(self):
 
         model_string = getattr(self.instance, "get_admin_display_title", None)
         if model_string:
             model_string = model_string()
         else:
             model_string = getattr(self.instance, "title", str(self.instance))
 
@@ -182,15 +182,15 @@
 
         meta_field = self.model._meta.get_field(self.field_name)
         
         log(
             instance=self.instance,
             action="wagtail_fedit.edit_block",
             user=request.user,
-            title=self.get_page_title(),
+            title=self.get_header_title(),
             data={
                 "block_id": self.block_id,
                 "field_name": self.field_name,
                 "model_id": self.model_id,
                 "model_name": self.model_name,
                 "app_label": self.app_label,
                 "verbose_field_name": str(meta_field.verbose_name),
```

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.1.2/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.1.2/wagtail_fedit/views/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             self.form_class = field_forms.get_form_class_for_fields(
                 self.model,
                 [field_name],
             )
 
         return super().dispatch(request, field_name, model_name, app_label, model_id)
 
-    def get_page_title(self):
+    def get_header_title(self):
         meta_field: models.Field = self.model._meta.get_field(self.field_name)
 
         model_string = field_forms.get_model_string(self.original_instance)
         if self.original_instance != self.instance:
             instance_string = field_forms.get_model_string(self.instance)
             return _("Edit model %(instance_string)s for %(model_name)s %(model_string)s") % {
                 "instance_string": instance_string,
@@ -193,15 +193,15 @@
                     content_changed=True,
                 )
             
             log(
                 instance=self.original_instance,
                 action="wagtail_fedit.edit_field",
                 user=request.user,
-                title=self.get_page_title(),
+                title=self.get_header_title(),
                 uuid=uid,
                 data=data,
                 content_changed=True,
                 **extra_log_kwargs,
             )
 
             # Check for a rendering method if it exists
```

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.1.2/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.1.1
+Version: 1.1.2
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.1 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.2 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.1.1/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.1.2/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

