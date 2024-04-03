# Comparing `tmp/wagtail_fedit-1.2.1.tar.gz` & `tmp/wagtail_fedit-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.2.1.tar", last modified: Wed Apr  3 17:51:17 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.2.2.tar", last modified: Wed Apr  3 18:55:44 2024, max compression
```

## Comparing `wagtail_fedit-1.2.1.tar` & `wagtail_fedit-1.2.2.tar`

### file list

```diff
@@ -1,97 +1,95 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.221769 wagtail_fedit-1.2.1/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5493 2024-04-03 17:51:17.221769 wagtail_fedit-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.2.1/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-03 17:51:17.233291 wagtail_fedit-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.050311 wagtail_fedit-1.2.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.051317 wagtail_fedit-1.2.1/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.052446 wagtail_fedit-1.2.1/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.053450 wagtail_fedit-1.2.1/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.055965 wagtail_fedit-1.2.1/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.1/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.091799 wagtail_fedit-1.2.1/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.1/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.1/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.1/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.103307 wagtail_fedit-1.2.1/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.2.1/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.2.1/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.2.1/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      625 2024-04-03 15:41:06.000000 wagtail_fedit-1.2.1/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.103307 wagtail_fedit-1.2.1/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.1/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.104811 wagtail_fedit-1.2.1/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.1/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0       60 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.1/wagtail_fedit/models.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.042900 wagtail_fedit-1.2.1/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.043900 wagtail_fedit-1.2.1/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.107817 wagtail_fedit-1.2.1/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.2.1/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4167 2024-04-01 16:12:24.000000 wagtail_fedit-1.2.1/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.2.1/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.138966 wagtail_fedit-1.2.1/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    11876 2024-04-03 17:44:07.000000 wagtail_fedit-1.2.1/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.043900 wagtail_fedit-1.2.1/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.044900 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.143974 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.144950 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:52.000000 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      466 2024-04-01 17:10:28.000000 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      469 2024-04-01 17:10:33.000000 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.153085 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
--rw-rw-rw-   0        0        0     3002 2024-04-03 17:39:24.000000 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.157594 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-03 17:05:19.000000 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.166159 wagtail_fedit-1.2.1/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.2.1/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.168161 wagtail_fedit-1.2.1/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.1/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16665 2024-04-03 17:01:12.000000 wagtail_fedit-1.2.1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13707 2024-04-03 15:30:16.000000 wagtail_fedit-1.2.1/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.182693 wagtail_fedit-1.2.1/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.2.1/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.2.1/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0       63 2024-04-02 18:34:47.000000 wagtail_fedit-1.2.1/wagtail_fedit/tests.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.2.1/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.2.1/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     5512 2024-04-03 17:02:56.000000 wagtail_fedit-1.2.1/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.209321 wagtail_fedit-1.2.1/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.2.1/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8659 2024-04-03 12:33:35.000000 wagtail_fedit-1.2.1/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.2.1/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     9046 2024-04-03 15:44:02.000000 wagtail_fedit-1.2.1/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.220785 wagtail_fedit-1.2.1/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      132 2024-04-03 15:22:27.000000 wagtail_fedit-1.2.1/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.2.1/wagtail_fedit/wagtail_hooks/editorjs.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.2.1/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.2.1/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.2.1/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.2.1/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.2.1/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-03 17:51:17.221769 wagtail_fedit-1.2.1/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     5493 2024-04-03 17:51:16.000000 wagtail_fedit-1.2.1/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2711 2024-04-03 17:51:16.000000 wagtail_fedit-1.2.1/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 17:51:16.000000 wagtail_fedit-1.2.1/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-03 17:51:16.000000 wagtail_fedit-1.2.1/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-03 17:51:16.000000 wagtail_fedit-1.2.1/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.665964 wagtail_fedit-1.2.2/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5493 2024-04-03 18:55:44.665964 wagtail_fedit-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.2.2/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-03 18:55:44.676590 wagtail_fedit-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.362094 wagtail_fedit-1.2.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.364340 wagtail_fedit-1.2.2/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.367818 wagtail_fedit-1.2.2/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.370080 wagtail_fedit-1.2.2/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.376704 wagtail_fedit-1.2.2/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.420832 wagtail_fedit-1.2.2/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.2/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.2/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.2/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.460529 wagtail_fedit-1.2.2/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.2.2/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.2.2/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.2.2/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      625 2024-04-03 15:41:06.000000 wagtail_fedit-1.2.2/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.461520 wagtail_fedit-1.2.2/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.2/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.462519 wagtail_fedit-1.2.2/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.349178 wagtail_fedit-1.2.2/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.350179 wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.466519 wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/css/admin.css
+-rw-rw-rw-   0        0        0     4102 2024-04-03 18:51:45.000000 wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.489205 wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    11926 2024-04-03 18:52:32.000000 wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.350179 wagtail_fedit-1.2.2/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.352683 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.497223 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.500710 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:52.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      310 2024-04-03 18:53:15.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      296 2024-04-03 18:53:06.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.537398 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
+-rw-rw-rw-   0        0        0     3002 2024-04-03 17:39:24.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.553141 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0     1023 2024-04-03 17:05:19.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.568145 wagtail_fedit-1.2.2/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.2.2/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.571147 wagtail_fedit-1.2.2/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16665 2024-04-03 17:01:12.000000 wagtail_fedit-1.2.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13707 2024-04-03 15:30:16.000000 wagtail_fedit-1.2.2/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.586861 wagtail_fedit-1.2.2/wagtail_fedit/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.2.2/wagtail_fedit/tests/__init__.py
+-rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.2.2/wagtail_fedit/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.2.2/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.2.2/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0     5512 2024-04-03 17:02:56.000000 wagtail_fedit-1.2.2/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.629917 wagtail_fedit-1.2.2/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.2.2/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8659 2024-04-03 12:33:35.000000 wagtail_fedit-1.2.2/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.2.2/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     9046 2024-04-03 15:44:02.000000 wagtail_fedit-1.2.2/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.662963 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      132 2024-04-03 15:22:27.000000 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/editorjs.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.663965 wagtail_fedit-1.2.2/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     5493 2024-04-03 18:55:44.000000 wagtail_fedit-1.2.2/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2664 2024-04-03 18:55:44.000000 wagtail_fedit-1.2.2/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 18:55:44.000000 wagtail_fedit-1.2.2/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-03 18:55:44.000000 wagtail_fedit-1.2.2/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-03 18:55:44.000000 wagtail_fedit-1.2.2/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.2.1/LICENSE` & `wagtail_fedit-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/PKG-INFO` & `wagtail_fedit-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.2.1
+Version: 1.2.2
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.1 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.2 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.2.1/README.md` & `wagtail_fedit-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/setup.cfg` & `wagtail_fedit-1.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 322e  ..version = 1.2.
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

### Comparing `wagtail_fedit-1.2.1/tests/testapp/manage.py` & `wagtail_fedit-1.2.2/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.2.2/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.2.2/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.2.2/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.2.2/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/hooks.py` & `wagtail_fedit-1.2.2/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 }
 
 .wagtail-fedit-field-wrapper,
 .wagtail-fedit-block-wrapper {
     position: relative;
 }
 .wagtail-fedit-buttons {
-    position: absolute;
-    right: 0.5em;
     display: flex;
     gap: 0.5em;
     background-color: white;
     border-radius: 0.5em;
     padding: 0.1em 0.5em;
+    position: absolute;
+    right: 0.5em;
     /* display: none; */
     z-index: 1;
 }
+
 /* .wagtail-fedit-field-wrapper > .wagtail-fedit-buttons { */
     /* position: relative; */
 /* } */
 .wagtail-fedit-field-wrapper > .wagtail-fedit-buttons button {
     display: inline-block;
 }
 .wagtail-fedit-buttons button {
@@ -43,15 +44,15 @@
 .wagtail-fedit-buttons > a:active{
     color: rgb(14, 49, 100) !important;
 }
 .wagtail-fedit-buttons svg {
     vertical-align: middle;
     color: rgb(14, 49, 100);
 }
-body:has(.wagtail-fedit-modal-wrapper .wagtail-fedit-modal) {
+body:has(.wagtail-fedit-modal) {
     overflow: hidden;
 }
 /* *:target::after { */
     /* content: ''; */
     /* display: block; */
     /* position: absolute; */
     /* top: 0; */
@@ -98,16 +99,15 @@
     overflow: hidden;
     display: flex;
 }
 .wagtail-fedit-modal-wrapper .wagtail-fedit-modal:not(.fedit-full) {
     margin-top: -5%;
 }
 
-.wagtail-fedit-field-wrapper iframe,
-.wagtail-fedit-block-wrapper iframe {
+.wagtail-fedit-modal-wrapper iframe {
     width: 100%;
     height: 100%;
     border: none;
     flex: 1;
 }
 /* .wagtail-fedit-field-wrapper .wagtail-fedit-field-content, */
 /* .wagtail-fedit-block-wrapper .wagtail-fedit-block-content { */
```

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -200,19 +200,14 @@
                         (this.iframe.formElement.dataset.isRelation || "").toLowerCase() === "true"
                     )) ||
                     (formHeight > window.innerHeight)
                 ) {
                     this.modal.classList.add("fedit-full");
                 }
 
-                // Check if we should adjust the modal height to the height of the iframe form.
-                if (formHeight > this.modal.getBoundingClientRect().height) {
-                    this.modal.style.height = `${formHeight}px`;
-                }
-
                 const url = window.location.href.split("#")[0];
                 window.history.pushState(null, this.iframe.document.title, url + `#${this.wrapperElement.id}`);
                 document.title = this.iframe.document.title;
             },
         });
         this.modal.appendChild(this.iframe.element);
 
@@ -230,21 +225,29 @@
         this.wrapperElement.parentNode.insertBefore(blockWrapper, this.wrapperElement);
         this.wrapperElement.parentNode.removeChild(this.wrapperElement);
         this.wrapperElement = blockWrapper;
         this.init();
     }
 
     closeModal() {
-        this.modalWrapper.innerHTML = "";
+        this.modalWrapper.remove();
         window.history.pushState(null, this.initialTitle, window.location.href.split("#")[0]);
         document.title = this.initialTitle;
     }
 
     get modalWrapper() {
-        return this.wrapperElement.querySelector(".wagtail-fedit-frontend-edit");
+        const modalWrapper = document.querySelector("#wagtail-fedit-modal-wrapper");
+        if (modalWrapper) {
+            return modalWrapper;
+        }
+        const wrapper = document.createElement("div");
+        wrapper.id = "wagtail-fedit-modal-wrapper";
+        wrapper.classList.add("wagtail-fedit-modal-wrapper");
+        document.body.appendChild(wrapper);
+        return wrapper;
     }
 
     init() {
         this.editUrl = this.wrapperElement.dataset.editUrl;
         this.modalHtml = modalHtml.replace("__ID__", this.wrapperElement.dataset.id);
         this.editBtn = this.wrapperElement.querySelector(".wagtail-fedit-edit-button");
```

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.2.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.2.2/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.2.2/wagtail_fedit/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.2.2/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/urls.py` & `wagtail_fedit-1.2.2/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/utils.py` & `wagtail_fedit-1.2.2/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.2.2/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.2.2/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.2.2/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.2.2/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.2.1
+Version: 1.2.2
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.1 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.2 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.2.1/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.2.2/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 tests/testapp/testapp/settings.py
 tests/testapp/testapp/urls.py
 tests/testapp/testapp/wsgi.py
 wagtail_fedit/__init__.py
 wagtail_fedit/admin.py
 wagtail_fedit/apps.py
 wagtail_fedit/hooks.py
-wagtail_fedit/models.py
-wagtail_fedit/tests.py
 wagtail_fedit/toolbar.py
 wagtail_fedit/urls.py
 wagtail_fedit/utils.py
 wagtail_fedit.egg-info/PKG-INFO
 wagtail_fedit.egg-info/SOURCES.txt
 wagtail_fedit.egg-info/dependency_links.txt
 wagtail_fedit.egg-info/requires.txt
```

