# Comparing `tmp/designate-dashboard-9.0.0.0rc1.tar.gz` & `tmp/designate-dashboard-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/designate-dashboard-9.0.0.0rc1.tar", last modified: Fri Sep 27 17:13:47 2019, max compression
+gzip compressed data, was "dist/designate-dashboard-9.0.1.tar", last modified: Thu Jun 18 17:09:32 2020, max compression
```

## Comparing `designate-dashboard-9.0.0.0rc1.tar` & `designate-dashboard-9.0.1.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3900 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2831 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/lower-constraints.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2430 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/package.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      576 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3198 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/test-shim.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2048 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/test
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/LICENSE
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/doc/source/readme.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2695 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/api/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/api/rest/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4015 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/api/rest/passthrough.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/api/rest/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/zh_CN/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ja/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ne/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ne/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ne/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ko_KR/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/cs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/cs/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/en_GB/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/tr_TR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/tr_TR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/locale/tr_TR/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/ngdns/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/ngdns/zones/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/ngdns/zones/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/ngdns/zones/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/ngdns/zones/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/ngdns/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/ngdns/reverse_dns/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/ngdns/reverse_dns/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/ngdns/reverse_dns/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/ngdns/reverse_dns/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/enabled/_1710_project_dns_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/enabled/_1721_dns_zones_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/enabled/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1347 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/enabled/_1722_dns_reversedns_panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4479 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/os-designate-floatingip.module.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1955 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/details/details.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/details/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/details/overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/details/overview.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3628 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/api.service.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1806 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/actions/actions.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4004 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/actions/unset.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4915 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/actions/set.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1227 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/resources.module.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7085 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/os-designate-recordset.module.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3246 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/details.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1191 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/zone-recordsets.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1403 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/overview.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/zone-recordsets.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4418 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/api.service.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2306 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/actions.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5798 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/delete.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4878 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/common-forms.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5139 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/update.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/create.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3319 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/util.service.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/details.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1756 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1574 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/overview.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4320 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/api.service.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2106 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/actions.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4953 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/delete.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1495 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/actions.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5452 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/common-forms.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4509 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/update.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3779 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/create.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5726 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/os-designate-zone.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2126 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/designatedashboard.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/designatedashboard.scss
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/zones.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/reverse_dns.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1373 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/tests/settings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/tests/.secret_key_store
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1928 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/designatedashboard/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/babel-django.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4734 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/karma.conf.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/openstack-common.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2104 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10131 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/ChangeLog
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designate_dashboard.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3900 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designate_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6639 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designate_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designate_dashboard.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designate_dashboard.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designate_dashboard.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designate_dashboard.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/designate_dashboard.egg-info/dependency_links.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/releasenotes/notes/removed-v1-dashboard-56d4697d57baef09.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1177 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8630 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2306 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2019-09-27 17:13:47.000000 designate-dashboard-9.0.0.0rc1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/setup.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      883 2019-09-27 17:12:36.000000 designate-dashboard-9.0.0.0rc1/manage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2103 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/releasenotes/source/unreleased.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1177 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8630 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/releasenotes/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/releasenotes/notes/removed-v1-dashboard-56d4697d57baef09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/openstack-common.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designate_dashboard.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6639 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designate_dashboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designate_dashboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designate_dashboard.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designate_dashboard.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3895 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designate_dashboard.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designate_dashboard.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designate_dashboard.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10265 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2344 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/HACKING.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      883 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      576 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/package.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/doc/source/readme.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/doc/source/index.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2695 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2831 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/lower-constraints.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3198 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/test-shim.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3895 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2048 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/test
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4734 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/karma.conf.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/babel-django.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/tests/.secret_key_store
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1928 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1373 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/tests/settings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/api/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/api/rest/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4015 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/api/rest/passthrough.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/api/rest/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/dashboards/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/dashboards/project/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/dashboards/project/ngdns/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/dashboards/project/ngdns/reverse_dns/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/dashboards/project/ngdns/reverse_dns/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/dashboards/project/ngdns/reverse_dns/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/dashboards/project/ngdns/reverse_dns/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/dashboards/project/ngdns/zones/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/dashboards/project/ngdns/zones/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/dashboards/project/ngdns/zones/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/dashboards/project/ngdns/zones/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/dashboards/project/ngdns/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/dashboards/project/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/dashboards/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/zones.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/reverse_dns.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/designatedashboard.scss
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2126 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/designatedashboard.module.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3319 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/util.service.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4320 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/api.service.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1756 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/details.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1574 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/overview.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/drawer.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3779 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/create.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1495 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/actions.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4509 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/update.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2106 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/actions.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4953 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/delete.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5452 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/common-forms.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5732 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/os-designate-zone.module.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4479 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/os-designate-floatingip.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3628 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/api.service.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/details/overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1955 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/details/details.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/details/overview.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/details/drawer.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4915 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/actions/set.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1806 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/actions/actions.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4004 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/actions/unset.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1227 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/resources.module.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7085 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/os-designate-recordset.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4418 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/api.service.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1403 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3246 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/details.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1191 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/zone-recordsets.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/zone-recordsets.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/overview.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/drawer.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/create.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5139 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/update.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2306 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/actions.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5798 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/delete.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4878 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/common-forms.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1347 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/enabled/_1722_dns_reversedns_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/enabled/_1721_dns_zones_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/enabled/_1710_project_dns_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/enabled/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/ne/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/ne/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/locale/ne/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/cs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/locale/zh_CN/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/locale/en_GB/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/tr_TR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/tr_TR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/locale/tr_TR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/locale/ko_KR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-18 17:09:32.000000 designate-dashboard-9.0.1/designatedashboard/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/designatedashboard/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2430 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2020-06-18 17:07:28.000000 designate-dashboard-9.0.1/LICENSE
```

### Comparing `designate-dashboard-9.0.0.0rc1/PKG-INFO` & `designate-dashboard-9.0.1/designate_dashboard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: designate-dashboard
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: Designate Horizon UI bits
 Home-page: https://docs.openstack.org/developer/designate-dashboard/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `designate-dashboard-9.0.0.0rc1/lower-constraints.txt` & `designate-dashboard-9.0.1/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/test-requirements.txt` & `designate-dashboard-9.0.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/README.rst` & `designate-dashboard-9.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/package.json` & `designate-dashboard-9.0.1/package.json`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/CONTRIBUTING.rst` & `designate-dashboard-9.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/test-shim.js` & `designate-dashboard-9.0.1/test-shim.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/test` & `designate-dashboard-9.0.1/test`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/LICENSE` & `designate-dashboard-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/doc/source/index.rst` & `designate-dashboard-9.0.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/doc/source/conf.py` & `designate-dashboard-9.0.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/api/rest/passthrough.py` & `designate-dashboard-9.0.1/designatedashboard/api/rest/passthrough.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/api/rest/__init__.py` & `designate-dashboard-9.0.1/designatedashboard/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/locale/zh_CN/LC_MESSAGES/django.po` & `designate-dashboard-9.0.1/designatedashboard/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ja/LC_MESSAGES/django.po` & `designate-dashboard-9.0.1/designatedashboard/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/locale/pt_BR/LC_MESSAGES/django.po` & `designate-dashboard-9.0.1/designatedashboard/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ne/LC_MESSAGES/django.po` & `designate-dashboard-9.0.1/designatedashboard/locale/ne/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ko_KR/LC_MESSAGES/django.po` & `designate-dashboard-9.0.1/designatedashboard/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/locale/cs/LC_MESSAGES/django.po` & `designate-dashboard-9.0.1/designatedashboard/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/locale/de/LC_MESSAGES/django.po` & `designate-dashboard-9.0.1/designatedashboard/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/locale/id/LC_MESSAGES/django.po` & `designate-dashboard-9.0.1/designatedashboard/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/locale/es/LC_MESSAGES/django.po` & `designate-dashboard-9.0.1/designatedashboard/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/locale/fr/LC_MESSAGES/django.po` & `designate-dashboard-9.0.1/designatedashboard/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/locale/en_GB/LC_MESSAGES/django.po` & `designate-dashboard-9.0.1/designatedashboard/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/locale/ru/LC_MESSAGES/django.po` & `designate-dashboard-9.0.1/designatedashboard/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/locale/tr_TR/LC_MESSAGES/django.po` & `designate-dashboard-9.0.1/designatedashboard/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/ngdns/zones/panel.py` & `designate-dashboard-9.0.1/designatedashboard/dashboards/project/ngdns/zones/panel.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/ngdns/zones/urls.py` & `designate-dashboard-9.0.1/designatedashboard/dashboards/project/ngdns/zones/urls.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/ngdns/reverse_dns/panel.py` & `designate-dashboard-9.0.1/designatedashboard/dashboards/project/ngdns/reverse_dns/panel.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/dashboards/project/ngdns/reverse_dns/urls.py` & `designate-dashboard-9.0.1/designatedashboard/dashboards/project/ngdns/reverse_dns/urls.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/exceptions.py` & `designate-dashboard-9.0.1/designatedashboard/exceptions.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/enabled/_1710_project_dns_panel_group.py` & `designate-dashboard-9.0.1/designatedashboard/enabled/_1710_project_dns_panel_group.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/enabled/_1721_dns_zones_panel.py` & `designate-dashboard-9.0.1/designatedashboard/enabled/_1721_dns_zones_panel.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/enabled/_1722_dns_reversedns_panel.py` & `designate-dashboard-9.0.1/designatedashboard/enabled/_1722_dns_reversedns_panel.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/os-designate-floatingip.module.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/os-designate-floatingip.module.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/details/details.module.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/details/details.module.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/details/overview.controller.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/details/overview.controller.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/api.service.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/api.service.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/actions/actions.module.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/actions/actions.module.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/actions/unset.service.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/actions/unset.service.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/actions/set.service.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-floatingip/actions/set.service.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/resources.module.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/resources.module.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/os-designate-recordset.module.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/os-designate-recordset.module.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/details.module.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/details.module.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/zone-recordsets.controller.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/zone-recordsets.controller.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/overview.html` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/overview.html`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/overview.controller.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/details/overview.controller.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/api.service.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/api.service.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/actions.module.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/actions.module.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/delete.service.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/delete.service.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/common-forms.service.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/common-forms.service.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/update.service.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/update.service.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/create.service.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-recordset/actions/create.service.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/util.service.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/util.service.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/details.module.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/details.module.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/overview.html` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/overview.html`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/overview.controller.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/details/overview.controller.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/api.service.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/api.service.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/actions.module.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/actions.module.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/delete.service.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/delete.service.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/actions.module.spec.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/actions.module.spec.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/common-forms.service.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/common-forms.service.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/update.service.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/update.service.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/create.service.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/actions/create.service.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/resources/os-designate-zone/os-designate-zone.module.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/resources/os-designate-zone/os-designate-zone.module.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -196,15 +196,15 @@
         }
 
         function listZones() {
             return zoneApi.list().then(function onList(response) {
                 // listFunctions are expected to return data in "items"
                 response.data.items = response.data.zones;
 
-                util.addTimestampIds(response.data.items, 'updated_at');
+                util.addTimestampIds(response.data.items, 'id', 'updated_at');
 
                 return response;
             });
         }
     }
 
 })();
```

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/static/designatedashboard/designatedashboard.module.js` & `designate-dashboard-9.0.1/designatedashboard/static/designatedashboard/designatedashboard.module.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/__init__.py` & `designate-dashboard-9.0.1/designatedashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/tests/settings.py` & `designate-dashboard-9.0.1/designatedashboard/tests/settings.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/designatedashboard/tests/base.py` & `designate-dashboard-9.0.1/designatedashboard/tests/base.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/karma.conf.js` & `designate-dashboard-9.0.1/karma.conf.js`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/tox.ini` & `designate-dashboard-9.0.1/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
          NOSE_OPENSTACK_COLOR=1
          NOSE_OPENSTACK_RED=0.05
          NOSE_OPENSTACK_YELLOW=0.025
          NOSE_OPENSTACK_SHOW_ELAPSED=1
          PYTHONDONTWRITEBYTECODE=1
          DJANGO_SETTINGS_MODULE=designatedashboard.settings
 whitelist_externals = find
-deps = -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+deps = -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/train}
        -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 
 commands =
     find . -type f -name "*.pyc" -delete
     {toxinidir}/manage.py test designatedashboard --settings=designatedashboard.tests.settings
 passenv = http_proxy HTTP_PROXY https_proxy HTTPS_PROXY no_proxy NO_PROXY
```

### Comparing `designate-dashboard-9.0.0.0rc1/ChangeLog` & `designate-dashboard-9.0.1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 CHANGES
 =======
 
-9.0.0.0rc1
-----------
+9.0.1
+-----
+
+* Fix list zones updated at same time
+* Update TOX/UPPER\_CONSTRAINTS\_FILE for stable/train
+* Update .gitreview for stable/train
+
+9.0.0
+-----
 
 * Imported Translations from Zanata
 * Update the constraints url
 * Cleanup release notes
 * Fix releasenotes index page
 * Swith nodejs10 jobs to voting
 * Add release-note-job to designate-dashboard
```

### Comparing `designate-dashboard-9.0.0.0rc1/designate_dashboard.egg-info/PKG-INFO` & `designate-dashboard-9.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: designate-dashboard
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: Designate Horizon UI bits
 Home-page: https://docs.openstack.org/developer/designate-dashboard/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `designate-dashboard-9.0.0.0rc1/designate_dashboard.egg-info/SOURCES.txt` & `designate-dashboard-9.0.1/designate_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `designate-dashboard-9.0.1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/releasenotes/source/conf.py` & `designate-dashboard-9.0.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/AUTHORS` & `designate-dashboard-9.0.1/AUTHORS`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 Erik Olof Gunnar Andersson <eandersson@blizzard.com>
 Federico Ceratto <federico.ceratto@hpe.com>
 Flavio Percoco <flaper87@gmail.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Graham Hayes <gr@ham.ie>
 Graham Hayes <graham.hayes@hp.com>
 Graham Hayes <graham.hayes@hpe.com>
+Ingo Fischer <i.fischer@syseleven.de>
 Ivan Kolodyazhny <e0ne@e0ne.info>
 James E. Blair <jeblair@redhat.com>
 Janonymous <janonymous.codevulture@gmail.com>
 Jens Harbott <j.harbott@x-ion.de>
 Jingjing Ren <jingjing_ren@symantec.com>
 Kiall Mac Innes <kiall@hp.com>
 Kiall Mac Innes <kiall@macinnes.ie>
```

### Comparing `designate-dashboard-9.0.0.0rc1/setup.cfg` & `designate-dashboard-9.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/setup.py` & `designate-dashboard-9.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `designate-dashboard-9.0.0.0rc1/manage.py` & `designate-dashboard-9.0.1/manage.py`

 * *Files identical despite different names*

