# Comparing `tmp/wagtail_fedit-1.2.5.tar.gz` & `tmp/wagtail_fedit-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_fedit-1.2.5.tar", last modified: Wed Apr  3 20:04:06 2024, max compression
+gzip compressed data, was "wagtail_fedit-1.2.6.tar", last modified: Wed Apr  3 20:07:46 2024, max compression
```

## Comparing `wagtail_fedit-1.2.5.tar` & `wagtail_fedit-1.2.6.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.508141 wagtail_fedit-1.2.5/
--rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     5493 2024-04-03 20:04:06.508141 wagtail_fedit-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.2.5/README.md
--rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/pyproject.toml
--rw-rw-rw-   0        0        0     1036 2024-04-03 20:04:06.523911 wagtail_fedit-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:05.803960 wagtail_fedit-1.2.5/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:05.823817 wagtail_fedit-1.2.5/tests/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/tests/testapp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:05.840526 wagtail_fedit-1.2.5/tests/testapp/core/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/tests/testapp/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:05.842531 wagtail_fedit-1.2.5/tests/testapp/core/migrations/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/tests/testapp/core/migrations/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/tests/testapp/core/tests.py
--rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/tests/testapp/manage.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:05.912943 wagtail_fedit-1.2.5/tests/testapp/testapp/
--rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/tests/testapp/testapp/__init__.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/tests/testapp/testapp/asgi.py
--rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/tests/testapp/testapp/settings.py
--rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/tests/testapp/testapp/urls.py
--rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.5/tests/testapp/testapp/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:05.996422 wagtail_fedit-1.2.5/wagtail_fedit/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.5/wagtail_fedit/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.5/wagtail_fedit/admin.py
--rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.5/wagtail_fedit/apps.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.072293 wagtail_fedit-1.2.5/wagtail_fedit/forms/
--rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.2.5/wagtail_fedit/forms/__init__.py
--rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.2.5/wagtail_fedit/forms/blocks.py
--rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.2.5/wagtail_fedit/forms/fields.py
--rw-rw-rw-   0        0        0      625 2024-04-03 15:41:06.000000 wagtail_fedit-1.2.5/wagtail_fedit/hooks.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.075826 wagtail_fedit-1.2.5/wagtail_fedit/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.5/wagtail_fedit/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.077820 wagtail_fedit-1.2.5/wagtail_fedit/migrations/__pycache__/
--rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.5/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:05.753675 wagtail_fedit-1.2.5/wagtail_fedit/static/
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:05.756709 wagtail_fedit-1.2.5/wagtail_fedit/static/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.109161 wagtail_fedit-1.2.5/wagtail_fedit/static/wagtail_fedit/css/
--rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.2.5/wagtail_fedit/static/wagtail_fedit/css/admin.css
--rw-rw-rw-   0        0        0     4135 2024-04-03 19:34:43.000000 wagtail_fedit-1.2.5/wagtail_fedit/static/wagtail_fedit/css/frontend.css
--rw-rw-rw-   0        0        0     4431 2024-04-03 20:01:24.000000 wagtail_fedit-1.2.5/wagtail_fedit/static/wagtail_fedit/css/furniture.css
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.134262 wagtail_fedit-1.2.5/wagtail_fedit/static/wagtail_fedit/js/
--rw-rw-rw-   0        0        0    12165 2024-04-03 20:03:43.000000 wagtail_fedit-1.2.5/wagtail_fedit/static/wagtail_fedit/js/frontend.js
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:05.759709 wagtail_fedit-1.2.5/wagtail_fedit/templates/
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:05.764223 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.162641 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/content/
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.194345 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/
--rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
--rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
--rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
--rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.267551 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/editor/
--rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
--rw-rw-rw-   0        0        0     3002 2024-04-03 17:39:24.000000 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
--rw-rw-rw-   0        0        0     1283 2024-04-03 19:57:11.000000 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
--rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/editor/field.html
--rw-rw-rw-   0        0        0     1593 2024-04-03 19:52:48.000000 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
--rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.311889 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/userbar/
--rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
--rw-rw-rw-   0        0        0     1023 2024-04-03 17:05:19.000000 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
--rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.329860 wagtail_fedit-1.2.5/wagtail_fedit/templatetags/
--rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.2.5/wagtail_fedit/templatetags/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.335365 wagtail_fedit-1.2.5/wagtail_fedit/templatetags/__pycache__/
--rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.5/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16924 2024-04-03 19:52:53.000000 wagtail_fedit-1.2.5/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
--rw-rw-rw-   0        0        0    13828 2024-04-03 19:45:20.000000 wagtail_fedit-1.2.5/wagtail_fedit/templatetags/fedit.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.350906 wagtail_fedit-1.2.5/wagtail_fedit/tests/
--rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.2.5/wagtail_fedit/tests/__init__.py
--rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.2.5/wagtail_fedit/tests/test_blocks.py
--rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.2.5/wagtail_fedit/toolbar.py
--rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.2.5/wagtail_fedit/urls.py
--rw-rw-rw-   0        0        0     5512 2024-04-03 17:02:56.000000 wagtail_fedit-1.2.5/wagtail_fedit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.410876 wagtail_fedit-1.2.5/wagtail_fedit/views/
--rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.2.5/wagtail_fedit/views/__init__.py
--rw-rw-rw-   0        0        0     8705 2024-04-03 19:57:05.000000 wagtail_fedit-1.2.5/wagtail_fedit/views/blocks.py
--rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.2.5/wagtail_fedit/views/editable.py
--rw-rw-rw-   0        0        0     9164 2024-04-03 19:55:52.000000 wagtail_fedit-1.2.5/wagtail_fedit/views/fields.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.502600 wagtail_fedit-1.2.5/wagtail_fedit/wagtail_hooks/
--rw-rw-rw-   0        0        0      132 2024-04-03 15:22:27.000000 wagtail_fedit-1.2.5/wagtail_fedit/wagtail_hooks/__init__.py
--rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.2.5/wagtail_fedit/wagtail_hooks/editorjs.py
--rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.2.5/wagtail_fedit/wagtail_hooks/excluded_relations.py
--rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.2.5/wagtail_fedit/wagtail_hooks/log_actions.py
--rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.2.5/wagtail_fedit/wagtail_hooks/renderers.py
--rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.2.5/wagtail_fedit/wagtail_hooks/urls.py
--rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.2.5/wagtail_fedit/wagtail_hooks/userbar.py
-drwxrwxrwx   0        0        0        0 2024-04-03 20:04:06.506140 wagtail_fedit-1.2.5/wagtail_fedit.egg-info/
--rw-rw-rw-   0        0        0     5493 2024-04-03 20:04:05.000000 wagtail_fedit-1.2.5/wagtail_fedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2664 2024-04-03 20:04:05.000000 wagtail_fedit-1.2.5/wagtail_fedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 20:04:05.000000 wagtail_fedit-1.2.5/wagtail_fedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-03 20:04:05.000000 wagtail_fedit-1.2.5/wagtail_fedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-03 20:04:05.000000 wagtail_fedit-1.2.5/wagtail_fedit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:46.118295 wagtail_fedit-1.2.6/
+-rw-rw-rw-   0        0        0    18429 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     5493 2024-04-03 20:07:46.116293 wagtail_fedit-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4443 2024-04-02 21:04:55.000000 wagtail_fedit-1.2.6/README.md
+-rw-rw-rw-   0        0        0       90 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1036 2024-04-03 20:07:46.132084 wagtail_fedit-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.890517 wagtail_fedit-1.2.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.894068 wagtail_fedit-1.2.6/tests/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/tests/testapp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.896079 wagtail_fedit-1.2.6/tests/testapp/core/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/tests/testapp/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.897085 wagtail_fedit-1.2.6/tests/testapp/core/migrations/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/tests/testapp/core/migrations/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/tests/testapp/core/tests.py
+-rw-rw-rw-   0        0        0      685 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/tests/testapp/manage.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.904589 wagtail_fedit-1.2.6/tests/testapp/testapp/
+-rw-rw-rw-   0        0        0        0 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/tests/testapp/testapp/__init__.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/tests/testapp/testapp/asgi.py
+-rw-rw-rw-   0        0        0     3513 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/tests/testapp/testapp/settings.py
+-rw-rw-rw-   0        0        0      785 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/tests/testapp/testapp/urls.py
+-rw-rw-rw-   0        0        0      407 2024-04-01 21:25:40.000000 wagtail_fedit-1.2.6/tests/testapp/testapp/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.926836 wagtail_fedit-1.2.6/wagtail_fedit/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.6/wagtail_fedit/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.6/wagtail_fedit/admin.py
+-rw-rw-rw-   0        0        0      163 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.6/wagtail_fedit/apps.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.945352 wagtail_fedit-1.2.6/wagtail_fedit/forms/
+-rw-rw-rw-   0        0        0       71 2024-04-02 19:03:21.000000 wagtail_fedit-1.2.6/wagtail_fedit/forms/__init__.py
+-rw-rw-rw-   0        0        0     2437 2024-04-02 23:35:48.000000 wagtail_fedit-1.2.6/wagtail_fedit/forms/blocks.py
+-rw-rw-rw-   0        0        0     1680 2024-04-02 20:02:53.000000 wagtail_fedit-1.2.6/wagtail_fedit/forms/fields.py
+-rw-rw-rw-   0        0        0      625 2024-04-03 15:41:06.000000 wagtail_fedit-1.2.6/wagtail_fedit/hooks.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.946297 wagtail_fedit-1.2.6/wagtail_fedit/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:25.000000 wagtail_fedit-1.2.6/wagtail_fedit/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.947299 wagtail_fedit-1.2.6/wagtail_fedit/migrations/__pycache__/
+-rw-rw-rw-   0        0        0      215 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.6/wagtail_fedit/migrations/__pycache__/__init__.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.877524 wagtail_fedit-1.2.6/wagtail_fedit/static/
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.878841 wagtail_fedit-1.2.6/wagtail_fedit/static/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.952297 wagtail_fedit-1.2.6/wagtail_fedit/static/wagtail_fedit/css/
+-rw-rw-rw-   0        0        0        0 2024-04-01 14:13:57.000000 wagtail_fedit-1.2.6/wagtail_fedit/static/wagtail_fedit/css/admin.css
+-rw-rw-rw-   0        0        0     4135 2024-04-03 19:34:43.000000 wagtail_fedit-1.2.6/wagtail_fedit/static/wagtail_fedit/css/frontend.css
+-rw-rw-rw-   0        0        0     4431 2024-04-03 20:01:24.000000 wagtail_fedit-1.2.6/wagtail_fedit/static/wagtail_fedit/css/furniture.css
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.973162 wagtail_fedit-1.2.6/wagtail_fedit/static/wagtail_fedit/js/
+-rw-rw-rw-   0        0        0    12165 2024-04-03 20:03:43.000000 wagtail_fedit-1.2.6/wagtail_fedit/static/wagtail_fedit/js/frontend.js
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.878841 wagtail_fedit-1.2.6/wagtail_fedit/templates/
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.880856 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.978730 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/content/
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:45.984206 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/
+-rw-rw-rw-   0        0        0      841 2024-04-03 17:50:55.000000 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html
+-rw-rw-rw-   0        0        0      841 2024-04-03 18:56:57.000000 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html
+-rw-rw-rw-   0        0        0      304 2024-04-03 19:23:41.000000 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/content/editable_block.html
+-rw-rw-rw-   0        0        0      337 2024-04-03 19:23:54.000000 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/content/editable_field.html
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:46.000742 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/editor/
+-rw-rw-rw-   0        0        0      473 2024-04-02 19:41:57.000000 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/editor/base_errors.html
+-rw-rw-rw-   0        0        0     3002 2024-04-03 17:39:24.000000 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html
+-rw-rw-rw-   0        0        0     1283 2024-04-03 19:57:11.000000 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html
+-rw-rw-rw-   0        0        0      496 2024-04-02 17:46:59.000000 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/editor/field.html
+-rw-rw-rw-   0        0        0     1939 2024-04-03 20:05:44.000000 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html
+-rw-rw-rw-   0        0        0     1979 2024-04-01 14:40:40.000000 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:46.013874 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/userbar/
+-rw-rw-rw-   0        0        0      867 2024-04-03 17:05:21.000000 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html
+-rw-rw-rw-   0        0        0     1023 2024-04-03 17:05:19.000000 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html
+-rw-rw-rw-   0        0        0      876 2024-04-03 16:59:31.000000 wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:46.027961 wagtail_fedit-1.2.6/wagtail_fedit/templatetags/
+-rw-rw-rw-   0        0        0        0 2024-03-29 20:13:42.000000 wagtail_fedit-1.2.6/wagtail_fedit/templatetags/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:46.032482 wagtail_fedit-1.2.6/wagtail_fedit/templatetags/__pycache__/
+-rw-rw-rw-   0        0        0      217 2024-03-29 21:05:00.000000 wagtail_fedit-1.2.6/wagtail_fedit/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16924 2024-04-03 19:52:53.000000 wagtail_fedit-1.2.6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13828 2024-04-03 19:45:20.000000 wagtail_fedit-1.2.6/wagtail_fedit/templatetags/fedit.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:46.045296 wagtail_fedit-1.2.6/wagtail_fedit/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-01 19:16:20.000000 wagtail_fedit-1.2.6/wagtail_fedit/tests/__init__.py
+-rw-rw-rw-   0        0        0     8737 2024-04-02 19:03:52.000000 wagtail_fedit-1.2.6/wagtail_fedit/tests/test_blocks.py
+-rw-rw-rw-   0        0        0     1571 2024-04-01 17:16:59.000000 wagtail_fedit-1.2.6/wagtail_fedit/toolbar.py
+-rw-rw-rw-   0        0        0      649 2024-04-01 13:49:58.000000 wagtail_fedit-1.2.6/wagtail_fedit/urls.py
+-rw-rw-rw-   0        0        0     5512 2024-04-03 17:02:56.000000 wagtail_fedit-1.2.6/wagtail_fedit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:46.080314 wagtail_fedit-1.2.6/wagtail_fedit/views/
+-rw-rw-rw-   0        0        0      143 2024-04-01 13:49:52.000000 wagtail_fedit-1.2.6/wagtail_fedit/views/__init__.py
+-rw-rw-rw-   0        0        0     8705 2024-04-03 19:57:05.000000 wagtail_fedit-1.2.6/wagtail_fedit/views/blocks.py
+-rw-rw-rw-   0        0        0     5323 2024-04-02 20:03:57.000000 wagtail_fedit-1.2.6/wagtail_fedit/views/editable.py
+-rw-rw-rw-   0        0        0     9314 2024-04-03 20:07:15.000000 wagtail_fedit-1.2.6/wagtail_fedit/views/fields.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:46.110900 wagtail_fedit-1.2.6/wagtail_fedit/wagtail_hooks/
+-rw-rw-rw-   0        0        0      132 2024-04-03 15:22:27.000000 wagtail_fedit-1.2.6/wagtail_fedit/wagtail_hooks/__init__.py
+-rw-rw-rw-   0        0        0      394 2024-04-02 18:34:41.000000 wagtail_fedit-1.2.6/wagtail_fedit/wagtail_hooks/editorjs.py
+-rw-rw-rw-   0        0        0      388 2024-04-01 18:08:02.000000 wagtail_fedit-1.2.6/wagtail_fedit/wagtail_hooks/excluded_relations.py
+-rw-rw-rw-   0        0        0     2503 2024-04-01 18:57:04.000000 wagtail_fedit-1.2.6/wagtail_fedit/wagtail_hooks/log_actions.py
+-rw-rw-rw-   0        0        0      472 2024-04-03 15:42:09.000000 wagtail_fedit-1.2.6/wagtail_fedit/wagtail_hooks/renderers.py
+-rw-rw-rw-   0        0        0      340 2024-03-30 17:10:05.000000 wagtail_fedit-1.2.6/wagtail_fedit/wagtail_hooks/urls.py
+-rw-rw-rw-   0        0        0     3192 2024-04-02 20:15:41.000000 wagtail_fedit-1.2.6/wagtail_fedit/wagtail_hooks/userbar.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:46.113897 wagtail_fedit-1.2.6/wagtail_fedit.egg-info/
+-rw-rw-rw-   0        0        0     5493 2024-04-03 20:07:45.000000 wagtail_fedit-1.2.6/wagtail_fedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2664 2024-04-03 20:07:45.000000 wagtail_fedit-1.2.6/wagtail_fedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 20:07:45.000000 wagtail_fedit-1.2.6/wagtail_fedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-03 20:07:45.000000 wagtail_fedit-1.2.6/wagtail_fedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-03 20:07:45.000000 wagtail_fedit-1.2.6/wagtail_fedit.egg-info/top_level.txt
```

### Comparing `wagtail_fedit-1.2.5/LICENSE` & `wagtail_fedit-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/PKG-INFO` & `wagtail_fedit-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.2.5
+Version: 1.2.6
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.5 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.6 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.2.5/README.md` & `wagtail_fedit-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/setup.cfg` & `wagtail_fedit-1.2.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 5f66 6564 6974   = wagtail_fedit
 00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 322e  ..version = 1.2.
-00000030: 350d 0a64 6573 6372 6970 7469 6f6e 203d  5..description =
+00000030: 360d 0a64 6573 6372 6970 7469 6f6e 203d  6..description =
 00000040: 2041 6e20 6170 706c 6963 6174 696f 6e20   An application 
 00000050: 6d61 6465 2066 6f72 2074 6865 2044 6a61  made for the Dja
 00000060: 6e67 6f20 5765 6220 4672 616d 6577 6f72  ngo Web Framewor
 00000070: 6b2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  k...long_descrip
 00000080: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000090: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 000000a0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `wagtail_fedit-1.2.5/tests/testapp/manage.py` & `wagtail_fedit-1.2.6/tests/testapp/manage.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/tests/testapp/testapp/settings.py` & `wagtail_fedit-1.2.6/tests/testapp/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/tests/testapp/testapp/urls.py` & `wagtail_fedit-1.2.6/tests/testapp/testapp/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/forms/blocks.py` & `wagtail_fedit-1.2.6/wagtail_fedit/forms/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/forms/fields.py` & `wagtail_fedit-1.2.6/wagtail_fedit/forms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/hooks.py` & `wagtail_fedit-1.2.6/wagtail_fedit/hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/static/wagtail_fedit/css/frontend.css` & `wagtail_fedit-1.2.6/wagtail_fedit/static/wagtail_fedit/css/frontend.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/static/wagtail_fedit/css/furniture.css` & `wagtail_fedit-1.2.6/wagtail_fedit/static/wagtail_fedit/css/furniture.css`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/static/wagtail_fedit/js/frontend.js` & `wagtail_fedit-1.2.6/wagtail_fedit/static/wagtail_fedit/js/frontend.js`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html` & `wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html` & `wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/content/buttons/edit_field.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html` & `wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/editor/base_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html` & `wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/editor/block_iframe.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html` & `wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/editor/field_iframe.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 {% extends "./base_iframe.html" %}
 
 {% load i18n wagtailadmin_tags %}
 
 {% block content %}
     <div class="wagtail-fedit-form-wrapper{% if form.block.block.meta.fedit_full %} fedit-full{% endif %}">
+        {% if not is_draft_capable %}
+            {% help_block status="info" %}
+                <p>{% translate "The object you are editing does not support drafts." %}</p>
+                <p>{% translate "You are not required to publish this object to make this change visible." %}</p>
+            {% endhelp_block %}
+        {% endif %}
         {% block errors %}
             {% if form.errors or form.non_field_errors %}
                 <div class="error-message">
                     <h2>{% translate "Validation errors" %}</h2>
                     <ul>
                         {% for error in form.non_field_errors %}
                             <li>{{ error }}</li>
```

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html` & `wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/editor/publish_confirm.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html` & `wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html` & `wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_publishing.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html` & `wagtail_fedit-1.2.6/wagtail_fedit/templates/wagtail_fedit/userbar/item_fedit_view_live.html`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc` & `wagtail_fedit-1.2.6/wagtail_fedit/templatetags/__pycache__/fedit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/templatetags/fedit.py` & `wagtail_fedit-1.2.6/wagtail_fedit/templatetags/fedit.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/tests/test_blocks.py` & `wagtail_fedit-1.2.6/wagtail_fedit/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/toolbar.py` & `wagtail_fedit-1.2.6/wagtail_fedit/toolbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/urls.py` & `wagtail_fedit-1.2.6/wagtail_fedit/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/utils.py` & `wagtail_fedit-1.2.6/wagtail_fedit/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/views/blocks.py` & `wagtail_fedit-1.2.6/wagtail_fedit/views/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/views/editable.py` & `wagtail_fedit-1.2.6/wagtail_fedit/views/editable.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/views/fields.py` & `wagtail_fedit-1.2.6/wagtail_fedit/views/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Type
+from typing import Any
 from django.db import models
 from django.shortcuts import render
 from django.template.loader import render_to_string
 from django.utils.translation import gettext as _
 from django.utils.decorators import method_decorator
 from django.views.decorators.clickjacking import xframe_options_sameorigin
 from django.views.generic import View
@@ -12,14 +12,15 @@
     JsonResponse,
     HttpResponse,
 )
 from django.apps import apps
 
 from wagtail.log_actions import log
 from wagtail.models import (
+    DraftStateMixin,
     RevisionMixin, 
 )
 from wagtail.admin.views.generic import WagtailAdminTemplateMixin
 
 import uuid
 
 from ..templatetags.fedit import (
@@ -129,14 +130,16 @@
                 "data-original-pk": self.original_instance.pk,
                 "data-original-model": self.model_name,
                 "data-original-app": self.app_label,
                 "data-original-field": self.field_name,
                 "data-is-relation": self.meta_field.is_relation\
                     and isinstance(self.field_value, models.Model),
             },
+            "is_draft_capable": issubclass(self.model, RevisionMixin)\
+                and issubclass(self.model, DraftStateMixin),
             "meta_field": self.meta_field,
             "field_name": self.field_name,
         }
 
     def get(self, request: HttpRequest, *args: Any, **kwargs: Any) -> HttpResponse:
         # Can omit data from context - we are not rendering the content.
         form = self.form_class(request=request, instance=self.instance)
```

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/wagtail_hooks/log_actions.py` & `wagtail_fedit-1.2.6/wagtail_fedit/wagtail_hooks/log_actions.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit/wagtail_hooks/userbar.py` & `wagtail_fedit-1.2.6/wagtail_fedit/wagtail_hooks/userbar.py`

 * *Files identical despite different names*

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit.egg-info/PKG-INFO` & `wagtail_fedit-1.2.6/wagtail_fedit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_fedit
-Version: 1.2.5
+Version: 1.2.6
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
-Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.5 Summary: An
+Metadata-Version: 2.1 Name: wagtail_fedit Version: 1.2.6 Summary: An
 application made for the Django Web Framework. Home-page: https://github.com/
 Nigel2392/wagtail_fedit Author: Nigel Author-email: nigel@goodadvice.it
 License: GPL-3.0-only Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.2 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
```

### Comparing `wagtail_fedit-1.2.5/wagtail_fedit.egg-info/SOURCES.txt` & `wagtail_fedit-1.2.6/wagtail_fedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

