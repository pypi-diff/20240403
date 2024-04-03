# Comparing `tmp/magnum-ui-9.0.0.tar.gz` & `tmp/magnum-ui-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnum-ui-9.0.0.tar", last modified: Wed Oct  6 11:16:19 2021, max compression
+gzip compressed data, was "magnum-ui-9.0.0.0rc1.tar", last modified: Wed Sep 15 02:26:26 2021, max compression
```

## Comparing `magnum-ui-9.0.0.tar` & `magnum-ui-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,320 +1,320 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.142369 magnum-ui-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1587 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/.eslintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2021-10-06 11:15:38.000000 magnum-ui-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2518 2021-10-06 11:16:18.000000 magnum-ui-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20815 2021-10-06 11:16:18.000000 magnum-ui-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3769 2021-10-06 11:16:19.142369 magnum-ui-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2431 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/babel-django.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/babel-djangojs.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.114368 magnum-ui-9.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1984 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.114368 magnum-ui-9.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5568 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.114368 magnum-ui-9.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10641 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.114368 magnum-ui-9.0.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3243 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.114368 magnum-ui-9.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/doc/source/contributor/api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.114368 magnum-ui-9.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1897 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2750 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.118368 magnum-ui-9.0.0/magnum_ui/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.118368 magnum-ui-9.0.0/magnum_ui/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1910 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/api/heat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9199 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/api/magnum.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.118368 magnum-ui-9.0.0/magnum_ui/api/rest/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/api/rest/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15351 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/api/rest/magnum.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.118368 magnum-ui-9.0.0/magnum_ui/content/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/content/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.118368 magnum-ui-9.0.0/magnum_ui/content/cluster_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/content/cluster_templates/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/content/cluster_templates/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/content/cluster_templates/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/content/cluster_templates/urls.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.118368 magnum-ui-9.0.0/magnum_ui/content/clusters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/content/clusters/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      915 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/content/clusters/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/content/clusters/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/content/clusters/urls.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.118368 magnum-ui-9.0.0/magnum_ui/content/container_infra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/content/container_infra/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.118368 magnum-ui-9.0.0/magnum_ui/content/container_infra/quotas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/content/container_infra/quotas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/content/container_infra/quotas/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/content/container_infra/quotas/urls.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.118368 magnum-ui-9.0.0/magnum_ui/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1237 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/enabled/_1370_project_container_infra_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/enabled/_1371_project_container_infra_clusters_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/enabled/_1372_project_container_infra_cluster_templates_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/enabled/_2370_admin_container_infra_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/enabled/_2371_admin_container_infra_quotas_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/enabled/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5537 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/karma.conf.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/magnum_ui/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.106368 magnum-ui-9.0.0/magnum_ui/locale/cs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.122368 magnum-ui-9.0.0/magnum_ui/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/cs/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12014 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/cs/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.106368 magnum-ui-9.0.0/magnum_ui/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.122368 magnum-ui-9.0.0/magnum_ui/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19489 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/de/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.106368 magnum-ui-9.0.0/magnum_ui/locale/en_AU/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.122368 magnum-ui-9.0.0/magnum_ui/locale/en_AU/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12871 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/en_AU/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/magnum_ui/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.122368 magnum-ui-9.0.0/magnum_ui/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/en_GB/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28167 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/en_GB/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/magnum_ui/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.122368 magnum-ui-9.0.0/magnum_ui/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16389 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/fr/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/magnum_ui/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.122368 magnum-ui-9.0.0/magnum_ui/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/id/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18180 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/id/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/magnum_ui/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.122368 magnum-ui-9.0.0/magnum_ui/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/ja/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19794 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/ja/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/magnum_ui/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.122368 magnum-ui-9.0.0/magnum_ui/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/ko_KR/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18435 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/ko_KR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/magnum_ui/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.122368 magnum-ui-9.0.0/magnum_ui/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/pt_BR/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18651 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/magnum_ui/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.122368 magnum-ui-9.0.0/magnum_ui/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1304 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/ru/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31999 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/ru/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/magnum_ui/locale/tr_TR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.122368 magnum-ui-9.0.0/magnum_ui/locale/tr_TR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/tr_TR/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14818 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/tr_TR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/magnum_ui/locale/zh_Hans/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.122368 magnum-ui-9.0.0/magnum_ui/locale/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13418 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/locale/zh_Hans/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/magnum_ui/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/magnum_ui/static/dashboard/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.126369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.126369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2965 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/actions.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2166 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/actions.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4985 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2154 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1917 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.126369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/create/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2945 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/create/create.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2509 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/create/create.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.126369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/delete/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5858 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/delete/delete.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4288 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/delete/delete.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.126369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/details.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1381 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/drawer.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/drawer.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1655 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/overview.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1678 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/overview.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4210 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/panel.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.126369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/update/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6309 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/update/update.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2945 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/update/update.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.126369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/info.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/labels.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/network.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/spec.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20688 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/workflow.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2587 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/workflow.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.130369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3643 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/actions.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2762 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/actions.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2981 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/cluster-stats.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2721 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/cluster-stats.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5914 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/clusters.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      851 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/clusters.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/clusters.scss
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1959 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/clusters.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2426 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/clusters.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.130369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/create/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6521 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/create/create.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4009 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/create/create.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.130369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/delete/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5698 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/delete/delete.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4213 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/delete/delete.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.130369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/details.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1343 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/drawer.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1069 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/drawer.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1526 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/overview.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1648 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/overview.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4514 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1005 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/panel.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.130369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/resize/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6188 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/resize/resize.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/resize/resize.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.130369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/rolling-upgrade/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7460 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/rolling-upgrade/upgrade.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4801 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/rolling-upgrade/upgrade.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.130369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/rotate-certificate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2382 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/rotate-certificate/rotate-certificate.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1678 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/rotate-certificate/rotate-certificate.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.130369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/show-certificate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2097 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/show-certificate/show-certificate.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1712 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/show-certificate/show-certificate.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.134369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1534 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-modal.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-modal.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1740 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-model.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1580 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-model.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2979 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.134369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/advanced.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4764 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/cluster-template.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9484 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/cluster-template.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/cluster-template.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/details.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/management.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/network.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/size.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23750 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/workflow.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3861 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/workflow.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1333 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/container-infra.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/container-infra.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/container-infra.scss
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10423 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/magnum.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8721 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/magnum.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.134369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/actions.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/actions.module.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.134369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/create/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2941 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/create/create.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2341 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/create/create.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.134369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/delete/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5832 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/delete/delete.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4096 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/delete/delete.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/panel.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4050 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/quotas.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/quotas.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1664 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/quotas.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/quotas.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.134369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/update/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3424 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/update/update.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2773 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/update/update.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.134369 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/workflow/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3277 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/workflow/workflow.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/workflow/workflow.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2120 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/utils.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/utils.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.138369 magnum-ui-9.0.0/magnum_ui/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/test/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.138369 magnum-ui-9.0.0/magnum_ui/test/api_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/test/api_tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5511 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/test/api_tests/test_rest_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1563 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/test/helpers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.138369 magnum-ui-9.0.0/magnum_ui/test/integration_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/test/integration_tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/test/settings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3203 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/test/test_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/magnum_ui/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.118368 magnum-ui-9.0.0/magnum_ui.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3769 2021-10-06 11:16:18.000000 magnum-ui-9.0.0/magnum_ui.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12653 2021-10-06 11:16:19.000000 magnum-ui-9.0.0/magnum_ui.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-10-06 11:16:18.000000 magnum-ui-9.0.0/magnum_ui.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-10-06 11:16:18.000000 magnum-ui-9.0.0/magnum_ui.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-10-06 11:16:18.000000 magnum-ui-9.0.0/magnum_ui.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-10-06 11:16:18.000000 magnum-ui-9.0.0/magnum_ui.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2021-10-06 11:16:18.000000 magnum-ui-9.0.0/magnum_ui.egg-info/top_level.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      825 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1067 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/package.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.138369 magnum-ui-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/add-fedora-coreos-7882a33d801371fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/add-reno-7d46796dbf41c247.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/bugfix-cluster-template-hidden-arg-38909eaa92bd8d56.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/bugfix-set-floating_ip_enabled-default_in-cluster-template-true-ce06118f0e6064ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/improve-cluster-launch-dfc514b51cfa7f0e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1515 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/newton-dac21adfe6c6b8ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/ocata-b08d6b024c63296b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      965 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/ocata-summary-a717111a782c7a68.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1672 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/pike-b1af664f1033a131.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2070 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/queens-f99244e9db54ccf3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/resize-actions-1436a2a0dccbd13b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1339 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/rocky-56165675d959b593.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/show-health-status-ff92b2fe2bfad5ae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1974 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/stein-a6adf485dbbbbd1a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/update-actions-02db7b9f8e5d36b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/notes/upgrade-actions-adf2f749ec0cc817.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.142369 magnum-ui-9.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8833 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2021-10-06 11:15:38.000000 magnum-ui-9.0.0/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.114368 magnum-ui-9.0.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.142369 magnum-ui-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21571 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.142369 magnum-ui-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25576 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.142369 magnum-ui-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1726 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/releasenotes/source/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.142369 magnum-ui-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19942 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/releasenotes/source/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.142369 magnum-ui-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28052 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.142369 magnum-ui-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24240 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.110368 magnum-ui-9.0.0/releasenotes/source/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.142369 magnum-ui-9.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17745 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.114368 magnum-ui-9.0.0/releasenotes/source/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.142369 magnum-ui-9.0.0/releasenotes/source/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1438 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.114368 magnum-ui-9.0.0/releasenotes/source/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.142369 magnum-ui-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11482 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2021-10-06 11:16:19.142369 magnum-ui-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2635 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/test-shim.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-10-06 11:16:19.142369 magnum-ui-9.0.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2404 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/tools/install_venv.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5920 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/tools/install_venv_common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3505 2021-10-06 11:15:37.000000 magnum-ui-9.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.593264 magnum-ui-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1587 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/.eslintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2518 2021-09-15 02:26:26.000000 magnum-ui-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20825 2021-09-15 02:26:26.000000 magnum-ui-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3774 2021-09-15 02:26:26.593264 magnum-ui-9.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2431 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/babel-django.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/babel-djangojs.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.557263 magnum-ui-9.0.0.0rc1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1984 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.557263 magnum-ui-9.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5568 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.557263 magnum-ui-9.0.0.0rc1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10641 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.557263 magnum-ui-9.0.0.0rc1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3243 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.557263 magnum-ui-9.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/doc/source/contributor/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.557263 magnum-ui-9.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1897 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2750 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.557263 magnum-ui-9.0.0.0rc1/magnum_ui/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.561263 magnum-ui-9.0.0.0rc1/magnum_ui/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1910 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/api/heat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9199 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/api/magnum.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.561263 magnum-ui-9.0.0.0rc1/magnum_ui/api/rest/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/api/rest/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15351 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/api/rest/magnum.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.561263 magnum-ui-9.0.0.0rc1/magnum_ui/content/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/content/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.561263 magnum-ui-9.0.0.0rc1/magnum_ui/content/cluster_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/content/cluster_templates/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/content/cluster_templates/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/content/cluster_templates/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/content/cluster_templates/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.561263 magnum-ui-9.0.0.0rc1/magnum_ui/content/clusters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/content/clusters/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      915 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/content/clusters/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/content/clusters/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/content/clusters/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.561263 magnum-ui-9.0.0.0rc1/magnum_ui/content/container_infra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/content/container_infra/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.561263 magnum-ui-9.0.0.0rc1/magnum_ui/content/container_infra/quotas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/content/container_infra/quotas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/content/container_infra/quotas/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/content/container_infra/quotas/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.561263 magnum-ui-9.0.0.0rc1/magnum_ui/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1237 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/enabled/_1370_project_container_infra_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/enabled/_1371_project_container_infra_clusters_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/enabled/_1372_project_container_infra_cluster_templates_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/enabled/_2370_admin_container_infra_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/enabled/_2371_admin_container_infra_quotas_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/enabled/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5537 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/karma.conf.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/locale/cs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.565264 magnum-ui-9.0.0.0rc1/magnum_ui/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/cs/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12014 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/cs/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.565264 magnum-ui-9.0.0.0rc1/magnum_ui/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19489 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/de/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/locale/en_AU/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.565264 magnum-ui-9.0.0.0rc1/magnum_ui/locale/en_AU/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12871 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/en_AU/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.565264 magnum-ui-9.0.0.0rc1/magnum_ui/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/en_GB/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28167 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/en_GB/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.565264 magnum-ui-9.0.0.0rc1/magnum_ui/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16389 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/fr/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.565264 magnum-ui-9.0.0.0rc1/magnum_ui/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/id/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18180 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/id/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.565264 magnum-ui-9.0.0.0rc1/magnum_ui/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/ja/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19794 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/ja/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.565264 magnum-ui-9.0.0.0rc1/magnum_ui/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/ko_KR/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18435 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/ko_KR/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.565264 magnum-ui-9.0.0.0rc1/magnum_ui/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/pt_BR/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18651 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.565264 magnum-ui-9.0.0.0rc1/magnum_ui/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1304 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/ru/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31999 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/ru/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/locale/tr_TR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.565264 magnum-ui-9.0.0.0rc1/magnum_ui/locale/tr_TR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/tr_TR/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14818 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/tr_TR/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/locale/zh_Hans/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.569264 magnum-ui-9.0.0.0rc1/magnum_ui/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13418 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/locale/zh_Hans/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.545263 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.569264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.569264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2965 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/actions.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2166 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/actions.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4985 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2154 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1917 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.569264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/create/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2945 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/create/create.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2509 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/create/create.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.569264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/delete/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5858 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/delete/delete.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4288 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/delete/delete.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.573264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/details.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1381 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/drawer.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/drawer.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/drawer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1655 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/overview.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1678 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/overview.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4210 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/panel.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.573264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/update/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6309 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/update/update.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2945 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/update/update.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.573264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/info.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/labels.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/network.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/spec.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20688 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/workflow.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2587 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/workflow.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.577264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3643 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/actions.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2762 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/actions.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2981 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/cluster-stats.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2721 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/cluster-stats.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5914 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/clusters.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      851 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/clusters.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/clusters.scss
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1959 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/clusters.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2426 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/clusters.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.577264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/create/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6521 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/create/create.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4009 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/create/create.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.577264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/delete/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5698 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/delete/delete.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4213 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/delete/delete.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.577264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/details.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1343 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/drawer.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1069 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/drawer.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/drawer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1526 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/overview.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1648 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/overview.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4514 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1005 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/panel.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.577264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/resize/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6188 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/resize/resize.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/resize/resize.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.577264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/rolling-upgrade/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7460 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/rolling-upgrade/upgrade.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4801 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/rolling-upgrade/upgrade.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.577264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/rotate-certificate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2382 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/rotate-certificate/rotate-certificate.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1678 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/rotate-certificate/rotate-certificate.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.577264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/show-certificate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2097 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/show-certificate/show-certificate.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1712 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/show-certificate/show-certificate.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.581264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1534 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-modal.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-modal.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1740 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-model.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1580 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-model.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2979 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.581264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/advanced.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4764 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/cluster-template.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9484 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/cluster-template.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/cluster-template.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/details.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/management.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/network.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/size.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23750 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/workflow.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3861 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/workflow.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1333 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/container-infra.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/container-infra.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/container-infra.scss
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10423 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/magnum.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8721 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/magnum.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.585264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/actions.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/actions.module.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.585264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/create/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2941 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/create/create.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2341 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/create/create.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.585264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/delete/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5832 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/delete/delete.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4096 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/delete/delete.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/panel.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4050 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/quotas.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/quotas.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1664 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/quotas.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/quotas.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.585264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/update/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3424 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/update/update.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2773 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/update/update.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.585264 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/workflow/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3277 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/workflow/workflow.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/workflow/workflow.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2120 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/utils.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/utils.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.585264 magnum-ui-9.0.0.0rc1/magnum_ui/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/test/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.585264 magnum-ui-9.0.0.0rc1/magnum_ui/test/api_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/test/api_tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5511 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/test/api_tests/test_rest_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1563 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/test/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.585264 magnum-ui-9.0.0.0rc1/magnum_ui/test/integration_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/test/integration_tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/test/settings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3203 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/test/test_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/magnum_ui/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.557263 magnum-ui-9.0.0.0rc1/magnum_ui.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3774 2021-09-15 02:26:26.000000 magnum-ui-9.0.0.0rc1/magnum_ui.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12653 2021-09-15 02:26:26.000000 magnum-ui-9.0.0.0rc1/magnum_ui.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-09-15 02:26:26.000000 magnum-ui-9.0.0.0rc1/magnum_ui.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-09-15 02:26:26.000000 magnum-ui-9.0.0.0rc1/magnum_ui.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-09-15 02:26:26.000000 magnum-ui-9.0.0.0rc1/magnum_ui.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-09-15 02:26:26.000000 magnum-ui-9.0.0.0rc1/magnum_ui.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2021-09-15 02:26:26.000000 magnum-ui-9.0.0.0rc1/magnum_ui.egg-info/top_level.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      825 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1067 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/package.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.549264 magnum-ui-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.589264 magnum-ui-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/add-fedora-coreos-7882a33d801371fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/add-reno-7d46796dbf41c247.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/bugfix-cluster-template-hidden-arg-38909eaa92bd8d56.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/bugfix-set-floating_ip_enabled-default_in-cluster-template-true-ce06118f0e6064ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/improve-cluster-launch-dfc514b51cfa7f0e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1515 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/newton-dac21adfe6c6b8ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/ocata-b08d6b024c63296b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      965 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/ocata-summary-a717111a782c7a68.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1672 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/pike-b1af664f1033a131.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2070 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/queens-f99244e9db54ccf3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/resize-actions-1436a2a0dccbd13b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1339 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/rocky-56165675d959b593.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/show-health-status-ff92b2fe2bfad5ae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1974 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/stein-a6adf485dbbbbd1a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/update-actions-02db7b9f8e5d36b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/notes/upgrade-actions-adf2f749ec0cc817.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.593264 magnum-ui-9.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8833 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.553264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.549264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.593264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21571 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.549264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.593264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25576 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.549264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.593264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1726 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.549264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.593264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19942 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.549264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.593264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28052 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.549264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.593264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24240 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.549264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.593264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17745 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.553264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.593264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1438 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.553264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.593264 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11482 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2021-09-15 02:26:26.597264 magnum-ui-9.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2635 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/test-shim.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-15 02:26:26.593264 magnum-ui-9.0.0.0rc1/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2404 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/tools/install_venv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5920 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/tools/install_venv_common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3505 2021-09-15 02:25:51.000000 magnum-ui-9.0.0.0rc1/tox.ini
```

### Comparing `magnum-ui-9.0.0/.eslintrc` & `magnum-ui-9.0.0.0rc1/.eslintrc`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/AUTHORS` & `magnum-ui-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/CONTRIBUTING.rst` & `magnum-ui-9.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/ChangeLog` & `magnum-ui-9.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * Default \`floating\_ip\_enabled\` to true in cluster template
 * Update horizon nodejs template
 * Add overlay2 to Docker storage driver dropdown
 * Support zero workers nodes on Horizon dashboard
 * Remove hard\_limit check in dashboard
 * Add Python3 xena unit tests
```

### Comparing `magnum-ui-9.0.0/LICENSE` & `magnum-ui-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/PKG-INFO` & `magnum-ui-9.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: magnum-ui
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Magnum User Interface
 Home-page: https://docs.openstack.org/developer/magnum-ui/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `magnum-ui-9.0.0/README.rst` & `magnum-ui-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/devstack/plugin.sh` & `magnum-ui-9.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/doc/Makefile` & `magnum-ui-9.0.0.0rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/doc/requirements.txt` & `magnum-ui-9.0.0.0rc1/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/doc/source/conf.py` & `magnum-ui-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/doc/source/configuration/index.rst` & `magnum-ui-9.0.0.0rc1/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/doc/source/index.rst` & `magnum-ui-9.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/doc/source/install/index.rst` & `magnum-ui-9.0.0.0rc1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/lower-constraints.txt` & `magnum-ui-9.0.0.0rc1/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/api/heat.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/api/heat.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/api/magnum.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/api/magnum.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/api/rest/__init__.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/api/rest/magnum.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/api/rest/magnum.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/content/cluster_templates/panel.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/content/cluster_templates/panel.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/content/cluster_templates/tests.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/content/cluster_templates/tests.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/content/cluster_templates/urls.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/content/cluster_templates/urls.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/content/clusters/panel.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/content/clusters/panel.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/content/clusters/tests.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/content/clusters/tests.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/content/clusters/urls.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/content/clusters/urls.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/content/container_infra/quotas/panel.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/content/container_infra/quotas/panel.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/content/container_infra/quotas/urls.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/content/container_infra/quotas/urls.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/enabled/_1370_project_container_infra_panel_group.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/enabled/_1370_project_container_infra_panel_group.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/enabled/_1371_project_container_infra_clusters_panel.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/enabled/_1371_project_container_infra_clusters_panel.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/enabled/_1372_project_container_infra_cluster_templates_panel.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/enabled/_1372_project_container_infra_cluster_templates_panel.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/enabled/_2370_admin_container_infra_panel_group.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/enabled/_2370_admin_container_infra_panel_group.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/enabled/_2371_admin_container_infra_quotas_panel.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/enabled/_2371_admin_container_infra_quotas_panel.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/karma.conf.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/karma.conf.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/cs/LC_MESSAGES/django.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/cs/LC_MESSAGES/djangojs.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/de/LC_MESSAGES/django.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/de/LC_MESSAGES/djangojs.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/en_AU/LC_MESSAGES/djangojs.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/en_AU/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/en_GB/LC_MESSAGES/django.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/en_GB/LC_MESSAGES/djangojs.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/en_GB/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/fr/LC_MESSAGES/django.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/fr/LC_MESSAGES/djangojs.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/id/LC_MESSAGES/django.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/id/LC_MESSAGES/djangojs.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/id/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/ja/LC_MESSAGES/django.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/ja/LC_MESSAGES/djangojs.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/ja/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/ko_KR/LC_MESSAGES/django.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/ko_KR/LC_MESSAGES/djangojs.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/ko_KR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/pt_BR/LC_MESSAGES/django.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/pt_BR/LC_MESSAGES/djangojs.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/ru/LC_MESSAGES/django.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/ru/LC_MESSAGES/djangojs.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/tr_TR/LC_MESSAGES/django.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/tr_TR/LC_MESSAGES/djangojs.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/zh_Hans/LC_MESSAGES/django.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/locale/zh_Hans/LC_MESSAGES/djangojs.po` & `magnum-ui-9.0.0.0rc1/magnum_ui/locale/zh_Hans/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/actions.module.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/actions.module.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/actions.module.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/actions.module.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.module.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.module.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.module.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.module.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/cluster-templates.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/create/create.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/create/create.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/create/create.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/create/create.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/delete/delete.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/delete/delete.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/delete/delete.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/delete/delete.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/details.module.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/details.module.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/drawer.controller.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/drawer.controller.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/drawer.controller.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/drawer.controller.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/drawer.html` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/drawer.html`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/overview.controller.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/overview.controller.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/overview.controller.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/overview.controller.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/details/overview.html` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/details/overview.html`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/update/update.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/update/update.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/update/update.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/update/update.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/info.help.html` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/info.help.html`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/network.help.html` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/network.help.html`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/spec.help.html` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/spec.help.html`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/workflow.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/workflow.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/workflow.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/cluster-templates/workflow/workflow.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/actions.module.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/actions.module.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/actions.module.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/actions.module.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/cluster-stats.controller.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/cluster-stats.controller.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/cluster-stats.controller.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/cluster-stats.controller.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/clusters.module.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/clusters.module.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/clusters.module.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/clusters.module.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/clusters.scss` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/clusters.scss`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/clusters.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/clusters.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/clusters.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/clusters.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/create/create.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/create/create.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/create/create.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/create/create.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/delete/delete.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/delete/delete.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/delete/delete.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/delete/delete.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/details.module.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/details.module.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/drawer.controller.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/drawer.controller.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/drawer.controller.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/drawer.controller.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/drawer.html` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/drawer.html`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/overview.controller.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/overview.controller.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/overview.controller.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/overview.controller.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/details/overview.html` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/details/overview.html`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/panel.html` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/panel.html`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/resize/resize.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/resize/resize.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/resize/resize.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/resize/resize.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/rolling-upgrade/upgrade.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/rolling-upgrade/upgrade.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/rolling-upgrade/upgrade.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/rolling-upgrade/upgrade.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/rotate-certificate/rotate-certificate.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/rotate-certificate/rotate-certificate.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/rotate-certificate/rotate-certificate.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/rotate-certificate/rotate-certificate.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/show-certificate/show-certificate.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/show-certificate/show-certificate.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/show-certificate/show-certificate.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/show-certificate/show-certificate.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-modal.controller.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-modal.controller.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-modal.html` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-modal.html`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-model.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-model.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-model.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate-model.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/sign-certificate/sign-certificate.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/cluster-template.controller.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/cluster-template.controller.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/cluster-template.controller.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/cluster-template.controller.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/cluster-template.html` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/cluster-template.html`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/network.help.html` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/network.help.html`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/size.help.html` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/size.help.html`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/workflow.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/workflow.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/clusters/workflow/workflow.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/clusters/workflow/workflow.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/container-infra.module.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/container-infra.module.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/container-infra.module.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/container-infra.module.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/magnum.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/magnum.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/magnum.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/magnum.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/actions.module.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/actions.module.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/actions.module.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/actions.module.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/create/create.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/create/create.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/create/create.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/create/create.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/delete/delete.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/delete/delete.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/delete/delete.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/delete/delete.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/quotas.module.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/quotas.module.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/quotas.module.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/quotas.module.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/quotas.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/quotas.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/quotas.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/quotas.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/update/update.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/update/update.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/update/update.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/update/update.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/workflow/workflow.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/workflow/workflow.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/quotas/workflow/workflow.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/quotas/workflow/workflow.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/utils.service.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/utils.service.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/static/dashboard/container-infra/utils.service.spec.js` & `magnum-ui-9.0.0.0rc1/magnum_ui/static/dashboard/container-infra/utils.service.spec.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/test/api_tests/test_rest_api.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/test/api_tests/test_rest_api.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/test/helpers.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/test/helpers.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/test/settings.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/test/settings.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/test/test_data.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/test/test_data.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui/version.py` & `magnum-ui-9.0.0.0rc1/magnum_ui/version.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/magnum_ui.egg-info/PKG-INFO` & `magnum-ui-9.0.0.0rc1/magnum_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: magnum-ui
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Magnum User Interface
 Home-page: https://docs.openstack.org/developer/magnum-ui/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `magnum-ui-9.0.0/magnum_ui.egg-info/SOURCES.txt` & `magnum-ui-9.0.0.0rc1/magnum_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/manage.py` & `magnum-ui-9.0.0.0rc1/manage.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/package.json` & `magnum-ui-9.0.0.0rc1/package.json`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/notes/newton-dac21adfe6c6b8ee.yaml` & `magnum-ui-9.0.0.0rc1/releasenotes/notes/newton-dac21adfe6c6b8ee.yaml`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/notes/ocata-b08d6b024c63296b.yaml` & `magnum-ui-9.0.0.0rc1/releasenotes/notes/ocata-b08d6b024c63296b.yaml`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/notes/ocata-summary-a717111a782c7a68.yaml` & `magnum-ui-9.0.0.0rc1/releasenotes/notes/ocata-summary-a717111a782c7a68.yaml`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/notes/pike-b1af664f1033a131.yaml` & `magnum-ui-9.0.0.0rc1/releasenotes/notes/pike-b1af664f1033a131.yaml`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/notes/queens-f99244e9db54ccf3.yaml` & `magnum-ui-9.0.0.0rc1/releasenotes/notes/queens-f99244e9db54ccf3.yaml`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/notes/rocky-56165675d959b593.yaml` & `magnum-ui-9.0.0.0rc1/releasenotes/notes/rocky-56165675d959b593.yaml`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/notes/stein-a6adf485dbbbbd1a.yaml` & `magnum-ui-9.0.0.0rc1/releasenotes/notes/stein-a6adf485dbbbbd1a.yaml`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/source/conf.py` & `magnum-ui-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `magnum-ui-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `magnum-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `magnum-ui-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po` & `magnum-ui-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po` & `magnum-ui-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `magnum-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po` & `magnum-ui-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po` & `magnum-ui-9.0.0.0rc1/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po` & `magnum-ui-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/requirements.txt` & `magnum-ui-9.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/setup.cfg` & `magnum-ui-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/setup.py` & `magnum-ui-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/test-requirements.txt` & `magnum-ui-9.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/test-shim.js` & `magnum-ui-9.0.0.0rc1/test-shim.js`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/tools/install_venv.py` & `magnum-ui-9.0.0.0rc1/tools/install_venv.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/tools/install_venv_common.py` & `magnum-ui-9.0.0.0rc1/tools/install_venv_common.py`

 * *Files identical despite different names*

### Comparing `magnum-ui-9.0.0/tox.ini` & `magnum-ui-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

