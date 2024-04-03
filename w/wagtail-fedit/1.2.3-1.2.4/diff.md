# Comparing `tmp/wagtail_fedit-1.2.3.tar.gz` & `tmp/wagtail_fedit-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.2.3.tar", last modified: Wed Apr  3 19:34:17 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.2.4.tar", last modified: Wed Apr  3 19:46:27 2024, max compression
```

## Comparing `wagtail_fedit-1.2.3.tar` & `wagtail_fedit-1.2.4.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.711019 wagtail_fedit-1.2.3/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     5493 2024-04-03 19:34:17.711019 wagtail_fedit-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.2.3/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-03 19:34:17.716698 wagtail_fedit-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.552022 wagtail_fedit-1.2.3/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.553670 wagtail_fedit-1.2.3/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.556651 wagtail_fedit-1.2.3/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.557621 wagtail_fedit-1.2.3/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.563627 wagtail_fedit-1.2.3/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.3/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.575425 wagtail_fedit-1.2.3/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.3/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.3/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.3/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.588825 wagtail_fedit-1.2.3/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.2.3/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.2.3/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.2.3/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      625 2024-04-03 15:41:06.000000 wagtail_fedit-1.2.3/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.589793 wagtail_fedit-1.2.3/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.3/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.590790 wagtail_fedit-1.2.3/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.3/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.543388 wagtail_fedit-1.2.3/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.543388 wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.596828 wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4225 2024-04-03 19:33:47.000000 wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.619884 wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    11781 2024-04-03 19:13:47.000000 wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.543957 wagtail_fedit-1.2.3/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.545008 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.623390 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.627400 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.637925 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
--rw-rw-rw-   0        0        0     3002 2024-04-03 17:39:24.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.643430 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-03 17:05:19.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.652451 wagtail_fedit-1.2.3/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.2.3/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.655092 wagtail_fedit-1.2.3/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.3/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16811 2024-04-03 19:12:53.000000 wagtail_fedit-1.2.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13805 2024-04-03 19:12:51.000000 wagtail_fedit-1.2.3/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.662048 wagtail_fedit-1.2.3/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.2.3/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.2.3/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.2.3/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.2.3/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     5512 2024-04-03 17:02:56.000000 wagtail_fedit-1.2.3/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.688951 wagtail_fedit-1.2.3/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.2.3/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8659 2024-04-03 12:33:35.000000 wagtail_fedit-1.2.3/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.2.3/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     9076 2024-04-03 19:10:55.000000 wagtail_fedit-1.2.3/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.707994 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      132 2024-04-03 15:22:27.000000 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/editorjs.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:34:17.710061 wagtail_fedit-1.2.3/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     5493 2024-04-03 19:34:17.000000 wagtail_fedit-1.2.3/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2664 2024-04-03 19:34:17.000000 wagtail_fedit-1.2.3/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 19:34:17.000000 wagtail_fedit-1.2.3/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-03 19:34:17.000000 wagtail_fedit-1.2.3/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-03 19:34:17.000000 wagtail_fedit-1.2.3/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.789026 wagtail_fedit-1.2.4/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5493 2024-04-03 19:46:27.787018 wagtail_fedit-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.2.4/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-03 19:46:27.807798 wagtail_fedit-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.149489 wagtail_fedit-1.2.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.152481 wagtail_fedit-1.2.4/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.157459 wagtail_fedit-1.2.4/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.159520 wagtail_fedit-1.2.4/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.174294 wagtail_fedit-1.2.4/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.4/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.270224 wagtail_fedit-1.2.4/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.4/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.4/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.4/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.360941 wagtail_fedit-1.2.4/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.2.4/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.2.4/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.2.4/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      625 2024-04-03 15:41:06.000000 wagtail_fedit-1.2.4/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.363944 wagtail_fedit-1.2.4/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.4/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.366136 wagtail_fedit-1.2.4/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.4/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.125991 wagtail_fedit-1.2.4/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.126981 wagtail_fedit-1.2.4/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.392227 wagtail_fedit-1.2.4/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.2.4/wagtail_fedit/static/wagtail_fedit/css/admin.css
+-rw-rw-rw-   0        0        0     4135 2024-04-03 19:34:43.000000 wagtail_fedit-1.2.4/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4052 2024-03-31 20:57:59.000000 wagtail_fedit-1.2.4/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.420867 wagtail_fedit-1.2.4/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    11781 2024-04-03 19:13:47.000000 wagtail_fedit-1.2.4/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.128978 wagtail_fedit-1.2.4/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.130982 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.430403 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.438947 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.501522 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
+-rw-rw-rw-   0        0        0     3002 2024-04-03 17:39:24.000000 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0     1289 2024-04-02 19:59:07.000000 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0     1581 2024-04-02 19:18:49.000000 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.516984 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0     1023 2024-04-03 17:05:19.000000 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.525066 wagtail_fedit-1.2.4/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.2.4/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.531063 wagtail_fedit-1.2.4/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.4/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16811 2024-04-03 19:12:53.000000 wagtail_fedit-1.2.4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13828 2024-04-03 19:45:20.000000 wagtail_fedit-1.2.4/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.552919 wagtail_fedit-1.2.4/wagtail_fedit/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.2.4/wagtail_fedit/tests/__init__.py
+-rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.2.4/wagtail_fedit/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.2.4/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.2.4/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0     5512 2024-04-03 17:02:56.000000 wagtail_fedit-1.2.4/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.650681 wagtail_fedit-1.2.4/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.2.4/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8659 2024-04-03 12:33:35.000000 wagtail_fedit-1.2.4/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.2.4/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     9076 2024-04-03 19:10:55.000000 wagtail_fedit-1.2.4/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.779466 wagtail_fedit-1.2.4/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      132 2024-04-03 15:22:27.000000 wagtail_fedit-1.2.4/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.2.4/wagtail_fedit/wagtail_hooks/editorjs.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.2.4/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.2.4/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.2.4/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.2.4/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.2.4/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:46:27.784078 wagtail_fedit-1.2.4/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     5493 2024-04-03 19:46:26.000000 wagtail_fedit-1.2.4/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2664 2024-04-03 19:46:27.000000 wagtail_fedit-1.2.4/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 19:46:26.000000 wagtail_fedit-1.2.4/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-03 19:46:26.000000 wagtail_fedit-1.2.4/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-03 19:46:26.000000 wagtail_fedit-1.2.4/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.2.3/LICENSE` & `wagtail_fedit-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/PKG-INFO` & `wagtail_fedit-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.2.3
+Version: 1.2.4
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.3 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.4 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.2.3/README.md` & `wagtail_fedit-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/setup.cfg` & `wagtail_fedit-1.2.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 322e  ..version = 1.2.
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

### Comparing `wagtail_fedit-1.2.3/tests/testapp/manage.py` & `wagtail_fedit-1.2.4/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.2.4/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.2.4/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.2.4/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.2.4/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/hooks.py` & `wagtail_fedit-1.2.4/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.2.4/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,15 @@
     width: 100%;
     height: 100%;
     background-color: rgba(0, 0, 0, 0.05);
     outline: 2px solid #333333;
     pointer-events: none;
     z-index: 300;
 }
-.wagtail-fedit-field-wrapper:has(.wagtail-fedit-block-wrapper) > .wagtail-fedit-buttons,
-.wagtail-fedit-block-wrapper:has(.wagtail-fedit-block-wrapper) > .wagtail-fedit-buttons {
+.wagtail-fedit-field-wrapper:has(.wagtail-fedit-block-wrapper) > .wagtail-fedit-buttons {
     right: 30px;
 }
 .wagtail-fedit-buttons {
     display: flex;
     gap: 0.5em;
     border-radius: 0.5em;
     position: absolute;
```

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.2.4/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.2.4/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.2.4/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.2.4/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.2.4/wagtail_fedit/templatetags/fedit.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,15 +367,15 @@
         {
             "edit_url": edit_url,
             "field_name": field_name,
             "model": model,
             "content": content,
             "parent_context": context,
             "toolbar_items": items,
-            "inline": kwargs.get("inline", False),
+            "inline": str(kwargs.get("inline", False)).lower() == "true",
             **kwargs,
         },
         request=request,
     )
 
 def get_kwargs(parser: Parser, kwarg_list: list[str], tokens: list[str]) -> dict:
     had_kwargs = False
```

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.2.4/wagtail_fedit/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.2.4/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/urls.py` & `wagtail_fedit-1.2.4/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/utils.py` & `wagtail_fedit-1.2.4/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.2.4/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.2.4/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.2.4/wagtail_fedit/views/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.2.4/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.2.4/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.2.4/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.2.3
+Version: 1.2.4
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.3 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.4 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.2.3/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.2.4/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

