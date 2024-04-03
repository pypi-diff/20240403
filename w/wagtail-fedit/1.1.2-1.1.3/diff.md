# Comparing `tmp/wagtail_fedit-1.1.2.tar.gz` & `tmp/wagtail_fedit-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.1.2.tar", last modified: Wed Apr  3 12:33:54 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.1.3.tar", last modified: Wed Apr  3 13:02:39 2024, max compression
```

## Comparing `wagtail_fedit-1.1.2.tar` & `wagtail_fedit-1.1.3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.631238 wagtail_fedit-1.1.2/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5493 2024-04-03 12:33:54.631238 wagtail_fedit-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.1.2/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-03 12:33:54.643238 wagtail_fedit-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.495952 wagtail_fedit-1.1.2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.498952 wagtail_fedit-1.1.2/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.501956 wagtail_fedit-1.1.2/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.503953 wagtail_fedit-1.1.2/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.510236 wagtail_fedit-1.1.2/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.2/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.522503 wagtail_fedit-1.1.2/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.2/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.2/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.2/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.553518 wagtail_fedit-1.1.2/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.1.2/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.1.2/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.1.2/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.1.2/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.554524 wagtail_fedit-1.1.2/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.2/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.556517 wagtail_fedit-1.1.2/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.2/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.477934 wagtail_fedit-1.1.2/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.478935 wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.561562 wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.563558 wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    10561 2024-04-02 19:44:50.000000 wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.479936 wagtail_fedit-1.1.2/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.482934 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.568159 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.573261 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.587381 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
--rw-rw-rw-   0        0        0     1959 2024-04-02 19:17:17.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.594389 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-02 20:15:18.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
--rw-rw-rw-   0        0        0      845 2024-04-02 20:15:27.000000 wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.599149 wagtail_fedit-1.1.2/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.1.2/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.604150 wagtail_fedit-1.1.2/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16610 2024-04-02 18:36:53.000000 wagtail_fedit-1.1.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13337 2024-04-02 18:34:03.000000 wagtail_fedit-1.1.2/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.608669 wagtail_fedit-1.1.2/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.1.2/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.1.2/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0       63 2024-04-02 18:34:47.000000 wagtail_fedit-1.1.2/wagtail_fedit/tests.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.1.2/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.1.2/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     3806 2024-04-02 18:36:29.000000 wagtail_fedit-1.1.2/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.616239 wagtail_fedit-1.1.2/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.1.2/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8659 2024-04-03 12:33:35.000000 wagtail_fedit-1.1.2/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.1.2/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     9478 2024-04-03 12:33:35.000000 wagtail_fedit-1.1.2/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.626234 wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      106 2024-04-02 18:12:22.000000 wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/editorjs.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:54.629233 wagtail_fedit-1.1.2/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     5493 2024-04-03 12:33:54.000000 wagtail_fedit-1.1.2/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2670 2024-04-03 12:33:54.000000 wagtail_fedit-1.1.2/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 12:33:54.000000 wagtail_fedit-1.1.2/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-03 12:33:54.000000 wagtail_fedit-1.1.2/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-03 12:33:54.000000 wagtail_fedit-1.1.2/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.512817 wagtail_fedit-1.1.3/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5493 2024-04-03 13:02:39.512817 wagtail_fedit-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.1.3/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-03 13:02:39.523156 wagtail_fedit-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.338351 wagtail_fedit-1.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.340321 wagtail_fedit-1.1.3/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.341325 wagtail_fedit-1.1.3/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.341325 wagtail_fedit-1.1.3/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.346138 wagtail_fedit-1.1.3/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.1.3/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.361471 wagtail_fedit-1.1.3/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.3/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.3/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.3/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.399508 wagtail_fedit-1.1.3/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.1.3/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.1.3/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.1.3/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      274 2024-04-01 18:05:08.000000 wagtail_fedit-1.1.3/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.400509 wagtail_fedit-1.1.3/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.3/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.400509 wagtail_fedit-1.1.3/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.1.3/wagtail_fedit/models.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.328518 wagtail_fedit-1.1.3/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.328518 wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.405815 wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/css/admin.css
+-rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.425205 wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    10561 2024-04-02 19:44:50.000000 wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.329519 wagtail_fedit-1.1.3/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.330813 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.427588 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.429658 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:28.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      782 2024-04-01 17:06:47.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.436208 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
+-rw-rw-rw-   0        0        0     1959 2024-04-02 19:17:17.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.439589 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      835 2024-04-01 13:18:33.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0     1023 2024-04-02 20:15:18.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+-rw-rw-rw-   0        0        0      845 2024-04-02 20:15:27.000000 wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.451779 wagtail_fedit-1.1.3/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.1.3/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.454218 wagtail_fedit-1.1.3/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.1.3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16682 2024-04-03 13:00:40.000000 wagtail_fedit-1.1.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13617 2024-04-03 13:00:38.000000 wagtail_fedit-1.1.3/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.469113 wagtail_fedit-1.1.3/wagtail_fedit/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.1.3/wagtail_fedit/tests/__init__.py
+-rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.1.3/wagtail_fedit/tests/test_blocks.py
+-rw-rw-rw-   0        0        0       63 2024-04-02 18:34:47.000000 wagtail_fedit-1.1.3/wagtail_fedit/tests.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.1.3/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.1.3/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0     3806 2024-04-02 18:36:29.000000 wagtail_fedit-1.1.3/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.497437 wagtail_fedit-1.1.3/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.1.3/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8659 2024-04-03 12:33:35.000000 wagtail_fedit-1.1.3/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.1.3/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     9478 2024-04-03 12:33:35.000000 wagtail_fedit-1.1.3/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.510799 wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      106 2024-04-02 18:12:22.000000 wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/editorjs.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:02:39.511805 wagtail_fedit-1.1.3/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     5493 2024-04-03 13:02:39.000000 wagtail_fedit-1.1.3/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2670 2024-04-03 13:02:39.000000 wagtail_fedit-1.1.3/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 13:02:39.000000 wagtail_fedit-1.1.3/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-03 13:02:39.000000 wagtail_fedit-1.1.3/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-03 13:02:39.000000 wagtail_fedit-1.1.3/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.1.2/LICENSE` & `wagtail_fedit-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/PKG-INFO` & `wagtail_fedit-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.1.2
+Version: 1.1.3
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.2 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.3 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.1.2/README.md` & `wagtail_fedit-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/setup.cfg` & `wagtail_fedit-1.1.3/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 312e  ..version = 1.1.
-00000030: 320d 0a64 6573 6372 6970 7469 6f6e 203d  2..description =
+00000030: 330d 0a64 6573 6372 6970 7469 6f6e 203d  3..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.1.2/tests/testapp/manage.py` & `wagtail_fedit-1.1.3/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.1.3/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.1.3/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.1.3/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.1.3/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.1.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.1.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.1.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x9b4f0c66 (Tue Apr  2 18:34:03 2024 UTC)
-files sz: 13337
+moddate:  0xf6520d66 (Wed Apr  3 13:00:38 2024 UTC)
+files sz: 13617
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -163,73 +163,73 @@
                272 MAKE_FUNCTION            0
                274 LOAD_CONST              18 ('BlockEditNode')
                276 LOAD_NAME                2 (Node)
                278 PRECALL                  3
                282 CALL                     3
                292 STORE_NAME              38 (BlockEditNode)
    
-   216         294 LOAD_NAME               35 (register)
+   224         294 LOAD_NAME               35 (register)
                296 LOAD_METHOD             39 (tag)
                318 LOAD_CONST              19 ('fedit_block')
                320 KW_NAMES                20
                322 PRECALL                  1
                326 CALL                     1
    
-   217         336 LOAD_CONST              21 ('parser')
+   225         336 LOAD_CONST              21 ('parser')
                338 LOAD_NAME                7 (Parser)
                340 LOAD_CONST              22 ('token')
                342 LOAD_NAME                8 (Token)
                344 BUILD_TUPLE              4
-               346 LOAD_CONST              23 (<code object do_render_fedit_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 216>)
+               346 LOAD_CONST              23 (<code object do_render_fedit_block, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 224>)
                348 MAKE_FUNCTION            4 (annotations)
    
-   216         350 PRECALL                  0
+   224         350 PRECALL                  0
                354 CALL                     0
    
-   217         364 STORE_NAME              40 (do_render_fedit_block)
+   225         364 STORE_NAME              40 (do_render_fedit_block)
    
-   278         366 LOAD_NAME               35 (register)
+   284         366 LOAD_NAME               35 (register)
                368 LOAD_METHOD             41 (simple_tag)
                390 LOAD_CONST              24 (True)
                392 LOAD_CONST              25 ('fedit_field')
                394 KW_NAMES                26
                396 PRECALL                  2
                400 CALL                     2
    
-   279         410 LOAD_CONST              35 ((None,))
-               412 LOAD_CONST              28 (<code object do_render_fedit_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 278>)
+   285         410 LOAD_CONST              35 ((None,))
+               412 LOAD_CONST              28 (<code object do_render_fedit_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 284>)
                414 MAKE_FUNCTION            1 (defaults)
    
-   278         416 PRECALL                  0
+   284         416 PRECALL                  0
                420 CALL                     0
    
-   279         430 STORE_NAME              42 (do_render_fedit_field)
+   285         430 STORE_NAME              42 (do_render_fedit_field)
    
-   334         432 LOAD_CONST              29 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 334>)
+   340         432 LOAD_CONST              29 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 340>)
                434 MAKE_FUNCTION            0
                436 STORE_NAME              43 (render_editable_field)
    
-   370         438 LOAD_CONST              21 ('parser')
+   376         438 LOAD_CONST              21 ('parser')
                440 LOAD_NAME                7 (Parser)
                442 LOAD_CONST              30 ('kwarg_list')
                444 LOAD_NAME               44 (list)
                446 LOAD_NAME               45 (str)
                448 BINARY_SUBSCR
                458 LOAD_CONST              31 ('tokens')
                460 LOAD_NAME               44 (list)
                462 LOAD_NAME               45 (str)
                464 BINARY_SUBSCR
                474 LOAD_CONST              32 ('return')
                476 LOAD_NAME               46 (dict)
                478 BUILD_TUPLE              8
-               480 LOAD_CONST              33 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 370>)
+               480 LOAD_CONST              33 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 376>)
                482 MAKE_FUNCTION            4 (annotations)
                484 STORE_NAME              47 (get_kwargs)
    
-   397         486 LOAD_CONST              34 (<code object _get_from_context_or_set, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 397>)
+   403         486 LOAD_CONST              34 (<code object _get_from_context_or_set, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 403>)
                488 MAKE_FUNCTION            0
                490 STORE_NAME              48 (_get_from_context_or_set)
                492 LOAD_CONST              27 (None)
                494 RETURN_VALUE
    consts
       0
       ('library', 'Node', 'NodeList')
@@ -315,64 +315,64 @@
                       84 MAKE_FUNCTION            5 (defaults, annotations)
                       86 STORE_NAME              10 (__init__)
          
           51          88 LOAD_CONST              10 (<code object render, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 51>)
                       90 MAKE_FUNCTION            0
                       92 STORE_NAME              11 (render)
          
-         167          94 LOAD_NAME               12 (staticmethod)
+         175          94 LOAD_NAME               12 (staticmethod)
          
-         168          96 LOAD_CONST              11 ('return')
+         176          96 LOAD_CONST              11 ('return')
                       98 LOAD_NAME               13 (dict)
                      100 BUILD_TUPLE              2
-                     102 LOAD_CONST              12 (<code object pack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 167>)
+                     102 LOAD_CONST              12 (<code object pack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 175>)
                      104 MAKE_FUNCTION            4 (annotations)
          
-         167         106 PRECALL                  0
+         175         106 PRECALL                  0
                      110 CALL                     0
          
-         168         120 STORE_NAME              14 (pack)
+         176         120 STORE_NAME              14 (pack)
          
-         176         122 LOAD_NAME               15 (classmethod)
+         184         122 LOAD_NAME               15 (classmethod)
          
-         177         124 LOAD_CONST               3 (None)
+         185         124 LOAD_CONST               3 (None)
                      126 LOAD_CONST              13 (('request',))
                      128 BUILD_CONST_KEY_MAP      1
                      130 LOAD_CONST              14 ('expected')
                      132 LOAD_NAME                7 (str)
                      134 LOAD_CONST              11 ('return')
                      136 LOAD_NAME               13 (dict)
                      138 BUILD_TUPLE              4
-                     140 LOAD_CONST              15 (<code object unpack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 176>)
+                     140 LOAD_CONST              15 (<code object unpack, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 184>)
                      142 MAKE_FUNCTION            6 (kwdefaults, annotations)
          
-         176         144 PRECALL                  0
+         184         144 PRECALL                  0
                      148 CALL                     0
          
-         177         158 STORE_NAME              16 (unpack)
+         185         158 STORE_NAME              16 (unpack)
          
-         199         160 LOAD_NAME               12 (staticmethod)
+         207         160 LOAD_NAME               12 (staticmethod)
          
-         200         162 LOAD_CONST               6 ('block_id')
+         208         162 LOAD_CONST               6 ('block_id')
                      164 LOAD_NAME                7 (str)
                      166 LOAD_CONST               7 ('field_name')
                      168 LOAD_NAME                7 (str)
                      170 LOAD_CONST              16 ('instance')
                      172 LOAD_NAME                8 (models)
                      174 LOAD_ATTR                9 (Model)
                      184 LOAD_CONST              11 ('return')
                      186 LOAD_NAME                7 (str)
                      188 BUILD_TUPLE              8
-                     190 LOAD_CONST              17 (<code object get_edit_url, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 199>)
+                     190 LOAD_CONST              17 (<code object get_edit_url, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 207>)
                      192 MAKE_FUNCTION            4 (annotations)
          
-         199         194 PRECALL                  0
+         207         194 PRECALL                  0
                      198 CALL                     0
          
-         200         208 STORE_NAME              17 (get_edit_url)
+         208         208 STORE_NAME              17 (get_edit_url)
                      210 LOAD_CONST               3 (None)
                      212 RETURN_VALUE
          consts
             'BlockEditNode'
             code
                argcount  : 0
                nlocals   : 0
@@ -451,80 +451,81 @@
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '__init__'
                firstlineno 35
                lnotab 0x02090e010e010e010e010e01
             code
                argcount  : 2
                nlocals   : 12
-               stacksize : 12
+               stacksize : 14
                flags     : 3
                code
                   0x870c870d97007c006a0000000000000000007d027c006a010000000000
                   0000007d037c006a0200000000000000007d047c006a0300000000000000
                   008a0c7c006a0400000000000000007d057c05a005000000000000000000
                   0000000000000000000000a6000000ab00000000000000000044005d325c
                   0200007d067d07740d000000000000000000007c07740e00000000000000
                   000000a6020000ab02000000000000000072187c07a00800000000000000
                   000000000000000000000000007c01a6010000ab0100000000000000007c
-                  057c063c0000008c33740d000000000000000000007c02740e0000000000
-                  0000000000a6020000ab02000000000000000072157c02a0080000000000
-                  0000000000000000000000000000007c01a6010000ab0100000000000000
-                  007d02740d000000000000000000007c03740e00000000000000000000a6
-                  020000ab02000000000000000072157c03a0080000000000000000000000
-                  0000000000000000007c01a6010000ab0100000000000000007d03740d00
-                  0000000000000000007c04740e00000000000000000000a6020000ab0200
-                  0000000000000072157c04a0080000000000000000000000000000000000
-                  0000007c01a6010000ab0100000000000000007d04740d00000000000000
-                  000000890c740e00000000000000000000a6020000ab0200000000000000
-                  007215890ca00800000000000000000000000000000000000000007c01a6
-                  010000ab0100000000000000008a0c7c04730f7413000000000000000000
-                  006401a6010000ab01000000000000000082017c03731564027c01760172
-                  117c02730f7413000000000000000000006403a6010000ab010000000000
-                  0000008201890c731364047c017601720f74130000000000000000000064
-                  05a6010000ab01000000000000000082017c02725809007c01a00a000000
-                  0000000000000000000000000000000000a6000000ab0000000000000000
-                  007d016e10230074160000000000000000000024007203010059006e0477
-                  007803590077017c01a00c00000000000000000000000000000000000000
-                  007c05a6010000ab01000000000000000001007c02a00d00000000000000
+                  057c063c0000008c337c04730c64017c01760072087c0164011900000000
+                  00000000007d04740d000000000000000000007c02740e00000000000000
+                  000000a6020000ab02000000000000000072157c02a00800000000000000
                   000000000000000000000000007c01a6010000ab0100000000000000007d
-                  0864067c005f0e00000000000000006e4c7c006a0f000000000000000072
-                  367c006a0f0000000000000000a010000000000000000000000000000000
-                  00000000007c01a6010000ab0100000000000000007d087c01a011000000
-                  000000000000000000000000000000000064076408a6020000ab02000000
-                  00000000007c005f0e00000000000000006e0f7413000000000000000000
-                  006409a6010000ab01000000000000000082017c03730d64027c01760072
-                  097c016402190000000000000000007d036e2d7c03731a7c027218742500
-                  0000000000000000007c02640aa6020000ab02000000000000000072087c
-                  026a1300000000000000007d036e117c03730f7413000000000000000000
-                  006403a6010000ab0100000000000000008201890c70077c016404190000
-                  000000000000008a0c7c01a0110000000000000000000000000000000000
-                  000000640ba6010000ab0100000000000000008a0d890d7271890d6a1400
-                  000000000000006a1500000000000000007263890d6a1400000000000000
-                  00a0160000000000000000000000000000000000000000640ca6010000ab
-                  0100000000000000007249890d6a140000000000000000a0160000000000
-                  000000000000000000000000000000890c6a1700000000000000006a1800
-                  000000000000009b00640d890c6a1700000000000000006a190000000000
-                  0000009b009d03a6010000ab010000000000000000721674350000000000
-                  0000000000890d7436000000000000000000006408a6030000ab03000000
-                  000000000073027c085300740d00000000000000000000890c7438000000
-                  00000000000000a6020000ab020000000000000000721d743b0000000000
-                  00000000007c01640e880c6601640f8408a6030000ab0300000000000000
-                  007d097c099b0064107c039b0064119d047d096e0264007d097c05a01e00
-                  0000000000000000000000000000000000000064127c006a0e0000000000
-                  000000a6020000ab0200000000000000000100743f000000000000000000
-                  00a6000000ab00000000000000000067017d0a7441000000000000000000
-                  006a210000000000000000744400000000000000000000a6010000ab0100
-                  0000000000000044005d127d0b02007c0b890d7c0a890c7c037c04ac13a6
-                  050000ab05000000000000000001008c13880d6601641484087c0a4400a6
-                  000000ab0000000000000000007d0a744700000000000000000000744900
-                  00000000000000000064007c0aa6020000ab020000000000000000a60100
-                  00ab0100000000000000007d0a744b00000000000000000000641502007c
-                  006a2600000000000000007c037c0466026416890c69017c05a4018e017c
-                  097c03890c7c087c047c017c0a64179c08a6020000ab0200000000000000
-                  005300
+                  02740d000000000000000000007c03740e00000000000000000000a60200
+                  00ab02000000000000000072157c03a00800000000000000000000000000
+                  000000000000007c01a6010000ab0100000000000000007d03740d000000
+                  000000000000007c04740e00000000000000000000a6020000ab02000000
+                  000000000072157c04a00800000000000000000000000000000000000000
+                  007c01a6010000ab0100000000000000007d04740d000000000000000000
+                  00890c740e00000000000000000000a6020000ab02000000000000000072
+                  15890ca00800000000000000000000000000000000000000007c01a60100
+                  00ab0100000000000000008a0c7c04730f74130000000000000000000064
+                  02a6010000ab01000000000000000082017c03731564037c01760172117c
+                  02730f7413000000000000000000006404a6010000ab0100000000000000
+                  008201890c731364057c017601720f7413000000000000000000006406a6
+                  010000ab01000000000000000082017c047c0164013c000000890c7c0164
+                  053c0000007c02725809007c01a00a000000000000000000000000000000
+                  0000000000a6000000ab0000000000000000007d016e1023007416000000
+                  0000000000000024007203010059006e0477007803590077017c01a00c00
+                  000000000000000000000000000000000000007c05a6010000ab01000000
+                  000000000001007c02a00d00000000000000000000000000000000000000
+                  007c01a6010000ab0100000000000000007d0864077c005f0e0000000000
+                  0000006e4c7c006a0f000000000000000072367c006a0f00000000000000
+                  00a01000000000000000000000000000000000000000007c01a6010000ab
+                  0100000000000000007d087c01a011000000000000000000000000000000
+                  000000000064086409a6020000ab0200000000000000007c005f0e000000
+                  00000000006e0f741300000000000000000000640aa6010000ab01000000
+                  000000000082017c03730d64037c01760072097c01640319000000000000
+                  0000007d036e2d7c03731a7c0272187425000000000000000000007c0264
+                  0ba6020000ab02000000000000000072087c026a1300000000000000007d
+                  036e117c03730f7413000000000000000000006404a6010000ab01000000
+                  00000000008201890c70077c016405190000000000000000008a0c7c01a0
+                  110000000000000000000000000000000000000000640ca6010000ab0100
+                  000000000000008a0d890d7271890d6a1400000000000000006a15000000
+                  00000000007263890d6a140000000000000000a016000000000000000000
+                  0000000000000000000000640da6010000ab010000000000000000724989
+                  0d6a140000000000000000a0160000000000000000000000000000000000
+                  000000890c6a1700000000000000006a1800000000000000009b00640e89
+                  0c6a1700000000000000006a1900000000000000009b009d03a6010000ab
+                  0100000000000000007216743500000000000000000000890d7436000000
+                  000000000000006409a6030000ab03000000000000000073027c08530074
+                  0d00000000000000000000890c743800000000000000000000a6020000ab
+                  020000000000000000721d743b000000000000000000007c01640f880c66
+                  0164108408a6030000ab0300000000000000007d097c099b0064117c039b
+                  0064129d047d096e0264007d097c05a01e00000000000000000000000000
+                  0000000000000064137c006a0e0000000000000000a6020000ab02000000
+                  00000000000100743f00000000000000000000a6000000ab000000000000
+                  00000067017d0a7441000000000000000000006a21000000000000000074
+                  4400000000000000000000a6010000ab01000000000000000044005d127d
+                  0b02007c0b890d7c0a890c7c037c04ac14a6050000ab0500000000000000
+                  0001008c13880d6601641584087c0a4400a6000000ab0000000000000000
+                  007d0a74470000000000000000000074490000000000000000000064007c
+                  0aa6020000ab020000000000000000a6010000ab0100000000000000007d
+                  0a744b00000000000000000000641602007c006a2600000000000000007c
+                  037c0466026417890c69017c05a4018e017c097c03890c7c087c047c017c
+                  04890c7c0a64189c0aa6020000ab0200000000000000005300
                              0 MAKE_CELL               12 (model)
                              2 MAKE_CELL               13 (request)
                
                 51           4 RESUME                   0
                
                 52           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (block)
@@ -569,421 +570,448 @@
                            194 PRECALL                  1
                            198 CALL                     1
                            208 LOAD_FAST                5 (extra)
                            210 LOAD_FAST                6 (k)
                            212 STORE_SUBSCR
                        >>  216 JUMP_BACKWARD           51 (to 116)
                
-                63     >>  218 LOAD_GLOBAL             13 (NULL + isinstance)
-                           230 LOAD_FAST                2 (block)
-                           232 LOAD_GLOBAL             14 (FilterExpression)
-                           244 PRECALL                  2
-                           248 CALL                     2
-                           258 POP_JUMP_FORWARD_IF_FALSE    21 (to 302)
-               
-                64         260 LOAD_FAST                2 (block)
-                           262 LOAD_METHOD              8 (resolve)
-                           284 LOAD_FAST                1 (context)
-                           286 PRECALL                  1
-                           290 CALL                     1
-                           300 STORE_FAST               2 (block)
-               
-                65     >>  302 LOAD_GLOBAL             13 (NULL + isinstance)
-                           314 LOAD_FAST                3 (block_id)
-                           316 LOAD_GLOBAL             14 (FilterExpression)
-                           328 PRECALL                  2
-                           332 CALL                     2
-                           342 POP_JUMP_FORWARD_IF_FALSE    21 (to 386)
-               
-                66         344 LOAD_FAST                3 (block_id)
-                           346 LOAD_METHOD              8 (resolve)
-                           368 LOAD_FAST                1 (context)
-                           370 PRECALL                  1
-                           374 CALL                     1
-                           384 STORE_FAST               3 (block_id)
-               
-                67     >>  386 LOAD_GLOBAL             13 (NULL + isinstance)
-                           398 LOAD_FAST                4 (field_name)
-                           400 LOAD_GLOBAL             14 (FilterExpression)
-                           412 PRECALL                  2
-                           416 CALL                     2
-                           426 POP_JUMP_FORWARD_IF_FALSE    21 (to 470)
-               
-                68         428 LOAD_FAST                4 (field_name)
-                           430 LOAD_METHOD              8 (resolve)
-                           452 LOAD_FAST                1 (context)
-                           454 PRECALL                  1
-                           458 CALL                     1
-                           468 STORE_FAST               4 (field_name)
-               
-                69     >>  470 LOAD_GLOBAL             13 (NULL + isinstance)
-                           482 LOAD_DEREF              12 (model)
-                           484 LOAD_GLOBAL             14 (FilterExpression)
-                           496 PRECALL                  2
-                           500 CALL                     2
-                           510 POP_JUMP_FORWARD_IF_FALSE    21 (to 554)
-               
-                70         512 LOAD_DEREF              12 (model)
-                           514 LOAD_METHOD              8 (resolve)
-                           536 LOAD_FAST                1 (context)
-                           538 PRECALL                  1
-                           542 CALL                     1
-                           552 STORE_DEREF             12 (model)
-               
-                73     >>  554 LOAD_FAST                4 (field_name)
-                           556 POP_JUMP_FORWARD_IF_TRUE    15 (to 588)
-               
-                74         558 LOAD_GLOBAL             19 (NULL + ValueError)
-                           570 LOAD_CONST               1 ('Field name is required')
-                           572 PRECALL                  1
-                           576 CALL                     1
-                           586 RAISE_VARARGS            1
-               
-                76     >>  588 LOAD_FAST                3 (block_id)
-                           590 POP_JUMP_FORWARD_IF_TRUE    21 (to 634)
-                           592 LOAD_CONST               2 ('block_id')
-                           594 LOAD_FAST                1 (context)
-                           596 CONTAINS_OP              1
-                           598 POP_JUMP_FORWARD_IF_FALSE    17 (to 634)
-                           600 LOAD_FAST                2 (block)
-                           602 POP_JUMP_FORWARD_IF_TRUE    15 (to 634)
-               
-                77         604 LOAD_GLOBAL             19 (NULL + ValueError)
-                           616 LOAD_CONST               3 ('Block ID is required')
-                           618 PRECALL                  1
-                           622 CALL                     1
-                           632 RAISE_VARARGS            1
-               
-                79     >>  634 LOAD_DEREF              12 (model)
-                           636 POP_JUMP_FORWARD_IF_TRUE    19 (to 676)
-                           638 LOAD_CONST               4 ('wagtail_fedit_instance')
-                           640 LOAD_FAST                1 (context)
-                           642 CONTAINS_OP              1
-                           644 POP_JUMP_FORWARD_IF_FALSE    15 (to 676)
-               
-                80         646 LOAD_GLOBAL             19 (NULL + ValueError)
-                           658 LOAD_CONST               5 ('Model instance is required')
-                           660 PRECALL                  1
-                           664 CALL                     1
-                           674 RAISE_VARARGS            1
-               
-                84     >>  676 LOAD_FAST                2 (block)
-                           678 POP_JUMP_FORWARD_IF_FALSE    88 (to 856)
-               
-                85         680 NOP
-               
-                86         682 LOAD_FAST                1 (context)
-                           684 LOAD_METHOD             10 (flatten)
-                           706 PRECALL                  0
-                           710 CALL                     0
-                           720 STORE_FAST               1 (context)
-                           722 JUMP_FORWARD            16 (to 756)
-                       >>  724 PUSH_EXC_INFO
-               
-                87         726 LOAD_GLOBAL             22 (AttributeError)
-                           738 CHECK_EXC_MATCH
-                           740 POP_JUMP_FORWARD_IF_FALSE     3 (to 748)
-                           742 POP_TOP
-               
-                88         744 POP_EXCEPT
-                           746 JUMP_FORWARD             4 (to 756)
-               
-                87     >>  748 RERAISE                  0
-                       >>  750 COPY                     3
-                           752 POP_EXCEPT
-                           754 RERAISE                  1
-               
-                89     >>  756 LOAD_FAST                1 (context)
-                           758 LOAD_METHOD             12 (update)
-                           780 LOAD_FAST                5 (extra)
-                           782 PRECALL                  1
-                           786 CALL                     1
-                           796 POP_TOP
-               
-                90         798 LOAD_FAST                2 (block)
-                           800 LOAD_METHOD             13 (render_as_block)
-                           822 LOAD_FAST                1 (context)
-                           824 PRECALL                  1
-                           828 CALL                     1
-                           838 STORE_FAST               8 (rendered)
-               
-                91         840 LOAD_CONST               6 (True)
-                           842 LOAD_FAST                0 (self)
-                           844 STORE_ATTR              14 (has_block)
-                           854 JUMP_FORWARD            76 (to 1008)
-               
-                92     >>  856 LOAD_FAST                0 (self)
-                           858 LOAD_ATTR               15 (nl)
-                           868 POP_JUMP_FORWARD_IF_FALSE    54 (to 978)
-               
-                93         870 LOAD_FAST                0 (self)
-                           872 LOAD_ATTR               15 (nl)
-                           882 LOAD_METHOD             16 (render)
-                           904 LOAD_FAST                1 (context)
-                           906 PRECALL                  1
-                           910 CALL                     1
-                           920 STORE_FAST               8 (rendered)
-               
-                94         922 LOAD_FAST                1 (context)
-                           924 LOAD_METHOD             17 (get)
-                           946 LOAD_CONST               7 ('wagtail_fedit_has_block')
-                           948 LOAD_CONST               8 (False)
-                           950 PRECALL                  2
-                           954 CALL                     2
-                           964 LOAD_FAST                0 (self)
-                           966 STORE_ATTR              14 (has_block)
-                           976 JUMP_FORWARD            15 (to 1008)
-               
-                96     >>  978 LOAD_GLOBAL             19 (NULL + ValueError)
-                           990 LOAD_CONST               9 ('Block or nodelist is required')
-                           992 PRECALL                  1
-                           996 CALL                     1
-                          1006 RAISE_VARARGS            1
-               
-                99     >> 1008 LOAD_FAST                3 (block_id)
-                          1010 POP_JUMP_FORWARD_IF_TRUE    13 (to 1038)
-                          1012 LOAD_CONST               2 ('block_id')
-                          1014 LOAD_FAST                1 (context)
-                          1016 CONTAINS_OP              0
-                          1018 POP_JUMP_FORWARD_IF_FALSE     9 (to 1038)
-               
-               100        1020 LOAD_FAST                1 (context)
-                          1022 LOAD_CONST               2 ('block_id')
-                          1024 BINARY_SUBSCR
-                          1034 STORE_FAST               3 (block_id)
-                          1036 JUMP_FORWARD            45 (to 1128)
-               
-               101     >> 1038 LOAD_FAST                3 (block_id)
-                          1040 POP_JUMP_FORWARD_IF_TRUE    26 (to 1094)
-                          1042 LOAD_FAST                2 (block)
-                          1044 POP_JUMP_FORWARD_IF_FALSE    24 (to 1094)
-                          1046 LOAD_GLOBAL             37 (NULL + hasattr)
-                          1058 LOAD_FAST                2 (block)
-                          1060 LOAD_CONST              10 ('id')
-                          1062 PRECALL                  2
-                          1066 CALL                     2
-                          1076 POP_JUMP_FORWARD_IF_FALSE     8 (to 1094)
-               
-               102        1078 LOAD_FAST                2 (block)
-                          1080 LOAD_ATTR               19 (id)
-                          1090 STORE_FAST               3 (block_id)
-                          1092 JUMP_FORWARD            17 (to 1128)
-               
-               103     >> 1094 LOAD_FAST                3 (block_id)
-                          1096 POP_JUMP_FORWARD_IF_TRUE    15 (to 1128)
-               
-               104        1098 LOAD_GLOBAL             19 (NULL + ValueError)
-                          1110 LOAD_CONST               3 ('Block ID is required')
-                          1112 PRECALL                  1
-                          1116 CALL                     1
-                          1126 RAISE_VARARGS            1
-               
-               109     >> 1128 LOAD_DEREF              12 (model)
-                          1130 JUMP_IF_TRUE_OR_POP      7 (to 1146)
-                          1132 LOAD_FAST                1 (context)
-                          1134 LOAD_CONST               4 ('wagtail_fedit_instance')
-                          1136 BINARY_SUBSCR
-                       >> 1146 STORE_DEREF             12 (model)
-               
-               112        1148 LOAD_FAST                1 (context)
-                          1150 LOAD_METHOD             17 (get)
-                          1172 LOAD_CONST              11 ('request')
-                          1174 PRECALL                  1
-                          1178 CALL                     1
-                          1188 STORE_DEREF             13 (request)
-               
-               113        1190 LOAD_DEREF              13 (request)
-                          1192 POP_JUMP_FORWARD_IF_FALSE   113 (to 1420)
-               
-               115        1194 LOAD_DEREF              13 (request)
-                          1196 LOAD_ATTR               20 (user)
-                          1206 LOAD_ATTR               21 (is_authenticated)
-               
-               114        1216 POP_JUMP_FORWARD_IF_FALSE    99 (to 1416)
-               
-               116        1218 LOAD_DEREF              13 (request)
-                          1220 LOAD_ATTR               20 (user)
-                          1230 LOAD_METHOD             22 (has_perm)
-                          1252 LOAD_CONST              12 ('wagtailadmin.access_admin')
-                          1254 PRECALL                  1
-                          1258 CALL                     1
-               
-               114        1268 POP_JUMP_FORWARD_IF_FALSE    73 (to 1416)
-               
-               117        1270 LOAD_DEREF              13 (request)
-                          1272 LOAD_ATTR               20 (user)
-                          1282 LOAD_METHOD             22 (has_perm)
-                          1304 LOAD_DEREF              12 (model)
-                          1306 LOAD_ATTR               23 (_meta)
-                          1316 LOAD_ATTR               24 (app_label)
-                          1326 FORMAT_VALUE             0
-                          1328 LOAD_CONST              13 ('.change_')
-                          1330 LOAD_DEREF              12 (model)
-                          1332 LOAD_ATTR               23 (_meta)
-                          1342 LOAD_ATTR               25 (model_name)
-                          1352 FORMAT_VALUE             0
-                          1354 BUILD_STRING             3
-                          1356 PRECALL                  1
-                          1360 CALL                     1
-               
-               114        1370 POP_JUMP_FORWARD_IF_FALSE    22 (to 1416)
-               
-               118        1372 LOAD_GLOBAL             53 (NULL + getattr)
-                          1384 LOAD_DEREF              13 (request)
-                          1386 LOAD_GLOBAL             54 (FEDIT_PREVIEW_VAR)
-                          1398 LOAD_CONST               8 (False)
-                          1400 PRECALL                  3
-                          1404 CALL                     3
-               
-               114        1414 POP_JUMP_FORWARD_IF_TRUE     2 (to 1420)
-               
-               121     >> 1416 LOAD_FAST                8 (rendered)
-                          1418 RETURN_VALUE
-               
-               125     >> 1420 LOAD_GLOBAL             13 (NULL + isinstance)
-                          1432 LOAD_DEREF              12 (model)
-                          1434 LOAD_GLOBAL             56 (Page)
-                          1446 PRECALL                  2
-                          1450 CALL                     2
-                          1460 POP_JUMP_FORWARD_IF_FALSE    29 (to 1520)
-               
-               126        1462 LOAD_GLOBAL             59 (NULL + _get_from_context_or_set)
-               
-               127        1474 LOAD_FAST                1 (context)
-                          1476 LOAD_CONST              14 ('page_base_edit_url')
-               
-               128        1478 LOAD_CLOSURE            12 (model)
-                          1480 BUILD_TUPLE              1
-                          1482 LOAD_CONST              15 (<code object <lambda>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 128>)
-                          1484 MAKE_FUNCTION            8 (closure)
-               
-               126        1486 PRECALL                  3
-                          1490 CALL                     3
-                          1500 STORE_FAST               9 (admin_edit_url)
-               
-               133        1502 LOAD_FAST                9 (admin_edit_url)
-                          1504 FORMAT_VALUE             0
-                          1506 LOAD_CONST              16 ('#block-')
-                          1508 LOAD_FAST                3 (block_id)
-                          1510 FORMAT_VALUE             0
-                          1512 LOAD_CONST              17 ('-section')
-                          1514 BUILD_STRING             4
-                          1516 STORE_FAST               9 (admin_edit_url)
-                          1518 JUMP_FORWARD             2 (to 1524)
-               
-               135     >> 1520 LOAD_CONST               0 (None)
-                          1522 STORE_FAST               9 (admin_edit_url)
-               
-               137     >> 1524 LOAD_FAST                5 (extra)
-                          1526 LOAD_METHOD             30 (setdefault)
-                          1548 LOAD_CONST              18 ('has_block')
-                          1550 LOAD_FAST                0 (self)
-                          1552 LOAD_ATTR               14 (has_block)
-                          1562 PRECALL                  2
-                          1566 CALL                     2
-                          1576 POP_TOP
-               
-               140        1578 LOAD_GLOBAL             63 (NULL + FeditBlockEditButton)
-                          1590 PRECALL                  0
-                          1594 CALL                     0
-               
-               139        1604 BUILD_LIST               1
-                          1606 STORE_FAST              10 (items)
-               
-               143        1608 LOAD_GLOBAL             65 (NULL + hooks)
-                          1620 LOAD_ATTR               33 (get_hooks)
-                          1630 LOAD_GLOBAL             68 (CONSTRUCT_BLOCK_TOOLBAR)
-                          1642 PRECALL                  1
-                          1646 CALL                     1
-                          1656 GET_ITER
-                       >> 1658 FOR_ITER                18 (to 1696)
-                          1660 STORE_FAST              11 (hook)
-               
-               144        1662 PUSH_NULL
-                          1664 LOAD_FAST               11 (hook)
-                          1666 LOAD_DEREF              13 (request)
-                          1668 LOAD_FAST               10 (items)
-                          1670 LOAD_DEREF              12 (model)
-                          1672 LOAD_FAST                3 (block_id)
-                          1674 LOAD_FAST                4 (field_name)
-                          1676 KW_NAMES                19
-                          1678 PRECALL                  5
-                          1682 CALL                     5
-                          1692 POP_TOP
-                          1694 JUMP_BACKWARD           19 (to 1658)
-               
-               146     >> 1696 LOAD_CLOSURE            13 (request)
-                          1698 BUILD_TUPLE              1
-                          1700 LOAD_CONST              20 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 146>)
-                          1702 MAKE_FUNCTION            8 (closure)
-                          1704 LOAD_FAST               10 (items)
-                          1706 GET_ITER
-                          1708 PRECALL                  0
-                          1712 CALL                     0
-                          1722 STORE_FAST              10 (items)
-               
-               147        1724 LOAD_GLOBAL             71 (NULL + list)
-                          1736 LOAD_GLOBAL             73 (NULL + filter)
-                          1748 LOAD_CONST               0 (None)
-                          1750 LOAD_FAST               10 (items)
-                          1752 PRECALL                  2
-                          1756 CALL                     2
-                          1766 PRECALL                  1
-                          1770 CALL                     1
-                          1780 STORE_FAST              10 (items)
-               
-               149        1782 LOAD_GLOBAL             75 (NULL + render_to_string)
-               
-               150        1794 LOAD_CONST              21 ('wagtail_fedit/content/editable_block.html')
-               
-               152        1796 PUSH_NULL
-                          1798 LOAD_FAST                0 (self)
-                          1800 LOAD_ATTR               38 (get_edit_url)
-               
-               153        1810 LOAD_FAST                3 (block_id)
-                          1812 LOAD_FAST                4 (field_name)
-               
-               152        1814 BUILD_TUPLE              2
-                          1816 LOAD_CONST              22 ('instance')
-               
-               154        1818 LOAD_DEREF              12 (model)
-               
-               152        1820 BUILD_MAP                1
-               
-               155        1822 LOAD_FAST                5 (extra)
-               
-               152        1824 DICT_MERGE               1
-                          1826 CALL_FUNCTION_EX         1
-               
-               157        1828 LOAD_FAST                9 (admin_edit_url)
-               
-               158        1830 LOAD_FAST                3 (block_id)
-               
-               159        1832 LOAD_DEREF              12 (model)
-               
-               160        1834 LOAD_FAST                8 (rendered)
-               
-               161        1836 LOAD_FAST                4 (field_name)
-               
-               162        1838 LOAD_FAST                1 (context)
-               
-               163        1840 LOAD_FAST               10 (items)
-               
-               151        1842 LOAD_CONST              23 (('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'toolbar_items'))
-                          1844 BUILD_CONST_KEY_MAP      8
-               
-               149        1846 PRECALL                  2
-                          1850 CALL                     2
-                          1860 RETURN_VALUE
+                63     >>  218 LOAD_FAST                4 (field_name)
+                           220 POP_JUMP_FORWARD_IF_TRUE    12 (to 246)
+                           222 LOAD_CONST               1 ('wagtail_fedit_field_name')
+                           224 LOAD_FAST                1 (context)
+                           226 CONTAINS_OP              0
+                           228 POP_JUMP_FORWARD_IF_FALSE     8 (to 246)
+               
+                64         230 LOAD_FAST                1 (context)
+                           232 LOAD_CONST               1 ('wagtail_fedit_field_name')
+                           234 BINARY_SUBSCR
+                           244 STORE_FAST               4 (field_name)
+               
+                66     >>  246 LOAD_GLOBAL             13 (NULL + isinstance)
+                           258 LOAD_FAST                2 (block)
+                           260 LOAD_GLOBAL             14 (FilterExpression)
+                           272 PRECALL                  2
+                           276 CALL                     2
+                           286 POP_JUMP_FORWARD_IF_FALSE    21 (to 330)
+               
+                67         288 LOAD_FAST                2 (block)
+                           290 LOAD_METHOD              8 (resolve)
+                           312 LOAD_FAST                1 (context)
+                           314 PRECALL                  1
+                           318 CALL                     1
+                           328 STORE_FAST               2 (block)
+               
+                68     >>  330 LOAD_GLOBAL             13 (NULL + isinstance)
+                           342 LOAD_FAST                3 (block_id)
+                           344 LOAD_GLOBAL             14 (FilterExpression)
+                           356 PRECALL                  2
+                           360 CALL                     2
+                           370 POP_JUMP_FORWARD_IF_FALSE    21 (to 414)
+               
+                69         372 LOAD_FAST                3 (block_id)
+                           374 LOAD_METHOD              8 (resolve)
+                           396 LOAD_FAST                1 (context)
+                           398 PRECALL                  1
+                           402 CALL                     1
+                           412 STORE_FAST               3 (block_id)
+               
+                70     >>  414 LOAD_GLOBAL             13 (NULL + isinstance)
+                           426 LOAD_FAST                4 (field_name)
+                           428 LOAD_GLOBAL             14 (FilterExpression)
+                           440 PRECALL                  2
+                           444 CALL                     2
+                           454 POP_JUMP_FORWARD_IF_FALSE    21 (to 498)
+               
+                71         456 LOAD_FAST                4 (field_name)
+                           458 LOAD_METHOD              8 (resolve)
+                           480 LOAD_FAST                1 (context)
+                           482 PRECALL                  1
+                           486 CALL                     1
+                           496 STORE_FAST               4 (field_name)
+               
+                72     >>  498 LOAD_GLOBAL             13 (NULL + isinstance)
+                           510 LOAD_DEREF              12 (model)
+                           512 LOAD_GLOBAL             14 (FilterExpression)
+                           524 PRECALL                  2
+                           528 CALL                     2
+                           538 POP_JUMP_FORWARD_IF_FALSE    21 (to 582)
+               
+                73         540 LOAD_DEREF              12 (model)
+                           542 LOAD_METHOD              8 (resolve)
+                           564 LOAD_FAST                1 (context)
+                           566 PRECALL                  1
+                           570 CALL                     1
+                           580 STORE_DEREF             12 (model)
+               
+                76     >>  582 LOAD_FAST                4 (field_name)
+                           584 POP_JUMP_FORWARD_IF_TRUE    15 (to 616)
+               
+                77         586 LOAD_GLOBAL             19 (NULL + ValueError)
+                           598 LOAD_CONST               2 ('Field name is required')
+                           600 PRECALL                  1
+                           604 CALL                     1
+                           614 RAISE_VARARGS            1
+               
+                79     >>  616 LOAD_FAST                3 (block_id)
+                           618 POP_JUMP_FORWARD_IF_TRUE    21 (to 662)
+                           620 LOAD_CONST               3 ('block_id')
+                           622 LOAD_FAST                1 (context)
+                           624 CONTAINS_OP              1
+                           626 POP_JUMP_FORWARD_IF_FALSE    17 (to 662)
+                           628 LOAD_FAST                2 (block)
+                           630 POP_JUMP_FORWARD_IF_TRUE    15 (to 662)
+               
+                80         632 LOAD_GLOBAL             19 (NULL + ValueError)
+                           644 LOAD_CONST               4 ('Block ID is required')
+                           646 PRECALL                  1
+                           650 CALL                     1
+                           660 RAISE_VARARGS            1
+               
+                82     >>  662 LOAD_DEREF              12 (model)
+                           664 POP_JUMP_FORWARD_IF_TRUE    19 (to 704)
+                           666 LOAD_CONST               5 ('wagtail_fedit_instance')
+                           668 LOAD_FAST                1 (context)
+                           670 CONTAINS_OP              1
+                           672 POP_JUMP_FORWARD_IF_FALSE    15 (to 704)
+               
+                83         674 LOAD_GLOBAL             19 (NULL + ValueError)
+                           686 LOAD_CONST               6 ('Model instance is required')
+                           688 PRECALL                  1
+                           692 CALL                     1
+                           702 RAISE_VARARGS            1
+               
+                85     >>  704 LOAD_FAST                4 (field_name)
+                           706 LOAD_FAST                1 (context)
+                           708 LOAD_CONST               1 ('wagtail_fedit_field_name')
+                           710 STORE_SUBSCR
+               
+                86         714 LOAD_DEREF              12 (model)
+                           716 LOAD_FAST                1 (context)
+                           718 LOAD_CONST               5 ('wagtail_fedit_instance')
+                           720 STORE_SUBSCR
+               
+                90         724 LOAD_FAST                2 (block)
+                           726 POP_JUMP_FORWARD_IF_FALSE    88 (to 904)
+               
+                91         728 NOP
+               
+                92         730 LOAD_FAST                1 (context)
+                           732 LOAD_METHOD             10 (flatten)
+                           754 PRECALL                  0
+                           758 CALL                     0
+                           768 STORE_FAST               1 (context)
+                           770 JUMP_FORWARD            16 (to 804)
+                       >>  772 PUSH_EXC_INFO
+               
+                93         774 LOAD_GLOBAL             22 (AttributeError)
+                           786 CHECK_EXC_MATCH
+                           788 POP_JUMP_FORWARD_IF_FALSE     3 (to 796)
+                           790 POP_TOP
+               
+                94         792 POP_EXCEPT
+                           794 JUMP_FORWARD             4 (to 804)
+               
+                93     >>  796 RERAISE                  0
+                       >>  798 COPY                     3
+                           800 POP_EXCEPT
+                           802 RERAISE                  1
+               
+                95     >>  804 LOAD_FAST                1 (context)
+                           806 LOAD_METHOD             12 (update)
+                           828 LOAD_FAST                5 (extra)
+                           830 PRECALL                  1
+                           834 CALL                     1
+                           844 POP_TOP
+               
+                96         846 LOAD_FAST                2 (block)
+                           848 LOAD_METHOD             13 (render_as_block)
+                           870 LOAD_FAST                1 (context)
+                           872 PRECALL                  1
+                           876 CALL                     1
+                           886 STORE_FAST               8 (rendered)
+               
+                97         888 LOAD_CONST               7 (True)
+                           890 LOAD_FAST                0 (self)
+                           892 STORE_ATTR              14 (has_block)
+                           902 JUMP_FORWARD            76 (to 1056)
+               
+                98     >>  904 LOAD_FAST                0 (self)
+                           906 LOAD_ATTR               15 (nl)
+                           916 POP_JUMP_FORWARD_IF_FALSE    54 (to 1026)
+               
+                99         918 LOAD_FAST                0 (self)
+                           920 LOAD_ATTR               15 (nl)
+                           930 LOAD_METHOD             16 (render)
+                           952 LOAD_FAST                1 (context)
+                           954 PRECALL                  1
+                           958 CALL                     1
+                           968 STORE_FAST               8 (rendered)
+               
+               100         970 LOAD_FAST                1 (context)
+                           972 LOAD_METHOD             17 (get)
+                           994 LOAD_CONST               8 ('wagtail_fedit_has_block')
+                           996 LOAD_CONST               9 (False)
+                           998 PRECALL                  2
+                          1002 CALL                     2
+                          1012 LOAD_FAST                0 (self)
+                          1014 STORE_ATTR              14 (has_block)
+                          1024 JUMP_FORWARD            15 (to 1056)
+               
+               102     >> 1026 LOAD_GLOBAL             19 (NULL + ValueError)
+                          1038 LOAD_CONST              10 ('Block or nodelist is required')
+                          1040 PRECALL                  1
+                          1044 CALL                     1
+                          1054 RAISE_VARARGS            1
+               
+               105     >> 1056 LOAD_FAST                3 (block_id)
+                          1058 POP_JUMP_FORWARD_IF_TRUE    13 (to 1086)
+                          1060 LOAD_CONST               3 ('block_id')
+                          1062 LOAD_FAST                1 (context)
+                          1064 CONTAINS_OP              0
+                          1066 POP_JUMP_FORWARD_IF_FALSE     9 (to 1086)
+               
+               106        1068 LOAD_FAST                1 (context)
+                          1070 LOAD_CONST               3 ('block_id')
+                          1072 BINARY_SUBSCR
+                          1082 STORE_FAST               3 (block_id)
+                          1084 JUMP_FORWARD            45 (to 1176)
+               
+               107     >> 1086 LOAD_FAST                3 (block_id)
+                          1088 POP_JUMP_FORWARD_IF_TRUE    26 (to 1142)
+                          1090 LOAD_FAST                2 (block)
+                          1092 POP_JUMP_FORWARD_IF_FALSE    24 (to 1142)
+                          1094 LOAD_GLOBAL             37 (NULL + hasattr)
+                          1106 LOAD_FAST                2 (block)
+                          1108 LOAD_CONST              11 ('id')
+                          1110 PRECALL                  2
+                          1114 CALL                     2
+                          1124 POP_JUMP_FORWARD_IF_FALSE     8 (to 1142)
+               
+               108        1126 LOAD_FAST                2 (block)
+                          1128 LOAD_ATTR               19 (id)
+                          1138 STORE_FAST               3 (block_id)
+                          1140 JUMP_FORWARD            17 (to 1176)
+               
+               109     >> 1142 LOAD_FAST                3 (block_id)
+                          1144 POP_JUMP_FORWARD_IF_TRUE    15 (to 1176)
+               
+               110        1146 LOAD_GLOBAL             19 (NULL + ValueError)
+                          1158 LOAD_CONST               4 ('Block ID is required')
+                          1160 PRECALL                  1
+                          1164 CALL                     1
+                          1174 RAISE_VARARGS            1
+               
+               115     >> 1176 LOAD_DEREF              12 (model)
+                          1178 JUMP_IF_TRUE_OR_POP      7 (to 1194)
+                          1180 LOAD_FAST                1 (context)
+                          1182 LOAD_CONST               5 ('wagtail_fedit_instance')
+                          1184 BINARY_SUBSCR
+                       >> 1194 STORE_DEREF             12 (model)
+               
+               118        1196 LOAD_FAST                1 (context)
+                          1198 LOAD_METHOD             17 (get)
+                          1220 LOAD_CONST              12 ('request')
+                          1222 PRECALL                  1
+                          1226 CALL                     1
+                          1236 STORE_DEREF             13 (request)
+               
+               119        1238 LOAD_DEREF              13 (request)
+                          1240 POP_JUMP_FORWARD_IF_FALSE   113 (to 1468)
+               
+               121        1242 LOAD_DEREF              13 (request)
+                          1244 LOAD_ATTR               20 (user)
+                          1254 LOAD_ATTR               21 (is_authenticated)
+               
+               120        1264 POP_JUMP_FORWARD_IF_FALSE    99 (to 1464)
+               
+               122        1266 LOAD_DEREF              13 (request)
+                          1268 LOAD_ATTR               20 (user)
+                          1278 LOAD_METHOD             22 (has_perm)
+                          1300 LOAD_CONST              13 ('wagtailadmin.access_admin')
+                          1302 PRECALL                  1
+                          1306 CALL                     1
+               
+               120        1316 POP_JUMP_FORWARD_IF_FALSE    73 (to 1464)
+               
+               123        1318 LOAD_DEREF              13 (request)
+                          1320 LOAD_ATTR               20 (user)
+                          1330 LOAD_METHOD             22 (has_perm)
+                          1352 LOAD_DEREF              12 (model)
+                          1354 LOAD_ATTR               23 (_meta)
+                          1364 LOAD_ATTR               24 (app_label)
+                          1374 FORMAT_VALUE             0
+                          1376 LOAD_CONST              14 ('.change_')
+                          1378 LOAD_DEREF              12 (model)
+                          1380 LOAD_ATTR               23 (_meta)
+                          1390 LOAD_ATTR               25 (model_name)
+                          1400 FORMAT_VALUE             0
+                          1402 BUILD_STRING             3
+                          1404 PRECALL                  1
+                          1408 CALL                     1
+               
+               120        1418 POP_JUMP_FORWARD_IF_FALSE    22 (to 1464)
+               
+               124        1420 LOAD_GLOBAL             53 (NULL + getattr)
+                          1432 LOAD_DEREF              13 (request)
+                          1434 LOAD_GLOBAL             54 (FEDIT_PREVIEW_VAR)
+                          1446 LOAD_CONST               9 (False)
+                          1448 PRECALL                  3
+                          1452 CALL                     3
+               
+               120        1462 POP_JUMP_FORWARD_IF_TRUE     2 (to 1468)
+               
+               127     >> 1464 LOAD_FAST                8 (rendered)
+                          1466 RETURN_VALUE
+               
+               131     >> 1468 LOAD_GLOBAL             13 (NULL + isinstance)
+                          1480 LOAD_DEREF              12 (model)
+                          1482 LOAD_GLOBAL             56 (Page)
+                          1494 PRECALL                  2
+                          1498 CALL                     2
+                          1508 POP_JUMP_FORWARD_IF_FALSE    29 (to 1568)
+               
+               132        1510 LOAD_GLOBAL             59 (NULL + _get_from_context_or_set)
+               
+               133        1522 LOAD_FAST                1 (context)
+                          1524 LOAD_CONST              15 ('page_base_edit_url')
+               
+               134        1526 LOAD_CLOSURE            12 (model)
+                          1528 BUILD_TUPLE              1
+                          1530 LOAD_CONST              16 (<code object <lambda>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 134>)
+                          1532 MAKE_FUNCTION            8 (closure)
+               
+               132        1534 PRECALL                  3
+                          1538 CALL                     3
+                          1548 STORE_FAST               9 (admin_edit_url)
+               
+               139        1550 LOAD_FAST                9 (admin_edit_url)
+                          1552 FORMAT_VALUE             0
+                          1554 LOAD_CONST              17 ('#block-')
+                          1556 LOAD_FAST                3 (block_id)
+                          1558 FORMAT_VALUE             0
+                          1560 LOAD_CONST              18 ('-section')
+                          1562 BUILD_STRING             4
+                          1564 STORE_FAST               9 (admin_edit_url)
+                          1566 JUMP_FORWARD             2 (to 1572)
+               
+               141     >> 1568 LOAD_CONST               0 (None)
+                          1570 STORE_FAST               9 (admin_edit_url)
+               
+               143     >> 1572 LOAD_FAST                5 (extra)
+                          1574 LOAD_METHOD             30 (setdefault)
+                          1596 LOAD_CONST              19 ('has_block')
+                          1598 LOAD_FAST                0 (self)
+                          1600 LOAD_ATTR               14 (has_block)
+                          1610 PRECALL                  2
+                          1614 CALL                     2
+                          1624 POP_TOP
+               
+               146        1626 LOAD_GLOBAL             63 (NULL + FeditBlockEditButton)
+                          1638 PRECALL                  0
+                          1642 CALL                     0
+               
+               145        1652 BUILD_LIST               1
+                          1654 STORE_FAST              10 (items)
+               
+               149        1656 LOAD_GLOBAL             65 (NULL + hooks)
+                          1668 LOAD_ATTR               33 (get_hooks)
+                          1678 LOAD_GLOBAL             68 (CONSTRUCT_BLOCK_TOOLBAR)
+                          1690 PRECALL                  1
+                          1694 CALL                     1
+                          1704 GET_ITER
+                       >> 1706 FOR_ITER                18 (to 1744)
+                          1708 STORE_FAST              11 (hook)
+               
+               150        1710 PUSH_NULL
+                          1712 LOAD_FAST               11 (hook)
+                          1714 LOAD_DEREF              13 (request)
+                          1716 LOAD_FAST               10 (items)
+                          1718 LOAD_DEREF              12 (model)
+                          1720 LOAD_FAST                3 (block_id)
+                          1722 LOAD_FAST                4 (field_name)
+                          1724 KW_NAMES                20
+                          1726 PRECALL                  5
+                          1730 CALL                     5
+                          1740 POP_TOP
+                          1742 JUMP_BACKWARD           19 (to 1706)
+               
+               152     >> 1744 LOAD_CLOSURE            13 (request)
+                          1746 BUILD_TUPLE              1
+                          1748 LOAD_CONST              21 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 152>)
+                          1750 MAKE_FUNCTION            8 (closure)
+                          1752 LOAD_FAST               10 (items)
+                          1754 GET_ITER
+                          1756 PRECALL                  0
+                          1760 CALL                     0
+                          1770 STORE_FAST              10 (items)
+               
+               153        1772 LOAD_GLOBAL             71 (NULL + list)
+                          1784 LOAD_GLOBAL             73 (NULL + filter)
+                          1796 LOAD_CONST               0 (None)
+                          1798 LOAD_FAST               10 (items)
+                          1800 PRECALL                  2
+                          1804 CALL                     2
+                          1814 PRECALL                  1
+                          1818 CALL                     1
+                          1828 STORE_FAST              10 (items)
+               
+               155        1830 LOAD_GLOBAL             75 (NULL + render_to_string)
+               
+               156        1842 LOAD_CONST              22 ('wagtail_fedit/content/editable_block.html')
+               
+               158        1844 PUSH_NULL
+                          1846 LOAD_FAST                0 (self)
+                          1848 LOAD_ATTR               38 (get_edit_url)
+               
+               159        1858 LOAD_FAST                3 (block_id)
+                          1860 LOAD_FAST                4 (field_name)
+               
+               158        1862 BUILD_TUPLE              2
+                          1864 LOAD_CONST              23 ('instance')
+               
+               160        1866 LOAD_DEREF              12 (model)
+               
+               158        1868 BUILD_MAP                1
+               
+               161        1870 LOAD_FAST                5 (extra)
+               
+               158        1872 DICT_MERGE               1
+                          1874 CALL_FUNCTION_EX         1
+               
+               163        1876 LOAD_FAST                9 (admin_edit_url)
+               
+               164        1878 LOAD_FAST                3 (block_id)
+               
+               165        1880 LOAD_DEREF              12 (model)
+               
+               166        1882 LOAD_FAST                8 (rendered)
+               
+               167        1884 LOAD_FAST                4 (field_name)
+               
+               168        1886 LOAD_FAST                1 (context)
+               
+               169        1888 LOAD_FAST                4 (field_name)
+               
+               170        1890 LOAD_DEREF              12 (model)
+               
+               171        1892 LOAD_FAST               10 (items)
+               
+               157        1894 LOAD_CONST              24 (('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items'))
+                          1896 BUILD_CONST_KEY_MAP     10
+               
+               155        1898 PRECALL                  2
+                          1902 CALL                     2
+                          1912 RETURN_VALUE
                ExceptionTable:
-                 682 to 720 -> 724 [0]
-                 724 to 742 -> 750 [1] lasti
-                 748 to 748 -> 750 [1] lasti
+                 730 to 768 -> 772 [0]
+                 772 to 790 -> 798 [1] lasti
+                 796 to 796 -> 798 [1] lasti
                consts
                   None
+                  'wagtail_fedit_field_name'
                   'Field name is required'
                   'block_id'
                   'Block ID is required'
                   'wagtail_fedit_instance'
                   'Model instance is required'
                   True
                   'wagtail_fedit_has_block'
@@ -1000,38 +1028,38 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x95019700740100000000000000000000640189006a0100000000000000
                         006701ac02a6020000ab0200000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                     128           2 RESUME                   0
+                     134           2 RESUME                   0
                                    4 LOAD_GLOBAL              1 (NULL + reverse)
                      
-                     129          16 LOAD_CONST               1 ('wagtailadmin_pages:edit')
+                     135          16 LOAD_CONST               1 ('wagtailadmin_pages:edit')
                      
-                     130          18 LOAD_DEREF               0 (model)
+                     136          18 LOAD_DEREF               0 (model)
                                   20 LOAD_ATTR                1 (id)
                                   30 BUILD_LIST               1
                      
-                     128          32 KW_NAMES                 2
+                     134          32 KW_NAMES                 2
                                   34 PRECALL                  2
                                   38 CALL                     2
                                   48 RETURN_VALUE
                      consts
                         None
                         'wagtailadmin_pages:edit'
                         ('args',)
                      names      ('reverse', 'id')
                      varnames   ()
                      freevars   ('model',)
                      cellvars   ()
                      filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<lambda>'
-                     firstlineno 128
+                     firstlineno 134
                      lnotab 0x100102010efe
                   '#block-'
                   '-section'
                   'has_block'
                   ('request', 'items', 'model', 'block_id', 'field_name')
                   code
                      argcount  : 1
@@ -1039,15 +1067,15 @@
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d177d017c01a00000000000000000000000000000
                         000000000000008902a6010000ab01000000000000000091028c185300
                                    0 COPY_FREE_VARS           1
                      
-                     146           2 RESUME                   0
+                     152           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                23 (to 56)
                                   10 STORE_FAST               1 (item)
                                   12 LOAD_FAST                1 (item)
                                   14 LOAD_METHOD              0 (render)
                                   36 LOAD_DEREF               2 (request)
@@ -1059,84 +1087,85 @@
                      consts
                      names      ('render',)
                      varnames   ('.0', 'item')
                      freevars   ('request',)
                      cellvars   ()
                      filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<listcomp>'
-                     firstlineno 146
+                     firstlineno 152
                      lnotab 0x
                   'wagtail_fedit/content/editable_block.html'
                   'instance'
-                  ('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'toolbar_items')
+                  ('edit_url', 'admin_edit_url', 'block_id', 'model', 'content', 'field_name', 'parent_context', 'wagtail_fedit_field_name', 'wagtail_fedit_instance', 'toolbar_items')
                names      ('block', 'block_id', 'field_name', 'model', 'extra', 'items', 'isinstance', 'FilterExpression', 'resolve', 'ValueError', 'flatten', 'AttributeError', 'update', 'render_as_block', 'has_block', 'nl', 'render', 'get', 'hasattr', 'id', 'user', 'is_authenticated', 'has_perm', '_meta', 'app_label', 'model_name', 'getattr', 'FEDIT_PREVIEW_VAR', 'Page', '_get_from_context_or_set', 'setdefault', 'FeditBlockEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_BLOCK_TOOLBAR', 'list', 'filter', 'render_to_string', 'get_edit_url')
                varnames   ('self', 'context', 'block', 'block_id', 'field_name', 'extra', 'k', 'e', 'rendered', 'admin_edit_url', 'items', 'hook')
                freevars   ()
                cellvars   ('model', 'request')
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'render'
                firstlineno 51
                lnotab
-                  0x06010e010e010e010e010e0332012a0132022a012a012a012a012a012a
-                  012a012a0304011e0210011e020c011e04040102012c01120104ff08022a
-                  012a0110010e01340138021e030c0112012801100104011e0514032a0104
-                  0216ff020232fe020364fd02042afc020704042a010c01040108fe100712
-                  02040236031aff0404360122021c013a020c0102020e0104ff040202fe02
-                  0302fd040502010201020102010201020102f404fe
+                  0x06010e010e010e010e010e0332012a0132020c0110022a012a012a012a
+                  012a012a012a012a0304011e0210011e020c011e020a010a04040102012c
+                  01120104ff08022a012a0110010e01340138021e030c0112012801100104
+                  011e0514032a01040216ff020232fe020364fd02042afc020704042a010c
+                  01040108fe10071202040236031aff0404360122021c013a020c0102020e
+                  0104ff040202fe020302fd04050201020102010201020102010201020102
+                  f204fe
             'return'
             code
                argcount  : 0
                nlocals   : 4
                stacksize : 6
                flags     : 11
                code
                   0x970069007d017c00a00000000000000000000000000000000000000000
                   00a6000000ab00000000000000000044005d2f5c0200007d027d03740200
                   000000000000000000a00200000000000000000000000000000000000000
                   007407000000000000000000007c03a6010000ab010000000000000000a6
                   010000ab0100000000000000007c017c023c0000008c307c015300
-               167           0 RESUME                   0
+               175           0 RESUME                   0
                
-               170           2 BUILD_MAP                0
+               178           2 BUILD_MAP                0
                              4 STORE_FAST               1 (packed)
                
-               171           6 LOAD_FAST                0 (kwargs)
+               179           6 LOAD_FAST                0 (kwargs)
                              8 LOAD_METHOD              0 (items)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 GET_ITER
                        >>   46 FOR_ITER                47 (to 142)
                             48 UNPACK_SEQUENCE          2
                             52 STORE_FAST               2 (k)
                             54 STORE_FAST               3 (v)
                
-               172          56 LOAD_GLOBAL              2 (url_value_signer)
+               180          56 LOAD_GLOBAL              2 (url_value_signer)
                             68 LOAD_METHOD              2 (sign)
                             90 LOAD_GLOBAL              7 (NULL + str)
                            102 LOAD_FAST                3 (v)
                            104 PRECALL                  1
                            108 CALL                     1
                            118 PRECALL                  1
                            122 CALL                     1
                            132 LOAD_FAST                1 (packed)
                            134 LOAD_FAST                2 (k)
                            136 STORE_SUBSCR
                            140 JUMP_BACKWARD           48 (to 46)
                
-               174     >>  142 LOAD_FAST                1 (packed)
+               182     >>  142 LOAD_FAST                1 (packed)
                            144 RETURN_VALUE
                consts
                   None
                names      ('items', 'url_value_signer', 'sign', 'str')
                varnames   ('kwargs', 'packed', 'k', 'v')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'pack'
-               firstlineno 167
+               firstlineno 175
                lnotab 0x0203040132015602
             ('request',)
             'expected'
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 7
@@ -1157,130 +1186,130 @@
                   057c039b009d02a6010000ab010000000000000000820177007803590077
                   0174150000000000000000000088046601640684087c024400a6000000ab
                   000000000000000000a6010000ab01000000000000000073187c00a00700
                   0000000000000000000000000000000000000064057c039b009d02a60100
                   00ab010000000000000000820189045300
                              0 MAKE_CELL                4 (unpacked)
                
-               176           2 RESUME                   0
+               184           2 RESUME                   0
                
-               178           4 LOAD_FAST                1 (request)
+               186           4 LOAD_FAST                1 (request)
                              6 POP_JUMP_FORWARD_IF_TRUE    15 (to 38)
                
-               179           8 LOAD_GLOBAL              1 (NULL + ValueError)
+               187           8 LOAD_GLOBAL              1 (NULL + ValueError)
                             20 LOAD_CONST               1 ('Request is required')
                             22 PRECALL                  1
                             26 CALL                     1
                             36 RAISE_VARARGS            1
                
-               181     >>   38 BUILD_MAP                0
+               189     >>   38 BUILD_MAP                0
                             40 STORE_DEREF              4 (unpacked)
                
-               182          42 LOAD_FAST                2 (expected)
+               190          42 LOAD_FAST                2 (expected)
                             44 GET_ITER
                        >>   46 FOR_ITER               171 (to 390)
                             48 STORE_FAST               3 (key)
                
-               183          50 NOP
+               191          50 NOP
                
-               184          52 LOAD_GLOBAL              2 (url_value_signer)
+               192          52 LOAD_GLOBAL              2 (url_value_signer)
                             64 LOAD_METHOD              2 (unsign)
                
-               185          86 LOAD_FAST                1 (request)
+               193          86 LOAD_FAST                1 (request)
                             88 LOAD_ATTR                3 (GET)
                             98 LOAD_METHOD              4 (get)
                            120 LOAD_FAST                3 (key)
                            122 PRECALL                  1
                            126 CALL                     1
                
-               184         136 PRECALL                  1
+               192         136 PRECALL                  1
                            140 CALL                     1
                            150 LOAD_DEREF               4 (unpacked)
                            152 LOAD_FAST                3 (key)
                            154 STORE_SUBSCR
                            158 JUMP_BACKWARD           57 (to 46)
                        >>  160 PUSH_EXC_INFO
                
-               187         162 LOAD_GLOBAL             10 (signing)
+               195         162 LOAD_GLOBAL             10 (signing)
                            174 LOAD_ATTR                6 (SignatureExpired)
                            184 CHECK_EXC_MATCH
                            186 POP_JUMP_FORWARD_IF_FALSE    26 (to 240)
                            188 POP_TOP
                
-               188         190 LOAD_FAST                0 (cls)
+               196         190 LOAD_FAST                0 (cls)
                            192 LOAD_METHOD              7 (UnpackError)
                            214 LOAD_CONST               2 ('Value for ')
                            216 LOAD_FAST                3 (key)
                            218 FORMAT_VALUE             0
                            220 LOAD_CONST               3 (' has expired')
                            222 BUILD_STRING             3
                            224 PRECALL                  1
                            228 CALL                     1
                            238 RAISE_VARARGS            1
                
-               189     >>  240 LOAD_GLOBAL             10 (signing)
+               197     >>  240 LOAD_GLOBAL             10 (signing)
                            252 LOAD_ATTR                8 (BadSignature)
                            262 CHECK_EXC_MATCH
                            264 POP_JUMP_FORWARD_IF_FALSE    25 (to 316)
                            266 POP_TOP
                
-               190         268 LOAD_FAST                0 (cls)
+               198         268 LOAD_FAST                0 (cls)
                            270 LOAD_METHOD              7 (UnpackError)
                            292 LOAD_CONST               4 ('Invalid value for ')
                            294 LOAD_FAST                3 (key)
                            296 FORMAT_VALUE             0
                            298 BUILD_STRING             2
                            300 PRECALL                  1
                            304 CALL                     1
                            314 RAISE_VARARGS            1
                
-               191     >>  316 LOAD_GLOBAL             18 (TypeError)
+               199     >>  316 LOAD_GLOBAL             18 (TypeError)
                            328 CHECK_EXC_MATCH
                            330 POP_JUMP_FORWARD_IF_FALSE    25 (to 382)
                            332 POP_TOP
                
-               192         334 LOAD_FAST                0 (cls)
+               200         334 LOAD_FAST                0 (cls)
                            336 LOAD_METHOD              7 (UnpackError)
                            358 LOAD_CONST               5 ('Missing value for ')
                            360 LOAD_FAST                3 (key)
                            362 FORMAT_VALUE             0
                            364 BUILD_STRING             2
                            366 PRECALL                  1
                            370 CALL                     1
                            380 RAISE_VARARGS            1
                
-               191     >>  382 RERAISE                  0
+               199     >>  382 RERAISE                  0
                        >>  384 COPY                     3
                            386 POP_EXCEPT
                            388 RERAISE                  1
                
-               194     >>  390 LOAD_GLOBAL             21 (NULL + all)
+               202     >>  390 LOAD_GLOBAL             21 (NULL + all)
                            402 LOAD_CLOSURE             4 (unpacked)
                            404 BUILD_TUPLE              1
-                           406 LOAD_CONST               6 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 194>)
+                           406 LOAD_CONST               6 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 202>)
                            408 MAKE_FUNCTION            8 (closure)
                            410 LOAD_FAST                2 (expected)
                            412 GET_ITER
                            414 PRECALL                  0
                            418 CALL                     0
                            428 PRECALL                  1
                            432 CALL                     1
                            442 POP_JUMP_FORWARD_IF_TRUE    24 (to 492)
                
-               195         444 LOAD_FAST                0 (cls)
+               203         444 LOAD_FAST                0 (cls)
                            446 LOAD_METHOD              7 (UnpackError)
                            468 LOAD_CONST               5 ('Missing value for ')
                            470 LOAD_FAST                3 (key)
                            472 FORMAT_VALUE             0
                            474 BUILD_STRING             2
                            476 PRECALL                  1
                            480 CALL                     1
                            490 RAISE_VARARGS            1
                
-               197     >>  492 LOAD_DEREF               4 (unpacked)
+               205     >>  492 LOAD_DEREF               4 (unpacked)
                            494 RETURN_VALUE
                ExceptionTable:
                  52 to 156 -> 160 [1]
                  160 to 382 -> 384 [2] lasti
                consts
                   None
                   'Request is required'
@@ -1294,15 +1323,15 @@
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d177d018902a00000000000000000000000000000
                         000000000000007c01a6010000ab01000000000000000091028c185300
                                    0 COPY_FREE_VARS           1
                      
-                     194           2 RESUME                   0
+                     202           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                23 (to 56)
                                   10 STORE_FAST               1 (key)
                                   12 LOAD_DEREF               2 (unpacked)
                                   14 LOAD_METHOD              0 (get)
                                   36 LOAD_FAST                1 (key)
@@ -1314,23 +1343,23 @@
                      consts
                      names      ('get',)
                      varnames   ('.0', 'key')
                      freevars   ('unpacked',)
                      cellvars   ()
                      filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                      name       '<listcomp>'
-                     firstlineno 194
+                     firstlineno 202
                      lnotab 0x
                names      ('ValueError', 'url_value_signer', 'unsign', 'GET', 'get', 'signing', 'SignatureExpired', 'UnpackError', 'BadSignature', 'TypeError', 'all')
                varnames   ('cls', 'request', 'expected', 'key')
                freevars   ()
                cellvars   ('unpacked',)
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'unpack'
-               firstlineno 176
+               firstlineno 184
                lnotab
                   0x040204011e02040108010201220132ff1a031c0132011c013001120130
                   ff080336013002
             'instance'
             code
                argcount  : 3
                nlocals   : 6
@@ -1339,58 +1368,58 @@
                code
                   0x970074010000000000000000000064017c007c017c026a010000000000
                   0000006a0200000000000000007c026a0100000000000000006a03000000
                   00000000007c026a0400000000000000006705ac02a6020000ab02000000
                   00000000007d047c0373027c045300740b00000000000000000000740d00
                   0000000000000000006a070000000000000000640469007c03a4018e01a6
                   010000ab0100000000000000007d057c049b0064037c059b009d035300
-               199           0 RESUME                   0
+               207           0 RESUME                   0
                
-               201           2 LOAD_GLOBAL              1 (NULL + reverse)
+               209           2 LOAD_GLOBAL              1 (NULL + reverse)
                
-               202          14 LOAD_CONST               1 ('wagtail_fedit:edit_block')
+               210          14 LOAD_CONST               1 ('wagtail_fedit:edit_block')
                
-               203          16 LOAD_FAST                0 (block_id)
+               211          16 LOAD_FAST                0 (block_id)
                             18 LOAD_FAST                1 (field_name)
                             20 LOAD_FAST                2 (instance)
                             22 LOAD_ATTR                1 (_meta)
                             32 LOAD_ATTR                2 (app_label)
                             42 LOAD_FAST                2 (instance)
                             44 LOAD_ATTR                1 (_meta)
                             54 LOAD_ATTR                3 (model_name)
                             64 LOAD_FAST                2 (instance)
                             66 LOAD_ATTR                4 (pk)
                             76 BUILD_LIST               5
                
-               201          78 KW_NAMES                 2
+               209          78 KW_NAMES                 2
                             80 PRECALL                  2
                             84 CALL                     2
                             94 STORE_FAST               4 (base_url)
                
-               206          96 LOAD_FAST                3 (kwargs)
+               214          96 LOAD_FAST                3 (kwargs)
                             98 POP_JUMP_FORWARD_IF_TRUE     2 (to 104)
                
-               207         100 LOAD_FAST                4 (base_url)
+               215         100 LOAD_FAST                4 (base_url)
                            102 RETURN_VALUE
                
-               209     >>  104 LOAD_GLOBAL             11 (NULL + urlencode)
+               217     >>  104 LOAD_GLOBAL             11 (NULL + urlencode)
                
-               210         116 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+               218         116 LOAD_GLOBAL             13 (NULL + BlockEditNode)
                            128 LOAD_ATTR                7 (pack)
                            138 LOAD_CONST               4 (())
                            140 BUILD_MAP                0
                            142 LOAD_FAST                3 (kwargs)
                            144 DICT_MERGE               1
                            146 CALL_FUNCTION_EX         1
                
-               209         148 PRECALL                  1
+               217         148 PRECALL                  1
                            152 CALL                     1
                            162 STORE_FAST               5 (packed)
                
-               212         164 LOAD_FAST                4 (base_url)
+               220         164 LOAD_FAST                4 (base_url)
                            166 FORMAT_VALUE             0
                            168 LOAD_CONST               3 ('?')
                            170 LOAD_FAST                5 (packed)
                            172 FORMAT_VALUE             0
                            174 BUILD_STRING             3
                            176 RETURN_VALUE
                consts
@@ -1401,27 +1430,27 @@
                   ()
                names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack')
                varnames   ('block_id', 'field_name', 'instance', 'kwargs', 'base_url', 'packed')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       'get_edit_url'
-               firstlineno 199
+               firstlineno 207
                lnotab 0x02020c0102013efe1205040104020c0120ff1003
             (None, None, None, None, None)
          names      ('__name__', '__module__', '__qualname__', 'Exception', 'UnpackError', 'NodeList', 'BoundBlock', 'str', 'models', 'Model', '__init__', 'render', 'staticmethod', 'dict', 'pack', 'classmethod', 'unpack', 'get_edit_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'BlockEditNode'
          firstlineno 31
          lnotab
             0x0a011c04020102010201020102fb040102ff020202fe020302fd020402
-            fc02050cfb0810067402010aff0e010208020114ff0e010216020120ff0e
+            fc02050cfb0810067c02010aff0e010208020114ff0e010216020120ff0e
             01
       'BlockEditNode'
       'fedit_block'
       ('name',)
       'parser'
       'token'
       code
@@ -1430,173 +1459,160 @@
          stacksize : 10
          flags     : 3
          code
             0x97007c01a0000000000000000000000000000000000000000000a60000
             00ab0000000000000000007d027c02a00100000000000000000000000000
             000000000000006401a6010000ab0100000000000000007d0367006402a2
             017d047405000000000000000000007c007c047c02a6030000ab03000000
-            00000000007d0564037c057601720f7407000000000000000000006404a6
-            010000ab010000000000000000820164057c057601722a7c00a004000000
+            00000000007d0564037c057601722a7c00a0030000000000000000000000
+            0000000000000000006404a6010000ab0100000000000000007d067c00a0
+            040000000000000000000000000000000000000000a6000000ab00000000
+            000000000001006e0264057d0669007d077c05a005000000000000000000
+            0000000000000000000000a6000000ab00000000000000000044005d0e5c
+            0200007d087d097c087c04760172057c097c077c083c0000008c0f740d00
+            000000000000000000640a7c067c05a00700000000000000000000000000
+            000000000000006403a6010000ab0100000000000000007c05a007000000
             00000000000000000000000000000000006406a6010000ab010000000000
-            0000007d067c00a0050000000000000000000000000000000000000000a6
-            000000ab00000000000000000001006e0264077d0669007d077c05a00600
-            00000000000000000000000000000000000000a6000000ab000000000000
-            00000044005d0e5c0200007d087d097c087c04760172057c097c077c083c
-            0000008c0f740f00000000000000000000640b7c067c05a0080000000000
-            0000000000000000000000000000006405a6010000ab0100000000000000
-            007c05a00800000000000000000000000000000000000000006408a60100
-            00ab0100000000000000007c05a008000000000000000000000000000000
-            00000000006403a6010000ab0100000000000000007c05a0080000000000
-            0000000000000000000000000000006409a6010000ab0100000000000000
-            00640a9c057c07a4018e015300
-         216           0 RESUME                   0
+            0000007c05a00700000000000000000000000000000000000000006407a6
+            010000ab0100000000000000007c05a00700000000000000000000000000
+            000000000000006408a6010000ab01000000000000000064099c057c07a4
+            018e015300
+         224           0 RESUME                   0
          
-         246           2 LOAD_FAST                1 (token)
+         254           2 LOAD_FAST                1 (token)
                        4 LOAD_METHOD              0 (split_contents)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 STORE_FAST               2 (tokens)
          
-         247          42 LOAD_FAST                2 (tokens)
+         255          42 LOAD_FAST                2 (tokens)
                       44 LOAD_METHOD              1 (pop)
                       66 LOAD_CONST               1 (0)
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               3 (_)
          
-         248          84 BUILD_LIST               0
+         256          84 BUILD_LIST               0
                       86 LOAD_CONST               2 (('block', 'block_id', 'field_name', 'model'))
                       88 LIST_EXTEND              1
                       90 STORE_FAST               4 (kwargs_names)
          
-         253          92 LOAD_GLOBAL              5 (NULL + get_kwargs)
+         261          92 LOAD_GLOBAL              5 (NULL + get_kwargs)
                      104 LOAD_FAST                0 (parser)
                      106 LOAD_FAST                4 (kwargs_names)
                      108 LOAD_FAST                2 (tokens)
                      110 PRECALL                  3
                      114 CALL                     3
                      124 STORE_FAST               5 (kwargs)
          
-         254         126 LOAD_CONST               3 ('field_name')
+         263         126 LOAD_CONST               3 ('block')
                      128 LOAD_FAST                5 (kwargs)
                      130 CONTAINS_OP              1
-                     132 POP_JUMP_FORWARD_IF_FALSE    15 (to 164)
+                     132 POP_JUMP_FORWARD_IF_FALSE    42 (to 218)
          
-         255         134 LOAD_GLOBAL              7 (NULL + ValueError)
-                     146 LOAD_CONST               4 ('Field name is required')
-                     148 PRECALL                  1
-                     152 CALL                     1
-                     162 RAISE_VARARGS            1
-         
-         257     >>  164 LOAD_CONST               5 ('block')
-                     166 LOAD_FAST                5 (kwargs)
-                     168 CONTAINS_OP              1
-                     170 POP_JUMP_FORWARD_IF_FALSE    42 (to 256)
-         
-         258         172 LOAD_FAST                0 (parser)
-                     174 LOAD_METHOD              4 (parse)
-                     196 LOAD_CONST               6 (('unfedit_block',))
-                     198 PRECALL                  1
-                     202 CALL                     1
-                     212 STORE_FAST               6 (nodelist)
-         
-         259         214 LOAD_FAST                0 (parser)
-                     216 LOAD_METHOD              5 (delete_first_token)
-                     238 PRECALL                  0
-                     242 CALL                     0
-                     252 POP_TOP
-                     254 JUMP_FORWARD             2 (to 260)
-         
-         261     >>  256 LOAD_CONST               7 (None)
-                     258 STORE_FAST               6 (nodelist)
-         
-         263     >>  260 BUILD_MAP                0
-                     262 STORE_FAST               7 (extra)
-         
-         264         264 LOAD_FAST                5 (kwargs)
-                     266 LOAD_METHOD              6 (items)
-                     288 PRECALL                  0
-                     292 CALL                     0
-                     302 GET_ITER
-                 >>  304 FOR_ITER                14 (to 334)
-                     306 UNPACK_SEQUENCE          2
-                     310 STORE_FAST               8 (key)
-                     312 STORE_FAST               9 (value)
-         
-         265         314 LOAD_FAST                8 (key)
-                     316 LOAD_FAST                4 (kwargs_names)
-                     318 CONTAINS_OP              1
-                     320 POP_JUMP_FORWARD_IF_FALSE     5 (to 332)
-         
-         266         322 LOAD_FAST                9 (value)
-                     324 LOAD_FAST                7 (extra)
-                     326 LOAD_FAST                8 (key)
-                     328 STORE_SUBSCR
-                 >>  332 JUMP_BACKWARD           15 (to 304)
-         
-         268     >>  334 LOAD_GLOBAL             15 (NULL + BlockEditNode)
-                     346 LOAD_CONST              11 (())
-         
-         269         348 LOAD_FAST                6 (nodelist)
-         
-         270         350 LOAD_FAST                5 (kwargs)
-                     352 LOAD_METHOD              8 (get)
-                     374 LOAD_CONST               5 ('block')
-                     376 PRECALL                  1
-                     380 CALL                     1
-         
-         271         390 LOAD_FAST                5 (kwargs)
-                     392 LOAD_METHOD              8 (get)
-                     414 LOAD_CONST               8 ('block_id')
-                     416 PRECALL                  1
-                     420 CALL                     1
-         
-         272         430 LOAD_FAST                5 (kwargs)
-                     432 LOAD_METHOD              8 (get)
-                     454 LOAD_CONST               3 ('field_name')
-                     456 PRECALL                  1
-                     460 CALL                     1
-         
-         273         470 LOAD_FAST                5 (kwargs)
-                     472 LOAD_METHOD              8 (get)
-                     494 LOAD_CONST               9 ('model')
-                     496 PRECALL                  1
-                     500 CALL                     1
-         
-         268         510 LOAD_CONST              10 (('nodelist', 'block', 'block_id', 'field_name', 'model'))
-                     512 BUILD_CONST_KEY_MAP      5
-         
-         274         514 LOAD_FAST                7 (extra)
-         
-         268         516 DICT_MERGE               1
-                     518 CALL_FUNCTION_EX         1
-                     520 RETURN_VALUE
+         264         134 LOAD_FAST                0 (parser)
+                     136 LOAD_METHOD              3 (parse)
+                     158 LOAD_CONST               4 (('unfedit_block',))
+                     160 PRECALL                  1
+                     164 CALL                     1
+                     174 STORE_FAST               6 (nodelist)
+         
+         265         176 LOAD_FAST                0 (parser)
+                     178 LOAD_METHOD              4 (delete_first_token)
+                     200 PRECALL                  0
+                     204 CALL                     0
+                     214 POP_TOP
+                     216 JUMP_FORWARD             2 (to 222)
+         
+         267     >>  218 LOAD_CONST               5 (None)
+                     220 STORE_FAST               6 (nodelist)
+         
+         269     >>  222 BUILD_MAP                0
+                     224 STORE_FAST               7 (extra)
+         
+         270         226 LOAD_FAST                5 (kwargs)
+                     228 LOAD_METHOD              5 (items)
+                     250 PRECALL                  0
+                     254 CALL                     0
+                     264 GET_ITER
+                 >>  266 FOR_ITER                14 (to 296)
+                     268 UNPACK_SEQUENCE          2
+                     272 STORE_FAST               8 (key)
+                     274 STORE_FAST               9 (value)
+         
+         271         276 LOAD_FAST                8 (key)
+                     278 LOAD_FAST                4 (kwargs_names)
+                     280 CONTAINS_OP              1
+                     282 POP_JUMP_FORWARD_IF_FALSE     5 (to 294)
+         
+         272         284 LOAD_FAST                9 (value)
+                     286 LOAD_FAST                7 (extra)
+                     288 LOAD_FAST                8 (key)
+                     290 STORE_SUBSCR
+                 >>  294 JUMP_BACKWARD           15 (to 266)
+         
+         274     >>  296 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+                     308 LOAD_CONST              10 (())
+         
+         275         310 LOAD_FAST                6 (nodelist)
+         
+         276         312 LOAD_FAST                5 (kwargs)
+                     314 LOAD_METHOD              7 (get)
+                     336 LOAD_CONST               3 ('block')
+                     338 PRECALL                  1
+                     342 CALL                     1
+         
+         277         352 LOAD_FAST                5 (kwargs)
+                     354 LOAD_METHOD              7 (get)
+                     376 LOAD_CONST               6 ('block_id')
+                     378 PRECALL                  1
+                     382 CALL                     1
+         
+         278         392 LOAD_FAST                5 (kwargs)
+                     394 LOAD_METHOD              7 (get)
+                     416 LOAD_CONST               7 ('field_name')
+                     418 PRECALL                  1
+                     422 CALL                     1
+         
+         279         432 LOAD_FAST                5 (kwargs)
+                     434 LOAD_METHOD              7 (get)
+                     456 LOAD_CONST               8 ('model')
+                     458 PRECALL                  1
+                     462 CALL                     1
+         
+         274         472 LOAD_CONST               9 (('nodelist', 'block', 'block_id', 'field_name', 'model'))
+                     474 BUILD_CONST_KEY_MAP      5
+         
+         280         476 LOAD_FAST                7 (extra)
+         
+         274         478 DICT_MERGE               1
+                     480 CALL_FUNCTION_EX         1
+                     482 RETURN_VALUE
          consts
             '\n    This tag is used to render an editable block.\n\n    This block will be wrapped and is able to be edited by the user on the frontend.\n\n    We will require the block_id and field_name of the streamfield this block belongs to.\n\n    You could omit needing to pass a block ID by passing in the StreamChild instance as opposed to the StructValue instance.\n    \n    Usage example 1:\n        ```python\n        {% fedit_block my_structvalue_instance block_id my_streamfield_attribute_name page_instance %}\n        ```\n\n    Optionally you can omit the block and pass in the block_id and field_name as keyword arguments.\n\n    This will allow you to use the block as a block tag.\n\n    Usage example 2:\n        ```python\n        {% fedit_block block_id=my_structvalue_instance field_name=my_streamfield_attribute_name model=page_instance %}\n            <p>Some content before block</p>\n            {% include_block my_block %}\n            <p>Some content after block</p>\n        {% unfedit_block %}\n        ```\n    '
             0
             ('block', 'block_id', 'field_name', 'model')
-            'field_name'
-            'Field name is required'
             'block'
             ('unfedit_block',)
             None
             'block_id'
+            'field_name'
             'model'
             ('nodelist', 'block', 'block_id', 'field_name', 'model')
             ()
-         names      ('split_contents', 'pop', 'get_kwargs', 'ValueError', 'parse', 'delete_first_token', 'items', 'BlockEditNode', 'get')
+         names      ('split_contents', 'pop', 'get_kwargs', 'parse', 'delete_first_token', 'items', 'BlockEditNode', 'get')
          varnames   ('parser', 'token', 'tokens', '_', 'kwargs_names', 'kwargs', 'nodelist', 'extra', 'key', 'value')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit_block'
-         firstlineno 216
+         firstlineno 224
          lnotab
-            0x021e28012a010805220108011e0208012a012a0204020401320108010c
-            020e01020128012801280128fb040602fa
+            0x021e28012a010805220208012a012a0204020401320108010c020e0102
+            0128012801280128fb040602fa
       True
       'fedit_field'
       ('takes_context', 'name')
       None
       code
          argcount  : 4
          nlocals   : 9
@@ -1625,144 +1641,144 @@
             00000072497c086a090000000000000000a00b0000000000000000000000
             0000000000000000007c026a0c00000000000000006a0d00000000000000
             009b0064077c026a0c00000000000000006a0e00000000000000009b009d
             03a6010000ab0100000000000000007216740b000000000000000000007c
             08741e000000000000000000006408a6030000ab03000000000000000073
             027c0353007421000000000000000000007c087c037c017c027c00660569
             007c05a4018e015300
-         278           0 RESUME                   0
+         284           0 RESUME                   0
          
-         296           2 LOAD_GLOBAL              1 (NULL + all)
+         302           2 LOAD_GLOBAL              1 (NULL + all)
                       14 LOAD_FAST                1 (field_name)
                       16 LOAD_FAST                2 (model)
                       18 BUILD_LIST               2
                       20 PRECALL                  1
                       24 CALL                     1
                       34 POP_JUMP_FORWARD_IF_TRUE    15 (to 66)
          
-         297          36 LOAD_GLOBAL              3 (NULL + ValueError)
+         303          36 LOAD_GLOBAL              3 (NULL + ValueError)
                       48 LOAD_CONST               1 ('Field name, and model are required')
                       50 PRECALL                  1
                       54 CALL                     1
                       64 RAISE_VARARGS            1
          
-         299     >>   66 BUILD_MAP                0
+         305     >>   66 BUILD_MAP                0
                       68 STORE_FAST               5 (extra)
          
-         300          70 LOAD_FAST                4 (kwargs)
+         306          70 LOAD_FAST                4 (kwargs)
                       72 LOAD_METHOD              2 (items)
                       94 PRECALL                  0
                       98 CALL                     0
                      108 GET_ITER
                  >>  110 FOR_ITER                10 (to 132)
                      112 UNPACK_SEQUENCE          2
                      116 STORE_FAST               6 (key)
                      118 STORE_FAST               7 (value)
          
-         301         120 LOAD_FAST                7 (value)
+         307         120 LOAD_FAST                7 (value)
                      122 LOAD_FAST                5 (extra)
                      124 LOAD_FAST                6 (key)
                      126 STORE_SUBSCR
                      130 JUMP_BACKWARD           11 (to 110)
          
-         304     >>  132 LOAD_FAST                0 (context)
+         310     >>  132 LOAD_FAST                0 (context)
                      134 LOAD_METHOD              3 (get)
                      156 LOAD_CONST               2 ('request')
                      158 PRECALL                  1
                      162 CALL                     1
                      172 STORE_FAST               8 (request)
          
-         305         174 LOAD_FAST                3 (content)
+         311         174 LOAD_FAST                3 (content)
                      176 POP_JUMP_FORWARD_IF_TRUE    64 (to 306)
          
-         306         178 LOAD_GLOBAL              9 (NULL + hasattr)
+         312         178 LOAD_GLOBAL              9 (NULL + hasattr)
                      190 LOAD_FAST                2 (model)
                      192 LOAD_CONST               3 ('render_fedit_')
                      194 LOAD_FAST                1 (field_name)
                      196 FORMAT_VALUE             0
                      198 BUILD_STRING             2
                      200 PRECALL                  2
                      204 CALL                     2
                      214 POP_JUMP_FORWARD_IF_FALSE    29 (to 274)
          
-         307         216 PUSH_NULL
+         313         216 PUSH_NULL
                      218 LOAD_GLOBAL             11 (NULL + getattr)
                      230 LOAD_FAST                2 (model)
                      232 LOAD_CONST               3 ('render_fedit_')
                      234 LOAD_FAST                1 (field_name)
                      236 FORMAT_VALUE             0
                      238 BUILD_STRING             2
                      240 PRECALL                  2
                      244 CALL                     2
                      254 LOAD_FAST                8 (request)
                      256 PRECALL                  1
                      260 CALL                     1
                      270 STORE_FAST               3 (content)
                      272 JUMP_FORWARD            16 (to 306)
          
-         309     >>  274 LOAD_GLOBAL             11 (NULL + getattr)
+         315     >>  274 LOAD_GLOBAL             11 (NULL + getattr)
                      286 LOAD_FAST                2 (model)
                      288 LOAD_FAST                1 (field_name)
                      290 PRECALL                  2
                      294 CALL                     2
                      304 STORE_FAST               3 (content)
          
-         311     >>  306 LOAD_GLOBAL              9 (NULL + hasattr)
+         317     >>  306 LOAD_GLOBAL              9 (NULL + hasattr)
                      318 LOAD_FAST                0 (context)
                      320 LOAD_CONST               4 ('flatten')
                      322 PRECALL                  2
                      326 CALL                     2
                      336 POP_JUMP_FORWARD_IF_FALSE    20 (to 378)
          
-         312         338 LOAD_FAST                0 (context)
+         318         338 LOAD_FAST                0 (context)
                      340 LOAD_METHOD              6 (flatten)
                      362 PRECALL                  0
                      366 CALL                     0
                      376 STORE_FAST               0 (context)
          
-         314     >>  378 LOAD_GLOBAL              9 (NULL + hasattr)
+         320     >>  378 LOAD_GLOBAL              9 (NULL + hasattr)
                      390 LOAD_FAST                3 (content)
                      392 LOAD_CONST               5 ('render_as_block')
                      394 PRECALL                  2
                      398 CALL                     2
                      408 POP_JUMP_FORWARD_IF_FALSE    42 (to 494)
          
-         315         410 LOAD_FAST                0 (context)
+         321         410 LOAD_FAST                0 (context)
                      412 LOAD_METHOD              7 (update)
                      434 LOAD_FAST                4 (kwargs)
                      436 PRECALL                  1
                      440 CALL                     1
                      450 POP_TOP
          
-         316         452 LOAD_FAST                3 (content)
+         322         452 LOAD_FAST                3 (content)
                      454 LOAD_METHOD              8 (render_as_block)
                      476 LOAD_FAST                0 (context)
                      478 PRECALL                  1
                      482 CALL                     1
                      492 STORE_FAST               3 (content)
          
-         318     >>  494 LOAD_FAST                8 (request)
+         324     >>  494 LOAD_FAST                8 (request)
                      496 POP_JUMP_FORWARD_IF_FALSE   113 (to 724)
          
-         320         498 LOAD_FAST                8 (request)
+         326         498 LOAD_FAST                8 (request)
                      500 LOAD_ATTR                9 (user)
                      510 LOAD_ATTR               10 (is_authenticated)
          
-         319         520 POP_JUMP_FORWARD_IF_FALSE    99 (to 720)
+         325         520 POP_JUMP_FORWARD_IF_FALSE    99 (to 720)
          
-         321         522 LOAD_FAST                8 (request)
+         327         522 LOAD_FAST                8 (request)
                      524 LOAD_ATTR                9 (user)
                      534 LOAD_METHOD             11 (has_perm)
                      556 LOAD_CONST               6 ('wagtailadmin.access_admin')
                      558 PRECALL                  1
                      562 CALL                     1
          
-         319         572 POP_JUMP_FORWARD_IF_FALSE    73 (to 720)
+         325         572 POP_JUMP_FORWARD_IF_FALSE    73 (to 720)
          
-         322         574 LOAD_FAST                8 (request)
+         328         574 LOAD_FAST                8 (request)
                      576 LOAD_ATTR                9 (user)
                      586 LOAD_METHOD             11 (has_perm)
                      608 LOAD_FAST                2 (model)
                      610 LOAD_ATTR               12 (_meta)
                      620 LOAD_ATTR               13 (app_label)
                      630 FORMAT_VALUE             0
                      632 LOAD_CONST               7 ('.change_')
@@ -1770,44 +1786,44 @@
                      636 LOAD_ATTR               12 (_meta)
                      646 LOAD_ATTR               14 (model_name)
                      656 FORMAT_VALUE             0
                      658 BUILD_STRING             3
                      660 PRECALL                  1
                      664 CALL                     1
          
-         319         674 POP_JUMP_FORWARD_IF_FALSE    22 (to 720)
+         325         674 POP_JUMP_FORWARD_IF_FALSE    22 (to 720)
          
-         323         676 LOAD_GLOBAL             11 (NULL + getattr)
+         329         676 LOAD_GLOBAL             11 (NULL + getattr)
                      688 LOAD_FAST                8 (request)
                      690 LOAD_GLOBAL             30 (FEDIT_PREVIEW_VAR)
                      702 LOAD_CONST               8 (False)
                      704 PRECALL                  3
                      708 CALL                     3
          
-         319         718 POP_JUMP_FORWARD_IF_TRUE     2 (to 724)
+         325         718 POP_JUMP_FORWARD_IF_TRUE     2 (to 724)
          
-         325     >>  720 LOAD_FAST                3 (content)
+         331     >>  720 LOAD_FAST                3 (content)
                      722 RETURN_VALUE
          
-         327     >>  724 LOAD_GLOBAL             33 (NULL + render_editable_field)
+         333     >>  724 LOAD_GLOBAL             33 (NULL + render_editable_field)
          
-         328         736 LOAD_FAST                8 (request)
+         334         736 LOAD_FAST                8 (request)
                      738 LOAD_FAST                3 (content)
          
-         329         740 LOAD_FAST                1 (field_name)
+         335         740 LOAD_FAST                1 (field_name)
                      742 LOAD_FAST                2 (model)
          
-         330         744 LOAD_FAST                0 (context)
+         336         744 LOAD_FAST                0 (context)
          
-         327         746 BUILD_TUPLE              5
+         333         746 BUILD_TUPLE              5
                      748 BUILD_MAP                0
          
-         331         750 LOAD_FAST                5 (extra)
+         337         750 LOAD_FAST                5 (extra)
          
-         327         752 DICT_MERGE               1
+         333         752 DICT_MERGE               1
                      754 CALL_FUNCTION_EX         1
                      756 RETURN_VALUE
          consts
             '\n    This tag is used to render an editable field.\n\n    This field will be wrapped and is able to be edited by the user on the frontend.\n\n    We will require the field_name of the field and the model instance.\n\n    Usage example:\n        ```python\n        {% fedit_field my_field_name page_instance %}\n        ```\n\n    Optionally your model can define a `render_fedit_{field_name}` method that will be used to render the field.\n    This will allow you to use custom rendering logic if need be.\n    '
             'Field name, and model are required'
             'request'
             'render_fedit_'
@@ -1818,15 +1834,15 @@
             False
          names      ('all', 'ValueError', 'items', 'get', 'hasattr', 'getattr', 'flatten', 'update', 'render_as_block', 'user', 'is_authenticated', 'has_perm', '_meta', 'app_label', 'model_name', 'FEDIT_PREVIEW_VAR', 'render_editable_field')
          varnames   ('context', 'field_name', 'model', 'content', 'kwargs', 'extra', 'key', 'value', 'request')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit_field'
-         firstlineno 278
+         firstlineno 284
          lnotab
             0x021222011e02040132010c032a01040126013a0220022001280220012a
             012a02040216ff020232fe020364fd02042afc020604020c010401040102
             fd040402fc
       code
          argcount  : 5
          nlocals   : 10
@@ -1846,135 +1862,135 @@
             084400a6000000ab0000000000000000007d087419000000000000000000
             00741b0000000000000000000064007c08a6020000ab0200000000000000
             00a6010000ab0100000000000000007d08741d0000000000000000000064
             067c067c027c037c017c047c0864079c067c05a5018900ac08a6030000ab
             0300000000000000005300
                        0 MAKE_CELL                0 (request)
          
-         334           2 RESUME                   0
+         340           2 RESUME                   0
          
-         335           4 LOAD_GLOBAL              1 (NULL + reverse)
+         341           4 LOAD_GLOBAL              1 (NULL + reverse)
          
-         336          16 LOAD_CONST               1 ('wagtail_fedit:edit_field')
+         342          16 LOAD_CONST               1 ('wagtail_fedit:edit_field')
          
-         337          18 LOAD_FAST                2 (field_name)
+         343          18 LOAD_FAST                2 (field_name)
                       20 LOAD_FAST                3 (model)
                       22 LOAD_ATTR                1 (_meta)
                       32 LOAD_ATTR                2 (app_label)
                       42 LOAD_FAST                3 (model)
                       44 LOAD_ATTR                1 (_meta)
                       54 LOAD_ATTR                3 (model_name)
                       64 LOAD_FAST                3 (model)
                       66 LOAD_ATTR                4 (pk)
                       76 BUILD_LIST               4
          
-         335          78 KW_NAMES                 2
+         341          78 KW_NAMES                 2
                       80 PRECALL                  2
                       84 CALL                     2
                       94 STORE_FAST               6 (edit_url)
          
-         340          96 LOAD_FAST                5 (kwargs)
+         346          96 LOAD_FAST                5 (kwargs)
                       98 POP_JUMP_FORWARD_IF_FALSE    37 (to 174)
          
-         341         100 LOAD_GLOBAL             11 (NULL + urlencode)
+         347         100 LOAD_GLOBAL             11 (NULL + urlencode)
          
-         342         112 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+         348         112 LOAD_GLOBAL             13 (NULL + BlockEditNode)
                      124 LOAD_ATTR                7 (pack)
                      134 LOAD_CONST               9 (())
                      136 BUILD_MAP                0
                      138 LOAD_FAST                5 (kwargs)
                      140 DICT_MERGE               1
                      142 CALL_FUNCTION_EX         1
          
-         341         144 PRECALL                  1
+         347         144 PRECALL                  1
                      148 CALL                     1
                      158 STORE_FAST               7 (packed)
          
-         344         160 LOAD_FAST                6 (edit_url)
+         350         160 LOAD_FAST                6 (edit_url)
                      162 FORMAT_VALUE             0
                      164 LOAD_CONST               3 ('?')
                      166 LOAD_FAST                7 (packed)
                      168 FORMAT_VALUE             0
                      170 BUILD_STRING             3
                      172 STORE_FAST               6 (edit_url)
          
-         347     >>  174 LOAD_GLOBAL             17 (NULL + FeditFieldEditButton)
+         353     >>  174 LOAD_GLOBAL             17 (NULL + FeditFieldEditButton)
                      186 PRECALL                  0
                      190 CALL                     0
          
-         346         200 BUILD_LIST               1
+         352         200 BUILD_LIST               1
                      202 STORE_FAST               8 (items)
          
-         350         204 LOAD_GLOBAL             19 (NULL + hooks)
+         356         204 LOAD_GLOBAL             19 (NULL + hooks)
                      216 LOAD_ATTR               10 (get_hooks)
                      226 LOAD_GLOBAL             22 (CONSTRUCT_FIELD_TOOLBAR)
                      238 PRECALL                  1
                      242 CALL                     1
                      252 GET_ITER
                  >>  254 FOR_ITER                17 (to 290)
                      256 STORE_FAST               9 (hook)
          
-         351         258 PUSH_NULL
+         357         258 PUSH_NULL
                      260 LOAD_FAST                9 (hook)
                      262 LOAD_DEREF               0 (request)
                      264 LOAD_FAST                8 (items)
                      266 LOAD_FAST                3 (model)
                      268 LOAD_FAST                2 (field_name)
                      270 KW_NAMES                 4
                      272 PRECALL                  4
                      276 CALL                     4
                      286 POP_TOP
                      288 JUMP_BACKWARD           18 (to 254)
          
-         353     >>  290 LOAD_CLOSURE             0 (request)
+         359     >>  290 LOAD_CLOSURE             0 (request)
                      292 BUILD_TUPLE              1
-                     294 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 353>)
+                     294 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 359>)
                      296 MAKE_FUNCTION            8 (closure)
                      298 LOAD_FAST                8 (items)
                      300 GET_ITER
                      302 PRECALL                  0
                      306 CALL                     0
                      316 STORE_FAST               8 (items)
          
-         354         318 LOAD_GLOBAL             25 (NULL + list)
+         360         318 LOAD_GLOBAL             25 (NULL + list)
                      330 LOAD_GLOBAL             27 (NULL + filter)
                      342 LOAD_CONST               0 (None)
                      344 LOAD_FAST                8 (items)
                      346 PRECALL                  2
                      350 CALL                     2
                      360 PRECALL                  1
                      364 CALL                     1
                      374 STORE_FAST               8 (items)
          
-         356         376 LOAD_GLOBAL             29 (NULL + render_to_string)
+         362         376 LOAD_GLOBAL             29 (NULL + render_to_string)
          
-         357         388 LOAD_CONST               6 ('wagtail_fedit/content/editable_field.html')
+         363         388 LOAD_CONST               6 ('wagtail_fedit/content/editable_field.html')
          
-         359         390 LOAD_FAST                6 (edit_url)
+         365         390 LOAD_FAST                6 (edit_url)
          
-         360         392 LOAD_FAST                2 (field_name)
+         366         392 LOAD_FAST                2 (field_name)
          
-         361         394 LOAD_FAST                3 (model)
+         367         394 LOAD_FAST                3 (model)
          
-         362         396 LOAD_FAST                1 (content)
+         368         396 LOAD_FAST                1 (content)
          
-         363         398 LOAD_FAST                4 (context)
+         369         398 LOAD_FAST                4 (context)
          
-         364         400 LOAD_FAST                8 (items)
+         370         400 LOAD_FAST                8 (items)
          
-         358         402 LOAD_CONST               7 (('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items'))
+         364         402 LOAD_CONST               7 (('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items'))
                      404 BUILD_CONST_KEY_MAP      6
          
-         365         406 LOAD_FAST                5 (kwargs)
+         371         406 LOAD_FAST                5 (kwargs)
          
-         358         408 DICT_UPDATE              1
+         364         408 DICT_UPDATE              1
          
-         367         410 LOAD_DEREF               0 (request)
+         373         410 LOAD_DEREF               0 (request)
          
-         356         412 KW_NAMES                 8
+         362         412 KW_NAMES                 8
                      414 PRECALL                  3
                      418 CALL                     3
                      428 RETURN_VALUE
          consts
             None
             'wagtail_fedit:edit_field'
             ('args',)
@@ -1986,15 +2002,15 @@
                stacksize : 5
                flags     : 19
                code
                   0x9501970067007c005d177d017c01a00000000000000000000000000000
                   000000000000008902a6010000ab01000000000000000091028c185300
                              0 COPY_FREE_VARS           1
                
-               353           2 RESUME                   0
+               359           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                23 (to 56)
                             10 STORE_FAST               1 (item)
                             12 LOAD_FAST                1 (item)
                             14 LOAD_METHOD              0 (render)
                             36 LOAD_DEREF               2 (request)
@@ -2006,27 +2022,27 @@
                consts
                names      ('render',)
                varnames   ('.0', 'item')
                freevars   ('request',)
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '<listcomp>'
-               firstlineno 353
+               firstlineno 359
                lnotab 0x
             'wagtail_fedit/content/editable_field.html'
             ('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items')
             ('request',)
             ()
          names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack', 'FeditFieldEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_FIELD_TOOLBAR', 'list', 'filter', 'render_to_string')
          varnames   ('request', 'content', 'field_name', 'model', 'context', 'kwargs', 'edit_url', 'packed', 'items', 'hook')
          freevars   ()
          cellvars   ('request',)
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_editable_field'
-         firstlineno 334
+         firstlineno 340
          lnotab
             0x04010c0102013cfe120504010c0120ff10030e031aff0404360120021c
             013a020c0102020201020102010201020102fa040702f9020902f5
       'kwarg_list'
       'tokens'
       'return'
       code
@@ -2042,89 +2058,89 @@
             0064036b020000000072307c03720f7407000000000000000000006404a6
             010000ab01000000000000000082017c00a0040000000000000000000000
             0000000000000000007c06a6010000ab0100000000000000007c047c017c
             05190000000000000000003c0000008c5d7c076405190000000000000000
             007d087c00a00400000000000000000000000000000000000000007c0764
             0319000000000000000000a6010000ab0100000000000000007c047c083c
             00000064067d038c867c045300
-         370           0 RESUME                   0
+         376           0 RESUME                   0
          
-         371           2 LOAD_CONST               1 (False)
+         377           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               3 (had_kwargs)
          
-         372           6 BUILD_MAP                0
+         378           6 BUILD_MAP                0
                        8 STORE_FAST               4 (kwargs)
          
-         377          10 LOAD_GLOBAL              1 (NULL + enumerate)
+         383          10 LOAD_GLOBAL              1 (NULL + enumerate)
                       22 LOAD_FAST                2 (tokens)
                       24 PRECALL                  1
                       28 CALL                     1
                       38 GET_ITER
                  >>   40 FOR_ITER               133 (to 308)
                       42 UNPACK_SEQUENCE          2
                       46 STORE_FAST               5 (i)
                       48 STORE_FAST               6 (token)
          
-         378          50 LOAD_FAST                6 (token)
+         384          50 LOAD_FAST                6 (token)
                       52 LOAD_METHOD              1 (split)
                       74 LOAD_CONST               2 ('=')
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_FAST               7 (split)
          
-         379          92 LOAD_GLOBAL              5 (NULL + len)
+         385          92 LOAD_GLOBAL              5 (NULL + len)
                      104 LOAD_FAST                7 (split)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               3 (1)
                      122 COMPARE_OP               2 (==)
                      128 POP_JUMP_FORWARD_IF_FALSE    48 (to 226)
          
-         380         130 LOAD_FAST                3 (had_kwargs)
+         386         130 LOAD_FAST                3 (had_kwargs)
                      132 POP_JUMP_FORWARD_IF_FALSE    15 (to 164)
          
-         381         134 LOAD_GLOBAL              7 (NULL + ValueError)
+         387         134 LOAD_GLOBAL              7 (NULL + ValueError)
                      146 LOAD_CONST               4 ('Unexpected positional argument after keyword argument')
                      148 PRECALL                  1
                      152 CALL                     1
                      162 RAISE_VARARGS            1
          
-         383     >>  164 LOAD_FAST                0 (parser)
+         389     >>  164 LOAD_FAST                0 (parser)
                      166 LOAD_METHOD              4 (compile_filter)
                      188 LOAD_FAST                6 (token)
                      190 PRECALL                  1
                      194 CALL                     1
                      204 LOAD_FAST                4 (kwargs)
                      206 LOAD_FAST                1 (kwarg_list)
                      208 LOAD_FAST                5 (i)
                      210 BINARY_SUBSCR
                      220 STORE_SUBSCR
                      224 JUMP_BACKWARD           93 (to 40)
          
-         385     >>  226 LOAD_FAST                7 (split)
+         391     >>  226 LOAD_FAST                7 (split)
                      228 LOAD_CONST               5 (0)
                      230 BINARY_SUBSCR
                      240 STORE_FAST               8 (key)
          
-         389         242 LOAD_FAST                0 (parser)
+         395         242 LOAD_FAST                0 (parser)
                      244 LOAD_METHOD              4 (compile_filter)
                      266 LOAD_FAST                7 (split)
                      268 LOAD_CONST               3 (1)
                      270 BINARY_SUBSCR
                      280 PRECALL                  1
                      284 CALL                     1
                      294 LOAD_FAST                4 (kwargs)
                      296 LOAD_FAST                8 (key)
                      298 STORE_SUBSCR
          
-         390         302 LOAD_CONST               6 (True)
+         396         302 LOAD_CONST               6 (True)
                      304 STORE_FAST               3 (had_kwargs)
                      306 JUMP_BACKWARD          134 (to 40)
          
-         392     >>  308 LOAD_FAST                4 (kwargs)
+         398     >>  308 LOAD_FAST                4 (kwargs)
                      310 RETURN_VALUE
          consts
             None
             False
             '='
             1
             'Unexpected positional argument after keyword argument'
@@ -2132,74 +2148,74 @@
             True
          names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter')
          varnames   ('parser', 'kwarg_list', 'tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 370
+         firstlineno 376
          lnotab 0x02010401040528012a01260104011e023e0210043c010602
       code
          argcount  : 3
          nlocals   : 5
          stacksize : 5
          flags     : 15
          code
             0x97007c017c00760072087c007c01190000000000000000005300740100
             0000000000000000007c02a6010000ab010000000000000000720802007c
             027c0369007c04a4018e017d027c027c007c013c0000007c025300
-         397           0 RESUME                   0
+         403           0 RESUME                   0
          
-         398           2 LOAD_FAST                1 (key)
+         404           2 LOAD_FAST                1 (key)
                        4 LOAD_FAST                0 (context)
                        6 CONTAINS_OP              0
                        8 POP_JUMP_FORWARD_IF_FALSE     8 (to 26)
          
-         399          10 LOAD_FAST                0 (context)
+         405          10 LOAD_FAST                0 (context)
                       12 LOAD_FAST                1 (key)
                       14 BINARY_SUBSCR
                       24 RETURN_VALUE
          
-         401     >>   26 LOAD_GLOBAL              1 (NULL + callable)
+         407     >>   26 LOAD_GLOBAL              1 (NULL + callable)
                       38 LOAD_FAST                2 (value)
                       40 PRECALL                  1
                       44 CALL                     1
                       54 POP_JUMP_FORWARD_IF_FALSE     8 (to 72)
          
-         402          56 PUSH_NULL
+         408          56 PUSH_NULL
                       58 LOAD_FAST                2 (value)
                       60 LOAD_FAST                3 (args)
                       62 BUILD_MAP                0
                       64 LOAD_FAST                4 (kwargs)
                       66 DICT_MERGE               1
                       68 CALL_FUNCTION_EX         1
                       70 STORE_FAST               2 (value)
          
-         404     >>   72 LOAD_FAST                2 (value)
+         410     >>   72 LOAD_FAST                2 (value)
                       74 LOAD_FAST                0 (context)
                       76 LOAD_FAST                1 (key)
                       78 STORE_SUBSCR
          
-         405          82 LOAD_FAST                2 (value)
+         411          82 LOAD_FAST                2 (value)
                       84 RETURN_VALUE
          consts
             None
          names      ('callable',)
          varnames   ('context', 'key', 'value', 'args', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       '_get_from_context_or_set'
-         firstlineno 397
+         firstlineno 403
          lnotab 0x0201080110021e0110020a01
       (None,)
    names      ('django.template', 'library', 'Node', 'NodeList', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'TokenType', 'FilterExpression', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'django.db', 'models', 'wagtail.blocks', 'BoundBlock', 'wagtail.models', 'Page', 'wagtail', 'hooks', 'urllib.parse', 'urlencode', 'toolbar', 'FeditBlockEditButton', 'FeditFieldEditButton', 'utils', 'FEDIT_PREVIEW_VAR', 'CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR', 'Library', 'register', 'TimestampSigner', 'url_value_signer', 'BlockEditNode', 'tag', 'do_render_fedit_block', 'simple_tag', 'do_render_fedit_field', 'render_editable_field', 'list', 'str', 'dict', 'get_kwargs', '_get_from_context_or_set')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020114010c0114010c010c010c010c010c020c010c010c010c0210
-      040c0110061e021e031c7f003a2a010eff0e01023d2c0106ff0e01023706
+      040c0110061e021e031c7f00422a010eff0e01023b2c0106ff0e01023706
       24301b
```

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.1.3/wagtail_fedit/templatetags/fedit.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,17 @@
         extra = self.extra
 
         # Conversions for filterexpressions
         for k, e in extra.items():
             if isinstance(e, FilterExpression):
                 extra[k] = e.resolve(context)
 
+        if not field_name and "wagtail_fedit_field_name" in context:
+            field_name = context["wagtail_fedit_field_name"]
+
         if isinstance(block, FilterExpression):
             block = block.resolve(context)
         if isinstance(block_id, FilterExpression):
             block_id = block_id.resolve(context)
         if isinstance(field_name, FilterExpression):
             field_name = field_name.resolve(context)
         if isinstance(model, FilterExpression):
@@ -74,15 +77,18 @@
             raise ValueError("Field name is required")
 
         if not block_id and "block_id" not in context and not block:
             raise ValueError("Block ID is required")
         
         if not model and "wagtail_fedit_instance" not in context:
             raise ValueError("Model instance is required")
-
+        
+        context["wagtail_fedit_field_name"] = field_name
+        context["wagtail_fedit_instance"] = model
+        
         # Render the block or nodelist
         # This allows us to use the block as a block tag or as a simple tag.
         if block:
             try:
                 context = context.flatten()
             except AttributeError:
                 pass
@@ -156,14 +162,16 @@
                 ),
                 "admin_edit_url": admin_edit_url,
                 "block_id": block_id,
                 "model": model,
                 "content": rendered,
                 "field_name": field_name,
                 "parent_context": context,
+                "wagtail_fedit_field_name": field_name,
+                "wagtail_fedit_instance": model,
                 "toolbar_items": items,
             }
         )
     
     @staticmethod
     def pack(**kwargs) -> dict:
 
@@ -247,16 +255,14 @@
     _ = tokens.pop(0)
     kwargs_names = [
         "block", "block_id",
         "field_name", "model",
     ]
 
     kwargs = get_kwargs(parser, kwargs_names, tokens)
-    if "field_name" not in kwargs:
-        raise ValueError("Field name is required")
     
     if "block" not in kwargs:
         nodelist = parser.parse(("unfedit_block",))
         parser.delete_first_token()
     else:
         nodelist = None
```

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.1.3/wagtail_fedit/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.1.3/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/urls.py` & `wagtail_fedit-1.1.3/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/utils.py` & `wagtail_fedit-1.1.3/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.1.3/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.1.3/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.1.3/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.1.3/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.1.3/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.1.2
+Version: 1.1.3
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.2 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.1.3 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.1.2/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.1.3/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

