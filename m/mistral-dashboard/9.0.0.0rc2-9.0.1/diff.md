# Comparing `tmp/mistral-dashboard-9.0.0.0rc2.tar.gz` & `tmp/mistral-dashboard-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mistral-dashboard-9.0.0.0rc2.tar", last modified: Thu Oct 10 14:22:35 2019, max compression
+gzip compressed data, was "dist/mistral-dashboard-9.0.1.tar", last modified: Thu Nov 21 10:26:27 2019, max compression
```

## Comparing `mistral-dashboard-9.0.0.0rc2.tar` & `mistral-dashboard-9.0.1.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12997 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3615 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2237 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/.stestr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/doc/source/readme.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2008 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2019-10-10 14:21:49.000000 mistral-dashboard-9.0.0.0rc2/.zuul.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      840 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/manage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistral_dashboard.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3615 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistral_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6673 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistral_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistral_dashboard.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistral_dashboard.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistral_dashboard.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistral_dashboard.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistral_dashboard.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1925 2019-10-10 14:21:49.000000 mistral-dashboard-9.0.0.0rc2/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11512 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/ChangeLog
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/static/mistraldashboard/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/static/mistraldashboard/css/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/static/mistraldashboard/css/style.css
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/templates/default/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/templates/default/_label.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/templates/default/_prettyprint.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/templates/default/base.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/templates/default/_booleanfield.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/templates/default/_humantime.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       27 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/templates/default/_preprint.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/templates/default/_code.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/templates/default/table.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2378 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3155 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/smart_cell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/test/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/test/test_data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4883 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/test/test_data/mistral_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1136 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/test/test_data/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/test/test_data/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/test/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/test/helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/test/settings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/test/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3593 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/templates/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/templates/actions/run.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/templates/actions/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/templates/actions/_run.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/templates/actions/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/templates/actions/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      608 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/templates/actions/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      608 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/templates/actions/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/templates/actions/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5157 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3106 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6615 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12107 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2752 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/templates/workbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/templates/workbooks/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/templates/workbooks/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      612 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/templates/workbooks/_select_definition.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/templates/workbooks/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/templates/workbooks/select_definition.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/templates/workbooks/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/templates/workbooks/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/templates/workbooks/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4166 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5660 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4397 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2972 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/handle_errors.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1196 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3678 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/templates/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/templates/tasks/filtered.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2631 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/templates/tasks/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/templates/tasks/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4548 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1802 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4303 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/templates/action_executions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/templates/action_executions/filtered.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3635 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/templates/action_executions/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/templates/action_executions/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/templates/action_executions/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/templates/action_executions/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5486 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3551 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/forms.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6287 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/templates/executions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2465 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/templates/executions/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/templates/executions/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/templates/executions/update_description.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/templates/executions/index_filtered_task.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/templates/executions/_update_description.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9292 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2930 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1680 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/forms.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3199 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/templates/cron_triggers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3396 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/templates/cron_triggers/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/templates/cron_triggers/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/templates/cron_triggers/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/templates/cron_triggers/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2709 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3133 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7222 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/dashboard.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1508 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3754 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/templates/workflows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/templates/workflows/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/templates/workflows/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/templates/workflows/_select_definition.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/templates/workflows/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/templates/workflows/select_definition.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/templates/workflows/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/templates/workflows/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/templates/workflows/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/templates/workflows/_execute.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/templates/workflows/execute.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5931 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5729 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6349 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/forms.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/enabled/_50_mistral.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/mistraldashboard/enabled/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2089 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/queens.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/liberty.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2019-10-10 14:21:49.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/source/stein.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:22:35.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-10-10 14:21:45.000000 mistral-dashboard-9.0.0.0rc2/releasenotes/notes/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistral_dashboard.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistral_dashboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistral_dashboard.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistral_dashboard.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistral_dashboard.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6673 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistral_dashboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3610 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistral_dashboard.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistral_dashboard.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2237 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11502 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1925 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/.zuul.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/releasenotes/notes/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/releasenotes/source/stein.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/releasenotes/source/_static/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2089 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/releasenotes/source/liberty.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/setup.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      840 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/AUTHORS
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12997 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/run_tests.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2008 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/doc/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3610 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/default/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/default/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/default/templates/default/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/default/templates/default/base.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/default/templates/default/_humantime.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/default/templates/default/table.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/default/templates/default/_prettyprint.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       27 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/default/templates/default/_preprint.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/default/templates/default/_code.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/default/templates/default/_label.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/default/templates/default/_booleanfield.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3155 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/default/smart_cell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/default/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2378 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/default/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/default/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12107 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/static/mistraldashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/static/mistraldashboard/css/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/static/mistraldashboard/css/style.css
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/forms.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5931 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3754 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/templates/workflows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/templates/workflows/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/templates/workflows/select_definition.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/templates/workflows/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/templates/workflows/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/templates/workflows/execute.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/templates/workflows/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/templates/workflows/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/templates/workflows/_select_definition.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/templates/workflows/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/templates/workflows/_execute.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1508 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5729 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6349 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workflows/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5486 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4303 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/templates/action_executions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3635 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/templates/action_executions/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/templates/action_executions/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/templates/action_executions/filtered.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/templates/action_executions/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/templates/action_executions/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3551 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/action_executions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5157 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3593 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/templates/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/templates/actions/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/templates/actions/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/templates/actions/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/templates/actions/_run.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/templates/actions/run.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      608 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/templates/actions/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      608 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/templates/actions/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/templates/actions/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3106 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6615 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/actions/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4166 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2752 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/templates/workbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/templates/workbooks/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/templates/workbooks/select_definition.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/templates/workbooks/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/templates/workbooks/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/templates/workbooks/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/templates/workbooks/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      612 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/templates/workbooks/_select_definition.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/templates/workbooks/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5660 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4397 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/workbooks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2709 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3199 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/templates/cron_triggers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/templates/cron_triggers/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3396 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/templates/cron_triggers/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/templates/cron_triggers/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/templates/cron_triggers/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3133 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7222 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9292 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6287 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/templates/executions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2465 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/templates/executions/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/templates/executions/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/templates/executions/update_description.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/templates/executions/index_filtered_task.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/templates/executions/_update_description.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2930 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1680 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/executions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2972 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/handle_errors.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/test/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/test/test_data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4883 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/test/test_data/mistral_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1136 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/test/test_data/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/test/test_data/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/test/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/test/settings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/test/helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/test/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4548 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/tasks/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3678 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/tasks/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/tasks/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/tasks/templates/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2631 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/tasks/templates/tasks/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/tasks/templates/tasks/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/tasks/templates/tasks/filtered.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1196 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/tasks/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1802 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/tasks/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/tasks/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/tasks/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:26:27.000000 mistral-dashboard-9.0.1/mistraldashboard/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/enabled/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/enabled/_50_mistral.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/mistraldashboard/dashboard.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2019-11-21 10:25:29.000000 mistral-dashboard-9.0.1/LICENSE
```

### Comparing `mistral-dashboard-9.0.0.0rc2/run_tests.sh` & `mistral-dashboard-9.0.1/run_tests.sh`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/PKG-INFO` & `mistral-dashboard-9.0.1/mistral_dashboard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mistral-dashboard
-Version: 9.0.0.0rc2
+Version: 9.0.1
 Summary: Mistral dashboard
 Home-page: https://docs.openstack.org/mistral/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: ========================
         Team and repository tags
```

### Comparing `mistral-dashboard-9.0.0.0rc2/README.rst` & `mistral-dashboard-9.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/test-requirements.txt` & `mistral-dashboard-9.0.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/doc/source/conf.py` & `mistral-dashboard-9.0.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/setup.cfg` & `mistral-dashboard-9.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/manage.py` & `mistral-dashboard-9.0.1/manage.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistral_dashboard.egg-info/PKG-INFO` & `mistral-dashboard-9.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: mistral-dashboard
-Version: 9.0.0.0rc2
+Version: 9.0.1
 Summary: Mistral dashboard
 Home-page: https://docs.openstack.org/mistral/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache License, Version 2.0
 Description: ========================
         Team and repository tags
```

### Comparing `mistral-dashboard-9.0.0.0rc2/mistral_dashboard.egg-info/SOURCES.txt` & `mistral-dashboard-9.0.1/mistral_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/LICENSE` & `mistral-dashboard-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/tox.ini` & `mistral-dashboard-9.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/setup.py` & `mistral-dashboard-9.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/AUTHORS` & `mistral-dashboard-9.0.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/CONTRIBUTING.rst` & `mistral-dashboard-9.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/ChangeLog` & `mistral-dashboard-9.0.1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0.0rc2
-----------
+9.0.1
+-----
 
 * Update TOX/UPPER\_CONSTRAINTS\_FILE for stable/train
 * Update .gitreview for stable/train
 
 9.0.0.0rc1
 ----------
```

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/exceptions.py` & `mistral-dashboard-9.0.1/mistraldashboard/exceptions.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/static/mistraldashboard/css/style.css` & `mistral-dashboard-9.0.1/mistraldashboard/static/mistraldashboard/css/style.css`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/utils.py` & `mistral-dashboard-9.0.1/mistraldashboard/default/utils.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/smart_cell.py` & `mistral-dashboard-9.0.1/mistraldashboard/default/smart_cell.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/default/panel.py` & `mistral-dashboard-9.0.1/mistraldashboard/default/panel.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/test/test_data/mistral_data.py` & `mistral-dashboard-9.0.1/mistraldashboard/test/test_data/mistral_data.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/test/test_data/utils.py` & `mistral-dashboard-9.0.1/mistraldashboard/test/test_data/utils.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/test/urls.py` & `mistral-dashboard-9.0.1/mistraldashboard/test/urls.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/test/helpers.py` & `mistral-dashboard-9.0.1/mistraldashboard/test/helpers.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/test/settings.py` & `mistral-dashboard-9.0.1/mistraldashboard/test/settings.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/urls.py` & `mistral-dashboard-9.0.1/mistraldashboard/actions/urls.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/tables.py` & `mistral-dashboard-9.0.1/mistraldashboard/actions/tables.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/templates/actions/detail.html` & `mistral-dashboard-9.0.1/mistraldashboard/actions/templates/actions/detail.html`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/templates/actions/_create.html` & `mistral-dashboard-9.0.1/mistraldashboard/actions/templates/actions/_create.html`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/templates/actions/_update.html` & `mistral-dashboard-9.0.1/mistraldashboard/actions/templates/actions/_update.html`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/panel.py` & `mistral-dashboard-9.0.1/mistraldashboard/actions/panel.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/views.py` & `mistral-dashboard-9.0.1/mistraldashboard/actions/views.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/tests.py` & `mistral-dashboard-9.0.1/mistraldashboard/actions/tests.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/actions/forms.py` & `mistral-dashboard-9.0.1/mistraldashboard/actions/forms.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/api.py` & `mistral-dashboard-9.0.1/mistraldashboard/api.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/urls.py` & `mistral-dashboard-9.0.1/mistraldashboard/workbooks/urls.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/tables.py` & `mistral-dashboard-9.0.1/mistraldashboard/workbooks/tables.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/templates/workbooks/_select_definition.html` & `mistral-dashboard-9.0.1/mistraldashboard/workbooks/templates/workbooks/_select_definition.html`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/panel.py` & `mistral-dashboard-9.0.1/mistraldashboard/workbooks/panel.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/views.py` & `mistral-dashboard-9.0.1/mistraldashboard/workbooks/views.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/tests.py` & `mistral-dashboard-9.0.1/mistraldashboard/workbooks/tests.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workbooks/forms.py` & `mistral-dashboard-9.0.1/mistraldashboard/workbooks/forms.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/handle_errors.py` & `mistral-dashboard-9.0.1/mistraldashboard/handle_errors.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/urls.py` & `mistral-dashboard-9.0.1/mistraldashboard/tasks/urls.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/tables.py` & `mistral-dashboard-9.0.1/mistraldashboard/tasks/tables.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/templates/tasks/detail.html` & `mistral-dashboard-9.0.1/mistraldashboard/tasks/templates/tasks/detail.html`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/panel.py` & `mistral-dashboard-9.0.1/mistraldashboard/tasks/panel.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/views.py` & `mistral-dashboard-9.0.1/mistraldashboard/tasks/views.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/tasks/tests.py` & `mistral-dashboard-9.0.1/mistraldashboard/tasks/tests.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/urls.py` & `mistral-dashboard-9.0.1/mistraldashboard/action_executions/urls.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/tables.py` & `mistral-dashboard-9.0.1/mistraldashboard/action_executions/tables.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/templates/action_executions/detail.html` & `mistral-dashboard-9.0.1/mistraldashboard/action_executions/templates/action_executions/detail.html`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/templates/action_executions/_update.html` & `mistral-dashboard-9.0.1/mistraldashboard/action_executions/templates/action_executions/_update.html`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/panel.py` & `mistral-dashboard-9.0.1/mistraldashboard/action_executions/panel.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/views.py` & `mistral-dashboard-9.0.1/mistraldashboard/action_executions/views.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/tests.py` & `mistral-dashboard-9.0.1/mistraldashboard/action_executions/tests.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/action_executions/forms.py` & `mistral-dashboard-9.0.1/mistraldashboard/action_executions/forms.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/urls.py` & `mistral-dashboard-9.0.1/mistraldashboard/executions/urls.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/tables.py` & `mistral-dashboard-9.0.1/mistraldashboard/executions/tables.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/templates/executions/detail.html` & `mistral-dashboard-9.0.1/mistraldashboard/executions/templates/executions/detail.html`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/panel.py` & `mistral-dashboard-9.0.1/mistraldashboard/executions/panel.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/views.py` & `mistral-dashboard-9.0.1/mistraldashboard/executions/views.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/tests.py` & `mistral-dashboard-9.0.1/mistraldashboard/executions/tests.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/executions/forms.py` & `mistral-dashboard-9.0.1/mistraldashboard/executions/forms.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/urls.py` & `mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/urls.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/tables.py` & `mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/tables.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/templates/cron_triggers/detail.html` & `mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/templates/cron_triggers/detail.html`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/templates/cron_triggers/_create.html` & `mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/templates/cron_triggers/_create.html`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/panel.py` & `mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/panel.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/views.py` & `mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/views.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/tests.py` & `mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/tests.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/cron_triggers/forms.py` & `mistral-dashboard-9.0.1/mistraldashboard/cron_triggers/forms.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/dashboard.py` & `mistral-dashboard-9.0.1/mistraldashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/urls.py` & `mistral-dashboard-9.0.1/mistraldashboard/workflows/urls.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/tables.py` & `mistral-dashboard-9.0.1/mistraldashboard/workflows/tables.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/templates/workflows/_select_definition.html` & `mistral-dashboard-9.0.1/mistraldashboard/workflows/templates/workflows/_select_definition.html`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/templates/workflows/_execute.html` & `mistral-dashboard-9.0.1/mistraldashboard/workflows/templates/workflows/_execute.html`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/panel.py` & `mistral-dashboard-9.0.1/mistraldashboard/workflows/panel.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/views.py` & `mistral-dashboard-9.0.1/mistraldashboard/workflows/views.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/tests.py` & `mistral-dashboard-9.0.1/mistraldashboard/workflows/tests.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/workflows/forms.py` & `mistral-dashboard-9.0.1/mistraldashboard/workflows/forms.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/forms.py` & `mistral-dashboard-9.0.1/mistraldashboard/forms.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/mistraldashboard/enabled/_50_mistral.py` & `mistral-dashboard-9.0.1/mistraldashboard/enabled/_50_mistral.py`

 * *Files identical despite different names*

### Comparing `mistral-dashboard-9.0.0.0rc2/releasenotes/source/conf.py` & `mistral-dashboard-9.0.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

