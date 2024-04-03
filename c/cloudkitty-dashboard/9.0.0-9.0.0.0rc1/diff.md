# Comparing `tmp/cloudkitty-dashboard-9.0.0.tar.gz` & `tmp/cloudkitty-dashboard-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudkitty-dashboard-9.0.0.tar", last modified: Wed Oct 16 12:37:25 2019, max compression
+gzip compressed data, was "dist/cloudkitty-dashboard-9.0.0.0rc1.tar", last modified: Wed Sep 25 09:04:48 2019, max compression
```

## Comparing `cloudkitty-dashboard-9.0.0.tar` & `cloudkitty-dashboard-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2705 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/.stestr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/doc/source/readme.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8939 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2019-10-16 12:36:00.000000 cloudkitty-dashboard-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/babel-django.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/babel-djangojs.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/static/cloudkitty/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/static/cloudkitty/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/static/cloudkitty/templates/cloudkitty-help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/static/cloudkitty/templates/cloudkitty-step.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/static/cloudkitty/js/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5137 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/static/cloudkitty/js/pricing.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1558 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/static/cloudkitty/js/cloudkitty.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/static/cloudkitty/js/cloudkitty.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/static/cloudkitty/js/cloudkitty.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9413 2019-10-16 12:36:00.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/locale/en_GB/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8761 2019-10-16 12:36:00.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1374 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/overrides.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/templates/rating/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/templates/rating/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/templates/rating/_launch_details_price.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2650 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/reporting/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/reporting/urls.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/reporting/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/reporting/templates/reporting/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/reporting/templates/reporting/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4555 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/reporting/templates/reporting/this_month.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      879 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/reporting/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3397 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/reporting/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/reporting/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3493 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/templates/rating_modules/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/templates/rating_modules/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/templates/rating_modules/_priority_edit.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/templates/rating_modules/priority_edit.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/templates/rating_modules/details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3143 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1427 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/forms.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/summary/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/summary/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1583 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/summary/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/summary/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/summary/templates/rating_summary/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/summary/templates/rating_summary/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/summary/templates/rating_summary/details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/summary/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2628 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/summary/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/summary/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2757 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17099 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/_service_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3461 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/group_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/_group_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/services_list.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/group_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/_mapping_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/_field_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/mapping_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/service_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/threshold_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/service_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/field_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/field_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/_threshold_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16354 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12171 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/forms.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2668 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/templates/pyscripts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/templates/pyscripts/pyscripts_list.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/templates/pyscripts/_form.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/templates/pyscripts/form.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/templates/pyscripts/details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3445 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4913 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2100 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/api/cloudkitty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2994 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/tests/test_predictive_pricing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/tests/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/tests/test_cloudkittydashboard.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_12_project_reporting_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_11_admin_hashmap_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_10_admin_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_13_admin_pyscripts_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_11_project_rating_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_11_admin_rating_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_10_project_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_11_admin_summary_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_31000_cloudkitty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2019-10-16 12:36:00.000000 cloudkitty-dashboard-9.0.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkitty_dashboard.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2705 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkitty_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7220 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkitty_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkitty_dashboard.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkitty_dashboard.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkitty_dashboard.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkitty_dashboard.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/cloudkitty_dashboard.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1028 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1646 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5210 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/ChangeLog
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8513 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2444 2019-10-16 12:36:00.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2019-10-16 12:36:00.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/queens.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2019-10-16 12:36:00.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/releasenotes/source/stein.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:37:25.000000 cloudkitty-dashboard-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/releasenotes/notes/improve-total-tab-96df42d1e562fc4f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/releasenotes/notes/rework-reporting-tab-99cd8a8574911e09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2019-10-16 12:35:56.000000 cloudkitty-dashboard-9.0.0/releasenotes/notes/update-predictive-pricing-dc97030d8898af0d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/babel-djangojs.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/PKG-INFO
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/static/cloudkitty/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/static/cloudkitty/js/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/static/cloudkitty/js/cloudkitty.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/static/cloudkitty/js/cloudkitty.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1558 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/static/cloudkitty/js/cloudkitty.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5137 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/static/cloudkitty/js/pricing.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/static/cloudkitty/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/static/cloudkitty/templates/cloudkitty-step.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/static/cloudkitty/templates/cloudkitty-help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2100 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/api/cloudkitty.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/tests/test_cloudkittydashboard.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2994 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/tests/test_predictive_pricing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/tests/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9413 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/locale/en_GB/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8761 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/reporting/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/reporting/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/reporting/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/reporting/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/reporting/templates/reporting/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4555 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/reporting/templates/reporting/this_month.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/reporting/templates/reporting/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3397 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/reporting/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      879 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/reporting/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/templates/rating/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/templates/rating/_launch_details_price.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/templates/rating/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2650 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/templates/pyscripts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/templates/pyscripts/pyscripts_list.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/templates/pyscripts/form.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/templates/pyscripts/_form.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/templates/pyscripts/details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3445 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4913 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2668 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/templates/rating_modules/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/templates/rating_modules/_priority_edit.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/templates/rating_modules/priority_edit.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/templates/rating_modules/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/templates/rating_modules/details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3143 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1427 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3493 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2757 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/group_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/field_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3461 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/group_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/mapping_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/service_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/service_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/_threshold_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/threshold_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/_service_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/field_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/_field_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/services_list.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/_group_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/_mapping_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16354 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12171 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17099 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/summary/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/summary/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/summary/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/summary/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/summary/templates/rating_summary/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/summary/templates/rating_summary/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/summary/templates/rating_summary/details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2628 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/summary/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1583 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/summary/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/summary/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1374 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/overrides.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_12_project_reporting_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_11_admin_hashmap_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_11_admin_summary_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_11_admin_rating_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_31000_cloudkitty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_13_admin_pyscripts_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_10_project_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_10_admin_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_11_project_rating_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1028 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/setup.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8939 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkitty_dashboard.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkitty_dashboard.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkitty_dashboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkitty_dashboard.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkitty_dashboard.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkitty_dashboard.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7220 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkitty_dashboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/cloudkitty_dashboard.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/.zuul.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/notes/rework-reporting-tab-99cd8a8574911e09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/notes/update-predictive-pricing-dc97030d8898af0d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/notes/improve-total-tab-96df42d1e562fc4f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/notes/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8513 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/ocata.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2444 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1302 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/stein.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/_static/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1646 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5220 2019-09-25 09:04:48.000000 cloudkitty-dashboard-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/babel-django.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2019-09-25 09:03:57.000000 cloudkitty-dashboard-9.0.0.0rc1/HACKING.rst
```

### Comparing `cloudkitty-dashboard-9.0.0/PKG-INFO` & `cloudkitty-dashboard-9.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudkitty-dashboard
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: CloudKitty Horizon dashboard
 Home-page: https://docs.openstack.org/cloudkitty-dashboard/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `cloudkitty-dashboard-9.0.0/README.rst` & `cloudkitty-dashboard-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/doc/source/conf.py` & `cloudkitty-dashboard-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/doc/source/installation.rst` & `cloudkitty-dashboard-9.0.0.0rc1/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/doc/source/index.rst` & `cloudkitty-dashboard-9.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/setup.cfg` & `cloudkitty-dashboard-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/babel-djangojs.cfg` & `cloudkitty-dashboard-9.0.0.0rc1/babel-djangojs.cfg`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/static/cloudkitty/js/pricing.js` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/static/cloudkitty/js/pricing.js`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/static/cloudkitty/js/cloudkitty.controller.js` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/static/cloudkitty/js/cloudkitty.controller.js`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/static/cloudkitty/js/cloudkitty.module.js` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/static/cloudkitty/js/cloudkitty.module.js`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/utils.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/utils.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/locale/en_GB/LC_MESSAGES/django.po` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/locale/fr/LC_MESSAGES/django.po` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/overrides.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/overrides.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/urls.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/urls.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/tables.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/tables.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/panel.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/panel.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/rating/views.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/rating/views.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/reporting/templates/reporting/this_month.html` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/reporting/templates/reporting/this_month.html`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/reporting/panel.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/reporting/panel.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/project/reporting/views.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/project/reporting/views.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/urls.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/urls.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/tables.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/tables.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/templates/rating_modules/details.html` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/templates/rating_modules/details.html`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/panel.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/panel.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/views.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/views.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/modules/forms.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/modules/forms.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/summary/urls.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/summary/urls.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/summary/tables.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/summary/tables.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/summary/panel.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/summary/panel.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/summary/views.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/summary/views.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/urls.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/urls.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/tables.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/tables.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/group_details.html` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/templates/hashmap/group_details.html`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/panel.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/panel.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/views.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/views.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/tests.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/tests.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/hashmap/forms.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/forms.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/urls.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/urls.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/tables.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/tables.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/templates/pyscripts/details.html` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/templates/pyscripts/details.html`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/panel.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/panel.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/views.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/views.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/tests.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/hashmap/tests.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/dashboards/admin/pyscripts/forms.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/dashboards/admin/pyscripts/forms.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/__init__.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/api/cloudkitty.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/api/cloudkitty.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/tests/test_predictive_pricing.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/tests/test_predictive_pricing.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/tests/base.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/tests/base.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/tests/test_utils.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/tests/test_cloudkittydashboard.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/tests/test_cloudkittydashboard.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_12_project_reporting_panel.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_12_project_reporting_panel.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_11_admin_hashmap_panel.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_11_admin_hashmap_panel.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_10_admin_group.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_10_admin_group.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_11_project_rating_panel.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_11_project_rating_panel.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_11_admin_rating_panel.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_11_admin_rating_panel.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_10_project_group.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_10_project_group.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkittydashboard/enabled/_11_admin_summary_panel.py` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkittydashboard/enabled/_11_admin_summary_panel.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/LICENSE` & `cloudkitty-dashboard-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/tox.ini` & `cloudkitty-dashboard-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/cloudkitty_dashboard.egg-info/PKG-INFO` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkitty_dashboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudkitty-dashboard
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: CloudKitty Horizon dashboard
 Home-page: https://docs.openstack.org/cloudkitty-dashboard/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `cloudkitty-dashboard-9.0.0/cloudkitty_dashboard.egg-info/SOURCES.txt` & `cloudkitty-dashboard-9.0.0.0rc1/cloudkitty_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/setup.py` & `cloudkitty-dashboard-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/AUTHORS` & `cloudkitty-dashboard-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/CONTRIBUTING.rst` & `cloudkitty-dashboard-9.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/ChangeLog` & `cloudkitty-dashboard-9.0.0.0rc1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * Generate PDF documentation
 * Add exception to error messages
 * Adapt TemplatizableDict to python3 hasattr
 * Bump openstackdocstheme to 1.30.0
 * Remove unncessary '=='
 * Modify the url of upper\_constraints\_file
```

### Comparing `cloudkitty-dashboard-9.0.0/releasenotes/source/conf.py` & `cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `cloudkitty-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `cloudkitty-dashboard-9.0.0/releasenotes/notes/improve-total-tab-96df42d1e562fc4f.yaml` & `cloudkitty-dashboard-9.0.0.0rc1/releasenotes/notes/improve-total-tab-96df42d1e562fc4f.yaml`

 * *Files identical despite different names*

