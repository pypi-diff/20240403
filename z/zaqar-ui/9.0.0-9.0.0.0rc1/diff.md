# Comparing `tmp/zaqar-ui-9.0.0.tar.gz` & `tmp/zaqar-ui-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zaqar-ui-9.0.0.tar", last modified: Wed Oct 14 10:45:50 2020, max compression
+gzip compressed data, was "dist/zaqar-ui-9.0.0.0rc1.tar", last modified: Wed Sep 23 13:37:32 2020, max compression
```

## Comparing `zaqar-ui-9.0.0.tar` & `zaqar-ui-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1588 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/.eslintrc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8818 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/rocky.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7243 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5229 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6672 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6174 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7005 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/source/stein.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/notes/pool-flavor-panel-acf61d32e34246f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/notes/queens-ae86cb21aebaadfd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/notes/add-reno-73ba99b04ff2e5c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/notes/pool-panel-020bf94bc34b4cd8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1469 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/notes/pike-9c813ecd64a1e2f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/notes/init-action-fe41bfe3e2473364.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/releasenotes/notes/drop-py-2-7-d9e918f5c9f3bb33.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      830 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      631 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/babel-django.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/package.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1956 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5389 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/karma.conf.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/test/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/test/integration_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/test/integration_tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1303 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/test/settings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1483 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/test/helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/test/test_data.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/test/api_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/test/api_tests/test_rest_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/test/api_tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/test/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/tr_TR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/tr_TR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/tr_TR/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12621 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/tr_TR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/ko_KR/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11203 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/ko_KR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/ja/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13521 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/ja/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/zh_CN/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11270 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/zh_CN/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/ru/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9009 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/ru/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/pt_BR/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12662 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/en_GB/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12536 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/en_GB/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/id/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12361 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/id/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13623 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/locale/de/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/content/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/content/pool_flavors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/content/pool_flavors/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/content/pool_flavors/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/content/pool_flavors/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/content/queues/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/content/queues/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/content/queues/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      689 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/content/queues/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/content/pools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/content/pools/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/content/pools/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/content/pools/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/content/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6050 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/api/zaqar.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/api/rest/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12764 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/api/rest/zaqar.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1013 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/api/rest/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/enabled/_2520_admin_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/enabled/_1520_project_queues.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/enabled/_1510_project_messaging_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      879 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/enabled/_2530_admin_pool_flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      915 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/enabled/_2510_admin_messaging_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/enabled/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/app/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/app/core/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/app/core/openstack-service-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5978 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/app/core/openstack-service-api/zaqar.service.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2554 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/actions/create.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2861 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/actions/update.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4337 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/actions/delete.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/actions/actions.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3118 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/actions/workflow.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/pool-flavors.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/pool-flavors.scss
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/panel.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3081 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/pool-flavors.module.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2507 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/actions/create.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2878 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/actions/update.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4189 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/actions/delete.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2316 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/actions/actions.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3506 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/actions/workflow.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3394 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/pools.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1796 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/pools.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/panel.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/update-queue.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3862 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/delete-queue.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/list-message.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3006 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/list-message.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3970 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/purge-queue.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/list-message.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3714 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/post-message.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/post-message.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1758 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/create-subscription.workflow.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5989 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/signed-url.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/list-message.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3570 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/actions.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1558 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/update-queue.workflow.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2732 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/create-queue.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1842 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/create-queue.workflow.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3197 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/create-subscription.service.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/table/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4617 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/table/queue.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2822 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/table/subscription.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4053 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/table/queue.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/table/subscription.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/subscription/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1333 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/subscription/subscription.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2425 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/subscription/subscription.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/queue-details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1272 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/queue-details/queue-details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/queue-details/queue-details.controller.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/queue-metadata/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/queue-metadata/queue-metadata.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3366 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/queue-metadata/queue-metadata.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/queues.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2615 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/queues.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/queues.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/framework/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/framework/util/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui/static/framework/util/validators/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1666 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/static/framework/util/validators/validateSubscriber.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/zaqar_ui/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/babel-djangojs.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8943 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2247 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3135 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5920 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/tools/install_venv_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/tools/install_venv.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      506 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2636 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/test-shim.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2708 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/lower-constraints.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3508 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/AUTHORS
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1473 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/doc/source/contributor/api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10303 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2020-10-14 10:44:58.000000 zaqar-ui-9.0.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7125 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3508 2020-10-14 10:45:50.000000 zaqar-ui-9.0.0/zaqar_ui.egg-info/PKG-INFO
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/AUTHORS
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10303 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/doc/source/contributor/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1473 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/doc/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8818 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/unreleased.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7005 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6672 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5229 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7243 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6174 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/notes/init-action-fe41bfe3e2473364.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/notes/pool-panel-020bf94bc34b4cd8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/notes/pool-flavor-panel-acf61d32e34246f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1469 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/notes/pike-9c813ecd64a1e2f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/notes/queens-ae86cb21aebaadfd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/notes/add-reno-73ba99b04ff2e5c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/releasenotes/notes/drop-py-2-7-d9e918f5c9f3bb33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/package.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1588 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/.eslintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2708 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/lower-constraints.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3135 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8953 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/ChangeLog
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      830 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/LICENSE
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/framework/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/framework/util/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/framework/util/validators/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1666 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/framework/util/validators/validateSubscriber.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/pool-flavors.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3081 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/pool-flavors.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/panel.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/pool-flavors.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/actions/actions.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2554 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/actions/create.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4337 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/actions/delete.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2861 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/actions/update.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3118 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/actions/workflow.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/drawer.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/panel.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1796 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/pools.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3394 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/pools.module.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2316 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/actions/actions.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2507 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/actions/create.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4189 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/actions/delete.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2878 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/actions/update.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3506 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/actions/workflow.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/drawer.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/queues.module.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/table/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2822 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/table/subscription.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4053 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/table/queue.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4617 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/table/queue.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/table/subscription.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/queue-details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/queue-details/queue-details.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1272 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/queue-details/queue-details.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/queue-metadata/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/queue-metadata/queue-metadata.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3366 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/queue-metadata/queue-metadata.controller.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/subscription/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1333 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/subscription/subscription.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2425 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/subscription/subscription.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2615 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/queues.module.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/list-message.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5989 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/signed-url.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3006 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/list-message.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3570 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/actions.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1758 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/create-subscription.workflow.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1842 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/create-queue.workflow.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1558 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/update-queue.workflow.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3197 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/create-subscription.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/post-message.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2732 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/create-queue.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3714 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/post-message.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3862 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/delete-queue.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3970 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/purge-queue.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/update-queue.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/list-message.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/list-message.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/queues.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/app/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/app/core/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/app/core/openstack-service-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5978 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/static/app/core/openstack-service-api/zaqar.service.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/enabled/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/enabled/_1510_project_messaging_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      879 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/enabled/_2530_admin_pool_flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      915 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/enabled/_2510_admin_messaging_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      784 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/enabled/_2520_admin_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/enabled/_1520_project_queues.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5389 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/karma.conf.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/content/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/content/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/content/pool_flavors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/content/pool_flavors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/content/pool_flavors/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/content/pool_flavors/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/content/queues/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      689 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/content/queues/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/content/queues/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/content/queues/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/content/pools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/content/pools/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/content/pools/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/content/pools/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/api/rest/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1013 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/api/rest/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12764 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/api/rest/zaqar.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6050 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/api/zaqar.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9009 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ru/LC_MESSAGES/djangojs.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13623 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/de/LC_MESSAGES/djangojs.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11203 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ko_KR/LC_MESSAGES/djangojs.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ko_KR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12536 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/en_GB/LC_MESSAGES/djangojs.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/en_GB/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/tr_TR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/tr_TR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12621 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/tr_TR/LC_MESSAGES/djangojs.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/tr_TR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12662 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/pt_BR/LC_MESSAGES/djangojs.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11270 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/zh_CN/LC_MESSAGES/djangojs.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/zh_CN/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13521 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ja/LC_MESSAGES/djangojs.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12361 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/id/LC_MESSAGES/djangojs.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/test/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/test/test_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1303 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/test/settings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1483 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/test/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/test/api_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/test/api_tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/test/api_tests/test_rest_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/test/integration_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/test/integration_tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2636 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/test-shim.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/tools/install_venv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5920 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/tools/install_venv_common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      506 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/tools/with_venv.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1956 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/devstack/settings
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/babel-djangojs.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2247 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3513 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/PKG-INFO
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3513 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7125 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/zaqar_ui.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/babel-django.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2020-09-23 13:36:34.000000 zaqar-ui-9.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      631 2020-09-23 13:37:32.000000 zaqar-ui-9.0.0.0rc1/setup.cfg
```

### Comparing `zaqar-ui-9.0.0/.eslintrc` & `zaqar-ui-9.0.0.0rc1/.eslintrc`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/releasenotes/source/conf.py` & `zaqar-ui-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po` & `zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po` & `zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po` & `zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `zaqar-ui-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/releasenotes/notes/pike-9c813ecd64a1e2f2.yaml` & `zaqar-ui-9.0.0.0rc1/releasenotes/notes/pike-9c813ecd64a1e2f2.yaml`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/manage.py` & `zaqar-ui-9.0.0.0rc1/manage.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/requirements.txt` & `zaqar-ui-9.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/setup.cfg` & `zaqar-ui-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/package.json` & `zaqar-ui-9.0.0.0rc1/package.json`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/devstack/plugin.sh` & `zaqar-ui-9.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/version.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/version.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/karma.conf.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/karma.conf.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/test/settings.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/test/settings.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/test/helpers.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/test/helpers.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/test/test_data.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/test/test_data.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/test/api_tests/test_rest_api.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/test/api_tests/test_rest_api.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/tr_TR/LC_MESSAGES/django.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/tr_TR/LC_MESSAGES/djangojs.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/ko_KR/LC_MESSAGES/django.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/ko_KR/LC_MESSAGES/djangojs.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ko_KR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/ja/LC_MESSAGES/django.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/ja/LC_MESSAGES/djangojs.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ja/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/zh_CN/LC_MESSAGES/django.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/zh_CN/LC_MESSAGES/djangojs.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/zh_CN/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/ru/LC_MESSAGES/django.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/ru/LC_MESSAGES/djangojs.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/fr/LC_MESSAGES/django.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/pt_BR/LC_MESSAGES/django.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/pt_BR/LC_MESSAGES/djangojs.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/en_GB/LC_MESSAGES/django.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/en_GB/LC_MESSAGES/djangojs.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/en_GB/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/id/LC_MESSAGES/django.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/id/LC_MESSAGES/djangojs.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/id/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/de/LC_MESSAGES/django.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/locale/de/LC_MESSAGES/djangojs.po` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/content/pool_flavors/panel.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/content/pool_flavors/panel.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/content/pool_flavors/urls.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/content/pool_flavors/urls.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/content/queues/panel.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/content/queues/panel.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/content/queues/urls.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/content/queues/urls.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/content/queues/__init__.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/content/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/content/pools/panel.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/content/pools/panel.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/content/pools/urls.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/content/pools/urls.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/api/zaqar.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/api/zaqar.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/api/rest/zaqar.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/api/rest/zaqar.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/api/rest/__init__.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/api/__init__.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/api/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/enabled/_2520_admin_pools.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/enabled/_2520_admin_pools.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/enabled/_1520_project_queues.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/enabled/_1520_project_queues.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/enabled/_1510_project_messaging_group.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/enabled/_1510_project_messaging_group.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/enabled/_2530_admin_pool_flavors.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/enabled/_2530_admin_pool_flavors.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/enabled/_2510_admin_messaging_group.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/enabled/_2510_admin_messaging_group.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/app/core/openstack-service-api/zaqar.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/app/core/openstack-service-api/zaqar.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/actions/create.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/actions/create.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/actions/update.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/actions/update.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/actions/delete.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/actions/delete.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/actions/actions.module.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/actions/actions.module.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/actions/workflow.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/actions/workflow.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/pool-flavors.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/pool-flavors.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pool-flavors/pool-flavors.module.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pool-flavors/pool-flavors.module.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/actions/create.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/actions/create.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/actions/update.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/actions/update.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/actions/delete.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/actions/delete.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/actions/actions.module.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/actions/actions.module.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/actions/workflow.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/actions/workflow.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/pools.module.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/pools.module.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/admin/pools/pools.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/admin/pools/pools.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/update-queue.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/update-queue.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/delete-queue.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/delete-queue.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/list-message.controller.spec.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/list-message.controller.spec.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/list-message.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/list-message.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/purge-queue.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/purge-queue.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/list-message.controller.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/list-message.controller.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/post-message.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/post-message.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/post-message.help.html` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/post-message.help.html`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/create-subscription.workflow.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/create-subscription.workflow.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/signed-url.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/signed-url.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/list-message.html` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/list-message.html`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/actions.module.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/actions.module.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/update-queue.workflow.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/update-queue.workflow.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/create-queue.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/create-queue.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/create-queue.workflow.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/create-queue.workflow.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/actions/create-subscription.service.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/actions/create-subscription.service.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/table/queue.controller.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/table/queue.controller.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/table/subscription.controller.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/table/subscription.controller.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/table/queue.html` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/table/queue.html`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/table/subscription.html` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/table/subscription.html`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/subscription/subscription.controller.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/subscription/subscription.controller.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/subscription/subscription.html` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/subscription/subscription.html`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/queue-details/queue-details.html` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/queue-details/queue-details.html`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/queue-details/queue-details.controller.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/queue-details/queue-details.controller.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/steps/queue-metadata/queue-metadata.controller.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/steps/queue-metadata/queue-metadata.controller.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/queues.module.spec.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/queues.module.spec.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/dashboard/project/queues/queues.module.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/dashboard/project/queues/queues.module.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/static/framework/util/validators/validateSubscriber.js` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/static/framework/util/validators/validateSubscriber.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui/__init__.py` & `zaqar-ui-9.0.0.0rc1/zaqar_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/LICENSE` & `zaqar-ui-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/ChangeLog` & `zaqar-ui-9.0.0.0rc1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * [goal] Migrate testing to ubuntu focal
 * Fix npm jobs
 * Imported Translations from Zanata
 * Use unittest.mock instead of mock
 * Stop to use the \_\_future\_\_ module
 * Switch to newer openstackdocstheme and reno versions
```

### Comparing `zaqar-ui-9.0.0/README.rst` & `zaqar-ui-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/tox.ini` & `zaqar-ui-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/tools/install_venv_common.py` & `zaqar-ui-9.0.0.0rc1/tools/install_venv_common.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/tools/install_venv.py` & `zaqar-ui-9.0.0.0rc1/tools/install_venv.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/test-requirements.txt` & `zaqar-ui-9.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/test-shim.js` & `zaqar-ui-9.0.0.0rc1/test-shim.js`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/lower-constraints.txt` & `zaqar-ui-9.0.0.0rc1/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/PKG-INFO` & `zaqar-ui-9.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: zaqar-ui
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Zaqar User Interface
 Home-page: https://docs.openstack.org/zaqar/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `zaqar-ui-9.0.0/AUTHORS` & `zaqar-ui-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/doc/requirements.txt` & `zaqar-ui-9.0.0.0rc1/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/doc/source/install/index.rst` & `zaqar-ui-9.0.0.0rc1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/doc/source/conf.py` & `zaqar-ui-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/setup.py` & `zaqar-ui-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui.egg-info/SOURCES.txt` & `zaqar-ui-9.0.0.0rc1/zaqar_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zaqar-ui-9.0.0/zaqar_ui.egg-info/PKG-INFO` & `zaqar-ui-9.0.0.0rc1/zaqar_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: zaqar-ui
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Zaqar User Interface
 Home-page: https://docs.openstack.org/zaqar/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

