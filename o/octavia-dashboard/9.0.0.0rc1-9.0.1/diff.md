# Comparing `tmp/octavia-dashboard-9.0.0.0rc1.tar.gz` & `tmp/octavia-dashboard-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octavia-dashboard-9.0.0.0rc1.tar", last modified: Thu Mar 10 08:19:35 2022, max compression
+gzip compressed data, was "octavia-dashboard-9.0.1.tar", last modified: Fri Sep 29 08:41:04 2023, max compression
```

## Comparing `octavia-dashboard-9.0.0.0rc1.tar` & `octavia-dashboard-9.0.1.tar`

### file list

```diff
@@ -1,436 +1,437 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.230305 octavia-dashboard-9.0.0.0rc1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/.eslintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2483 2022-03-10 08:19:35.000000 octavia-dashboard-9.0.0.0rc1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15008 2022-03-10 08:19:35.000000 octavia-dashboard-9.0.0.0rc1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4000 2022-03-10 08:19:35.230305 octavia-dashboard-9.0.0.0rc1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2398 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/babel-django.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/babel-djangojs.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.194305 octavia-dashboard-9.0.0.0rc1/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/devstack/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1915 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.194305 octavia-dashboard-9.0.0.0rc1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.194305 octavia-dashboard-9.0.0.0rc1/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4881 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/doc/source/readme.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/doc/source/reference.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2833 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/lower-constraints.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/manage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.194305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      647 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/api/rest/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1074 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/api/rest/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3095 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/api/rest/barbican.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50556 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/api/rest/lbaasv2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/conf/.gitkeep
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/project/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/project/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/project/load_balancer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/project/load_balancer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/project/load_balancer/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.182305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/project/load_balancer/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/project/load_balancer/templates/load_balancer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/project/load_balancer/templates/load_balancer/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/project/load_balancer/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/project/load_balancer/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1192 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/enabled/_1482_project_load_balancer_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/enabled/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5272 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/karma.conf.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/local_settings.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1100 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/local_settings.d/_1499_load_balancer_settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44897 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/de/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/en_AU/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/en_AU/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      631 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/en_AU/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/en_GB/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42498 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/en_GB/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      631 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6210 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/id/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40956 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/id/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.202305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      609 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ja/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46436 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ja/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.202305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ko_KR/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42942 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ko_KR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.202305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.202305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8520 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ru/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28792 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ru/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/zh_Hans/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.202305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38366 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/zh_Hans/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/zh_Hant/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.202305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/zh_Hant/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/zh_Hant/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36420 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/zh_Hant/LC_MESSAGES/djangojs.po
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      444 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/post_install.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/app/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/app/core/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.202305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/app/core/openstack-service-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29832 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/app/core/openstack-service-api/lbaasv2.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15802 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/app/core/openstack-service-api/lbaasv2.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2641 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/app/core/openstack-service-api/octavia-barbican.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2378 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/app/core/openstack-service-api/octavia-barbican.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.202305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.202305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.202305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2364 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/create.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1590 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/create.action.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1551 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/wizard.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/wizard.controller.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.202305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/delete/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4751 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/delete/delete.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4826 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/delete/delete.action.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.206305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2332 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/edit.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1605 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/edit.action.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/wizard.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1941 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/wizard.controller.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.206305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5050 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/detail.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5386 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/detail.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2837 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4907 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/healthmonitors.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2270 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/healthmonitors.module.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.206305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.206305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2347 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/create.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1980 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/create.action.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/wizard.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1923 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/wizard.controller.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.206305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/delete/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4392 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/delete/delete.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3889 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/delete/delete.action.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.206305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2255 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/edit.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1742 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/edit.action.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2048 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/wizard.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2600 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/wizard.controller.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.206305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4964 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/detail.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4698 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/detail.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4823 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/l7policies.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2206 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/l7policies.module.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.206305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.206305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2325 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/create.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1973 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/create.action.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1510 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/wizard.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1919 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/wizard.controller.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.206305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/delete/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4424 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/delete/delete.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3920 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/delete/delete.action.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.210305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2229 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/edit.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/edit.action.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2030 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/wizard.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2584 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/wizard.controller.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.210305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5095 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/detail.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4764 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/detail.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2433 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4740 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/l7rules.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2186 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/l7rules.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20703 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/lbaasv2.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20713 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/lbaasv2.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3038 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/lbaasv2.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.210305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.186305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.210305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2249 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/create.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1854 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/create.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/wizard.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1885 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/wizard.controller.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.210305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/delete/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4205 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/delete/delete.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5348 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/delete/delete.action.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.210305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2259 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/edit.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/edit.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1992 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/wizard.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2633 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/wizard.controller.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.210305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4612 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/detail.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4650 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/detail.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3006 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5473 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/listeners.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2230 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/listeners.module.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.210305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.190305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.214305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3607 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5502 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1392 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3707 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4122 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.214305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2313 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/create.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/create.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/wizard.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1844 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/wizard.controller.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.214305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/delete/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5453 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/delete/delete.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5596 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/delete/delete.action.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.214305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/disassociate-ip/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3437 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/disassociate-ip/modal.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4078 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/disassociate-ip/modal.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.214305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/edit.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2079 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/edit.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/wizard.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2160 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/wizard.controller.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.214305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4603 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/detail.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4621 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/detail.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2807 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5686 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2431 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11169 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12688 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/panel.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2003 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/panel.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/panel.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.214305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.190305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.214305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/delete/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4554 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/delete/delete.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4748 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/delete/delete.action.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.214305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3263 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3799 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5598 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3414 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3404 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.218305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2360 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/update-member-list.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/update-member-list.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1518 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/wizard.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/wizard.controller.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.218305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5003 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/detail.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5307 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/detail.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2919 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4850 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/members.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2214 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/members.module.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.218305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.190305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.218305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2348 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/create.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1995 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/create.action.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/wizard.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2133 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/wizard.controller.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.218305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/delete/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4423 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/delete/delete.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4713 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/delete/delete.action.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.218305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2235 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/edit.action.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1874 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/edit.action.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/wizard.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2519 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/wizard.controller.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.218305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5054 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/detail.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5227 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/detail.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3097 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5002 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/pools.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2198 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/pools.module.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.190305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/util/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.218305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/util/validators/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2041 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/util/validators/validate-unique.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2252 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/util/validators/validate-unique.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.190305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.218305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/filterselect/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7941 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/filterselect/filter-select.component.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9305 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/filterselect/filter-select.component.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1603 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/filterselect/filter-select.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.218305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/table/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/table/table-status.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3671 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/table/table-status.directive.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/table/table-status.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.222305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.222305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1757 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2003 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3228 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.222305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1532 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3934 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.222305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7rule/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2094 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7rule/l7rule.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3719 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7rule/l7rule.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.222305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3031 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4643 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2514 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11854 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.222305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6236 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10373 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4095 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.222305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4644 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4474 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1902 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13436 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3305 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/modal.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3284 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/modal.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32155 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/model.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    99261 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/model.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.222305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2997 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2951 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1646 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7544 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.222305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1876 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5851 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4580 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/workflow.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3697 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/workflow.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.226305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/tests/settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.226305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      996 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/tests/unit/registration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/tests/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.198305 octavia-dashboard-9.0.0.0rc1/octavia_dashboard.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4000 2022-03-10 08:19:35.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21979 2022-03-10 08:19:35.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-10 08:19:35.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-10 08:19:35.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-03-10 08:19:35.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2022-03-10 08:19:35.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2022-03-10 08:19:35.000000 octavia-dashboard-9.0.0.0rc1/octavia_dashboard.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   160640 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/package-lock.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1169 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/package.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.190305 octavia-dashboard-9.0.0.0rc1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.226305 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/Add-ProxyV2-b5537c092737fe41.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/Fix-namespace-collision-with-barbican-ui-267f4ba074729ea6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/add-RBAC-43ee180e712294ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/add-allowed-cidrs-ad205b1524da3d2c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/add-az-support-efdd4e7c5dccef21.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/add-ciphers-options-for-listeners-and-pools-8440eaf5a551c44c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/add-draining-operating-status-48f59a204371ff0d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/add-insert-headers-a6fd80c837a89536.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/add-l7-support-05a790bc2965c38f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/add-member-backup-32e2ec2553c1ba24.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/add-sctp-support-a1ea956b7630f47d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/add-timeout-options-8988fc477fa46d31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/add-tls_enabled-support-for-pools-449e39f851535839.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/add-udp-support-acb1a22fb605d3a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/add-x-forwarded-proto-e30b52a3f853ed62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/allows-creation-of-single-resources-9ec5fe87acc7c93c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/auto-refresh-detail-pages-26166d5d9c26edee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/bp-horizon-lbaas-v2-ui-ba7e4c97a0460f85.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/cascade-delete-e4c9d80a31076540.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/drop-py-2-7-f3372b5c26171513.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/edit-default-pool-on-listener-206d8dfeea135360.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/filter-select-65160dcbe699a96d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/fix-auth-url-barbican-client-d41b03419fb31ba4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/fix-flavor-no-flavor-profile-c3e82325f16d5ab8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/fix-member-weight-value-range-9310678f967c771a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/flavor-support-0195a486faa16b7f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1806 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/initial-octavia-dashboard-35d1d7f923473f21.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/list-pools-on-lb-details-page-eb0400bdb2b3650f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/notes/pool-selection-hint-7f282ba1fa014d8c.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.230305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.230305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.230305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5083 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.190305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.190305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.230305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2897 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.190305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.230305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13192 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.190305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.230305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12003 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.190305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.230305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12976 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.190305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.230305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7999 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.190305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_TW/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.230305 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8002 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_TW/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2022-03-10 08:19:35.230305 octavia-dashboard-9.0.0.0rc1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2421 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:19:35.230305 octavia-dashboard-9.0.0.0rc1/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2022-03-10 08:19:01.000000 octavia-dashboard-9.0.0.0rc1/zuul.d/projects.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.571732 octavia-dashboard-9.0.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/.eslintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2560 2023-09-29 08:41:04.000000 octavia-dashboard-9.0.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15276 2023-09-29 08:41:04.000000 octavia-dashboard-9.0.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3995 2023-09-29 08:41:04.571732 octavia-dashboard-9.0.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2398 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/babel-django.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/babel-djangojs.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.507732 octavia-dashboard-9.0.1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/devstack/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1915 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.507732 octavia-dashboard-9.0.1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.511731 octavia-dashboard-9.0.1/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4881 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/doc/source/reference.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/manage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.511731 octavia-dashboard-9.0.1/octavia_dashboard/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      647 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.511731 octavia-dashboard-9.0.1/octavia_dashboard/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.511731 octavia-dashboard-9.0.1/octavia_dashboard/api/rest/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1074 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/api/rest/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3095 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/api/rest/barbican.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50789 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/api/rest/lbaasv2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.515731 octavia-dashboard-9.0.1/octavia_dashboard/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/conf/.gitkeep
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.515731 octavia-dashboard-9.0.1/octavia_dashboard/dashboards/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/dashboards/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.515731 octavia-dashboard-9.0.1/octavia_dashboard/dashboards/project/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/dashboards/project/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.515731 octavia-dashboard-9.0.1/octavia_dashboard/dashboards/project/load_balancer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/dashboards/project/load_balancer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/dashboards/project/load_balancer/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.487731 octavia-dashboard-9.0.1/octavia_dashboard/dashboards/project/load_balancer/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.515731 octavia-dashboard-9.0.1/octavia_dashboard/dashboards/project/load_balancer/templates/load_balancer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/dashboards/project/load_balancer/templates/load_balancer/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      791 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/dashboards/project/load_balancer/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/dashboards/project/load_balancer/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.515731 octavia-dashboard-9.0.1/octavia_dashboard/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1192 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/enabled/_1482_project_load_balancer_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/enabled/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5272 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/karma.conf.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.515731 octavia-dashboard-9.0.1/octavia_dashboard/local_settings.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1100 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/local_settings.d/_1499_load_balancer_settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.515731 octavia-dashboard-9.0.1/octavia_dashboard/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44897 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/de/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/locale/en_AU/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.515731 octavia-dashboard-9.0.1/octavia_dashboard/locale/en_AU/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      631 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/en_AU/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.515731 octavia-dashboard-9.0.1/octavia_dashboard/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/en_GB/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42498 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/en_GB/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.515731 octavia-dashboard-9.0.1/octavia_dashboard/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      631 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.515731 octavia-dashboard-9.0.1/octavia_dashboard/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6210 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.519731 octavia-dashboard-9.0.1/octavia_dashboard/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/id/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40956 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/id/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.519731 octavia-dashboard-9.0.1/octavia_dashboard/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      609 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/ja/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46436 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/ja/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.519731 octavia-dashboard-9.0.1/octavia_dashboard/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/ko_KR/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42942 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/ko_KR/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.519731 octavia-dashboard-9.0.1/octavia_dashboard/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.519731 octavia-dashboard-9.0.1/octavia_dashboard/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8520 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/ru/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28792 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/ru/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/locale/zh_Hans/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.519731 octavia-dashboard-9.0.1/octavia_dashboard/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38366 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/zh_Hans/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/locale/zh_Hant/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.519731 octavia-dashboard-9.0.1/octavia_dashboard/locale/zh_Hant/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/zh_Hant/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36420 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/locale/zh_Hant/LC_MESSAGES/djangojs.po
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      444 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/post_install.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/static/app/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/static/app/core/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.519731 octavia-dashboard-9.0.1/octavia_dashboard/static/app/core/openstack-service-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29832 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/app/core/openstack-service-api/lbaasv2.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15802 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/app/core/openstack-service-api/lbaasv2.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2641 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/app/core/openstack-service-api/octavia-barbican.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2378 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/app/core/openstack-service-api/octavia-barbican.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.491732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.523732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.523732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.495731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.523732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2364 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/create.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1590 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/create.action.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1551 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/wizard.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/wizard.controller.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.523732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/delete/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4751 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/delete/delete.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4826 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/delete/delete.action.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.523732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2332 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/edit.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1605 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/edit.action.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/wizard.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1941 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/wizard.controller.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.527732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5050 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/detail.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5386 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/detail.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2837 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/drawer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4907 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/healthmonitors.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2270 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/healthmonitors.module.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.527732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.495731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.527732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2347 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/create.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1980 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/create.action.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/wizard.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1923 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/wizard.controller.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.527732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/delete/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4392 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/delete/delete.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3889 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/delete/delete.action.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.527732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2255 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/edit.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1742 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/edit.action.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2048 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/wizard.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2600 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/wizard.controller.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.531731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4964 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/detail.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4698 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/detail.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/drawer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4823 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/l7policies.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2206 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/l7policies.module.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.531731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.495731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.531731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2325 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/create.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1973 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/create.action.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1510 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/wizard.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1919 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/wizard.controller.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.531731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/delete/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4424 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/delete/delete.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3920 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/delete/delete.action.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.531731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2229 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/edit.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/edit.action.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2030 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/wizard.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2584 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/wizard.controller.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.531731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5095 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/detail.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4764 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/detail.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2433 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/drawer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4740 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/l7rules.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2186 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/l7rules.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20703 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/lbaasv2.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20713 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/lbaasv2.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3038 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/lbaasv2.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.535732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.495731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.535732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2249 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/create.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1854 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/create.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/wizard.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1885 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/wizard.controller.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.535732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/delete/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4205 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/delete/delete.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5348 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/delete/delete.action.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.535732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2259 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/edit.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/edit.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1992 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/wizard.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2633 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/wizard.controller.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.535732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4612 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/detail.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4650 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/detail.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3006 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/drawer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5473 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/listeners.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2230 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/listeners.module.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.539732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.495731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.539732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3607 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5502 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1392 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3707 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4122 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.539732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2313 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/create.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/create.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/wizard.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1844 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/wizard.controller.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.539732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/delete/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5453 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/delete/delete.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5596 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/delete/delete.action.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.539732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/disassociate-ip/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3437 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/disassociate-ip/modal.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4078 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/disassociate-ip/modal.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.543732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/edit.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2079 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/edit.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/wizard.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2160 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/wizard.controller.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.543732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4603 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/detail.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4621 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/detail.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2807 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/drawer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5686 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2431 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11169 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12688 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/panel.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2003 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/panel.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/panel.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.543732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.499731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.543732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/delete/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4554 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/delete/delete.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4748 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/delete/delete.action.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.543732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3263 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3799 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5598 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3414 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3404 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.547731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2360 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/update-member-list.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/update-member-list.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1518 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/wizard.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2368 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/wizard.controller.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.547731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5003 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/detail.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5307 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/detail.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2919 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/drawer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4850 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/members.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2214 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/members.module.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.547731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.499731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.547731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2348 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/create.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1995 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/create.action.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/wizard.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2133 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/wizard.controller.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.547731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/delete/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4423 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/delete/delete.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4713 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/delete/delete.action.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.551732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2235 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/edit.action.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1874 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/edit.action.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/wizard.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2519 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/wizard.controller.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.551732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5054 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/detail.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5227 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/detail.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3097 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/drawer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5002 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/pools.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2198 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/pools.module.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.499731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/util/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.551732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/util/validators/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2041 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/util/validators/validate-unique.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2252 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/util/validators/validate-unique.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.499731 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.551732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/filterselect/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8124 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/filterselect/filter-select.component.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9769 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/filterselect/filter-select.component.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1603 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/filterselect/filter-select.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.551732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/table/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/table/table-status.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3671 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/table/table-status.directive.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/table/table-status.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.555732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.555732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1757 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2003 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3228 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.555732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1532 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1263 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3934 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.555732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7rule/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2094 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7rule/l7rule.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3719 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7rule/l7rule.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.555732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3031 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4643 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2514 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11854 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.559732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6236 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10373 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4095 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.559732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4644 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4474 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1902 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13416 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3305 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/modal.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3284 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/modal.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32155 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/model.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    99261 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/model.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.559732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2997 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2951 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1646 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7544 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.559732 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1766 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1876 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5851 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4580 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/workflow.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3697 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/workflow.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.559732 octavia-dashboard-9.0.1/octavia_dashboard/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/tests/settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.559732 octavia-dashboard-9.0.1/octavia_dashboard/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      996 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/tests/unit/registration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/tests/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/octavia_dashboard/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.511731 octavia-dashboard-9.0.1/octavia_dashboard.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3995 2023-09-29 08:41:04.000000 octavia-dashboard-9.0.1/octavia_dashboard.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22089 2023-09-29 08:41:04.000000 octavia-dashboard-9.0.1/octavia_dashboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-09-29 08:41:04.000000 octavia-dashboard-9.0.1/octavia_dashboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-09-29 08:41:04.000000 octavia-dashboard-9.0.1/octavia_dashboard.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-09-29 08:41:04.000000 octavia-dashboard-9.0.1/octavia_dashboard.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-09-29 08:41:04.000000 octavia-dashboard-9.0.1/octavia_dashboard.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2023-09-29 08:41:04.000000 octavia-dashboard-9.0.1/octavia_dashboard.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   160640 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/package-lock.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1169 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/package.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.503731 octavia-dashboard-9.0.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.567732 octavia-dashboard-9.0.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/Add-ProxyV2-b5537c092737fe41.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/Fix-namespace-collision-with-barbican-ui-267f4ba074729ea6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/add-RBAC-43ee180e712294ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/add-allowed-cidrs-ad205b1524da3d2c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/add-az-support-efdd4e7c5dccef21.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/add-ciphers-options-for-listeners-and-pools-8440eaf5a551c44c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/add-draining-operating-status-48f59a204371ff0d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/add-insert-headers-a6fd80c837a89536.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/add-l7-support-05a790bc2965c38f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/add-member-backup-32e2ec2553c1ba24.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/add-sctp-support-a1ea956b7630f47d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/add-timeout-options-8988fc477fa46d31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/add-tls_enabled-support-for-pools-449e39f851535839.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/add-udp-support-acb1a22fb605d3a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/add-x-forwarded-proto-e30b52a3f853ed62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/allows-creation-of-single-resources-9ec5fe87acc7c93c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/auto-refresh-detail-pages-26166d5d9c26edee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/bp-horizon-lbaas-v2-ui-ba7e4c97a0460f85.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/cascade-delete-e4c9d80a31076540.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/drop-py-2-7-f3372b5c26171513.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/edit-default-pool-on-listener-206d8dfeea135360.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/filter-select-65160dcbe699a96d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/fix-auth-url-barbican-client-d41b03419fb31ba4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/fix-chrome-member-dialog-154981a7794d5fb4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/fix-flavor-no-flavor-profile-c3e82325f16d5ab8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/fix-member-weight-value-range-9310678f967c771a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/fix-updating-non-http-hm-114180139961e441.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/flavor-support-0195a486faa16b7f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1806 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/initial-octavia-dashboard-35d1d7f923473f21.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/list-pools-on-lb-details-page-eb0400bdb2b3650f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/notes/pool-selection-hint-7f282ba1fa014d8c.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.571732 octavia-dashboard-9.0.1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.571732 octavia-dashboard-9.0.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.571732 octavia-dashboard-9.0.1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5083 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      801 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.503731 octavia-dashboard-9.0.1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.503731 octavia-dashboard-9.0.1/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.571732 octavia-dashboard-9.0.1/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2897 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.503731 octavia-dashboard-9.0.1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.571732 octavia-dashboard-9.0.1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13192 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.503731 octavia-dashboard-9.0.1/releasenotes/source/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.571732 octavia-dashboard-9.0.1/releasenotes/source/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12003 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.503731 octavia-dashboard-9.0.1/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.571732 octavia-dashboard-9.0.1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12976 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.503731 octavia-dashboard-9.0.1/releasenotes/source/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.571732 octavia-dashboard-9.0.1/releasenotes/source/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7999 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.503731 octavia-dashboard-9.0.1/releasenotes/source/locale/zh_TW/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.571732 octavia-dashboard-9.0.1/releasenotes/source/locale/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8002 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/locale/zh_TW/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2023-09-29 08:41:04.571732 octavia-dashboard-9.0.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2272 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-29 08:41:04.571732 octavia-dashboard-9.0.1/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-09-29 08:40:36.000000 octavia-dashboard-9.0.1/zuul.d/projects.yaml
```

### Comparing `octavia-dashboard-9.0.0.0rc1/.eslintrc` & `octavia-dashboard-9.0.1/.eslintrc`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/AUTHORS` & `octavia-dashboard-9.0.1/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 Doug Wiegley <dougw@a10networks.com>
 Elena Ezhova <eezhova@mirantis.com>
 Emmanuel MISSIAEN <emmanuel.missiaen@gendarmerie.interieur.gouv.fr>
 Erik Olof Gunnar Andersson <eandersson@blizzard.com>
 Flavio Percoco <flaper87@gmail.com>
 Frank Kloeker <f.kloeker@telekom.de>
 German Eichberger <German.eichberger@rackspace.com>
+Ghanshyam Mann <gmann@ghanshyammann.com>
 Gregory Thiemonge <gthiemon@redhat.com>
 Hervé Beraud <hberaud@redhat.com>
 Jacky Hu <hudayou@hotmail.com>
 James E. Blair <jeblair@redhat.com>
 Jesper Schmitz Mouridsen <jesper@schmitz.computer>
 Justin Pomeroy <jpomero@linux.vnet.ibm.com>
 Kyle Mestery <mestery@mestery.com>
@@ -42,14 +43,15 @@
 Sean McGinnis <sean.mcginnis@gmail.com>
 ShangXiao <shangxiaobj@inspur.com>
 Steven Glasford <stevenglasford@gmail.com>
 Swapnil Kulkarni (coolsvap) <me@coolsvap.net>
 Takashi Kajinami <tkajinam@redhat.com>
 Tom Weininger <tweining@redhat.com>
 Tong Liu <tongl@vmware.com>
+Vadym Markov <vmarkov@mirantis.com>
 Vieri <15050873171@163.com>
 Vivek Jain <v.jain007@gmail.com>
 avnish <avnish.pal@nectechnologies.in>
 chenxiangui <chenxiangui@inspur.com>
 coco-Gao <419546439@qq.com>
 howardlee <lihongweibj@inspur.com>
 huang.zhiping <huang.zhiping@99cloud.net>
```

### Comparing `octavia-dashboard-9.0.0.0rc1/CONTRIBUTING.rst` & `octavia-dashboard-9.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/ChangeLog` & `octavia-dashboard-9.0.1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 CHANGES
 =======
 
-9.0.0.0rc1
-----------
+9.0.1
+-----
+
+* Drop lower-constraints.txt and its testing
+* Fix popover attributes in member add dialog
+* Fix updating a non-HTTP(S) Health Monitor
+* Fix network selector filter at LB creation
+* Update TOX\_CONSTRAINTS\_FILE for stable/yoga
+* Update .gitreview for stable/yoga
+
+9.0.0
+-----
 
 * Display Draining state correctly
 * setup.cfg: Replace dashes by underscores
 * Updating python testing classifier as per Yoga testing runtime
 * Fix invalid value range for member weight
 * Add Python3 yoga unit tests
 * Update master for stable/xena
```

### Comparing `octavia-dashboard-9.0.0.0rc1/LICENSE` & `octavia-dashboard-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/PKG-INFO` & `octavia-dashboard-9.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: octavia-dashboard
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: Horizon panels for Octavia
 Home-page: https://docs.openstack.org/octavia-dashboard/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =================
         Octavia Dashboard
```

### Comparing `octavia-dashboard-9.0.0.0rc1/README.rst` & `octavia-dashboard-9.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/devstack/README.rst` & `octavia-dashboard-9.0.1/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/devstack/plugin.sh` & `octavia-dashboard-9.0.1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/doc/source/conf.py` & `octavia-dashboard-9.0.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/doc/source/installation.rst` & `octavia-dashboard-9.0.1/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/manage.py` & `octavia-dashboard-9.0.1/manage.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/__init__.py` & `octavia-dashboard-9.0.1/octavia_dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/api/rest/__init__.py` & `octavia-dashboard-9.0.1/octavia_dashboard/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/api/rest/barbican.py` & `octavia-dashboard-9.0.1/octavia_dashboard/api/rest/barbican.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/api/rest/lbaasv2.py` & `octavia-dashboard-9.0.1/octavia_dashboard/api/rest/lbaasv2.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,27 +627,35 @@
 
 def update_monitor(request, **kwargs):
     """Update a health monitor.
 
     """
     data = request.DATA
     monitor_id = data['monitor']['id']
+    hm_type = data['monitor']['type']
 
     conn = _get_sdk_connection(request)
+    healthmonitor_kwargs = {
+        'delay': data['monitor'].get('delay'),
+        'timeout': data['monitor'].get('timeout'),
+        'max_retries': data['monitor'].get('max_retries'),
+        'max_retries_down': data['monitor'].get('max_retries_down'),
+        'admin_state_up': data['monitor'].get('admin_state_up'),
+        'name': data['monitor'].get('name')
+    }
+    if hm_type in ('HTTP', 'HTTPS'):
+        healthmonitor_kwargs.update({
+            'http_method': data['monitor'].get('http_method'),
+            'url_path': data['monitor'].get('url_path'),
+            'expected_codes': data['monitor'].get('expected_codes')
+            })
+
     healthmonitor = conn.load_balancer.update_health_monitor(
         monitor_id,
-        delay=data['monitor'].get('delay'),
-        timeout=data['monitor'].get('timeout'),
-        max_retries=data['monitor'].get('max_retries'),
-        max_retries_down=data['monitor'].get('max_retries_down'),
-        http_method=data['monitor'].get('http_method'),
-        url_path=data['monitor'].get('url_path'),
-        expected_codes=data['monitor'].get('expected_codes'),
-        admin_state_up=data['monitor'].get('admin_state_up'),
-        name=data['monitor'].get('name')
+        **healthmonitor_kwargs
     )
 
     return _get_sdk_object_dict(healthmonitor)
 
 
 def update_flavor(request, **kwargs):
     """Update a flavor.
```

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/project/load_balancer/__init__.py` & `octavia-dashboard-9.0.1/octavia_dashboard/dashboards/project/load_balancer/__init__.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/project/load_balancer/panel.py` & `octavia-dashboard-9.0.1/octavia_dashboard/dashboards/project/load_balancer/panel.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/project/load_balancer/urls.py` & `octavia-dashboard-9.0.1/octavia_dashboard/dashboards/project/load_balancer/urls.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/dashboards/project/load_balancer/views.py` & `octavia-dashboard-9.0.1/octavia_dashboard/dashboards/project/load_balancer/views.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/enabled/_1482_project_load_balancer_panel.py` & `octavia-dashboard-9.0.1/octavia_dashboard/enabled/_1482_project_load_balancer_panel.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/karma.conf.js` & `octavia-dashboard-9.0.1/octavia_dashboard/karma.conf.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/local_settings.d/_1499_load_balancer_settings.py` & `octavia-dashboard-9.0.1/octavia_dashboard/local_settings.d/_1499_load_balancer_settings.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/de/LC_MESSAGES/django.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/de/LC_MESSAGES/djangojs.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/en_AU/LC_MESSAGES/django.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/en_AU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/en_GB/LC_MESSAGES/django.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/en_GB/LC_MESSAGES/djangojs.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/en_GB/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/es/LC_MESSAGES/django.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/fr/LC_MESSAGES/django.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/id/LC_MESSAGES/django.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/id/LC_MESSAGES/djangojs.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/id/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ja/LC_MESSAGES/django.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ja/LC_MESSAGES/djangojs.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/ja/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ko_KR/LC_MESSAGES/django.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ko_KR/LC_MESSAGES/djangojs.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/ko_KR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/pt_BR/LC_MESSAGES/django.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ru/LC_MESSAGES/django.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/ru/LC_MESSAGES/djangojs.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/zh_Hans/LC_MESSAGES/django.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/zh_Hans/LC_MESSAGES/djangojs.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/zh_Hans/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/zh_Hant/LC_MESSAGES/django.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/locale/zh_Hant/LC_MESSAGES/djangojs.po` & `octavia-dashboard-9.0.1/octavia_dashboard/locale/zh_Hant/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/app/core/openstack-service-api/lbaasv2.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/app/core/openstack-service-api/lbaasv2.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/app/core/openstack-service-api/lbaasv2.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/app/core/openstack-service-api/lbaasv2.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/app/core/openstack-service-api/octavia-barbican.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/app/core/openstack-service-api/octavia-barbican.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/app/core/openstack-service-api/octavia-barbican.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/app/core/openstack-service-api/octavia-barbican.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/create.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/create.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/create.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/create.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/wizard.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/wizard.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/wizard.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/create/wizard.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/delete/delete.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/delete/delete.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/delete/delete.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/delete/delete.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/edit.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/edit.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/edit.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/edit.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/wizard.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/wizard.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/wizard.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/actions/edit/wizard.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/detail.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/detail.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/detail.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/detail.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/detail.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/details/detail.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/healthmonitors.module.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/healthmonitors.module.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/healthmonitors.module.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/healthmonitors/healthmonitors.module.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/create.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/create.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/create.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/create.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/wizard.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/wizard.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/wizard.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/create/wizard.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/delete/delete.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/delete/delete.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/delete/delete.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/delete/delete.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/edit.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/edit.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/edit.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/edit.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/wizard.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/wizard.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/wizard.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/actions/edit/wizard.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/detail.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/detail.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/detail.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/detail.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/detail.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/details/detail.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/l7policies.module.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/l7policies.module.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/l7policies.module.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7policies/l7policies.module.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/create.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/create.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/create.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/create.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/wizard.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/wizard.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/wizard.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/create/wizard.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/delete/delete.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/delete/delete.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/delete/delete.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/delete/delete.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/edit.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/edit.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/edit.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/edit.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/wizard.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/wizard.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/wizard.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/actions/edit/wizard.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/detail.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/detail.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/detail.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/detail.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/detail.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/details/detail.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/l7rules.module.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/l7rules.module.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/l7rules.module.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/l7rules/l7rules.module.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/lbaasv2.module.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/lbaasv2.module.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/lbaasv2.module.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/lbaasv2.module.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/lbaasv2.scss` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/lbaasv2.scss`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/create.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/create.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/create.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/create.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/wizard.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/wizard.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/wizard.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/create/wizard.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/delete/delete.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/delete/delete.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/delete/delete.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/delete/delete.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/edit.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/edit.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/edit.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/edit.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/wizard.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/wizard.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/wizard.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/actions/edit/wizard.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/detail.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/detail.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/detail.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/detail.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/detail.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/details/detail.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/listeners.module.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/listeners.module.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/listeners.module.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/listeners/listeners.module.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/associate-ip/modal.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/create.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/create.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/create.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/create.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/wizard.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/wizard.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/wizard.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/create/wizard.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/delete/delete.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/delete/delete.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/delete/delete.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/delete/delete.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/disassociate-ip/modal.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/disassociate-ip/modal.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/disassociate-ip/modal.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/disassociate-ip/modal.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/edit.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/edit.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/edit.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/edit.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/wizard.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/wizard.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/wizard.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/actions/edit/wizard.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/detail.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/detail.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/detail.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/detail.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/detail.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/details/detail.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.module.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.module.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.module.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.module.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/loadbalancers.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/panel.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/panel.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/panel.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/panel.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/panel.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/loadbalancers/panel.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/delete/delete.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/delete/delete.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/delete/delete.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/delete/delete.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/edit-member/modal.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/update-member-list.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/update-member-list.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/update-member-list.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/update-member-list.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/wizard.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/wizard.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/wizard.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/actions/update-list/wizard.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/detail.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/detail.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/detail.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/detail.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/detail.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/details/detail.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/members.module.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/members.module.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/members/members.module.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/members/members.module.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/create.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/create.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/create.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/create.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/wizard.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/wizard.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/wizard.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/create/wizard.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/delete/delete.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/delete/delete.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/delete/delete.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/delete/delete.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/edit.action.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/edit.action.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/edit.action.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/edit.action.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/wizard.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/wizard.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/wizard.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/actions/edit/wizard.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/detail.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/detail.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/detail.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/detail.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/detail.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/details/detail.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/pools.module.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/pools.module.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/pools.module.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/pools/pools.module.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/util/validators/validate-unique.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/util/validators/validate-unique.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/util/validators/validate-unique.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/util/validators/validate-unique.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/filterselect/filter-select.component.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/filterselect/filter-select.component.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -130,14 +130,16 @@
         ctrl.textFilter = '';
         // Model for the filtering text input
         ctrl.text = '';
         // Model for the dropdown
         ctrl.isOpen = false;
         // Arrays of text to be displayed
         ctrl.rows = [];
+        // Array of non-rendered options after filter apply
+        ctrl.filtered_options = [];
 
         // Lifecycle methods
         ctrl.$onInit = function() {
             $document.on('click', ctrl.externalClick);
             ctrl.loaded = ctrl._setValue(ctrl.loaded, true);
             ctrl.disabled = ctrl._setValue(ctrl.disabled, false);
         };
@@ -180,15 +182,15 @@
 
         ctrl.openPopup = function(event) {
             event.stopPropagation();
             ctrl.isOpen = true;
         };
 
         ctrl.selectOption = function(index) {
-            var option = ctrl.options[index];
+            var option = ctrl.filtered_options[index];
             ctrl.onSelect({
                 option: option
             });
             ctrl.isOpen = false;
         };
 
         // Internal/Helper methods
@@ -214,19 +216,21 @@
                 return row;
             } else {
                 return null;
             }
         };
 
         ctrl._buildRows = function() {
+            ctrl.filtered_options.length = 0;
             ctrl.rows.length = 0;
             angular.forEach(ctrl.options, function(option) {
                 var row = ctrl._buildRow(option);
                 if (row) {
                     ctrl.rows.push(row);
+                    ctrl.filtered_options.push(option);
                 }
             });
         };
 
         ctrl._splitByFilter = function(text) {
             var split = {
                 values: [text, "", ""],
```

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/filterselect/filter-select.component.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/filterselect/filter-select.component.spec.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -193,14 +193,27 @@
             it('should select options', function() {
                 ctrl.selectOption(1);
                 expect(ctrl.onSelect).toHaveBeenCalledWith({
                     option: mockOptions[1]
                 });
                 expect(ctrl.isOpen).toBe(false);
             });
+
+            it('should select correct option after filter input', function() {
+                var mockInput = '2';
+                ctrl.text = mockInput;
+                ctrl.onTextChange();
+                ctrl.selectOption(0);
+                expect(ctrl.onSelect).toHaveBeenCalledWith({
+                    option: mockOptions[1]
+                });
+                expect(ctrl.filtered_options.length).toBe(1);
+                expect(ctrl.filtered_options[0].text).toContain(mockInput);
+                expect(ctrl.isOpen).toBe(false);
+            });
         });
 
         describe('controller', function() {
             var scope, ctrl;
 
             beforeEach(module('horizon.dashboard.project.lbaasv2'));
             beforeEach(
```

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/filterselect/filter-select.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/filterselect/filter-select.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/table/table-status.directive.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/table/table-status.directive.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/table/table-status.directive.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/table/table-status.directive.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/table/table-status.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/widgets/table/table-status.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.help.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.help.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/certificates/certificates.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.help.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.help.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7policy/l7policy.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7rule/l7rule.help.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7rule/l7rule.help.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7rule/l7rule.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/l7rule/l7rule.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.help.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.help.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/listener/listener.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.help.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.help.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/loadbalancer/loadbalancer.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.help.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.help.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/members/members.html`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                    class="form-group required member-address"
                    ng-class="{ 'has-error': memberDetailsForm['{$ ::row.id $}-address'].$invalid && memberDetailsForm['{$ ::row.id $}-address'].$dirty }">
                 <input name="{$ ::row.id $}-address" type="text" class="form-control"
                        ng-model="row.address" ng-pattern="::ctrl.ipPattern"
                        ng-required="true" ng-disabled="row.allocatedMember"
                        popover-placement="top" popover-append-to-body="true"
                        popover-trigger="focus"
-                       ng-attr-popover="{$ memberDetailsForm[row.id + '-address'].$invalid && memberDetailsForm[row.id + '-address'].$dirty ? ctrl.ipError : '' $}">
+                       uib-popover="{$ memberDetailsForm[row.id + '-address'].$invalid && memberDetailsForm[row.id + '-address'].$dirty ? ctrl.ipError : '' $}">
               </div>
               <span ng-if="row.addresses.length === 1">{$ row.address.ip $}</span>
               <div ng-if="row.addresses.length > 1"
                    class="form-group required member-address">
                 <select class="form-control input-sm"
                         ng-options="addr.ip for addr in row.addresses"
                         ng-model="row.address" ng-required="true" ng-if="row.addresses">
@@ -79,26 +79,26 @@
               <div class="form-group required member-port"
                    ng-class="{ 'has-error': memberDetailsForm['{$ ::row.id $}-port'].$invalid && memberDetailsForm['{$ ::row.id $}-port'].$dirty }">
                 <input name="{$ ::row.id $}-port" type="number" class="form-control"
                        ng-model="row.protocol_port" ng-pattern="/^\d+$/" min="1" max="65535"
                        ng-required="true" ng-disabled="row.allocatedMember"
                        popover-placement="top" popover-append-to-body="true"
                        popover-trigger="focus"
-                       ng-attr-popover="{$ memberDetailsForm[row.id + '-port'].$invalid && memberDetailsForm[row.id + '-port'].$dirty ? ctrl.portError : '' $}">
+                       uib-popover="{$ memberDetailsForm[row.id + '-port'].$invalid && memberDetailsForm[row.id + '-port'].$dirty ? ctrl.portError : '' $}">
               </div>
             </td>
             <td class="rsp-p1">
               <div class="form-group member-weight"
                    ng-class="{ 'has-error': memberDetailsForm['{$ ::row.id $}-weight'].$invalid && memberDetailsForm['{$ ::row.id $}-weight'].$dirty }">
                 <input name="{$ ::row.id $}-weight" type="number" class="form-control"
                        ng-model="row.weight" ng-pattern="/^\d+$/" min="0" max="256"
                        ng-disabled="row.allocatedMember"
                        popover-placement="top" popover-append-to-body="true"
                        popover-trigger="focus"
-                       ng-attr-popover="{$ memberDetailsForm[row.id + '-weight'].$invalid && memberDetailsForm[row.id + '-weight'].$dirty ? ctrl.weightError : '' $}">
+                       uib-popover="{$ memberDetailsForm[row.id + '-weight'].$invalid && memberDetailsForm[row.id + '-weight'].$dirty ? ctrl.weightError : '' $}">
               </div>
             </td>
             <td class="actions_column">
               <action-list>
                 <action action-classes="'btn btn-sm btn-default'"
                         callback="ctrl.deallocateMember" item="row">
                   <span translate>Remove</span>
@@ -122,27 +122,27 @@
                     class="form-group member-monitor-address"
                     ng-class="{ 'has-error': memberDetailsForm['{$ ::row.id $}-monitor-address'].$invalid && memberDetailsForm['{$ ::row.id $}-monitor-address'].$dirty }">
                     <input name="{$ ::row.id $}-monitor-address" type="text" class="form-control"
                                                                              ng-model="row.monitor_address" ng-pattern="::ctrl.ipPattern"
                                                                                                             ng-disabled="row.allocatedMember"
                                                                                                             popover-placement="top" popover-append-to-body="true"
                                                                                                                                     popover-trigger="focus"
-                                                                                                                                    ng-attr-popover="{$ memberDetailsForm[row.id + '-monitor-address'].$invalid && memberDetailsForm[row.id + '-monitor-address'].$dirty ? ctrl.ipError : '' $}">
+                                                                                                                                    uib-popover="{$ memberDetailsForm[row.id + '-monitor-address'].$invalid && memberDetailsForm[row.id + '-monitor-address'].$dirty ? ctrl.ipError : '' $}">
                   </dd>
                 </dl>
                 <dl class="col-lg-5 col-md-5 col-sm-5">
                   <dt translate>Monitor Port</dt>
                   <dd class="form-group member-monitor-port"
                        ng-class="{ 'has-error': memberDetailsForm['{$ ::row.id $}-monitor-port'].$invalid && memberDetailsForm['{$ ::row.id $}-monitor-port'].$dirty }">
                     <input name="{$ ::row.id $}-monitor-port" type="number" class="form-control"
                                                                             ng-model="row.monitor_port" ng-pattern="/^\d+$/" min="1" max="65535"
                                                                                                                                      ng-disabled="row.allocatedMember"
                                                                                                                                      popover-placement="top" popover-append-to-body="true"
                                                                                                                                                              popover-trigger="focus"
-                                                                                                                                                             ng-attr-popover="{$ memberDetailsForm[row.id + '-monitor-port'].$invalid && memberDetailsForm[row.id + '-monitor-port'].$dirty ? ctrl.portError : '' $}">
+                                                                                                                                                             uib-popover="{$ memberDetailsForm[row.id + '-monitor-port'].$invalid && memberDetailsForm[row.id + '-monitor-port'].$dirty ? ctrl.portError : '' $}">
                   </dd>
                 </dl>
                 <dl class="col-lg-5 col-md-5 col-sm-5">
                   <dt class="control-label required" translate>Admin State Up</dt>
                   <dd class="form-group">
                   <div class="form-field">
                     <div class="btn-group">
```

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/modal.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/modal.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/modal.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/modal.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/model.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/model.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/model.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/model.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.help.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.help.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/monitor/monitor.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.controller.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.controller.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.controller.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.controller.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.help.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.help.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.html` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/pool/pool.html`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/workflow.service.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/workflow.service.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/workflow.service.spec.js` & `octavia-dashboard-9.0.1/octavia_dashboard/static/dashboard/project/lbaasv2/workflow/workflow.service.spec.js`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/tests/settings.py` & `octavia-dashboard-9.0.1/octavia_dashboard/tests/settings.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/tests/unit/registration.py` & `octavia-dashboard-9.0.1/octavia_dashboard/tests/unit/registration.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/tests/urls.py` & `octavia-dashboard-9.0.1/octavia_dashboard/tests/urls.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard/version.py` & `octavia-dashboard-9.0.1/octavia_dashboard/version.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard.egg-info/PKG-INFO` & `octavia-dashboard-9.0.1/octavia_dashboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: octavia-dashboard
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: Horizon panels for Octavia
 Home-page: https://docs.openstack.org/octavia-dashboard/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =================
         Octavia Dashboard
```

### Comparing `octavia-dashboard-9.0.0.0rc1/octavia_dashboard.egg-info/SOURCES.txt` & `octavia-dashboard-9.0.1/octavia_dashboard.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 ChangeLog
 HACKING.rst
 LICENSE
 README.rst
 babel-django.cfg
 babel-djangojs.cfg
 bindep.txt
-lower-constraints.txt
 manage.py
 package-lock.json
 package.json
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
@@ -276,16 +275,18 @@
 releasenotes/notes/auto-refresh-detail-pages-26166d5d9c26edee.yaml
 releasenotes/notes/bp-horizon-lbaas-v2-ui-ba7e4c97a0460f85.yaml
 releasenotes/notes/cascade-delete-e4c9d80a31076540.yaml
 releasenotes/notes/drop-py-2-7-f3372b5c26171513.yaml
 releasenotes/notes/edit-default-pool-on-listener-206d8dfeea135360.yaml
 releasenotes/notes/filter-select-65160dcbe699a96d.yaml
 releasenotes/notes/fix-auth-url-barbican-client-d41b03419fb31ba4.yaml
+releasenotes/notes/fix-chrome-member-dialog-154981a7794d5fb4.yaml
 releasenotes/notes/fix-flavor-no-flavor-profile-c3e82325f16d5ab8.yaml
 releasenotes/notes/fix-member-weight-value-range-9310678f967c771a.yaml
+releasenotes/notes/fix-updating-non-http-hm-114180139961e441.yaml
 releasenotes/notes/flavor-support-0195a486faa16b7f.yaml
 releasenotes/notes/initial-octavia-dashboard-35d1d7f923473f21.yaml
 releasenotes/notes/list-pools-on-lb-details-page-eb0400bdb2b3650f.yaml
 releasenotes/notes/pool-selection-hint-7f282ba1fa014d8c.yaml
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/queens.rst
```

### Comparing `octavia-dashboard-9.0.0.0rc1/package-lock.json` & `octavia-dashboard-9.0.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/package.json` & `octavia-dashboard-9.0.1/package.json`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/releasenotes/notes/add-RBAC-43ee180e712294ed.yaml` & `octavia-dashboard-9.0.1/releasenotes/notes/add-RBAC-43ee180e712294ed.yaml`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/releasenotes/notes/bp-horizon-lbaas-v2-ui-ba7e4c97a0460f85.yaml` & `octavia-dashboard-9.0.1/releasenotes/notes/bp-horizon-lbaas-v2-ui-ba7e4c97a0460f85.yaml`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/releasenotes/notes/initial-octavia-dashboard-35d1d7f923473f21.yaml` & `octavia-dashboard-9.0.1/releasenotes/notes/initial-octavia-dashboard-35d1d7f923473f21.yaml`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/releasenotes/source/conf.py` & `octavia-dashboard-9.0.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/releasenotes/source/index.rst` & `octavia-dashboard-9.0.1/releasenotes/source/index.rst`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `octavia-dashboard-9.0.1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `octavia-dashboard-9.0.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po` & `octavia-dashboard-9.0.1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `octavia-dashboard-9.0.1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po` & `octavia-dashboard-9.0.1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_TW/LC_MESSAGES/releasenotes.po` & `octavia-dashboard-9.0.1/releasenotes/source/locale/zh_TW/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/setup.cfg` & `octavia-dashboard-9.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/setup.py` & `octavia-dashboard-9.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `octavia-dashboard-9.0.0.0rc1/tox.ini` & `octavia-dashboard-9.0.1/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [testenv]
 basepython = python3
 usedevelop = True
 setenv =
    VIRTUAL_ENV={envdir}
    CLIENT_NAME=octavia-dashboard
    DJANGO_SETTINGS_MODULE=octavia_dashboard.tests.settings
-deps = -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+deps = -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/yoga}
        -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 whitelist_externals = npm
                       bash
 commands =
    python manage.py test octavia_dashboard --settings=octavia_dashboard.tests.settings
 
@@ -30,15 +30,15 @@
 # sudo yum install npm (on RHEL/CentOS, enable EPEL repository)
 commands = npm install
            npm test
 
 [testenv:docs]
 whitelist_externals = rm
 deps =
-    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/yoga}
     -r{toxinidir}/requirements.txt
     -r{toxinidir}/doc/requirements.txt
 commands =
   rm -rf doc/build/html
   sphinx-build -W -b html doc/source doc/build/html
 
 [testenv:pdf-docs]
@@ -78,13 +78,7 @@
 # F405 TEMPLATES may be undefined, or defined from star imports
 # W504 line break after binary operator
 # (because it is not easy to avoid this in openstack_dashboard.test.settings)
 show-source = True
 ignore = E123,E125,F405,W504
 builtins = _
 exclude=.venv,.git,.tox,.tmp,dist,doc,*lib/python*,*egg,build,node_modules
-
-[testenv:lower-constraints]
-deps =
-  -c{toxinidir}/lower-constraints.txt
-  -r{toxinidir}/test-requirements.txt
-  -r{toxinidir}/requirements.txt
```

