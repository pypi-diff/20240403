# Comparing `tmp/wagtail_fedit-1.2.2.tar.gz` & `tmp/wagtail_fedit-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.2.2.tar", last modified: Wed Apr  3 18:55:44 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.2.3.tar", last modified: Wed Apr  3 19:34:17 2024, max compression
```

## Comparing `wagtail_fedit-1.2.2.tar` & `wagtail_fedit-1.2.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.665964 wagtail_fedit-1.2.2/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5493 2024-04-03 18:55:44.665964 wagtail_fedit-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.2.2/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-03 18:55:44.676590 wagtail_fedit-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.362094 wagtail_fedit-1.2.2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.364340 wagtail_fedit-1.2.2/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.367818 wagtail_fedit-1.2.2/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.370080 wagtail_fedit-1.2.2/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.376704 wagtail_fedit-1.2.2/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.2/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.420832 wagtail_fedit-1.2.2/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.2/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.2/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.2/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.460529 wagtail_fedit-1.2.2/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.2.2/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.2.2/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.2.2/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      625 2024-04-03 15:41:06.000000 wagtail_fedit-1.2.2/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.461520 wagtail_fedit-1.2.2/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.2/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.462519 wagtail_fedit-1.2.2/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.2/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.349178 wagtail_fedit-1.2.2/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.350179 wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.466519 wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4102 2024-04-03 18:51:45.000000 wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.489205 wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    11926 2024-04-03 18:52:32.000000 wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.350179 wagtail_fedit-1.2.2/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.352683 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.497223 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.500710 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:52.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      310 2024-04-03 18:53:15.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      296 2024-04-03 18:53:06.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.537398 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
--rw-rw-rw-   0        0        0     3002 2024-04-03 17:39:24.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.553141 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-03 17:05:19.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.568145 wagtail_fedit-1.2.2/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.2.2/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.571147 wagtail_fedit-1.2.2/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.2/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16665 2024-04-03 17:01:12.000000 wagtail_fedit-1.2.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13707 2024-04-03 15:30:16.000000 wagtail_fedit-1.2.2/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.586861 wagtail_fedit-1.2.2/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.2.2/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.2.2/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.2.2/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.2.2/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     5512 2024-04-03 17:02:56.000000 wagtail_fedit-1.2.2/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.629917 wagtail_fedit-1.2.2/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.2.2/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8659 2024-04-03 12:33:35.000000 wagtail_fedit-1.2.2/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.2.2/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     9046 2024-04-03 15:44:02.000000 wagtail_fedit-1.2.2/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.662963 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      132 2024-04-03 15:22:27.000000 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/editorjs.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-03 18:55:44.663965 wagtail_fedit-1.2.2/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     5493 2024-04-03 18:55:44.000000 wagtail_fedit-1.2.2/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2664 2024-04-03 18:55:44.000000 wagtail_fedit-1.2.2/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 18:55:44.000000 wagtail_fedit-1.2.2/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-03 18:55:44.000000 wagtail_fedit-1.2.2/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-03 18:55:44.000000 wagtail_fedit-1.2.2/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.711019 wagtail_fedit-1.2.3/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5493 2024-04-03 19:34:17.711019 wagtail_fedit-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.2.3/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-03 19:34:17.716698 wagtail_fedit-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.552022 wagtail_fedit-1.2.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.553670 wagtail_fedit-1.2.3/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.556651 wagtail_fedit-1.2.3/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.557621 wagtail_fedit-1.2.3/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.563627 wagtail_fedit-1.2.3/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.575425 wagtail_fedit-1.2.3/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.3/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.3/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.3/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.588825 wagtail_fedit-1.2.3/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.2.3/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.2.3/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.2.3/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      625 2024-04-03 15:41:06.000000 wagtail_fedit-1.2.3/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.589793 wagtail_fedit-1.2.3/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.3/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.590790 wagtail_fedit-1.2.3/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.543388 wagtail_fedit-1.2.3/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.543388 wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.596828 wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/css/admin.css
+-rw-rw-rw-   0        0        0     4225 2024-04-03 19:33:47.000000 wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.619884 wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    11781 2024-04-03 19:13:47.000000 wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.543957 wagtail_fedit-1.2.3/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.545008 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.623390 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.627400 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.637925 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
+-rw-rw-rw-   0        0        0     3002 2024-04-03 17:39:24.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.643430 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0     1023 2024-04-03 17:05:19.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.652451 wagtail_fedit-1.2.3/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.2.3/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.655092 wagtail_fedit-1.2.3/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16811 2024-04-03 19:12:53.000000 wagtail_fedit-1.2.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13805 2024-04-03 19:12:51.000000 wagtail_fedit-1.2.3/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.662048 wagtail_fedit-1.2.3/wagtail_fedit/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.2.3/wagtail_fedit/tests/__init__.py
+-rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.2.3/wagtail_fedit/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.2.3/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.2.3/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0     5512 2024-04-03 17:02:56.000000 wagtail_fedit-1.2.3/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.688951 wagtail_fedit-1.2.3/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.2.3/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8659 2024-04-03 12:33:35.000000 wagtail_fedit-1.2.3/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.2.3/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     9076 2024-04-03 19:10:55.000000 wagtail_fedit-1.2.3/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.707994 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      132 2024-04-03 15:22:27.000000 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/editorjs.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.710061 wagtail_fedit-1.2.3/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     5493 2024-04-03 19:34:17.000000 wagtail_fedit-1.2.3/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2664 2024-04-03 19:34:17.000000 wagtail_fedit-1.2.3/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 19:34:17.000000 wagtail_fedit-1.2.3/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-03 19:34:17.000000 wagtail_fedit-1.2.3/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-03 19:34:17.000000 wagtail_fedit-1.2.3/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.2.2/LICENSE` & `wagtail_fedit-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/PKG-INFO` & `wagtail_fedit-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.2.2
+Version: 1.2.3
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.2 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.3 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.2.2/README.md` & `wagtail_fedit-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/setup.cfg` & `wagtail_fedit-1.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 322e  ..version = 1.2.
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

### Comparing `wagtail_fedit-1.2.2/tests/testapp/manage.py` & `wagtail_fedit-1.2.3/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.2.3/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.2.3/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.2.3/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.2.3/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/hooks.py` & `wagtail_fedit-1.2.3/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files 16% similar despite different names*

```diff
@@ -7,35 +7,65 @@
     display: flex;
 }
 
 .wagtail-fedit-field-wrapper,
 .wagtail-fedit-block-wrapper {
     position: relative;
 }
+.wagtail-fedit-field-wrapper:has(> .wagtail-fedit-buttons button:hover)::after,
+.wagtail-fedit-block-wrapper:has(> .wagtail-fedit-buttons button:hover)::after {
+    content: '';
+    display: block;
+    position: absolute;
+    top: 0;
+    left: 0;
+    width: 100%;
+    height: 100%;
+    background-color: rgba(0, 0, 0, 0.05);
+    outline: 2px solid #333333;
+    pointer-events: none;
+    z-index: 300;
+}
+.wagtail-fedit-field-wrapper:has(.wagtail-fedit-block-wrapper) > .wagtail-fedit-buttons,
+.wagtail-fedit-block-wrapper:has(.wagtail-fedit-block-wrapper) > .wagtail-fedit-buttons {
+    right: 30px;
+}
 .wagtail-fedit-buttons {
     display: flex;
     gap: 0.5em;
-    background-color: white;
     border-radius: 0.5em;
-    padding: 0.1em 0.5em;
     position: absolute;
-    right: 0.5em;
-    /* display: none; */
+    right: 0;
     z-index: 1;
 }
 
+.wagtail-fedit-inline > .wagtail-fedit-buttons {
+    display: inline-block;
+    position: relative;
+    margin-left: 0.25rem;
+    margin-right: 0.25rem;
+    vertical-align: top;
+    left: unset;
+    right: unset;
+}
+
 /* .wagtail-fedit-field-wrapper > .wagtail-fedit-buttons { */
     /* position: relative; */
 /* } */
 .wagtail-fedit-field-wrapper > .wagtail-fedit-buttons button {
     display: inline-block;
+    vertical-align: middle;
 }
 .wagtail-fedit-buttons button {
     border: none;
-    background-color: transparent;
+    background-color: white;
+    padding: 0.1em;
+    border-radius: 0.25em;
+    width: 24px;
+    height: 24px;
     cursor: pointer;
 }
 .wagtail-fedit-buttons button,
 .wagtail-fedit-buttons button svg,
 .wagtail-fedit-buttons > a,
 .wagtail-fedit-buttons > a svg,
 .wagtail-fedit-buttons > a:hover svg,
@@ -105,32 +135,14 @@
 
 .wagtail-fedit-modal-wrapper iframe {
     width: 100%;
     height: 100%;
     border: none;
     flex: 1;
 }
-/* .wagtail-fedit-field-wrapper .wagtail-fedit-field-content, */
-/* .wagtail-fedit-block-wrapper .wagtail-fedit-block-content { */
-    /* position: relative; */
-/* } */
-/* .wagtail-fedit-field-wrapper .wagtail-fedit-field-content:not(:has(.wagtail-fedit-block-wrapper)):hover::after, */
-/* .wagtail-fedit-block-wrapper .wagtail-fedit-block-content:not(:has(.wagtail-fedit-block-wrapper:hover)):hover::after { */
-    /* content: ''; */
-    /* display: block; */
-    /* position: absolute; */
-    /* top: 0; */
-    /* left: 0; */
-    /* width: 100%; */
-    /* height: 100%; */
-    /* background-color: rgba(0, 0, 0, 0.05); */
-    /* outline: 2px solid #333333; */
-    /* pointer-events: none; */
-    /* z-index: 300; */
-/* } */
 .wagtail-fedit-modal-wrapper .wagtail-fedit-modal .wagtail-fedit-close-button {
     position: absolute;
     right: 0;
     top: 0;
     text-align: center;
     vertical-align: middle;
     padding: 0;
```

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -137,18 +137,15 @@
     }
 
     get wrapperElementContent() {
         return this.wrapperElement.querySelector(`.wagtail-fedit-${this.type}-content`);
     }
 
     focus() {
-        const rect = this.wrapperElementContent.getBoundingClientRect();
-        if ((rect.top + rect.height) > window.innerHeight) {
-            window.scrollTo(0, rect.top);
-        }
+        this.wrapperElementContent.focus();
     }
 
     makeModal() {
         this.modalWrapper.innerHTML = this.modalHtml;
         this.modal = this.modalWrapper.querySelector(".wagtail-fedit-modal");
         this.iframe = new iFrame({
             url: this.editUrl,
```

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.2.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x08760d66 (Wed Apr  3 15:30:16 2024 UTC)
-files sz: 13707
+moddate:  0x33aa0d66 (Wed Apr  3 19:12:51 2024 UTC)
+files sz: 13805
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -17,18 +17,18 @@
       225a226d235a230100020065016a240000000000000000a6000000ab0000
       000000000000005a25020065106a260000000000000000a6000000ab0000
       000000000000005a2764125a2864135a29020047006414840064156502a6
       030000ab0300000000000000005a2a6525a02b0000000000000000000000
       0000000000000000006416ac17a6010000ab010000000000000000641865
       07641965086604641a8404a6000000ab0000000000000000005a2c6525a0
       2d0000000000000000000000000000000000000000641b641cac1da60200
-      00ab0200000000000000006425641e8401a6000000ab0000000000000000
-      005a2e641f84005a2f641865076420653065311900000000000000000064
-      216530653119000000000000000000642265326608642384045a33642484
-      005a34640d5300
+      00ab0200000000000000006427641f652e660264208405a6000000ab0000
+      000000000000005a2f642184005a30641865076422653165321900000000
+      000000000064236531653219000000000000000000642465336608642584
+      045a34642684005a35640d5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('library', 'Node', 'NodeList'))
                  6 IMPORT_NAME              0 (django.template)
                  8 IMPORT_FROM              1 (library)
                 10 STORE_NAME               1 (library)
@@ -205,49 +205,52 @@
                388 LOAD_METHOD             45 (simple_tag)
                410 LOAD_CONST              27 (True)
                412 LOAD_CONST              28 ('fedit_field')
                414 KW_NAMES                29
                416 PRECALL                  2
                420 CALL                     2
    
-   290         430 LOAD_CONST              37 ((None,))
-               432 LOAD_CONST              30 (<code object do_render_fedit_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 289>)
-               434 MAKE_FUNCTION            1 (defaults)
-   
-   289         436 PRECALL                  0
-               440 CALL                     0
-   
-   290         450 STORE_NAME              46 (do_render_fedit_field)
-   
-   339         452 LOAD_CONST              31 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 339>)
-               454 MAKE_FUNCTION            0
-               456 STORE_NAME              47 (render_editable_field)
-   
-   378         458 LOAD_CONST              24 ('parser')
-               460 LOAD_NAME                7 (Parser)
-               462 LOAD_CONST              32 ('kwarg_list')
-               464 LOAD_NAME               48 (list)
-               466 LOAD_NAME               49 (str)
-               468 BINARY_SUBSCR
-               478 LOAD_CONST              33 ('tokens')
-               480 LOAD_NAME               48 (list)
-               482 LOAD_NAME               49 (str)
-               484 BINARY_SUBSCR
-               494 LOAD_CONST              34 ('return')
-               496 LOAD_NAME               50 (dict)
-               498 BUILD_TUPLE              8
-               500 LOAD_CONST              35 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 378>)
-               502 MAKE_FUNCTION            4 (annotations)
-               504 STORE_NAME              51 (get_kwargs)
-   
-   405         506 LOAD_CONST              36 (<code object _get_from_context_or_set, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 405>)
-               508 MAKE_FUNCTION            0
-               510 STORE_NAME              52 (_get_from_context_or_set)
-               512 LOAD_CONST              13 (None)
-               514 RETURN_VALUE
+   290         430 LOAD_CONST              39 ((None, False))
+               432 LOAD_CONST              31 ('inline')
+               434 LOAD_NAME               46 (bool)
+               436 BUILD_TUPLE              2
+               438 LOAD_CONST              32 (<code object do_render_fedit_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 289>)
+               440 MAKE_FUNCTION            5 (defaults, annotations)
+   
+   289         442 PRECALL                  0
+               446 CALL                     0
+   
+   290         456 STORE_NAME              47 (do_render_fedit_field)
+   
+   340         458 LOAD_CONST              33 (<code object render_editable_field, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 340>)
+               460 MAKE_FUNCTION            0
+               462 STORE_NAME              48 (render_editable_field)
+   
+   380         464 LOAD_CONST              24 ('parser')
+               466 LOAD_NAME                7 (Parser)
+               468 LOAD_CONST              34 ('kwarg_list')
+               470 LOAD_NAME               49 (list)
+               472 LOAD_NAME               50 (str)
+               474 BINARY_SUBSCR
+               484 LOAD_CONST              35 ('tokens')
+               486 LOAD_NAME               49 (list)
+               488 LOAD_NAME               50 (str)
+               490 BINARY_SUBSCR
+               500 LOAD_CONST              36 ('return')
+               502 LOAD_NAME               51 (dict)
+               504 BUILD_TUPLE              8
+               506 LOAD_CONST              37 (<code object get_kwargs, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 380>)
+               508 MAKE_FUNCTION            4 (annotations)
+               510 STORE_NAME              52 (get_kwargs)
+   
+   407         512 LOAD_CONST              38 (<code object _get_from_context_or_set, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 407>)
+               514 MAKE_FUNCTION            0
+               516 STORE_NAME              53 (_get_from_context_or_set)
+               518 LOAD_CONST              13 (None)
+               520 RETURN_VALUE
    consts
       0
       ('library', 'Node', 'NodeList')
       ('render_to_string',)
       ('Parser', 'Token', 'TokenType')
       ('FilterExpression',)
       ('mark_safe',)
@@ -1641,36 +1644,39 @@
          firstlineno 229
          lnotab
             0x021e28012a010805220208012a012a0204020401320108010c020e0102
             0128012801280128fb040602fa
       True
       'fedit_field'
       ('takes_context', 'name')
+      False
+      'inline'
       code
-         argcount  : 4
-         nlocals   : 9
+         argcount  : 5
+         nlocals   : 10
          stacksize : 7
          flags     : 11
          code
             0x97007401000000000000000000007c017c026702a6010000ab01000000
             0000000000730f7403000000000000000000006401a6010000ab01000000
-            0000000000820169007d057c04a002000000000000000000000000000000
-            0000000000a6000000ab00000000000000000044005d0a5c0200007d067d
-            077c077c057c063c0000008c0b7c00a00300000000000000000000000000
-            000000000000006402a6010000ab0100000000000000007d087409000000
-            000000000000007c087c027c017c007c03ac03a6050000ab050000000000
-            0000007d037c0872717c086a0500000000000000006a0600000000000000
-            0072637c086a050000000000000000a00700000000000000000000000000
-            000000000000006404a6010000ab01000000000000000072497c086a0500
+            0000000000820169007d067c05a002000000000000000000000000000000
+            0000000000a6000000ab00000000000000000044005d0a5c0200007d077d
+            087c087c067c073c0000008c0b7c00a00300000000000000000000000000
+            000000000000006402a6010000ab0100000000000000007d097409000000
+            000000000000007c097c027c017c007c03ac03a6050000ab050000000000
+            0000007d037c0972717c096a0500000000000000006a0600000000000000
+            0072637c096a050000000000000000a00700000000000000000000000000
+            000000000000006404a6010000ab01000000000000000072497c096a0500
             00000000000000a00700000000000000000000000000000000000000007c
             026a0800000000000000006a0900000000000000009b0064057c026a0800
             000000000000006a0a00000000000000009b009d03a6010000ab01000000
-            000000000072167417000000000000000000007c08741800000000000000
+            000000000072167417000000000000000000007c09741800000000000000
             0000006406a6030000ab03000000000000000073027c035300741b000000
-            000000000000007c087c037c017c027c00660569007c05a4018e015300
+            000000000000007c097c037c017c027c00660569007c06a40164077c0469
+            01a4018e015300
          289           0 RESUME                   0
          
          307           2 LOAD_GLOBAL              1 (NULL + all)
                       14 LOAD_FAST                1 (field_name)
                       16 LOAD_FAST                2 (model)
                       18 BUILD_LIST               2
                       20 PRECALL                  1
@@ -1680,75 +1686,75 @@
          308          36 LOAD_GLOBAL              3 (NULL + ValueError)
                       48 LOAD_CONST               1 ('Field name, and model are required')
                       50 PRECALL                  1
                       54 CALL                     1
                       64 RAISE_VARARGS            1
          
          310     >>   66 BUILD_MAP                0
-                      68 STORE_FAST               5 (extra)
+                      68 STORE_FAST               6 (extra)
          
-         311          70 LOAD_FAST                4 (kwargs)
+         311          70 LOAD_FAST                5 (kwargs)
                       72 LOAD_METHOD              2 (items)
                       94 PRECALL                  0
                       98 CALL                     0
                      108 GET_ITER
                  >>  110 FOR_ITER                10 (to 132)
                      112 UNPACK_SEQUENCE          2
-                     116 STORE_FAST               6 (key)
-                     118 STORE_FAST               7 (value)
+                     116 STORE_FAST               7 (key)
+                     118 STORE_FAST               8 (value)
          
-         312         120 LOAD_FAST                7 (value)
-                     122 LOAD_FAST                5 (extra)
-                     124 LOAD_FAST                6 (key)
+         312         120 LOAD_FAST                8 (value)
+                     122 LOAD_FAST                6 (extra)
+                     124 LOAD_FAST                7 (key)
                      126 STORE_SUBSCR
                      130 JUMP_BACKWARD           11 (to 110)
          
          314     >>  132 LOAD_FAST                0 (context)
                      134 LOAD_METHOD              3 (get)
                      156 LOAD_CONST               2 ('request')
                      158 PRECALL                  1
                      162 CALL                     1
-                     172 STORE_FAST               8 (request)
+                     172 STORE_FAST               9 (request)
          
          315         174 LOAD_GLOBAL              9 (NULL + get_field_content)
          
-         316         186 LOAD_FAST                8 (request)
+         316         186 LOAD_FAST                9 (request)
          
          317         188 LOAD_FAST                2 (model)
          
          318         190 LOAD_FAST                1 (field_name)
          
          319         192 LOAD_FAST                0 (context)
          
          320         194 LOAD_FAST                3 (content)
          
          315         196 KW_NAMES                 3
                      198 PRECALL                  5
                      202 CALL                     5
                      212 STORE_FAST               3 (content)
          
-         323         214 LOAD_FAST                8 (request)
+         323         214 LOAD_FAST                9 (request)
                      216 POP_JUMP_FORWARD_IF_FALSE   113 (to 444)
          
-         325         218 LOAD_FAST                8 (request)
+         325         218 LOAD_FAST                9 (request)
                      220 LOAD_ATTR                5 (user)
                      230 LOAD_ATTR                6 (is_authenticated)
          
          324         240 POP_JUMP_FORWARD_IF_FALSE    99 (to 440)
          
-         326         242 LOAD_FAST                8 (request)
+         326         242 LOAD_FAST                9 (request)
                      244 LOAD_ATTR                5 (user)
                      254 LOAD_METHOD              7 (has_perm)
                      276 LOAD_CONST               4 ('wagtailadmin.access_admin')
                      278 PRECALL                  1
                      282 CALL                     1
          
          324         292 POP_JUMP_FORWARD_IF_FALSE    73 (to 440)
          
-         327         294 LOAD_FAST                8 (request)
+         327         294 LOAD_FAST                9 (request)
                      296 LOAD_ATTR                5 (user)
                      306 LOAD_METHOD              7 (has_perm)
                      328 LOAD_FAST                2 (model)
                      330 LOAD_ATTR                8 (_meta)
                      340 LOAD_ATTR                9 (app_label)
                      350 FORMAT_VALUE             0
                      352 LOAD_CONST               5 ('.change_')
@@ -1759,220 +1765,235 @@
                      378 BUILD_STRING             3
                      380 PRECALL                  1
                      384 CALL                     1
          
          324         394 POP_JUMP_FORWARD_IF_FALSE    22 (to 440)
          
          328         396 LOAD_GLOBAL             23 (NULL + getattr)
-                     408 LOAD_FAST                8 (request)
+                     408 LOAD_FAST                9 (request)
                      410 LOAD_GLOBAL             24 (FEDIT_PREVIEW_VAR)
                      422 LOAD_CONST               6 (False)
                      424 PRECALL                  3
                      428 CALL                     3
          
          324         438 POP_JUMP_FORWARD_IF_TRUE     2 (to 444)
          
          330     >>  440 LOAD_FAST                3 (content)
                      442 RETURN_VALUE
          
          332     >>  444 LOAD_GLOBAL             27 (NULL + render_editable_field)
          
-         333         456 LOAD_FAST                8 (request)
+         333         456 LOAD_FAST                9 (request)
                      458 LOAD_FAST                3 (content)
          
          334         460 LOAD_FAST                1 (field_name)
                      462 LOAD_FAST                2 (model)
          
          335         464 LOAD_FAST                0 (context)
          
          332         466 BUILD_TUPLE              5
                      468 BUILD_MAP                0
          
-         336         470 LOAD_FAST                5 (extra)
+         336         470 LOAD_FAST                6 (extra)
          
          332         472 DICT_MERGE               1
-                     474 CALL_FUNCTION_EX         1
-                     476 RETURN_VALUE
+                     474 LOAD_CONST               7 ('inline')
+         
+         337         476 LOAD_FAST                4 (inline)
+         
+         332         478 BUILD_MAP                1
+                     480 DICT_MERGE               1
+                     482 CALL_FUNCTION_EX         1
+                     484 RETURN_VALUE
          consts
             '\n    This tag is used to render an editable field.\n\n    This field will be wrapped and is able to be edited by the user on the frontend.\n\n    We will require the field_name of the field and the model instance.\n\n    Usage example:\n        ```python\n        {% fedit_field my_field_name page_instance %}\n        ```\n\n    Optionally your model can define a `render_fedit_{field_name}` method that will be used to render the field.\n    This will allow you to use custom rendering logic if need be.\n    '
             'Field name, and model are required'
             'request'
             ('content',)
             'wagtailadmin.access_admin'
             '.change_'
             False
+            'inline'
          names      ('all', 'ValueError', 'items', 'get', 'get_field_content', 'user', 'is_authenticated', 'has_perm', '_meta', 'app_label', 'model_name', 'getattr', 'FEDIT_PREVIEW_VAR', 'render_editable_field')
-         varnames   ('context', 'field_name', 'model', 'content', 'kwargs', 'extra', 'key', 'value', 'request')
+         varnames   ('context', 'field_name', 'model', 'content', 'inline', 'kwargs', 'extra', 'key', 'value', 'request')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'do_render_fedit_field'
          firstlineno 289
          lnotab
             0x021222011e02040132010c022a010c01020102010201020102fb120804
             0216ff020232fe020364fd02042afc020604020c010401040102fd040402
-            fc
+            fc040502fb
       code
          argcount  : 5
          nlocals   : 10
-         stacksize : 10
+         stacksize : 13
          flags     : 11
          code
             0x8700970074010000000000000000000064017c027c036a010000000000
             0000006a0200000000000000007c036a0100000000000000006a03000000
             00000000007c036a0400000000000000006704ac02a6020000ab02000000
             00000000007d067c057225740b00000000000000000000740d0000000000
-            00000000006a070000000000000000640b69007c05a4018e01a6010000ab
+            00000000006a070000000000000000640d69007c05a4018e01a6010000ab
             0100000000000000007d077c069b0064037c079b009d037d067411000000
             00000000000000a6000000ab00000000000000000067017d087413000000
             000000000000006a0a0000000000000000741600000000000000000000a6
             010000ab01000000000000000044005d117d0902007c0989007c087c037c
             02ac04a6040000ab04000000000000000001008c1288006601640584087c
             084400a6000000ab0000000000000000007d087419000000000000000000
             00741b0000000000000000000064007c08a6020000ab0200000000000000
             00a6010000ab0100000000000000007d087c027c0564063c0000007c037c
             0564073c000000741d0000000000000000000064087c067c027c037c017c
-            047c0864099c067c05a5018900ac0aa6030000ab03000000000000000053
-            00
+            047c087c05a00f0000000000000000000000000000000000000000640964
+            0aa6020000ab020000000000000000640b9c077c05a5018900ac0ca60300
+            00ab0300000000000000005300
                        0 MAKE_CELL                0 (request)
          
-         339           2 RESUME                   0
+         340           2 RESUME                   0
          
-         340           4 LOAD_GLOBAL              1 (NULL + reverse)
+         341           4 LOAD_GLOBAL              1 (NULL + reverse)
          
-         341          16 LOAD_CONST               1 ('wagtail_fedit:edit_field')
+         342          16 LOAD_CONST               1 ('wagtail_fedit:edit_field')
          
-         342          18 LOAD_FAST                2 (field_name)
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
          
-         340          78 KW_NAMES                 2
+         341          78 KW_NAMES                 2
                       80 PRECALL                  2
                       84 CALL                     2
                       94 STORE_FAST               6 (edit_url)
          
-         345          96 LOAD_FAST                5 (kwargs)
+         346          96 LOAD_FAST                5 (kwargs)
                       98 POP_JUMP_FORWARD_IF_FALSE    37 (to 174)
          
-         346         100 LOAD_GLOBAL             11 (NULL + urlencode)
+         347         100 LOAD_GLOBAL             11 (NULL + urlencode)
          
-         347         112 LOAD_GLOBAL             13 (NULL + BlockEditNode)
+         348         112 LOAD_GLOBAL             13 (NULL + BlockEditNode)
                      124 LOAD_ATTR                7 (pack)
-                     134 LOAD_CONST              11 (())
+                     134 LOAD_CONST              13 (())
                      136 BUILD_MAP                0
                      138 LOAD_FAST                5 (kwargs)
                      140 DICT_MERGE               1
                      142 CALL_FUNCTION_EX         1
          
-         346         144 PRECALL                  1
+         347         144 PRECALL                  1
                      148 CALL                     1
                      158 STORE_FAST               7 (packed)
          
-         349         160 LOAD_FAST                6 (edit_url)
+         350         160 LOAD_FAST                6 (edit_url)
                      162 FORMAT_VALUE             0
                      164 LOAD_CONST               3 ('?')
                      166 LOAD_FAST                7 (packed)
                      168 FORMAT_VALUE             0
                      170 BUILD_STRING             3
                      172 STORE_FAST               6 (edit_url)
          
-         352     >>  174 LOAD_GLOBAL             17 (NULL + FeditFieldEditButton)
+         353     >>  174 LOAD_GLOBAL             17 (NULL + FeditFieldEditButton)
                      186 PRECALL                  0
                      190 CALL                     0
          
-         351         200 BUILD_LIST               1
+         352         200 BUILD_LIST               1
                      202 STORE_FAST               8 (items)
          
-         355         204 LOAD_GLOBAL             19 (NULL + hooks)
+         356         204 LOAD_GLOBAL             19 (NULL + hooks)
                      216 LOAD_ATTR               10 (get_hooks)
                      226 LOAD_GLOBAL             22 (CONSTRUCT_FIELD_TOOLBAR)
                      238 PRECALL                  1
                      242 CALL                     1
                      252 GET_ITER
                  >>  254 FOR_ITER                17 (to 290)
                      256 STORE_FAST               9 (hook)
          
-         356         258 PUSH_NULL
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
          
-         358     >>  290 LOAD_CLOSURE             0 (request)
+         359     >>  290 LOAD_CLOSURE             0 (request)
                      292 BUILD_TUPLE              1
-                     294 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 358>)
+                     294 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\NigelvanKeulenGoodad\Desktop\goodadvice\Projecten\WAG\tester\wagtail_fedit\templatetags\fedit.py", line 359>)
                      296 MAKE_FUNCTION            8 (closure)
                      298 LOAD_FAST                8 (items)
                      300 GET_ITER
                      302 PRECALL                  0
                      306 CALL                     0
                      316 STORE_FAST               8 (items)
          
-         359         318 LOAD_GLOBAL             25 (NULL + list)
+         360         318 LOAD_GLOBAL             25 (NULL + list)
                      330 LOAD_GLOBAL             27 (NULL + filter)
                      342 LOAD_CONST               0 (None)
                      344 LOAD_FAST                8 (items)
                      346 PRECALL                  2
                      350 CALL                     2
                      360 PRECALL                  1
                      364 CALL                     1
                      374 STORE_FAST               8 (items)
          
-         361         376 LOAD_FAST                2 (field_name)
+         362         376 LOAD_FAST                2 (field_name)
                      378 LOAD_FAST                5 (kwargs)
                      380 LOAD_CONST               6 ('wagtail_fedit_field_name')
                      382 STORE_SUBSCR
          
-         362         386 LOAD_FAST                3 (model)
+         363         386 LOAD_FAST                3 (model)
                      388 LOAD_FAST                5 (kwargs)
                      390 LOAD_CONST               7 ('wagtail_fedit_instance')
                      392 STORE_SUBSCR
          
-         364         396 LOAD_GLOBAL             29 (NULL + render_to_string)
+         365         396 LOAD_GLOBAL             29 (NULL + render_to_string)
          
-         365         408 LOAD_CONST               8 ('wagtail_fedit/content/editable_field.html')
+         366         408 LOAD_CONST               8 ('wagtail_fedit/content/editable_field.html')
          
-         367         410 LOAD_FAST                6 (edit_url)
+         368         410 LOAD_FAST                6 (edit_url)
          
-         368         412 LOAD_FAST                2 (field_name)
+         369         412 LOAD_FAST                2 (field_name)
          
-         369         414 LOAD_FAST                3 (model)
+         370         414 LOAD_FAST                3 (model)
          
-         370         416 LOAD_FAST                1 (content)
+         371         416 LOAD_FAST                1 (content)
          
-         371         418 LOAD_FAST                4 (context)
+         372         418 LOAD_FAST                4 (context)
          
-         372         420 LOAD_FAST                8 (items)
+         373         420 LOAD_FAST                8 (items)
          
-         366         422 LOAD_CONST               9 (('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items'))
-                     424 BUILD_CONST_KEY_MAP      6
+         374         422 LOAD_FAST                5 (kwargs)
+                     424 LOAD_METHOD             15 (get)
+                     446 LOAD_CONST               9 ('inline')
+                     448 LOAD_CONST              10 (False)
+                     450 PRECALL                  2
+                     454 CALL                     2
          
-         373         426 LOAD_FAST                5 (kwargs)
+         367         464 LOAD_CONST              11 (('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items', 'inline'))
+                     466 BUILD_CONST_KEY_MAP      7
          
-         366         428 DICT_UPDATE              1
+         375         468 LOAD_FAST                5 (kwargs)
          
-         375         430 LOAD_DEREF               0 (request)
+         367         470 DICT_UPDATE              1
          
-         364         432 KW_NAMES                10
-                     434 PRECALL                  3
-                     438 CALL                     3
-                     448 RETURN_VALUE
+         377         472 LOAD_DEREF               0 (request)
+         
+         365         474 KW_NAMES                12
+                     476 PRECALL                  3
+                     480 CALL                     3
+                     490 RETURN_VALUE
          consts
             None
             'wagtail_fedit:edit_field'
             ('args',)
             '?'
             ('request', 'items', 'model', 'field_name')
             code
@@ -1981,15 +2002,15 @@
                stacksize : 5
                flags     : 19
                code
                   0x9501970067007c005d177d017c01a00000000000000000000000000000
                   000000000000008902a6010000ab01000000000000000091028c185300
                              0 COPY_FREE_VARS           1
                
-               358           2 RESUME                   0
+               359           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                23 (to 56)
                             10 STORE_FAST               1 (item)
                             12 LOAD_FAST                1 (item)
                             14 LOAD_METHOD              0 (render)
                             36 LOAD_DEREF               2 (request)
@@ -2001,33 +2022,35 @@
                consts
                names      ('render',)
                varnames   ('.0', 'item')
                freevars   ('request',)
                cellvars   ()
                filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
                name       '<listcomp>'
-               firstlineno 358
+               firstlineno 359
                lnotab 0x
             'wagtail_fedit_field_name'
             'wagtail_fedit_instance'
             'wagtail_fedit/content/editable_field.html'
-            ('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items')
+            'inline'
+            False
+            ('edit_url', 'field_name', 'model', 'content', 'parent_context', 'toolbar_items', 'inline')
             ('request',)
             ()
-         names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack', 'FeditFieldEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_FIELD_TOOLBAR', 'list', 'filter', 'render_to_string')
+         names      ('reverse', '_meta', 'app_label', 'model_name', 'pk', 'urlencode', 'BlockEditNode', 'pack', 'FeditFieldEditButton', 'hooks', 'get_hooks', 'CONSTRUCT_FIELD_TOOLBAR', 'list', 'filter', 'render_to_string', 'get')
          varnames   ('request', 'content', 'field_name', 'model', 'context', 'kwargs', 'edit_url', 'packed', 'items', 'hook')
          freevars   ()
          cellvars   ('request',)
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'render_editable_field'
-         firstlineno 339
+         firstlineno 340
          lnotab
             0x04010c0102013cfe120504010c0120ff10030e031aff0404360120021c
-            013a020a010a020c0102020201020102010201020102fa040702f9020902
-            f5
+            013a020a010a020c0102020201020102010201020102012af9040802f802
+            0a02f4
       'kwarg_list'
       'tokens'
       'return'
       code
          argcount  : 3
          nlocals   : 9
          stacksize : 5
@@ -2040,89 +2063,89 @@
             0064036b020000000072307c03720f7407000000000000000000006404a6
             010000ab01000000000000000082017c00a0040000000000000000000000
             0000000000000000007c06a6010000ab0100000000000000007c047c017c
             05190000000000000000003c0000008c5d7c076405190000000000000000
             007d087c00a00400000000000000000000000000000000000000007c0764
             0319000000000000000000a6010000ab0100000000000000007c047c083c
             00000064067d038c867c045300
-         378           0 RESUME                   0
+         380           0 RESUME                   0
          
-         379           2 LOAD_CONST               1 (False)
+         381           2 LOAD_CONST               1 (False)
                        4 STORE_FAST               3 (had_kwargs)
          
-         380           6 BUILD_MAP                0
+         382           6 BUILD_MAP                0
                        8 STORE_FAST               4 (kwargs)
          
-         385          10 LOAD_GLOBAL              1 (NULL + enumerate)
+         387          10 LOAD_GLOBAL              1 (NULL + enumerate)
                       22 LOAD_FAST                2 (tokens)
                       24 PRECALL                  1
                       28 CALL                     1
                       38 GET_ITER
                  >>   40 FOR_ITER               133 (to 308)
                       42 UNPACK_SEQUENCE          2
                       46 STORE_FAST               5 (i)
                       48 STORE_FAST               6 (token)
          
-         386          50 LOAD_FAST                6 (token)
+         388          50 LOAD_FAST                6 (token)
                       52 LOAD_METHOD              1 (split)
                       74 LOAD_CONST               2 ('=')
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_FAST               7 (split)
          
-         387          92 LOAD_GLOBAL              5 (NULL + len)
+         389          92 LOAD_GLOBAL              5 (NULL + len)
                      104 LOAD_FAST                7 (split)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               3 (1)
                      122 COMPARE_OP               2 (==)
                      128 POP_JUMP_FORWARD_IF_FALSE    48 (to 226)
          
-         388         130 LOAD_FAST                3 (had_kwargs)
+         390         130 LOAD_FAST                3 (had_kwargs)
                      132 POP_JUMP_FORWARD_IF_FALSE    15 (to 164)
          
-         389         134 LOAD_GLOBAL              7 (NULL + ValueError)
+         391         134 LOAD_GLOBAL              7 (NULL + ValueError)
                      146 LOAD_CONST               4 ('Unexpected positional argument after keyword argument')
                      148 PRECALL                  1
                      152 CALL                     1
                      162 RAISE_VARARGS            1
          
-         391     >>  164 LOAD_FAST                0 (parser)
+         393     >>  164 LOAD_FAST                0 (parser)
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
          
-         393     >>  226 LOAD_FAST                7 (split)
+         395     >>  226 LOAD_FAST                7 (split)
                      228 LOAD_CONST               5 (0)
                      230 BINARY_SUBSCR
                      240 STORE_FAST               8 (key)
          
-         397         242 LOAD_FAST                0 (parser)
+         399         242 LOAD_FAST                0 (parser)
                      244 LOAD_METHOD              4 (compile_filter)
                      266 LOAD_FAST                7 (split)
                      268 LOAD_CONST               3 (1)
                      270 BINARY_SUBSCR
                      280 PRECALL                  1
                      284 CALL                     1
                      294 LOAD_FAST                4 (kwargs)
                      296 LOAD_FAST                8 (key)
                      298 STORE_SUBSCR
          
-         398         302 LOAD_CONST               6 (True)
+         400         302 LOAD_CONST               6 (True)
                      304 STORE_FAST               3 (had_kwargs)
                      306 JUMP_BACKWARD          134 (to 40)
          
-         400     >>  308 LOAD_FAST                4 (kwargs)
+         402     >>  308 LOAD_FAST                4 (kwargs)
                      310 RETURN_VALUE
          consts
             None
             False
             '='
             1
             'Unexpected positional argument after keyword argument'
@@ -2130,74 +2153,74 @@
             True
          names      ('enumerate', 'split', 'len', 'ValueError', 'compile_filter')
          varnames   ('parser', 'kwarg_list', 'tokens', 'had_kwargs', 'kwargs', 'i', 'token', 'split', 'key')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       'get_kwargs'
-         firstlineno 378
+         firstlineno 380
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
-         405           0 RESUME                   0
+         407           0 RESUME                   0
          
-         406           2 LOAD_FAST                1 (key)
+         408           2 LOAD_FAST                1 (key)
                        4 LOAD_FAST                0 (context)
                        6 CONTAINS_OP              0
                        8 POP_JUMP_FORWARD_IF_FALSE     8 (to 26)
          
-         407          10 LOAD_FAST                0 (context)
+         409          10 LOAD_FAST                0 (context)
                       12 LOAD_FAST                1 (key)
                       14 BINARY_SUBSCR
                       24 RETURN_VALUE
          
-         409     >>   26 LOAD_GLOBAL              1 (NULL + callable)
+         411     >>   26 LOAD_GLOBAL              1 (NULL + callable)
                       38 LOAD_FAST                2 (value)
                       40 PRECALL                  1
                       44 CALL                     1
                       54 POP_JUMP_FORWARD_IF_FALSE     8 (to 72)
          
-         410          56 PUSH_NULL
+         412          56 PUSH_NULL
                       58 LOAD_FAST                2 (value)
                       60 LOAD_FAST                3 (args)
                       62 BUILD_MAP                0
                       64 LOAD_FAST                4 (kwargs)
                       66 DICT_MERGE               1
                       68 CALL_FUNCTION_EX         1
                       70 STORE_FAST               2 (value)
          
-         412     >>   72 LOAD_FAST                2 (value)
+         414     >>   72 LOAD_FAST                2 (value)
                       74 LOAD_FAST                0 (context)
                       76 LOAD_FAST                1 (key)
                       78 STORE_SUBSCR
          
-         413          82 LOAD_FAST                2 (value)
+         415          82 LOAD_FAST                2 (value)
                       84 RETURN_VALUE
          consts
             None
          names      ('callable',)
          varnames   ('context', 'key', 'value', 'args', 'kwargs')
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
          name       '_get_from_context_or_set'
-         firstlineno 405
+         firstlineno 407
          lnotab 0x0201080110021e0110020a01
-      (None,)
-   names      ('django.template', 'library', 'Node', 'NodeList', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'TokenType', 'FilterExpression', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'django.db', 'models', 'wagtail.blocks', 'BoundBlock', 'wagtail.models', 'Page', 'wagtail', 'hooks', 'urllib.parse', 'urlencode', 'warnings', 'toolbar', 'FeditBlockEditButton', 'FeditFieldEditButton', 'utils', 'FEDIT_PREVIEW_VAR', 'get_field_content', 'CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR', 'Library', 'register', 'TimestampSigner', 'url_value_signer', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'BlockEditNode', 'tag', 'do_render_fedit_block', 'simple_tag', 'do_render_fedit_field', 'render_editable_field', 'list', 'str', 'dict', 'get_kwargs', '_get_from_context_or_set')
+      (None, False)
+   names      ('django.template', 'library', 'Node', 'NodeList', 'django.template.loader', 'render_to_string', 'django.template.base', 'Parser', 'Token', 'TokenType', 'FilterExpression', 'django.utils.safestring', 'mark_safe', 'django.urls', 'reverse', 'django.core', 'signing', 'django.db', 'models', 'wagtail.blocks', 'BoundBlock', 'wagtail.models', 'Page', 'wagtail', 'hooks', 'urllib.parse', 'urlencode', 'warnings', 'toolbar', 'FeditBlockEditButton', 'FeditFieldEditButton', 'utils', 'FEDIT_PREVIEW_VAR', 'get_field_content', 'CONSTRUCT_BLOCK_TOOLBAR', 'CONSTRUCT_FIELD_TOOLBAR', 'Library', 'register', 'TimestampSigner', 'url_value_signer', 'WARNING_FIELD_NAME_NOT_AVAILABLE', 'WARNING_MODEL_INSTANCE_NOT_AVAILABLE', 'BlockEditNode', 'tag', 'do_render_fedit_block', 'simple_tag', 'bool', 'do_render_fedit_field', 'render_editable_field', 'list', 'str', 'dict', 'get_kwargs', '_get_from_context_or_set')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\NigelvanKeulenGoodad\\Desktop\\goodadvice\\Projecten\\WAG\\tester\\wagtail_fedit\\templatetags\\fedit.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020114010c0114010c010c010c010c010c020c010c010c010c0208
-      021004100110061e011e03040104031c7f00422a010eff0e01023b2c0106
-      ff0e0102310627301b
+      021004100110061e011e03040104031c7f00422a010eff0e01023b2c010c
+      ff0e0102320628301b
```

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.2.3/wagtail_fedit/templatetags/fedit.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,15 +283,15 @@
         field_name=kwargs.get("field_name"),
         model=kwargs.get("model"),
         **extra,
     )
 
 
 @register.simple_tag(takes_context=True, name="fedit_field")
-def do_render_fedit_field(context, field_name, model, content=None, **kwargs):
+def do_render_fedit_field(context, field_name, model, content=None, inline: bool = False, **kwargs):
     """
     This tag is used to render an editable field.
 
     This field will be wrapped and is able to be edited by the user on the frontend.
 
     We will require the field_name of the field and the model instance.
 
@@ -330,14 +330,15 @@
             return content
 
     return render_editable_field(
         request, content,
         field_name, model,
         context,
         **extra,
+        inline=inline,
     )
 
 def render_editable_field(request, content, field_name, model, context, **kwargs):
     edit_url = reverse(
         "wagtail_fedit:edit_field",
         args=[field_name, model._meta.app_label, model._meta.model_name, model.pk]
     )
@@ -366,14 +367,15 @@
         {
             "edit_url": edit_url,
             "field_name": field_name,
             "model": model,
             "content": content,
             "parent_context": context,
             "toolbar_items": items,
+            "inline": kwargs.get("inline", False),
             **kwargs,
         },
         request=request,
     )
 
 def get_kwargs(parser: Parser, kwarg_list: list[str], tokens: list[str]) -> dict:
     had_kwargs = False
```

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.2.3/wagtail_fedit/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.2.3/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/urls.py` & `wagtail_fedit-1.2.3/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/utils.py` & `wagtail_fedit-1.2.3/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.2.3/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.2.3/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.2.3/wagtail_fedit/views/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,14 +213,15 @@
             )
 
             # Render the frame HTML
             html = render_editable_field(
                 self.request, content,
                 self.field_name, self.original_instance,
                 context=context,
+                **self.data,
             )
 
             return JsonResponse({
                 "success": True,
                 "html": html,
             })
```

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.2.3/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.2.2
+Version: 1.2.3
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.2 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.3 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.2.2/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.2.3/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

