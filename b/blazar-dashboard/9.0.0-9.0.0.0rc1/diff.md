# Comparing `tmp/blazar-dashboard-9.0.0.tar.gz` & `tmp/blazar-dashboard-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blazar-dashboard-9.0.0.tar", last modified: Wed Mar 22 12:16:16 2023, max compression
+gzip compressed data, was "blazar-dashboard-9.0.0.0rc1.tar", last modified: Tue Feb 28 13:56:09 2023, max compression
```

## Comparing `blazar-dashboard-9.0.0.tar` & `blazar-dashboard-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.206073 blazar-dashboard-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1587 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/.eslintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1061 2023-03-22 12:16:16.000000 blazar-dashboard-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4444 2023-03-22 12:16:16.000000 blazar-dashboard-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2441 2023-03-22 12:16:16.206073 blazar-dashboard-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/babel-django.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/babel-djangojs.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.186072 blazar-dashboard-9.0.0/blazar_dashboard/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.190072 blazar-dashboard-9.0.0/blazar_dashboard/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6086 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/api/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      900 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.190072 blazar-dashboard-9.0.0/blazar_dashboard/content/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.190072 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2203 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2716 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1443 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.182072 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.194072 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/templates/hosts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1643 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/templates/hosts/_detail_overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/templates/hosts/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/templates/hosts/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/templates/hosts/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/templates/hosts/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/templates/hosts/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9196 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2965 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4900 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/workflows.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.194072 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12969 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3668 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1714 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.182072 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.198073 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/templates/leases/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/templates/leases/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2597 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/templates/leases/_detail_overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/templates/leases/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1738 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/templates/leases/calendar.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/templates/leases/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/templates/leases/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/templates/leases/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/templates/leases/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12026 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4243 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/content/leases/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.198073 blazar-dashboard-9.0.0/blazar_dashboard/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/enabled/_90_admin_reservation_panelgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/enabled/_90_project_reservations_panelgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/enabled/_91_admin_reservation_hosts_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/enabled/_91_project_reservations_leases_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/enabled/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.182072 blazar-dashboard-9.0.0/blazar_dashboard/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.182072 blazar-dashboard-9.0.0/blazar_dashboard/static/leases/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.182072 blazar-dashboard-9.0.0/blazar_dashboard/static/leases/js/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.198073 blazar-dashboard-9.0.0/blazar_dashboard/static/leases/js/calendar/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5511 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/static/leases/js/calendar/lease_chart.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.198073 blazar-dashboard-9.0.0/blazar_dashboard/static/leases/js/vendor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   487568 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/static/leases/js/vendor/apexcharts.min.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.198073 blazar-dashboard-9.0.0/blazar_dashboard/static/leases/scss/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/static/leases/scss/calendar.scss
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/static/leases/scss/widgets.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.198073 blazar-dashboard-9.0.0/blazar_dashboard/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/test/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1403 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/test/helpers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.198073 blazar-dashboard-9.0.0/blazar_dashboard/test/integration_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/test/integration_tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/test/settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.202072 blazar-dashboard-9.0.0/blazar_dashboard/test/test_data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/test/test_data/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6395 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/test/test_data/blazar_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1805 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/test/test_data/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1074 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/test/test_data/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/blazar_dashboard/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.190072 blazar-dashboard-9.0.0/blazar_dashboard.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2441 2023-03-22 12:16:16.000000 blazar-dashboard-9.0.0/blazar_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4052 2023-03-22 12:16:16.000000 blazar-dashboard-9.0.0/blazar_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-22 12:16:16.000000 blazar-dashboard-9.0.0/blazar_dashboard.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-22 12:16:16.000000 blazar-dashboard-9.0.0/blazar_dashboard.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-22 12:16:16.000000 blazar-dashboard-9.0.0/blazar_dashboard.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-03-22 12:16:16.000000 blazar-dashboard-9.0.0/blazar_dashboard.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2023-03-22 12:16:16.000000 blazar-dashboard-9.0.0/blazar_dashboard.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.202072 blazar-dashboard-9.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.202072 blazar-dashboard-9.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      977 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/doc/source/calendar.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6664 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.202072 blazar-dashboard-9.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2081 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/doc/source/install/install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      993 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/lower-constraints.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      832 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/manage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.182072 blazar-dashboard-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.202072 blazar-dashboard-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/notes/add-affinity-support-de4c63de74da29ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/notes/dashboard-support-1b429d36f395d93a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/notes/display-error-details-cfd47a4e0a03bc5c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/notes/drop-python2-8f624e1c157ac04a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/notes/host-calendar-2ecf4058929b269e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/notes/host-panel-00836b98ea5dc8d8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/notes/remove-use-of-eval-ef359dec791c97cd.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:16:16.206073 blazar-dashboard-9.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9066 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      927 2023-03-22 12:16:16.210073 blazar-dashboard-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2422 2023-03-22 12:15:49.000000 blazar-dashboard-9.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.504223 blazar-dashboard-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1587 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/.eslintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1061 2023-02-28 13:56:09.000000 blazar-dashboard-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4454 2023-02-28 13:56:09.000000 blazar-dashboard-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2446 2023-02-28 13:56:09.508224 blazar-dashboard-9.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/babel-django.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/babel-djangojs.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.488219 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.488219 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6086 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/api/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      900 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.488219 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.492220 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2203 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2716 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1443 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.480217 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.492220 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/templates/hosts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1643 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/templates/hosts/_detail_overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/templates/hosts/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/templates/hosts/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/templates/hosts/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/templates/hosts/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/templates/hosts/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9196 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2965 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4900 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/workflows.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.492220 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12969 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3668 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1714 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.480217 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.496221 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/templates/leases/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/templates/leases/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2597 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/templates/leases/_detail_overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/templates/leases/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1738 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/templates/leases/calendar.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/templates/leases/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/templates/leases/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/templates/leases/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/templates/leases/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12026 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4243 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.496221 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/enabled/_90_admin_reservation_panelgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/enabled/_90_project_reservations_panelgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/enabled/_91_admin_reservation_hosts_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/enabled/_91_project_reservations_leases_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/enabled/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.480217 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.480217 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/static/leases/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.480217 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/static/leases/js/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.496221 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/static/leases/js/calendar/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5511 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/static/leases/js/calendar/lease_chart.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.496221 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/static/leases/js/vendor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   487568 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/static/leases/js/vendor/apexcharts.min.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.500222 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/static/leases/scss/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/static/leases/scss/calendar.scss
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/static/leases/scss/widgets.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.500222 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1403 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.500222 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/integration_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/integration_tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.500222 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/test_data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/test_data/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6395 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/test_data/blazar_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1805 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/test_data/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1074 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/test_data/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.488219 blazar-dashboard-9.0.0.0rc1/blazar_dashboard.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2446 2023-02-28 13:56:09.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4052 2023-02-28 13:56:09.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-28 13:56:09.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-28 13:56:09.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-28 13:56:09.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-02-28 13:56:09.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2023-02-28 13:56:09.000000 blazar-dashboard-9.0.0.0rc1/blazar_dashboard.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.500222 blazar-dashboard-9.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.500222 blazar-dashboard-9.0.0.0rc1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      977 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/doc/source/calendar.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6664 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.500222 blazar-dashboard-9.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2081 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/doc/source/install/install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      993 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/lower-constraints.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      832 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/manage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.484218 blazar-dashboard-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.504223 blazar-dashboard-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/notes/add-affinity-support-de4c63de74da29ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/notes/dashboard-support-1b429d36f395d93a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/notes/display-error-details-cfd47a4e0a03bc5c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/notes/drop-python2-8f624e1c157ac04a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/notes/host-calendar-2ecf4058929b269e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/notes/host-panel-00836b98ea5dc8d8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/notes/remove-use-of-eval-ef359dec791c97cd.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:56:09.504223 blazar-dashboard-9.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9066 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      927 2023-02-28 13:56:09.508224 blazar-dashboard-9.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2422 2023-02-28 13:55:43.000000 blazar-dashboard-9.0.0.0rc1/tox.ini
```

### Comparing `blazar-dashboard-9.0.0/.eslintrc` & `blazar-dashboard-9.0.0.0rc1/.eslintrc`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/AUTHORS` & `blazar-dashboard-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/CONTRIBUTING.rst` & `blazar-dashboard-9.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/ChangeLog` & `blazar-dashboard-9.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * Update tox.ini for tox4
 * Ignore release note from yoga
 * Switch to 2023.1 Python3 unit tests and generic template name
 * Update master for stable/zed
 
 8.0.0
```

### Comparing `blazar-dashboard-9.0.0/LICENSE` & `blazar-dashboard-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/PKG-INFO` & `blazar-dashboard-9.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: blazar-dashboard
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Horizon plugin for the Blazar Reservation Service for OpenStack
 Home-page: https://docs.openstack.org/blazar-dashboard/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `blazar-dashboard-9.0.0/README.rst` & `blazar-dashboard-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/api/client.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/api/client.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/conf.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/conf.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/forms.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/forms.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/panel.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/panel.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/tables.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/tables.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/tabs.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/tabs.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/templates/hosts/_detail_overview.html` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/templates/hosts/_detail_overview.html`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/templates/hosts/_update.html` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/templates/hosts/_update.html`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/tests.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/tests.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/urls.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/urls.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/views.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/views.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/hosts/workflows.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/hosts/workflows.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/leases/forms.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/forms.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/leases/panel.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/panel.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/leases/tables.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/tables.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/leases/tabs.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/tabs.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/leases/templates/leases/_detail_overview.html` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/templates/leases/_detail_overview.html`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/leases/templates/leases/_update.html` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/templates/leases/_update.html`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/leases/templates/leases/calendar.html` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/templates/leases/calendar.html`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/leases/tests.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/tests.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/leases/urls.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/urls.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/content/leases/views.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/content/leases/views.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/enabled/_90_admin_reservation_panelgroup.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/enabled/_90_admin_reservation_panelgroup.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/enabled/_90_project_reservations_panelgroup.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/enabled/_90_project_reservations_panelgroup.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/enabled/_91_admin_reservation_hosts_panel.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/enabled/_91_admin_reservation_hosts_panel.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/enabled/_91_project_reservations_leases_panel.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/enabled/_91_project_reservations_leases_panel.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/static/leases/js/calendar/lease_chart.js` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/static/leases/js/calendar/lease_chart.js`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/static/leases/js/vendor/apexcharts.min.js` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/static/leases/js/vendor/apexcharts.min.js`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/static/leases/scss/calendar.scss` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/static/leases/scss/calendar.scss`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/test/helpers.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/helpers.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/test/settings.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/settings.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/test/test_data/blazar_data.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/test_data/blazar_data.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/test/test_data/exceptions.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/test_data/exceptions.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/test/test_data/utils.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/test/test_data/utils.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard/version.py` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard/version.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard.egg-info/PKG-INFO` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: blazar-dashboard
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Horizon plugin for the Blazar Reservation Service for OpenStack
 Home-page: https://docs.openstack.org/blazar-dashboard/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `blazar-dashboard-9.0.0/blazar_dashboard.egg-info/SOURCES.txt` & `blazar-dashboard-9.0.0.0rc1/blazar_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/doc/source/calendar.rst` & `blazar-dashboard-9.0.0.0rc1/doc/source/calendar.rst`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/doc/source/conf.py` & `blazar-dashboard-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/doc/source/index.rst` & `blazar-dashboard-9.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/doc/source/install/install.rst` & `blazar-dashboard-9.0.0.0rc1/doc/source/install/install.rst`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/lower-constraints.txt` & `blazar-dashboard-9.0.0.0rc1/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/manage.py` & `blazar-dashboard-9.0.0.0rc1/manage.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/releasenotes/source/conf.py` & `blazar-dashboard-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/requirements.txt` & `blazar-dashboard-9.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/setup.cfg` & `blazar-dashboard-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/setup.py` & `blazar-dashboard-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/test-requirements.txt` & `blazar-dashboard-9.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `blazar-dashboard-9.0.0/tox.ini` & `blazar-dashboard-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

