# Comparing `tmp/trove-dashboard-9.0.0.0rc1.tar.gz` & `tmp/trove-dashboard-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trove-dashboard-9.0.0.0rc1.tar", last modified: Fri Aug 11 13:14:26 2017, max compression
+gzip compressed data, was "dist/trove-dashboard-9.0.1.tar", last modified: Fri May 10 16:27:31 2019, max compression
```

## Comparing `trove-dashboard-9.0.0.0rc1.tar` & `trove-dashboard-9.0.1.tar`

### file list

```diff
@@ -1,294 +1,270 @@
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1508 2017-08-11 13:14:25.000000 trove-dashboard-9.0.0.0rc1/AUTHORS
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/babel-djangojs.cfg
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      152 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/ocata.rst
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/_static/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2978 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2698 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1604 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2998 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/ja/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1626 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3133 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1506 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/ru/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1293 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      107 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/unreleased.rst
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/_templates/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      198 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/index.rst
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9835 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/conf.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      154 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/source/newton.rst
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/releasenotes/notes/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/notes/.placeholder
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       68 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/notes/enable-cluster-mariabdb-cassandra-11f3f7f6badfc211.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      209 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/notes/fix-grow-cluster-cache-5625d1a519a4ee01.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       62 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/notes/enable-pxc-grow-shrink-17568a1c280f1c42.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      268 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/notes/conf-groups-7bc8115f8d0bcd14.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/notes/cluster-endpoints-52bbb9f1c146ae97.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      189 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/releasenotes/notes/logging-support-f999a1b1b342eb4d.yaml
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/devstack/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1630 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/devstack/plugin.sh
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       74 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/devstack/settings
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2057 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/tox.ini
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      569 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/test-requirements.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      432 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/requirements.txt
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)    16670 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/run_tests.sh
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/api/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       65 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/api/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13556 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/api/trove.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/api/rest/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      655 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/api/rest/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2735 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/api/rest/trove.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/__init__.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/id/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/id/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    38537 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/id/LC_MESSAGES/django.po
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1002 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/id/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/zh_CN/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    33543 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/zh_CN/LC_MESSAGES/django.po
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      893 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/zh_CN/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/fr/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    40902 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      932 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/fr/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/de/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/de/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    39474 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      947 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/de/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/cs/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    30483 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/cs/LC_MESSAGES/django.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/tr_TR/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/tr_TR/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    37764 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/tr_TR/LC_MESSAGES/django.po
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      974 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/tr_TR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ja/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    40294 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ja/LC_MESSAGES/django.po
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      983 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ja/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ko_KR/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    38889 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ko_KR/LC_MESSAGES/django.po
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ko_KR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/pt_BR/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    26656 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/en_GB/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      926 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/en_GB/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ru/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    48807 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ru/LC_MESSAGES/django.po
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1097 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ru/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/project/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/project/ngbackups/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1108 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/project/ngbackups/backups.module.js
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/project/ngbackups/backups.scss
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      825 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/project/ngbackups/backups.module.spec.js
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/project/ngbackups/table/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/project/ngbackups/table/table.controller.spec.js
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1466 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/project/ngbackups/table/table.controller.js
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1988 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/project/ngbackups/table/table.config.js
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/project/ngbackups/table/table.html
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/app/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/app/core/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/app/core/openstack-service-api/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1357 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/static/app/core/openstack-service-api/trove.service.js
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/enabled/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1578 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/enabled/_1731_project_database_backups_panel.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/enabled/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1188 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/enabled/_1760_project_database_configurations_panel.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1182 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/enabled/_1720_project_databases_panel.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      913 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/enabled/_1710_database_panel_group.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1239 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/enabled/_1740_project_database_clusters_panel.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1151 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/enabled/_1730_project_database_backups_panel.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      760 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/version.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/test/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/test/test_data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/test/test_data/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1951 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/test/test_data/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1030 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/test/test_data/keystone_data.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1220 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/test/test_data/exceptions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16377 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/test/test_data/trove_data.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1738 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/test/helpers.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/test/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      713 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/test/urls.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      979 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/test/settings.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      773 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/exceptions.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1044 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/panel.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3392 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/tabs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2587 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/cluster_manager.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1535 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/urls.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    20640 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/forms.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      348 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/cluster_grow_details.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      620 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_cassandra.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      121 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/add_instance.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      665 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_redis.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      848 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_mongodb.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      193 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_launch.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      886 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      505 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_add_instance.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/launch.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      272 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/cluster_shrink_details.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      620 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_mysql.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      278 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/index.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      204 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/reset_password.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      887 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_vertica.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      908 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_reset_password.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    30135 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/tests.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9842 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/views.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15576 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/tables.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      946 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/panel.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2500 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/tabs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1122 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/urls.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8019 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/forms.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6147 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/config_param_manager.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/templates/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/templates/database_configurations/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      213 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/templates/database_configurations/detail_param.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      204 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/templates/database_configurations/_add_parameter.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      192 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/templates/database_configurations/_create.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      797 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/templates/database_configurations/_detail_overview.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      145 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/templates/database_configurations/details.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      121 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/templates/database_configurations/create.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      129 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/templates/database_configurations/add_parameter.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/templates/database_configurations/index.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    22185 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/tests.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4621 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/views.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9291 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/tables.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      972 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/panel.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      932 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/urls.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/workflows/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4099 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/workflows/create_backup.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/workflows/__init__.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/templates/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/templates/database_backups/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      184 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/templates/database_backups/backup.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2456 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/templates/database_backups/details.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      158 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/templates/database_backups/index.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      357 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/templates/database_backups/_backup_details_help.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6710 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/tests.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4329 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/views.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6349 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/tables.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/__init__.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/panel.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6514 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/tabs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2213 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/urls.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/workflows/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/workflows/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    23818 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/workflows/create_instance.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11771 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/forms.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2167 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/db_capability.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      267 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_edit_user.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/resize_volume.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      323 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/manage_root.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/create_database.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      310 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_resize_volume.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      297 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_create_user.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      705 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_detail_overview_cassandra.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_promote_to_replica_source.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_launch_details_help.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      261 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_create_database.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      606 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_detail_overview_redis.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      746 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_launch_initialize_help.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      156 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/access_detail.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1066 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_detail_overview_mongodb.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      936 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_launch_networks.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      180 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_launch_advanced_help.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      627 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_detail_overview_couchbase.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      351 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_attach_config.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      114 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/attach_config.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      831 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_detail_overview_postgresql.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2771 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_detail_overview.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      184 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/launch.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      847 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_detail_overview_mysql.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      257 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_launch_network_help.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      117 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/resize_instance.html
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/logs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      375 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/logs/_log_contents.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/logs/log_contents.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      320 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/logs/view_log.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1200 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/logs/_detail_log.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      127 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/promote_to_replica_source.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      151 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/index.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      180 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_resize_instance.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      112 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/create_user.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/edit_user.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    51270 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/tests.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    19728 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/views.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/logs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/logs/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1036 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/logs/urls.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14835 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/logs/tests.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4548 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/logs/views.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4317 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/logs/tables.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    23796 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/tables.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/ng_database_backups/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      691 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/ng_database_backups/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      845 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/ng_database_backups/panel.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      748 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/ng_database_backups/urls.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/ng_database_backups/templates/
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/ng_database_backups/templates/ng_database_backups/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      302 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/ng_database_backups/templates/ng_database_backups/index.html
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      710 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard/content/ng_database_backups/views.py
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard.egg-info/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       46 2017-08-11 13:14:25.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard.egg-info/pbr.json
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2017-08-11 13:14:02.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard.egg-info/not-zip-safe
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11866 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4215 2017-08-11 13:14:25.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        1 2017-08-11 13:14:25.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      193 2017-08-11 13:14:25.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       16 2017-08-11 13:14:25.000000 trove-dashboard-9.0.0.0rc1/trove_dashboard.egg-info/top_level.txt
-drwxrwxr-x   0 jenkins   (1000) jenkins   (1000)        0 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/tools/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)     1533 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/tools/pip_install.sh
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1682 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/tools/clean_enabled_files.py
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)      218 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/tools/with_venv.sh
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5319 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/tools/install_venv.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      239 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/HACKING.rst
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/babel-django.cfg
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      623 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/CONTRIBUTING.rst
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)      831 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/manage.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4215 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6129 2017-08-11 13:14:25.000000 trove-dashboard-9.0.0.0rc1/ChangeLog
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2598 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/README.rst
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10143 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/LICENSE
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      864 2017-08-11 13:14:26.000000 trove-dashboard-9.0.0.0rc1/setup.cfg
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1028 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/setup.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       88 2017-08-11 13:11:58.000000 trove-dashboard-9.0.0.0rc1/MANIFEST.in
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       88 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/MANIFEST.in
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/devstack/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1630 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/devstack/plugin.sh
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       74 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/devstack/settings
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      239 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6485 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/ChangeLog
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)      831 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/manage.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      118 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/.zuul.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/zh_CN/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      892 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/locale/zh_CN/LC_MESSAGES/djangojs.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    33543 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/locale/zh_CN/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      932 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/locale/fr/LC_MESSAGES/djangojs.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    40902 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/en_GB/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      924 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/locale/en_GB/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      947 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/locale/de/LC_MESSAGES/djangojs.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    39354 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/pt_BR/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    38214 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      983 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/locale/ja/LC_MESSAGES/djangojs.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    40294 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/tr_TR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/tr_TR/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      974 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/locale/tr_TR/LC_MESSAGES/djangojs.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    37764 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/locale/tr_TR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/ko_KR/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      916 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/locale/ko_KR/LC_MESSAGES/djangojs.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    38889 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/locale/ko_KR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/cs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/cs/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30483 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/id/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1002 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/locale/id/LC_MESSAGES/djangojs.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    38537 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1097 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/locale/ru/LC_MESSAGES/djangojs.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    48807 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/locale/ru/LC_MESSAGES/django.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      773 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/test/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/test/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1181 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/test/settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/test/test_data/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/test/test_data/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1220 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/test/test_data/exceptions.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16377 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/test/test_data/trove_data.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1951 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/test/test_data/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1030 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/test/test_data/keystone_data.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1738 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/test/helpers.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      713 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/test/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/static/dashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/static/dashboard/project/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/static/dashboard/project/ngbackups/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/static/dashboard/project/ngbackups/table/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/static/dashboard/project/ngbackups/table/table.controller.spec.js
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1466 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/static/dashboard/project/ngbackups/table/table.controller.js
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      220 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/static/dashboard/project/ngbackups/table/table.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1988 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/static/dashboard/project/ngbackups/table/table.config.js
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1108 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/static/dashboard/project/ngbackups/backups.module.js
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/static/dashboard/project/ngbackups/backups.scss
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      825 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/static/dashboard/project/ngbackups/backups.module.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/static/app/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/static/app/core/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/static/app/core/openstack-service-api/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1357 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/static/app/core/openstack-service-api/trove.service.js
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      760 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/ng_database_backups/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      691 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/ng_database_backups/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      710 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/ng_database_backups/views.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      845 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/ng_database_backups/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/ng_database_backups/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/ng_database_backups/templates/ng_database_backups/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      302 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/ng_database_backups/templates/ng_database_backups/index.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      748 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/ng_database_backups/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4329 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/views.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      972 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/panel.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6710 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/tests.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6349 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/templates/database_backups/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      357 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/templates/database_backups/_backup_details_help.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      184 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/templates/database_backups/backup.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2456 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/templates/database_backups/details.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      158 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/templates/database_backups/index.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/workflows/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      102 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/workflows/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4099 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/workflows/create_backup.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      932 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_backups/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4621 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/views.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8019 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/forms.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      946 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/panel.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    22185 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/tests.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2500 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/tabs.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6147 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/config_param_manager.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9291 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/templates/database_configurations/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      204 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/templates/database_configurations/_add_parameter.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      121 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/templates/database_configurations/create.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      192 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/templates/database_configurations/_create.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      145 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/templates/database_configurations/details.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      129 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/templates/database_configurations/add_parameter.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       82 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/templates/database_configurations/index.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      797 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/templates/database_configurations/_detail_overview.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      213 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/templates/database_configurations/detail_param.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1122 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9842 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/views.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20640 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/forms.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1044 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/panel.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30135 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/tests.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3392 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/tabs.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15576 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      121 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/add_instance.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      348 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/cluster_grow_details.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      204 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/reset_password.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      908 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_reset_password.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      620 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_cassandra.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      665 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_redis.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      272 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/cluster_shrink_details.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      505 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_add_instance.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      848 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_mongodb.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      887 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_vertica.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      193 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_launch.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      118 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/launch.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      620 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_mysql.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      278 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/index.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      886 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2587 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/cluster_manager.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1535 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    19728 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/views.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11771 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/forms.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      917 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/panel.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2167 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/db_capability.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    51270 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/tests.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6514 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/tabs.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    23796 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      115 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/resize_volume.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      180 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_launch_advanced_help.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      110 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/edit_user.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      257 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_launch_network_help.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      156 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/access_detail.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      118 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/create_database.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      431 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_launch_details_help.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      705 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_detail_overview_cassandra.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      261 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_create_database.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      936 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_launch_networks.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      351 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_attach_config.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      606 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_detail_overview_redis.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      627 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_detail_overview_couchbase.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      117 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/resize_instance.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      267 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_edit_user.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      746 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_launch_initialize_help.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      127 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/promote_to_replica_source.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      297 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_create_user.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      831 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_detail_overview_postgresql.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1066 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_detail_overview_mongodb.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1431 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_promote_to_replica_source.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      114 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/attach_config.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      323 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/manage_root.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      310 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_resize_volume.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      184 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/launch.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/logs/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1200 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/logs/_detail_log.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      320 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/logs/view_log.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      375 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/logs/_log_contents.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      258 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/logs/log_contents.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      847 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_detail_overview_mysql.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      151 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/index.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2771 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_detail_overview.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      180 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_resize_instance.html
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      112 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/create_user.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/logs/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/logs/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4548 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/logs/views.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14835 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/logs/tests.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4317 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/logs/tables.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1036 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/logs/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/workflows/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      106 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/workflows/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    23818 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/workflows/create_instance.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2213 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/content/databases/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/enabled/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1151 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/enabled/_1730_project_database_backups_panel.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1239 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/enabled/_1740_project_database_clusters_panel.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/enabled/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1182 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/enabled/_1720_project_databases_panel.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      913 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/enabled/_1710_database_panel_group.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1578 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/enabled/_1731_project_database_backups_panel.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1188 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/enabled/_1760_project_database_configurations_panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/api/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard/api/rest/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      655 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/api/rest/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2735 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/api/rest/trove.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       65 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/trove_dashboard/api/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13556 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/trove_dashboard/api/trove.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4264 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/PKG-INFO
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      569 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/test-requirements.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2085 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/tox.ini
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      577 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/babel-djangojs.cfg
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10143 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/LICENSE
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      864 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/setup.cfg
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1028 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/releasenotes/notes/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       62 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/releasenotes/notes/enable-pxc-grow-shrink-17568a1c280f1c42.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      268 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/releasenotes/notes/conf-groups-7bc8115f8d0bcd14.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       68 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/releasenotes/notes/enable-cluster-mariabdb-cassandra-11f3f7f6badfc211.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       91 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/releasenotes/notes/cluster-endpoints-52bbb9f1c146ae97.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      209 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/releasenotes/notes/fix-grow-cluster-cache-5625d1a519a4ee01.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/releasenotes/notes/.placeholder
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      189 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/releasenotes/notes/logging-support-f999a1b1b342eb4d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/releasenotes/source/_static/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/releasenotes/source/_templates/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/releasenotes/source/_templates/.placeholder
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9835 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/releasenotes/source/conf.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      198 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/releasenotes/source/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      152 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/releasenotes/source/ocata.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      107 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/releasenotes/source/unreleased.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      154 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/releasenotes/source/newton.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      623 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1612 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/AUTHORS
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/tools/
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1535 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/tools/pip_install.sh
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5319 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/tools/install_venv.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)      218 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/tools/with_venv.sh
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1682 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/tools/clean_enabled_files.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)    16670 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/run_tests.sh
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2652 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4264 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11404 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-05-10 16:27:31.000000 trove-dashboard-9.0.1/trove_dashboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      106 2019-05-10 16:25:39.000000 trove-dashboard-9.0.1/babel-django.cfg
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      432 2019-05-10 16:25:42.000000 trove-dashboard-9.0.1/requirements.txt
```

### Comparing `trove-dashboard-9.0.0.0rc1/AUTHORS` & `trove-dashboard-9.0.1/AUTHORS`

 * *Files 9% similar despite different names*

```diff
@@ -10,30 +10,33 @@
 David Lyle <david.lyle@intel.com>
 Devin Carlen <devin.carlen@gmail.com>
 Doug Hellmann <doug@doughellmann.com>
 Duk Loi <duk@tesora.com>
 Flavio Percoco <flaper87@gmail.com>
 Gene Kuo <igene@igene.tw>
 He Yongli <yongli.he@intel.com>
+Ian Wienand <iwienand@redhat.com>
 Ishita Mandhan <imandha@us.ibm.com>
 Masaki Matsushita <glass.saga@gmail.com>
 Masco Kaliyamoorthy <masco.kaliyamoorthy@enovance.com>
 Matt Van Dijk <mvandijk@tesora.com>
 Matthias Runge <mrunge@redhat.com>
 Michael Yu <michayu@ebaysf.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Peter Stachowski <peter@tesora.com>
 Rob Cresswell <robert.cresswell@outlook.com>
 Robert Myers <robert.myers@rackspace.com>
+Samuel Matzek <smatzek@us.ibm.com>
 Steve Leon <steve.leon@hp.com>
 Sushil Kumar <skm.net@gmail.com>
 Swapnil Kulkarni (coolsvap) <me@coolsvap.net>
 Thomas Goirand <zigo@debian.org>
 Tom Fifield <tom@openstack.org>
 Victor Stinner <vstinner@redhat.com>
+Zhao Chao <zhaochao1984@gmail.com>
 howardlee <lihongweibj@inspur.com>
 jiansong <jian.song@easystack.cn>
 lin-hua-cheng <lin-hua.cheng@hp.com>
 lin-hua-cheng <os.lcheng@gmail.com>
 liyingjun <yingjun.li@kylin-cloud.com>
 qiaomin <chen.qiaomin@99cloud.net>
 sharat.sharma <sharat.sharma@nectechnologies.in>
```

### Comparing `trove-dashboard-9.0.0.0rc1/babel-djangojs.cfg` & `trove-dashboard-9.0.1/babel-djangojs.cfg`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/releasenotes/source/conf.py` & `trove-dashboard-9.0.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/devstack/plugin.sh` & `trove-dashboard-9.0.1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/tox.ini` & `trove-dashboard-9.0.1/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 minversion = 1.6
 envlist = py27,pep8,py27dj18
 skipsdist = True
 
 [testenv]
 usedevelop = True
 install_command = {toxinidir}/tools/pip_install.sh \
-                -c{env:UPPER_CONSTRAINTS_FILE:https://git.openstack.org/cgit/openstack/requirements/plain/upper-constraints.txt} \
+                -c{env:UPPER_CONSTRAINTS_FILE:https://git.openstack.org/cgit/openstack/requirements/plain/upper-constraints.txt?h=stable/pike} \
                  {opts} {packages}
 setenv =
    VIRTUAL_ENV={envdir}
 deps = -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 commands = /bin/bash run_tests.sh -N --no-pep8 {posargs}
 
@@ -19,15 +19,15 @@
 
 [testenv:pep8]
 commands = flake8
 
 [testenv:venv]
 # This target does not use script since we do not need to install horizon.
 install_command = pip install \
-                -c{env:UPPER_CONSTRAINTS_FILE:https://git.openstack.org/cgit/openstack/requirements/plain/upper-constraints.txt} \
+                -c{env:UPPER_CONSTRAINTS_FILE:https://git.openstack.org/cgit/openstack/requirements/plain/upper-constraints.txt?h=stable/pike} \
                 -U --force-reinstall {opts} {packages}
 commands = {posargs}
 
 # Django-1.8 is LTS
 [testenv:py27dj18]
 basepython = python2.7
 commands = pip install django>=1.8,<1.9
```

### Comparing `trove-dashboard-9.0.0.0rc1/test-requirements.txt` & `trove-dashboard-9.0.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/run_tests.sh` & `trove-dashboard-9.0.1/run_tests.sh`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/api/trove.py` & `trove-dashboard-9.0.1/trove_dashboard/api/trove.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/api/rest/__init__.py` & `trove-dashboard-9.0.1/trove_dashboard/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/api/rest/trove.py` & `trove-dashboard-9.0.1/trove_dashboard/api/rest/trove.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/id/LC_MESSAGES/django.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/id/LC_MESSAGES/djangojs.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/id/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/zh_CN/LC_MESSAGES/django.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # BillXiang <1138647106@qq.com>, 2016. #zanata
 # Yu Long <yulongxn@163.com>, 2016. #zanata
 # sunanchen <KF.sunanchen@h3c.com>, 2016. #zanata
 # Bin <liubin@glab.cn>, 2017. #zanata
 # Gaoxiao Zhu <zhu.gaoxiao@h3c.com>, 2017. #zanata
 msgid ""
 msgstr ""
-"Project-Id-Version: trove-dashboard 9.0.0.0b3.dev4\n"
+"Project-Id-Version: trove-dashboard 9.0.0.0b4.dev1\n"
 "Report-Msgid-Bugs-To: https://bugs.launchpad.net/openstack-i18n/\n"
-"POT-Creation-Date: 2017-06-19 12:58+0000\n"
+"POT-Creation-Date: 2017-08-07 12:42+0000\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "PO-Revision-Date: 2017-07-24 03:51+0000\n"
 "Last-Translator: Bin <liubin@glab.cn>\n"
 "Language-Team: Chinese (China)\n"
-"Language: zh-CN\n"
-"X-Generator: Zanata 3.9.6\n"
+"Language: zh_CN\n"
+"X-Generator: Zanata 4.3.3\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 
 #, python-format
 msgid "%(name)s | %(RAM)s RAM"
 msgstr "%(name)s | %(RAM)s RAM"
 
 #, python-format
```

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/zh_CN/LC_MESSAGES/djangojs.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/zh_CN/LC_MESSAGES/djangojs.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # zzxwill <zzxwill@gmail.com>, 2016. #zanata
 msgid ""
 msgstr ""
-"Project-Id-Version: trove-dashboard 7.0.0.0b3.dev13\n"
+"Project-Id-Version: trove-dashboard 9.0.0.0b4.dev1\n"
 "Report-Msgid-Bugs-To: https://bugs.launchpad.net/openstack-i18n/\n"
-"POT-Creation-Date: 2016-08-24 16:43+0000\n"
+"POT-Creation-Date: 2017-08-07 12:42+0000\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "PO-Revision-Date: 2016-08-25 10:46+0000\n"
 "Last-Translator: zzxwill <zzxwill@gmail.com>\n"
 "Language-Team: Chinese (China)\n"
-"Language: zh-CN\n"
-"X-Generator: Zanata 3.7.3\n"
+"Language: zh_CN\n"
+"X-Generator: Zanata 4.3.3\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 
 msgid "Created"
 msgstr "已创建"
 
 msgid "Database"
 msgstr "数据库"
```

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/fr/LC_MESSAGES/django.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/fr/LC_MESSAGES/djangojs.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/de/LC_MESSAGES/django.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/de/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-# Andreas Jaeger <jaegerandi@gmail.com>, 2016. #zanata
 # Frank Kloeker <eumel@arcor.de>, 2016. #zanata
-# Robert Simai <robert.simai@suse.com>, 2016. #zanata
-# Robert Simai <robert.simai@suse.com>, 2017. #zanata
+# Frank Kloeker <eumel@arcor.de>, 2017. #zanata
 msgid ""
 msgstr ""
-"Project-Id-Version: trove-dashboard 9.0.0.0b3.dev4\n"
+"Project-Id-Version: trove-dashboard 9.0.0.0b4.dev1\n"
 "Report-Msgid-Bugs-To: https://bugs.launchpad.net/openstack-i18n/\n"
-"POT-Creation-Date: 2017-06-19 12:58+0000\n"
+"POT-Creation-Date: 2017-08-07 12:42+0000\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"PO-Revision-Date: 2017-06-01 04:35+0000\n"
-"Last-Translator: Robert Simai <robert.simai@suse.com>\n"
+"PO-Revision-Date: 2017-08-20 10:22+0000\n"
+"Last-Translator: Frank Kloeker <eumel@arcor.de>\n"
 "Language-Team: German\n"
 "Language: de\n"
 "X-Generator: Zanata 3.9.6\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 
 #, python-format
 msgid "%(name)s | %(RAM)s RAM"
@@ -846,15 +844,15 @@
 
 msgid "Password for root user."
 msgstr "Passwort des Root-Benutzers."
 
 msgid ""
 "Password is only visible immediately after the root is enabled or reset."
 msgstr ""
-"Passwort ist nur sichtbar, nachdem root aktiviert oder zurückgesetzt ist."
+"Passwort ist nur sichtbar, nachdem Root aktiviert oder zurückgesetzt ist."
 
 msgid ""
 "Please note:</strong> The new value must be greater than the existing volume "
 "size."
 msgstr ""
 "Bitte beachten:</strong> Der neue Wert muss grösser sein als die "
 "existierende Datenträgergrösse."
@@ -1145,15 +1143,15 @@
 msgstr "Spezifiziere die Nummer der zu erstellenden Replikas"
 
 msgid ""
 "Specify whether future replicated instances will be created on the same "
 "hypervisor (affinity) or on different hypervisors (anti-affinity). This "
 "value is ignored if the instance to be launched is a replica."
 msgstr ""
-"Spezifiere ob zukünftig replizierte Instanzen auf demselben Hypervisor "
+"Spezifiere, ob zukünftig replizierte Instanzen auf demselben Hypervisor "
 "erstellt werden (Affinität) oder auf verschiedenen (Anti-Affinität). Wert "
 "wird ignoriert, wenn die erstellte Instanz eine Replika ist."
 
 msgid ""
 "Specify whether instances in the cluster will be created on the same "
 "hypervisor (affinity) or on different hypervisors (anti-affinity)."
 msgstr ""
@@ -1310,15 +1308,15 @@
 msgid "Unable to obtain datastores."
 msgstr "Beziehen des Datastore nicht möglich."
 
 msgid "Unable to obtain flavors."
 msgstr "Die Varianten können nicht abgerufen werden."
 
 msgid "Unable to obtain information on root user"
-msgstr "Konnte keine Informationen über den Benutzer root erhalten"
+msgstr "Konnte keine Informationen über den Benutzer Root erhalten"
 
 msgid "Unable to obtain list of parameters."
 msgstr "Die Liste der Parameter können nicht abgerufen werden."
 
 #, python-format
 msgid "Unable to promote replica as the new replica source.  \"%s\""
 msgstr "Konnte neue Replicaquelle nicht anbieten. \"%s\""
```

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/de/LC_MESSAGES/djangojs.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/cs/LC_MESSAGES/django.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/tr_TR/LC_MESSAGES/django.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # işbaran akçayır <isbaran@gmail.com>, 2017. #zanata
 msgid ""
 msgstr ""
-"Project-Id-Version: trove-dashboard 9.0.0.0b3.dev4\n"
+"Project-Id-Version: trove-dashboard 9.0.0.0b4.dev1\n"
 "Report-Msgid-Bugs-To: https://bugs.launchpad.net/openstack-i18n/\n"
-"POT-Creation-Date: 2017-06-19 12:58+0000\n"
+"POT-Creation-Date: 2017-08-07 12:42+0000\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "PO-Revision-Date: 2017-05-25 09:22+0000\n"
 "Last-Translator: Copied by Zanata <copied-by-zanata@zanata.org>\n"
 "Language-Team: Turkish (Turkey)\n"
-"Language: tr-TR\n"
+"Language: tr_TR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"X-Generator: Zanata 3.9.6\n"
+"X-Generator: Zanata 4.3.3\n"
 "X-POOTLE-MTIME: 1495704069.000000\n"
 
 #, python-format
 msgid "%(name)s | %(RAM)s RAM"
 msgstr "%(name)s | %(RAM)s RAM"
 
 #, python-format
```

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/tr_TR/LC_MESSAGES/djangojs.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # işbaran akçayır <isbaran@gmail.com>, 2017. #zanata
 msgid ""
 msgstr ""
-"Project-Id-Version: trove-dashboard 9.0.0.0b2.dev2\n"
+"Project-Id-Version: trove-dashboard 9.0.0.0b4.dev1\n"
 "Report-Msgid-Bugs-To: https://bugs.launchpad.net/openstack-i18n/\n"
-"POT-Creation-Date: 2017-05-12 11:33+0000\n"
+"POT-Creation-Date: 2017-08-07 12:42+0000\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "PO-Revision-Date: 2017-05-24 02:16+0000\n"
 "Last-Translator: Copied by Zanata <copied-by-zanata@zanata.org>\n"
 "Language-Team: Turkish (Turkey)\n"
-"Language: tr-TR\n"
+"Language: tr_TR\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"X-Generator: Zanata 3.9.6\n"
+"X-Generator: Zanata 4.3.3\n"
 "X-POOTLE-MTIME: 1495635326.000000\n"
 
 msgid "Created"
 msgstr "Oluşturuldu"
 
 msgid "Database"
 msgstr "Veri tabanı"
```

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ja/LC_MESSAGES/django.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ja/LC_MESSAGES/djangojs.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/ja/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ko_KR/LC_MESSAGES/django.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Andreas Jaeger <jaegerandi@gmail.com>, 2016. #zanata
 # Ian Y. Choi <ianyrchoi@gmail.com>, 2016. #zanata
 # Ian Y. Choi <ianyrchoi@gmail.com>, 2017. #zanata
 # Sungjin Kang <gang.sungjin@gmail.com>, 2017. #zanata
 msgid ""
 msgstr ""
-"Project-Id-Version: trove-dashboard 9.0.0.0b3.dev5\n"
+"Project-Id-Version: trove-dashboard 9.0.0.0b4.dev1\n"
 "Report-Msgid-Bugs-To: https://bugs.launchpad.net/openstack-i18n/\n"
-"POT-Creation-Date: 2017-07-28 02:11+0000\n"
+"POT-Creation-Date: 2017-08-07 12:42+0000\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "PO-Revision-Date: 2017-08-03 05:00+0000\n"
 "Last-Translator: Sungjin Kang <gang.sungjin@gmail.com>\n"
 "Language-Team: Korean (South Korea)\n"
-"Language: ko-KR\n"
-"X-Generator: Zanata 3.9.6\n"
+"Language: ko_KR\n"
+"X-Generator: Zanata 4.3.3\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 
 #, python-format
 msgid "%(name)s | %(RAM)s RAM"
 msgstr "%(name)s | %(RAM)s RAM"
 
 #, python-format
```

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ko_KR/LC_MESSAGES/djangojs.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/ko_KR/LC_MESSAGES/djangojs.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Ian Y. Choi <ianyrchoi@gmail.com>, 2016. #zanata
 msgid ""
 msgstr ""
-"Project-Id-Version: trove-dashboard 7.0.0.0b4.dev15\n"
+"Project-Id-Version: trove-dashboard 9.0.0.0b4.dev1\n"
 "Report-Msgid-Bugs-To: https://bugs.launchpad.net/openstack-i18n/\n"
-"POT-Creation-Date: 2016-09-13 18:48+0000\n"
+"POT-Creation-Date: 2017-08-07 12:42+0000\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "PO-Revision-Date: 2016-09-14 05:49+0000\n"
 "Last-Translator: \n"
 "Language-Team: Korean (South Korea)\n"
-"Language: ko-KR\n"
-"X-Generator: Zanata 3.7.3\n"
+"Language: ko_KR\n"
+"X-Generator: Zanata 4.3.3\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 
 msgid "Created"
 msgstr "생성됨"
 
 msgid "Database"
 msgstr "데이터베이스"
```

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/pt_BR/LC_MESSAGES/django.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 # Andreas Jaeger <jaegerandi@gmail.com>, 2016. #zanata
+# Fernando Pimenta <fernando.c.pimenta@gmail.com>, 2017. #zanata
 msgid ""
 msgstr ""
-"Project-Id-Version: trove-dashboard 9.0.0.0b3.dev4\n"
+"Project-Id-Version: trove-dashboard 9.0.0.0b4.dev1\n"
 "Report-Msgid-Bugs-To: https://bugs.launchpad.net/openstack-i18n/\n"
-"POT-Creation-Date: 2017-06-19 12:58+0000\n"
+"POT-Creation-Date: 2017-08-07 12:42+0000\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"PO-Revision-Date: 2016-04-12 06:49+0000\n"
-"Last-Translator: Copied by Zanata <copied-by-zanata@zanata.org>\n"
+"PO-Revision-Date: 2017-09-04 07:24+0000\n"
+"Last-Translator: Fernando Pimenta <fernando.c.pimenta@gmail.com>\n"
 "Language-Team: Portuguese (Brazil)\n"
-"Language: pt-BR\n"
-"X-Generator: Zanata 3.9.6\n"
+"Language: pt_BR\n"
+"X-Generator: Zanata 4.3.3\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 
 #, python-format
 msgid "%(name)s | %(RAM)s RAM"
 msgstr "%(name)s | %(RAM)s RAM"
 
 #, python-format
 msgid "%(name)s | %(RAM)s RAM | %(instances)s instances"
 msgstr "%(name)s | %(RAM)s RAM | %(instances)s instâncias"
 
 msgid "-"
 msgstr "-"
 
 msgid ""
+"<strong>Please note:</strong> It may be necessary to reboot the database "
+"instance for this new configuration group to take effect."
+msgstr ""
+"<strong>Por favor, observe:</strong> Pode ser necessário reinicializar a "
+"instância de banco de dados para que esse novo grupo de configuração tenha "
+"efeito."
+
+msgid ""
 "<strong>Please note:</strong> The value specified in the Volume Size field "
 "should be greater than 0, however, some configurations do not support "
 "specifying volume size. If specifying the volume size results in an error "
 "stating volume support is not enabled, enter 0."
 msgstr ""
 "<strong>Por favor observe:</strong> O valor especificado no campo Tamanho do "
 "Volume deve ser maior que 0, entretanto, algumas configurações não suportam "
@@ -59,29 +68,66 @@
 
 msgid "Add"
 msgstr "Adicionar"
 
 msgid "Add Instance"
 msgstr "Adicionar Instância"
 
+msgid "Add Parameter"
+msgstr "Adicionar Parâmetro"
+
+msgid ""
+"Add parameters to the configuration group.  When all the parameters are "
+"added click 'Apply Changes' to persist changes."
+msgstr ""
+"Adicionar parâmetros ao grupo de configuração. Quando todos os parâmetros "
+"forem adicionados clique em 'Aplicar Mudanças' para que as alterações "
+"persistam."
+
 msgid "Advanced"
 msgstr "Avançado"
 
+msgid ""
+"Allow the user to connect from this host only. If not provided this user "
+"will be allowed to connect from anywhere."
+msgstr ""
+"Permite o usuário conectar somente a partir desse host. Se não for fornecido "
+"esse usuário terá permissão de conectar de qualquer lugar."
+
 msgid "Allowed Host"
 msgstr "Host Permitido"
 
 msgid "Allowed Host (optional)"
 msgstr "Host Permitido (opcional)"
 
+msgid "Any Availability Zone"
+msgstr "Qualquer Zona de Disponibilidade"
+
 msgid "Applicable only if the volume size is specified."
 msgstr "Aplicável apenas se o tamanho do volume é especificado."
 
+msgid "Applied changes to server"
+msgstr "Alterações aplicadas no servidor"
+
+msgid "Apply Changes"
+msgstr "Aplicar Alterações"
+
 msgid "At least one of the new fields must be changed."
 msgstr "Pelo menos um dos novos campos deve ser alterado."
 
+msgid "Attach Configuration Group"
+msgstr "Anexar Grupo de Configuração"
+
+#, python-format
+msgid "Attaching Configuration group \"%s\""
+msgstr "Anexando Grupo de Configuração \"%s\""
+
+msgid "Availability Zone"
+msgstr "Zona de Disponibilidade"
+
 msgid "Available networks"
 msgstr "Redes disponíveis"
 
 msgid "Backup"
 msgstr "Backup"
 
 msgctxt "Current status of a Database Instance"
@@ -119,29 +165,40 @@
 msgid "Blocked"
 msgstr "Bloqueado"
 
 msgctxt "Current status of a Database Backup"
 msgid "Building"
 msgstr "Construindo"
 
+msgctxt "Current status of a Database Instance"
+msgid "Building"
+msgstr "Construindo"
+
 msgid "Cancel"
 msgstr "Cancelar"
 
+#, python-format
+msgid "Cannot disable root access: %s"
+msgstr "Não é possível desabilitar acesso de root: %s"
+
 msgid "Cannot grow cluster.  No instances specified."
 msgstr "Não é possível aumentar Cluster. Nenhuma instância especificada."
 
 msgid "Character Set"
 msgstr "Codificação de Caracteres"
 
 msgid "Choose a new instance flavor."
 msgstr "Escolha um novo Flavor para a instância."
 
 msgid "Choose initial state."
 msgstr "Escolha o estado inicial"
 
+msgid "Close"
+msgstr "Fechar"
+
 msgid "Cluster Name"
 msgstr "Nome do Cluster"
 
 msgid "Cluster Size"
 msgstr "Tamanho do Cluster"
 
 msgid "Clusters"
@@ -153,40 +210,92 @@
 msgid "Comma separated list of databases to create"
 msgstr "Lista separada por vírgula de bases de dados a se criar."
 
 msgctxt "Current status of a Database Backup"
 msgid "Completed"
 msgstr "Completo"
 
+msgid "Configuration Defaults"
+msgstr "Padrões de Configuração"
+
+msgid "Configuration Group"
+msgstr "Grupo de Configuração"
+
+msgid "Configuration Group Details: {{configuration.name}}"
+msgstr "Detalhes do Grupo de Configuração: {{configuration.name}}"
+
+msgid "Configuration Group Instances"
+msgstr "Instâncias do Grupo de Configuração"
+
+msgid "Configuration Group Name"
+msgstr "Nome do Grupo de Configuração"
+
+msgid "Configuration Group Overview"
+msgstr "Visão Geral do Grupo de Configuração"
+
+msgid "Configuration Group Values"
+msgstr "Valores do Grupo de Configuração"
+
+msgid "Configuration Groups"
+msgstr "Grupos de Configuração"
+
+msgid ""
+"Confirm the current replica is to be promoted as the new replica source."
+msgstr ""
+"Confirmar que a réplica atual é para ser promovida como nova fonte de "
+"réplica."
+
 msgid "Connection Examples"
 msgstr "Exemplos de Conexão"
 
 msgid "Connection Information"
 msgstr "Informação de Conexão"
 
+msgid "Container"
+msgstr "Contêiner"
+
 msgid "Create Backup"
 msgstr "Criar Backup"
 
+msgid "Create Configuration Group"
+msgstr "Criar Grupo de Configuração"
+
 msgid "Create Database"
 msgstr "Criar Banco de Dados"
 
 msgid "Create User"
 msgstr "Criar Usuário"
 
+msgid ""
+"Create an optional initial user. This user will have access to all databases "
+"you create."
+msgstr ""
+"Criar um usuário inicial opcional. Esse usuário terá acesso a todos os "
+"bancos de dados que você criar."
+
 msgid "Created"
 msgstr "Criado"
 
+msgid "Created configuration group"
+msgstr "Criado grupo de configuração"
+
 #, python-format
 msgid "Created database \"%s\"."
 msgstr "Criada base de dados \"%s\"."
 
 #, python-format
 msgid "Created user \"%s\"."
 msgstr "Criado usuário \"%s\"."
 
+msgid "Current Replica"
+msgstr "Réplica atual."
+
+msgid "Current Replica Source"
+msgstr "Fonte de Réplica Atual"
+
 msgid "Current Size (GB)"
 msgstr "Tamanho Atual (GB)"
 
 msgid "Current Task"
 msgstr "Tarefa Atual"
 
 msgid "DATABASE"
@@ -221,114 +330,213 @@
 
 msgid "Datastore"
 msgstr "Datastore"
 
 msgid "Datastore Version"
 msgstr "Versão Datastore"
 
+msgid "Defaults"
+msgstr "Padrões"
+
 msgid "Delete Backup"
 msgid_plural "Delete Backups"
 msgstr[0] "Excluir Backup"
 msgstr[1] "Excluir Backups"
 
 msgid "Delete Cluster"
 msgid_plural "Delete Clusters"
 msgstr[0] "Excluir Cluster"
 msgstr[1] "Excluir Clusters"
 
+msgid "Delete Configuration Group"
+msgid_plural "Delete Configuration Groups"
+msgstr[0] "Excluir Grupo de Configuração"
+msgstr[1] "Excluir Grupos de Configuração"
+
 msgid "Delete Database"
 msgid_plural "Delete Databases"
 msgstr[0] "Excluir Banco de Dados"
 msgstr[1] "Excluir Bancos de Dados"
 
 msgctxt "Current status of a Database Backup"
 msgid "Delete Failed"
 msgstr "Falha na Exclusão."
 
 msgid "Delete Instance"
 msgid_plural "Delete Instances"
 msgstr[0] "Excluir Instância"
 msgstr[1] "Excluir Instâncias"
 
+msgid "Delete Parameter"
+msgid_plural "Delete Parameters"
+msgstr[0] "Excluir Parâmetro"
+msgstr[1] "Excluir Parâmetros"
+
 msgid "Delete User"
 msgid_plural "Delete Users"
 msgstr[0] "Excluir Usuário"
 msgstr[1] "Excluir Usuários"
 
 msgid "Deleted Backup"
 msgid_plural "Deleted Backups"
 msgstr[0] "Backup Excluído"
 msgstr[1] "Backups Excluídos"
 
+msgid "Deleted Configuration Group"
+msgid_plural "Deleted Configuration Groups"
+msgstr[0] "Excluir Grupo de Configuração"
+msgstr[1] "Excluir Grupos de Configuração"
+
 msgid "Deleted Database"
 msgid_plural "Deleted Databases"
 msgstr[0] "Banco de Dados Excluídos"
 msgstr[1] "Bancos de Dados Excluídos"
 
+msgid "Deleted Parameter"
+msgid_plural "Deleted Parameters"
+msgstr[0] "Parâmetros Excluídos"
+msgstr[1] "Parâmetros Excluídos"
+
 msgid "Deleted User"
 msgid_plural "Deleted Users"
 msgstr[0] "Usuário Excluído"
 msgstr[1] "Usuários Excluídos"
 
 msgid "Deleted cluster is not recoverable."
 msgstr "Cluster excluído não é recuperável."
 
 msgid "Deleted instances are not recoverable."
 msgstr "Instâncias excluídas não são recuperáveis."
 
 msgid "Description"
 msgstr "Descrição"
 
+msgid "Detach Configuration Group"
+msgid_plural "Detach Configuration Groups"
+msgstr[0] "Desconectar Grupo de Configuração"
+msgstr[1] "Desconetar Grupos de Configuração"
+
 msgid "Detach Replica"
 msgid_plural "Detach Replicas"
 msgstr[0] "Desanexar Réplica"
 msgstr[1] "Desanexar Réplicas"
 
+msgid "Detached Configuration Group"
+msgid_plural "Detached Configuration Groups"
+msgstr[0] "Grupo de Configuração Desconectado"
+msgstr[1] "Grupos de Configuração Desconectados"
+
 msgid "Details"
 msgstr "Detalhes"
 
+msgid "Disable Log"
+msgid_plural "Disable Logs"
+msgstr[0] "Desabilitar Log"
+msgstr[1] "Desabilitar Logs"
+
+msgid "Disable Root"
+msgstr "Desabilitar Root"
+
+msgid "Disabled Log"
+msgid_plural "Disabled Logs"
+msgstr[0] "Log Desabilitado"
+msgstr[1] "Logs Desabilitados"
+
+msgid "Discard Changes"
+msgstr "Descartar Alterações"
+
+msgid "Discard Log"
+msgid_plural "Discard Logs"
+msgstr[0] "Descartar Log"
+msgstr[1] "Descartar Logs"
+
+msgid "Discarded Log"
+msgid_plural "Discarded Logs"
+msgstr[0] "Log Descartado"
+msgstr[1] "Logs Descartados"
+
 msgid "Download"
 msgstr "Baixar"
 
 msgid "Download Backup"
 msgstr "Download do Backup"
 
 msgid "Edit User"
 msgstr "Editar Usuário"
 
+msgid "Eject Replica Source"
+msgid_plural "Eject Replica Sources"
+msgstr[0] "Ejetar Origem de Réplica"
+msgstr[1] "Ejetar Origens de Réplicas"
+
+msgid "Ejected Replica Source"
+msgid_plural "Ejected Replica Sources"
+msgstr[0] "Origem de Réplica Ejetada"
+msgstr[1] "Origens de Réplicas Ejetadas"
+
+msgid "Enable Log"
+msgid_plural "Enable Logs"
+msgstr[0] "Habilitar Log"
+msgstr[1] "Habilitar Logs"
+
 msgid "Enable Root"
 msgstr "Habilitar Raiz"
 
+msgid "Enabled Log"
+msgid_plural "Enabled Logs"
+msgstr[0] "Log Habilitado"
+msgstr[1] "Logs Habilitados"
+
 msgctxt "Current status of a Database Instance"
 msgid "Error"
 msgstr "Erro"
 
+msgid "Error applying changes"
+msgstr "Erro ao aplicar as alterações"
+
 msgid "Error creating database backup."
 msgstr "Erro criando backup da base de dados."
 
 msgid "Error deleting database on instance."
 msgstr "Erro excluindo base de dados na instância."
 
+#, python-format
+msgid "Error downloading log file: %s"
+msgstr "Erro ao baixar o arquivo de log: %s"
+
+msgid "Error getting configuration group list."
+msgstr "Erro ao obter a lista do grupo de configuração."
+
 msgid "Error getting database backup list."
 msgstr "Erro buscando lista de backup da base de dados."
 
+#, python-format
+msgid "Error resetting parameters: %s"
+msgstr "Erro ao redefinir parâmetros: %s"
+
 msgctxt "Current status of a Database Backup"
 msgid "Failed"
 msgstr "Falhou"
 
 msgctxt "Current status of a Database Instance"
 msgid "Failed"
 msgstr "Falhou"
 
+msgid "Fault"
+msgstr "Falha"
+
 msgid "Flavor"
 msgstr "Flavor"
 
 msgid "GB"
 msgstr "GB"
 
+msgid "Go"
+msgstr "Ir"
+
 msgid "Grant Access"
 msgid_plural "Grant Access"
 msgstr[0] "Conceder Acesso"
 msgstr[1] "Conceder Acessos"
 
 msgid "Granted Access to"
 msgid_plural "Granted Access to"
@@ -337,14 +545,17 @@
 
 msgid "Grow Cluster"
 msgstr "Aumentar Cluster"
 
 msgid "Grow Cluster: {{cluster_name}}"
 msgstr "Aumentar Cluster: {{cluster_name}}"
 
+msgid "Has Root Ever Been Enabled"
+msgstr "Root já foi ativado"
+
 msgid "Host"
 msgstr "Host"
 
 msgid "Host or IP that the user is allowed to connect through."
 msgstr "Host ou IP através do qual o usuário pode conectar-se."
 
 msgid "ID"
@@ -352,14 +563,17 @@
 
 msgid "Incremental"
 msgstr "Incremental"
 
 msgid "Incremental Backup"
 msgstr "Incremental Backup"
 
+msgid "Info"
+msgstr "Informações"
+
 msgid "Information"
 msgstr "Informação"
 
 msgid "Initial Admin User"
 msgstr "Usuário Inicial Admin"
 
 msgid "Initial Databases"
@@ -402,14 +616,35 @@
 msgid "Launched %(count)s named \"%(name)s\"."
 msgstr "Disparadas %(count)s chamadas \"%(name)s\"."
 
 #, python-format
 msgid "Launched cluster \"%s\""
 msgstr "Cluster iniciado \"%s\""
 
+msgid "Locality"
+msgstr "Localidade"
+
+msgid "Log"
+msgstr "Log"
+
+msgid "Log Contents"
+msgstr "Conteúdo do Log"
+
+msgid "Log Length"
+msgstr "Tamanho do Log"
+
+msgid "Log length must be a nonnegative integer."
+msgstr "Tamanho do log deve ser um número inteiro não negativo."
+
+msgid "Log: "
+msgstr "Log:"
+
+msgid "Logs"
+msgstr "Logs"
+
 msgid "Manage Access"
 msgstr "Gerenciar Acesso"
 
 msgid "Manage Root"
 msgstr "Gerenciar Root"
 
 msgid "Manage Root Access"
@@ -417,14 +652,25 @@
 
 msgid "Management Console"
 msgstr "Console de Gerenciamento"
 
 msgid "Master Instance Name"
 msgstr "Nome da Instância Mestre"
 
+msgid "Message"
+msgstr "Mensagem"
+
+msgid ""
+"Move networks from 'Available Networks' to 'Selected Networks' by clicking "
+"the button, or dragging and dropping. You can change the NIC order by "
+"dragging and dropping as well."
+msgstr ""
+"Mover redes de 'Redes Disponíveis' para 'Redes Selecionadas' ao clicar no "
+"botão, ou arrastar e soltar."
+
 msgid "Name"
 msgstr "Nome"
 
 msgid "Network"
 msgstr "Rede"
 
 msgid "Network attached to instance."
@@ -451,17 +697,23 @@
 
 msgid "New password for cluster access."
 msgstr "Nova senha para o acesso ao cluster."
 
 msgid "New size for volume must be greater than current size."
 msgstr "Novo tamanho para o volume tem de ser maior do que o tamanho atual."
 
+msgid "No availability zones found"
+msgstr "Não foram encontradas zonas de disponibilidade"
+
 msgid "No backups available"
 msgstr "Não há backups disponíveis"
 
+msgid "No configuration groups available"
+msgstr "Nenhum grupo de configuração disponível"
+
 msgid "No flavors available"
 msgstr "Nenhum flavor disponível."
 
 msgid "No instances available"
 msgstr "Não há instâncias disponíveis"
 
 msgid "No volume type"
@@ -563,14 +815,20 @@
 
 msgid "Overview"
 msgstr "Visão Geral"
 
 msgid "PASSWORD"
 msgstr "SENHA"
 
+msgid "Parameter"
+msgstr "Parâmetro"
+
+msgid "Parameters"
+msgstr "Parâmetros"
+
 msgid "Parent Backup"
 msgstr "Backup pai"
 
 msgid "Password"
 msgstr "Senha"
 
 msgid "Password (required)"
@@ -584,17 +842,60 @@
 
 msgid ""
 "Password is only visible immediately after the root is enabled or reset."
 msgstr ""
 "A senha é apenas visível imediatamente após o root ser habilitado ou "
 "redefinido."
 
+msgid ""
+"Please note:</strong> The new value must be greater than the existing volume "
+"size."
+msgstr ""
+"Por favor, observe:</strong> O novo valor deve ser maior do que o tamanho do "
+"volume existente."
+
+msgid "Promote"
+msgstr "Promover"
+
+msgid "Promote to Replica Source"
+msgstr "Promover para Origem de Réplica"
+
+#, python-format
+msgid "Promoted replica \"%s\" as the new replica source."
+msgstr "Promovido réplica \"%s\" como nova origem de réplica."
+
+msgid "Property"
+msgstr "Propriedade"
+
+msgid "Publish"
+msgstr "Publicar"
+
+msgid "Publish Log"
+msgid_plural "Publish Logs"
+msgstr[0] "Publicar Log"
+msgstr[1] "Publicar Logs"
+
+msgid "Publishable (bytes)"
+msgstr "Publicável (bytes)"
+
+msgid "Published (bytes)"
+msgstr "Publicado (bytes)"
+
+msgid "Published Log"
+msgid_plural "Published Logs"
+msgstr[0] "Log Publicado"
+msgstr[1] "Logs Publicados"
+
 msgid "RAM"
 msgstr "RAM"
 
+msgctxt "Current status of a Database Instance"
+msgid "Rebooting"
+msgstr "Reinicializando"
+
 msgid "Related To"
 msgstr "Relacionado a"
 
 msgid "Remove Instance"
 msgid_plural "Remove Instances"
 msgstr[0] "Remover Instância"
 msgstr[1] "Remover Instâncias"
@@ -603,28 +904,34 @@
 msgid_plural "Removed Instances"
 msgstr[0] "Instância Removida"
 msgstr[1] "Instâncias Removidas"
 
 msgid "Removed instances from cluster."
 msgstr "Removido instâncias do Cluster"
 
+msgid "Replica Count"
+msgstr "Contagem de Réplicas"
+
 msgid "Replica Detached"
 msgid_plural "Replicas Detached"
 msgstr[0] "Réplica Desanexada"
 msgstr[1] "Réplicas Desanexadas"
 
 msgid "Replicas"
 msgstr "Réplicas"
 
 msgid "Replicate from Instance"
 msgstr "Replicar da Instância"
 
 msgid "Replication"
 msgstr "Replicação"
 
+msgid "Reset Parameters"
+msgstr "Redefinir Parâmetros"
+
 msgid "Reset Root Password"
 msgstr "Redefinição da Senha Root"
 
 msgid "Resize Database Instance"
 msgstr "Redimensionar Instância de Banco de Dados"
 
 msgid "Resize Database Volume"
@@ -632,14 +939,18 @@
 
 msgid "Resize Instance"
 msgstr "Redimensionar Instância"
 
 msgid "Resize Volume"
 msgstr "Redimensionar volume"
 
+msgctxt "Current status of a Database Instance"
+msgid "Resizing"
+msgstr "Redimensionando"
+
 #, python-format
 msgid "Resizing instance \"%s\""
 msgstr "Redimensionando a instância \"%s\""
 
 #, python-format
 msgid "Resizing volume \"%s\""
 msgstr "Redimensionando volume \"%s\""
@@ -665,14 +976,17 @@
 
 msgid "Restore Backup"
 msgstr "Restaurar Backup"
 
 msgid "Restore from Backup"
 msgstr "Recuperar do Backup"
 
+msgid "Return to Log List"
+msgstr "Retornar à Lista de Log"
+
 msgid "Revoke Access"
 msgid_plural "Revoke Access"
 msgstr[0] "Remover Acesso"
 msgstr[1] "Remover Acessos"
 
 msgid "Root Enabled"
 msgstr "Root Habilitado"
@@ -709,23 +1023,37 @@
 
 msgid "Scheduled growing of cluster."
 msgstr "Agendado o aumento do cluster."
 
 msgid "Select a backup to restore"
 msgstr "Selecione um Backup para Restaurar"
 
+msgid "Select a configuration group"
+msgstr "Selecionar um grupo de configuração"
+
+msgid "Select a configuration group to attach to the database instance."
+msgstr ""
+"Selecione um grupo de configuração para anexar à instância de banco de dados."
+
 msgid "Select a master instance"
 msgstr "Selecione a instância mestre"
 
 msgid "Select a new flavor"
 msgstr "Selecione um novo flavor"
 
+msgid "Select a parameter and provide a value for the configuration parameter."
+msgstr ""
+"Selecione um parâmetro e forneça um valor para o parâmetro de configuração."
+
 msgid "Select backup"
 msgstr "Selecionar Backup"
 
+msgid "Select configuration group"
+msgstr "Selecionar grupo de configuração"
+
 msgid "Select datastore type and version"
 msgstr "Selecione o tipo de armazenamento de dados e versão"
 
 msgid "Select instance"
 msgstr "Selecione uma instância"
 
 msgid "Select parent backup"
@@ -797,23 +1125,36 @@
 msgid "Specify the new root password for vertica cluster."
 msgstr "Especifique a nova senha de root para o vertica cluster."
 
 msgid "Specify the new volume size for the database instance."
 msgstr ""
 "Especifique o novo tamanho do volume para a instância de banco de dados."
 
+msgid ""
+"Specify whether instances in the cluster will be created on the same "
+"hypervisor (affinity) or on different hypervisors (anti-affinity)."
+msgstr ""
+"Especifique se as instâncias no cluster serão criadas no mesmo hypervisor "
+"(afinidade) ou em um hypervisor diferente (anti-afinidade)."
+
 msgid "Specs"
 msgstr "Especificações"
 
 msgid "Status"
 msgstr "Status"
 
 msgid "Status if root was ever enabled for an instance."
 msgstr "Situação se o root sempre foi habilitado para uma instância."
 
+msgid "Successfully added parameter"
+msgstr "Parâmetro adicionado com sucesso."
+
+msgid "Successfully disabled root access."
+msgstr "Acesso de root desabilitado com sucesso."
+
 msgid ""
 "The 'Instance Type' and 'Related To' fields are datastore specific and "
 "optional.  See the Trove documentation for more information on using these "
 "fields."
 msgstr ""
 "O 'Tipo de Instância' e 'Relacionados' campos são armazenamento de dados "
 "específico e opcional. Consulte a documentação do Trove para obter mais "
@@ -834,44 +1175,65 @@
 
 msgid "The number of shards must be greater than 1."
 msgstr "O número de shards precisar ser maior que 1."
 
 msgid "There was a problem enabling root."
 msgstr "Houve um problema ao habilitar raiz."
 
+msgid "This action cannot be undone."
+msgstr "Essa ação não poderá ser desfeita."
+
 msgid "Type"
 msgstr "Tipo"
 
 msgid "Type and version of datastore."
 msgstr "Tipo e versão do armazenamento de dados."
 
 msgid "USERNAME"
 msgstr "USUÁRIO"
 
 #, python-format
 msgid "Unable to %(action)s: %(objs)s"
 msgstr "Não foi possível %(action)s: %(objs)s"
 
 #, python-format
+msgid "Unable to add new parameter: %s"
+msgstr "Não é possível adicionar novo parâmetro: %s"
+
+#, python-format
+msgid "Unable to attach configuration group. %s"
+msgstr "Não é possível anexar grupo de configuração. %s"
+
+#, python-format
+msgid "Unable to create configuration group. %s"
+msgstr "Não é possível criar grupo de configuração. %s"
+
+#, python-format
 msgid "Unable to create database. %s"
 msgstr "Não foi possível criar base de dados: %s"
 
+msgid "Unable to create list of parameters."
+msgstr "Não é possível criar lista de parâmetros."
+
 #, python-format
 msgid "Unable to create user. %s"
 msgstr "Não é possível criar usuário. %s"
 
 msgid "Unable to determine if instance root is enabled."
 msgstr "Não foi possível determinar se o root está habilitado na instância"
 
 msgid "Unable to find backup!"
 msgstr "Não foi possível encontrar o backup!"
 
 msgid "Unable to find master instance!"
 msgstr "Incapaz de encontrar instância mestre!"
 
+msgid "Unable to get configuration data."
+msgstr "Não é possível obter dados de configuração"
+
 msgid "Unable to get database backup data."
 msgstr "Não é possível obter dados de backup de banco de dados."
 
 msgid "Unable to get databases data."
 msgstr "Não é possível obter dados de bancos de dados."
 
 msgid "Unable to get instances data."
@@ -901,26 +1263,43 @@
 
 msgid "Unable to list database backups for parent."
 msgstr "Não foi possível listar os backups de banco de dados para o pai."
 
 msgid "Unable to list database instances to backup."
 msgstr "Não foi possível listar as instâncias de banco de dados para backup."
 
+msgid ""
+"Unable to load {0} log\n"
+"{1}"
+msgstr ""
+"Não é possível carregar {0} log\n"
+"{1}"
+
+msgid "Unable to load {0} log for instance \"{1}\"."
+msgstr "Não é possível carregar {0} log para a instância \"{1}\"."
+
 msgid "Unable to obtain datastore versions."
 msgstr "Não é possível obter versões de datastores."
 
 msgid "Unable to obtain datastores."
 msgstr "Não é possível obter datastores."
 
 msgid "Unable to obtain flavors."
 msgstr "Não é possível obter flavors."
 
 msgid "Unable to obtain information on root user"
 msgstr "Não é possível obter informação do usuário root"
 
+msgid "Unable to obtain list of parameters."
+msgstr "Não é possível obter lista de parâmetros."
+
+#, python-format
+msgid "Unable to promote replica as the new replica source.  \"%s\""
+msgstr "Não é possível promover a réplica como nova origem de réplica. \"%s\""
+
 #, python-format
 msgid "Unable to remove instances from cluster: %s"
 msgstr "Não é possível remover instâncias do cluster: %s"
 
 #, python-format
 msgid "Unable to reset password. %s"
 msgstr "Não é possível redefinir a senha. %s"
@@ -932,14 +1311,17 @@
 #, python-format
 msgid "Unable to resize volume. %s"
 msgstr "Não é possível redimensionar volume. %s"
 
 msgid "Unable to retrieve accessible databases."
 msgstr "Não foi possível obter as bases de dados acessíveis."
 
+msgid "Unable to retrieve availability zones."
+msgstr "Não é possível recuperar zonas de disponibilidade"
+
 msgid "Unable to retrieve cluster details."
 msgstr "Não foi possível recuperar os detalhes do cluster."
 
 msgid "Unable to retrieve database clusters."
 msgstr "Não é possível recuperar os clusters de banco de dados."
 
 msgid "Unable to retrieve database instances."
@@ -952,14 +1334,18 @@
 msgstr "Não foi possível obter as bases de dados."
 
 #, python-format
 msgid "Unable to retrieve details for backup: %s"
 msgstr "Não foi possível obter detalhes do backup: %s"
 
 #, python-format
+msgid "Unable to retrieve details for configuration group: %s"
+msgstr "Não é possível obter detalhes para o grupo de configuração: %s"
+
+#, python-format
 msgid "Unable to retrieve details for database cluster: %s"
 msgstr "Não foi possível obter detalhes para a base de dados do Cluster: %s"
 
 #, python-format
 msgid "Unable to retrieve details for database instance: %s"
 msgstr "Não foi possível obter detalhes para a instância da base de dados: %s"
 
@@ -969,21 +1355,32 @@
 
 msgid "Unable to retrieve flavors."
 msgstr "Não foi possível recuperar flavors."
 
 msgid "Unable to retrieve instance details."
 msgstr "Não foi possível recuperar os detalhes da instância."
 
+#, python-format
+msgid ""
+"Unable to retrieve list of logs.\n"
+"%s"
+msgstr ""
+"Não é possível recuperar lista de logs.\n"
+"%s"
+
 msgid "Unable to retrieve networks."
 msgstr "Não é possível recuperar redes."
 
 #, python-format
 msgid "Unable to update user. %s"
 msgstr "Não é possível atualizar usuário. %s"
 
+msgid "Unknown"
+msgstr "Desconhecido"
+
 msgid "Updated"
 msgstr "Atualizado"
 
 #, python-format
 msgid "Updated user \"%s\"."
 msgstr "Atualizado usuário \"%s\"."
 
@@ -992,14 +1389,48 @@
 
 msgid "Username (required)"
 msgstr "Nome de usuário (requerido)"
 
 msgid "Users"
 msgstr "Usuários"
 
+msgid "Value"
+msgstr "Valor"
+
+msgid "Value must be \"true\" or \"false\"."
+msgstr "Valor deve ser \"true\" ou\"false\"."
+
+#, python-format
+msgid "Value must be a number between %(min)s and %(max)s."
+msgstr "Valor deve ser um número entre %(min)s e %(max)s."
+
+#, python-format
+msgid "Value must be a number greater than or equal to %s."
+msgstr "Valor deve ser um número maior que ou igual a %s."
+
+#, python-format
+msgid "Value must be a number less than or equal to %s."
+msgstr "Valor deve seu um número menor que ou igual a %s."
+
+msgid "Value must be a number."
+msgstr "Valor deve ser um número."
+
+#, python-format
+msgid "Value must be of type %s."
+msgstr "Valor deve ser do tipo %s."
+
+msgid "Values"
+msgstr "Valores"
+
+msgid "View Full Log"
+msgstr "Ver Log Completo"
+
+msgid "View Log"
+msgstr "Visualizar Log"
+
 msgid "Volume"
 msgstr "Volume"
 
 msgid "Volume Size"
 msgstr "Tamanho do Volume"
 
 msgid "Volume Type"
@@ -1017,16 +1448,27 @@
 "Você pode realizar um backup incremental, especificando um backup pai. "
 "<strong> No entanto, </strong> nem todos os bancos de dados oferece suporte "
 "a backups incrementais, caso em que esta operação irá resultar em um erro."
 
 msgid "You must select a datastore type and version."
 msgstr "Você deve selecionar um tipo de armazenamento de dados e versão."
 
+msgid "You must select a flavor."
+msgstr "Você deve selecionar um flavor."
+
 msgid "You must specify a password if you create a user."
 msgstr "Você deve especificar uma senha se você criar um usuário."
 
 msgid "You must specify at least one database if you create a user."
 msgstr ""
 "Você deve especificar ao menos uma base de dados se você criar um usuário."
 
+#, python-format
+msgid ""
+"[flavor=%(flavor)s, volume=%(volume)s, name=%(name)s, type=%(type)s, "
+"related_to=%(related_to)s, nics=%(nics)s]"
+msgstr ""
+"[flavor=%(flavor)s, volume=%(volume)s, nome=%(name)s, tipo=%(type)s, "
+"relacionado_a=%(related_to)s, nics=%(nics)s]"
+
 msgid "instance"
 msgstr "instância"
```

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ru/LC_MESSAGES/django.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/locale/ru/LC_MESSAGES/djangojs.po` & `trove-dashboard-9.0.1/trove_dashboard/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/project/ngbackups/backups.module.js` & `trove-dashboard-9.0.1/trove_dashboard/static/dashboard/project/ngbackups/backups.module.js`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/project/ngbackups/backups.module.spec.js` & `trove-dashboard-9.0.1/trove_dashboard/static/dashboard/project/ngbackups/backups.module.spec.js`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/project/ngbackups/table/table.controller.js` & `trove-dashboard-9.0.1/trove_dashboard/static/dashboard/project/ngbackups/table/table.controller.js`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/static/dashboard/project/ngbackups/table/table.config.js` & `trove-dashboard-9.0.1/trove_dashboard/static/dashboard/project/ngbackups/table/table.config.js`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/static/app/core/openstack-service-api/trove.service.js` & `trove-dashboard-9.0.1/trove_dashboard/static/app/core/openstack-service-api/trove.service.js`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/enabled/_1731_project_database_backups_panel.py` & `trove-dashboard-9.0.1/trove_dashboard/enabled/_1731_project_database_backups_panel.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/enabled/_1760_project_database_configurations_panel.py` & `trove-dashboard-9.0.1/trove_dashboard/enabled/_1760_project_database_configurations_panel.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/enabled/_1720_project_databases_panel.py` & `trove-dashboard-9.0.1/trove_dashboard/enabled/_1720_project_databases_panel.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/enabled/_1710_database_panel_group.py` & `trove-dashboard-9.0.1/trove_dashboard/enabled/_1710_database_panel_group.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/enabled/_1740_project_database_clusters_panel.py` & `trove-dashboard-9.0.1/trove_dashboard/enabled/_1740_project_database_clusters_panel.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/enabled/_1730_project_database_backups_panel.py` & `trove-dashboard-9.0.1/trove_dashboard/enabled/_1730_project_database_backups_panel.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/version.py` & `trove-dashboard-9.0.1/trove_dashboard/version.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/test/test_data/utils.py` & `trove-dashboard-9.0.1/trove_dashboard/test/test_data/utils.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/test/test_data/keystone_data.py` & `trove-dashboard-9.0.1/trove_dashboard/test/test_data/keystone_data.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/test/test_data/exceptions.py` & `trove-dashboard-9.0.1/trove_dashboard/test/test_data/exceptions.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/test/test_data/trove_data.py` & `trove-dashboard-9.0.1/trove_dashboard/test/test_data/trove_data.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/test/helpers.py` & `trove-dashboard-9.0.1/trove_dashboard/test/helpers.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/test/urls.py` & `trove-dashboard-9.0.1/trove_dashboard/test/urls.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/test/settings.py` & `trove-dashboard-9.0.1/trove_dashboard/test/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,7 +15,17 @@
 from openstack_dashboard.test.settings import *  # noqa
 
 INSTALLED_APPS = list(INSTALLED_APPS)
 INSTALLED_APPS.append('trove_dashboard.content.database_backups')
 INSTALLED_APPS.append('trove_dashboard.content.database_clusters')
 INSTALLED_APPS.append('trove_dashboard.content.database_configurations')
 INSTALLED_APPS.append('trove_dashboard.content.databases')
+
+CACHES = {
+    'default': {
+        'BACKEND': 'django.core.cache.backends.locmem.LocMemCache',
+        'OPTIONS': {
+            'MAX_ENTRIES': 1200,
+            'CULL_FREQUENCY': 20
+        }
+    }
+}
```

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/exceptions.py` & `trove-dashboard-9.0.1/trove_dashboard/exceptions.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/panel.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/panel.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/tabs.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/tabs.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/cluster_manager.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/urls.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/urls.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/forms.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/forms.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_cassandra.html` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_cassandra.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_redis.html` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_redis.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_mongodb.html` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_mongodb.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview.html` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_mysql.html` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_mysql.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_vertica.html` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_detail_overview_vertica.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/templates/database_clusters/_reset_password.html` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/templates/database_clusters/_reset_password.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/tests.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/tests.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/views.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/views.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_clusters/tables.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_clusters/tables.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/panel.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/panel.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/tabs.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/tabs.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/urls.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/urls.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/forms.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/forms.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/config_param_manager.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/config_param_manager.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/templates/database_configurations/_detail_overview.html` & `trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/templates/database_configurations/_detail_overview.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/tests.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/tests.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/views.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/views.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_configurations/tables.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_configurations/tables.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/panel.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_backups/panel.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/urls.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_backups/urls.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/workflows/create_backup.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_backups/workflows/create_backup.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/templates/database_backups/details.html` & `trove-dashboard-9.0.1/trove_dashboard/content/database_backups/templates/database_backups/details.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/tests.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_backups/tests.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/views.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_backups/views.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/database_backups/tables.py` & `trove-dashboard-9.0.1/trove_dashboard/content/database_backups/tables.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/panel.py` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/panel.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/tabs.py` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/tabs.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/urls.py` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/urls.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/workflows/create_instance.py` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/workflows/create_instance.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/forms.py` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/forms.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/db_capability.py` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/db_capability.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_detail_overview_cassandra.html` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_detail_overview_cassandra.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_promote_to_replica_source.html` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_promote_to_replica_source.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_detail_overview_redis.html` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_detail_overview_redis.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_launch_initialize_help.html` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_launch_initialize_help.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_detail_overview_mongodb.html` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_detail_overview_mongodb.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_launch_networks.html` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_launch_networks.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_detail_overview_couchbase.html` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_detail_overview_couchbase.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_detail_overview_postgresql.html` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_detail_overview_postgresql.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_detail_overview.html` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_detail_overview.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/_detail_overview_mysql.html` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/_detail_overview_mysql.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/templates/databases/logs/_detail_log.html` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/templates/databases/logs/_detail_log.html`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/tests.py` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/tests.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/views.py` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/views.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/logs/urls.py` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/logs/urls.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/logs/tests.py` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/logs/tests.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/logs/views.py` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/logs/views.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/logs/tables.py` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/logs/tables.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/databases/tables.py` & `trove-dashboard-9.0.1/trove_dashboard/content/databases/tables.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/ng_database_backups/__init__.py` & `trove-dashboard-9.0.1/trove_dashboard/content/ng_database_backups/__init__.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/ng_database_backups/panel.py` & `trove-dashboard-9.0.1/trove_dashboard/content/ng_database_backups/panel.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/ng_database_backups/urls.py` & `trove-dashboard-9.0.1/trove_dashboard/content/ng_database_backups/urls.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard/content/ng_database_backups/views.py` & `trove-dashboard-9.0.1/trove_dashboard/content/ng_database_backups/views.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard.egg-info/SOURCES.txt` & `trove-dashboard-9.0.1/trove_dashboard.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.zuul.yaml
 AUTHORS
 CONTRIBUTING.rst
 ChangeLog
 HACKING.rst
 LICENSE
 MANIFEST.in
 README.rst
@@ -26,22 +27,14 @@
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/_static/.placeholder
 releasenotes/source/_templates/.placeholder
-releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
-releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
-releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
-releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po
-releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
 tools/clean_enabled_files.py
 tools/install_venv.py
 tools/pip_install.sh
 tools/with_venv.sh
 trove_dashboard/__init__.py
 trove_dashboard/exceptions.py
 trove_dashboard/version.py
```

### Comparing `trove-dashboard-9.0.0.0rc1/trove_dashboard.egg-info/PKG-INFO` & `trove-dashboard-9.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: trove-dashboard
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: Trove Management Dashboard
 Home-page: http://docs.openstack.org/developer/trove/
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: OpenStack Dashboard plugin for Trove project
         ============================================
@@ -22,15 +22,15 @@
         pick up the trove plugin when it starts.
         
         How to use with devstack:
         -------------------------
         
         Add the following to your devstack ``local.conf`` file::
         
-            enable_plugin trove-dashboard git://git.openstack.org/openstack/trove-dashboard
+            enable_plugin trove-dashboard https://git.openstack.org/openstack/trove-dashboard
         
         
         To run unit tests:
         ------------------
         ::
         
             ./run_tests.sh
@@ -67,32 +67,32 @@
         Settings
         ~~~~~~~~
         
         The use of a cross-process cache such as Memcached is required.
         
         Install Memcached itself and a Memcached binding such as python-memcached.
         
-        For a single horizon instance use the CACHES setting like the example below.
+        For a single horizon instance use the CACHES setting like the example below.::
         
-        CACHES = {
-            'default': {
-                'BACKEND': 'django.core.cache.backends.memcached.MemcachedCache',
-                'LOCATION': '127.0.0.1:11211',
-            },
-        }
+            CACHES = {
+                'default': {
+                    'BACKEND': 'django.core.cache.backends.memcached.MemcachedCache',
+                    'LOCATION': '127.0.0.1:11211',
+                },
+            }
         
         For multiple horizon instances behind a load balancer configure each instance
-        to use the same cache like the example below.
+        to use the same cache like the example below.::
         
-        CACHES = {
-            'default': {
-                'BACKEND': 'django.core.cache.backends.memcached.MemcachedCache',
-                'LOCATION': [u'10.2.100.133:11211', u'10.2.100.134:11211'']
-            },
-        }
+            CACHES = {
+                'default': {
+                    'BACKEND': 'django.core.cache.backends.memcached.MemcachedCache',
+                    'LOCATION': [u'10.2.100.133:11211', u'10.2.100.134:11211'']
+                },
+            }
         
         
         NOTE:
         =====
         
         As of the Mitaka release, the dashboard for trove is now maintained outside of
         the Horizon codebase, in this repository.
```

### Comparing `trove-dashboard-9.0.0.0rc1/tools/pip_install.sh` & `trove-dashboard-9.0.1/tools/pip_install.sh`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     export ZUUL_BRANCH=${ZUUL_BRANCH-$BRANCH}
     echo "ZUUL CLONER" > /tmp/tox_install.txt
     cwd=$(/bin/pwd)
     cd /tmp
     $ZUUL_CLONER --cache-dir \
         /opt/git \
         --branch $BRANCH_NAME \
-        git://git.openstack.org \
+        https://git.openstack.org \
         openstack/horizon
     cd openstack/horizon
     $install_cmd -e .
     cd "$cwd"
 else
     echo "PIP HARDCODE" > /tmp/tox_install.txt
     if [ -z "$HORIZON_PIP_LOCATION" ]; then
```

### Comparing `trove-dashboard-9.0.0.0rc1/tools/clean_enabled_files.py` & `trove-dashboard-9.0.1/tools/clean_enabled_files.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/tools/install_venv.py` & `trove-dashboard-9.0.1/tools/install_venv.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/CONTRIBUTING.rst` & `trove-dashboard-9.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/manage.py` & `trove-dashboard-9.0.1/manage.py`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/PKG-INFO` & `trove-dashboard-9.0.1/trove_dashboard.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: trove-dashboard
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: Trove Management Dashboard
 Home-page: http://docs.openstack.org/developer/trove/
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: OpenStack Dashboard plugin for Trove project
         ============================================
@@ -22,15 +22,15 @@
         pick up the trove plugin when it starts.
         
         How to use with devstack:
         -------------------------
         
         Add the following to your devstack ``local.conf`` file::
         
-            enable_plugin trove-dashboard git://git.openstack.org/openstack/trove-dashboard
+            enable_plugin trove-dashboard https://git.openstack.org/openstack/trove-dashboard
         
         
         To run unit tests:
         ------------------
         ::
         
             ./run_tests.sh
@@ -67,32 +67,32 @@
         Settings
         ~~~~~~~~
         
         The use of a cross-process cache such as Memcached is required.
         
         Install Memcached itself and a Memcached binding such as python-memcached.
         
-        For a single horizon instance use the CACHES setting like the example below.
+        For a single horizon instance use the CACHES setting like the example below.::
         
-        CACHES = {
-            'default': {
-                'BACKEND': 'django.core.cache.backends.memcached.MemcachedCache',
-                'LOCATION': '127.0.0.1:11211',
-            },
-        }
+            CACHES = {
+                'default': {
+                    'BACKEND': 'django.core.cache.backends.memcached.MemcachedCache',
+                    'LOCATION': '127.0.0.1:11211',
+                },
+            }
         
         For multiple horizon instances behind a load balancer configure each instance
-        to use the same cache like the example below.
+        to use the same cache like the example below.::
         
-        CACHES = {
-            'default': {
-                'BACKEND': 'django.core.cache.backends.memcached.MemcachedCache',
-                'LOCATION': [u'10.2.100.133:11211', u'10.2.100.134:11211'']
-            },
-        }
+            CACHES = {
+                'default': {
+                    'BACKEND': 'django.core.cache.backends.memcached.MemcachedCache',
+                    'LOCATION': [u'10.2.100.133:11211', u'10.2.100.134:11211'']
+                },
+            }
         
         
         NOTE:
         =====
         
         As of the Mitaka release, the dashboard for trove is now maintained outside of
         the Horizon codebase, in this repository.
```

### Comparing `trove-dashboard-9.0.0.0rc1/ChangeLog` & `trove-dashboard-9.0.1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 CHANGES
 =======
 
-9.0.0.0rc1
-----------
+9.0.1
+-----
+
+* OpenDev Migration Patch
+* Fix README syntax to meet PyPI requirements
+* Replace openstack.org git:// URLs with https://
+* import zuul job settings from project-config
+* Imported Translations from Zanata
+* Update UPPER\_CONSTRAINTS\_FILE for stable/pike
+* Update .gitreview for stable/pike
+* Fix unstable test case
+* Imported Translations from Zanata
+
+9.0.0
+-----
 
 * Imported Translations from Zanata
 
 9.0.0.0b3
 ---------
 
 * Imported Translations from Zanata
```

### Comparing `trove-dashboard-9.0.0.0rc1/README.rst` & `trove-dashboard-9.0.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 pick up the trove plugin when it starts.
 
 How to use with devstack:
 -------------------------
 
 Add the following to your devstack ``local.conf`` file::
 
-    enable_plugin trove-dashboard git://git.openstack.org/openstack/trove-dashboard
+    enable_plugin trove-dashboard https://git.openstack.org/openstack/trove-dashboard
 
 
 To run unit tests:
 ------------------
 ::
 
     ./run_tests.sh
@@ -59,32 +59,32 @@
 Settings
 ~~~~~~~~
 
 The use of a cross-process cache such as Memcached is required.
 
 Install Memcached itself and a Memcached binding such as python-memcached.
 
-For a single horizon instance use the CACHES setting like the example below.
+For a single horizon instance use the CACHES setting like the example below.::
 
-CACHES = {
-    'default': {
-        'BACKEND': 'django.core.cache.backends.memcached.MemcachedCache',
-        'LOCATION': '127.0.0.1:11211',
-    },
-}
+    CACHES = {
+        'default': {
+            'BACKEND': 'django.core.cache.backends.memcached.MemcachedCache',
+            'LOCATION': '127.0.0.1:11211',
+        },
+    }
 
 For multiple horizon instances behind a load balancer configure each instance
-to use the same cache like the example below.
+to use the same cache like the example below.::
 
-CACHES = {
-    'default': {
-        'BACKEND': 'django.core.cache.backends.memcached.MemcachedCache',
-        'LOCATION': [u'10.2.100.133:11211', u'10.2.100.134:11211'']
-    },
-}
+    CACHES = {
+        'default': {
+            'BACKEND': 'django.core.cache.backends.memcached.MemcachedCache',
+            'LOCATION': [u'10.2.100.133:11211', u'10.2.100.134:11211'']
+        },
+    }
 
 
 NOTE:
 =====
 
 As of the Mitaka release, the dashboard for trove is now maintained outside of
 the Horizon codebase, in this repository.
```

### Comparing `trove-dashboard-9.0.0.0rc1/LICENSE` & `trove-dashboard-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/setup.cfg` & `trove-dashboard-9.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `trove-dashboard-9.0.0.0rc1/setup.py` & `trove-dashboard-9.0.1/setup.py`

 * *Files identical despite different names*

