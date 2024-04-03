# Comparing `tmp/masakari-dashboard-9.0.0.tar.gz` & `tmp/masakari-dashboard-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masakari-dashboard-9.0.0.tar", last modified: Wed Oct  4 11:06:50 2023, max compression
+gzip compressed data, was "masakari-dashboard-9.0.0.0rc1.tar", last modified: Fri Sep 15 13:59:26 2023, max compression
```

## Comparing `masakari-dashboard-9.0.0.tar` & `masakari-dashboard-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.265773 masakari-dashboard-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1158 2023-10-04 11:06:50.000000 masakari-dashboard-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2794 2023-10-04 11:06:50.000000 masakari-dashboard-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3475 2023-10-04 11:06:50.265773 masakari-dashboard-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2196 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.241773 masakari-dashboard-9.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5619 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.241773 masakari-dashboard-9.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10330 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.241773 masakari-dashboard-9.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2392 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/manage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.245773 masakari-dashboard-9.0.0/masakari_dashboard.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3475 2023-10-04 11:06:50.000000 masakari-dashboard-9.0.0/masakari_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4041 2023-10-04 11:06:50.000000 masakari-dashboard-9.0.0/masakari_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-10-04 11:06:50.000000 masakari-dashboard-9.0.0/masakari_dashboard.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-10-04 11:06:50.000000 masakari-dashboard-9.0.0/masakari_dashboard.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-10-04 11:06:50.000000 masakari-dashboard-9.0.0/masakari_dashboard.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2023-10-04 11:06:50.000000 masakari-dashboard-9.0.0/masakari_dashboard.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2023-10-04 11:06:50.000000 masakari-dashboard-9.0.0/masakari_dashboard.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.245773 masakari-dashboard-9.0.0/masakaridashboard/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.245773 masakari-dashboard-9.0.0/masakaridashboard/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6515 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/api/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.245773 masakari-dashboard-9.0.0/masakaridashboard/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/conf/masakari_policy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1972 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/dashboard.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.245773 masakari-dashboard-9.0.0/masakaridashboard/default/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/default/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/default/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.233773 masakari-dashboard-9.0.0/masakaridashboard/default/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.245773 masakari-dashboard-9.0.0/masakaridashboard/default/templates/default/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/default/templates/default/base.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/default/templates/default/table.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3010 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/handle_errors.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.249773 masakari-dashboard-9.0.0/masakaridashboard/hosts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/hosts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2648 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/hosts/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/hosts/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3287 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/hosts/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/hosts/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.233773 masakari-dashboard-9.0.0/masakaridashboard/hosts/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.249773 masakari-dashboard-9.0.0/masakaridashboard/hosts/templates/hosts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/hosts/templates/hosts/_detail_overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/hosts/templates/hosts/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1190 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/hosts/templates/hosts/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/hosts/templates/hosts/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/hosts/templates/hosts/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6271 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/hosts/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/hosts/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4857 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/hosts/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.249773 masakari-dashboard-9.0.0/masakaridashboard/local/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/local/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.249773 masakari-dashboard-9.0.0/masakaridashboard/local/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/local/enabled/_50_masakaridashboard.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/local/enabled/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.253773 masakari-dashboard-9.0.0/masakaridashboard/local/local_settings.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/local/local_settings.d/_50_masakari.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.253773 masakari-dashboard-9.0.0/masakaridashboard/notifications/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/notifications/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/notifications/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2493 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/notifications/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2787 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/notifications/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.237773 masakari-dashboard-9.0.0/masakaridashboard/notifications/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.253773 masakari-dashboard-9.0.0/masakaridashboard/notifications/templates/notifications/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/notifications/templates/notifications/_detail_overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/notifications/templates/notifications/_progress_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/notifications/templates/notifications/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5710 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/notifications/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      880 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/notifications/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4205 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/notifications/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.257773 masakari-dashboard-9.0.0/masakaridashboard/segments/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7238 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3614 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1773 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.237773 masakari-dashboard-9.0.0/masakaridashboard/segments/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.257773 masakari-dashboard-9.0.0/masakaridashboard/segments/templates/segments/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      580 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/templates/segments/_addhost.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1084 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/templates/segments/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/templates/segments/_detail_overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/templates/segments/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/templates/segments/addhost.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/templates/segments/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/templates/segments/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/templates/segments/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9764 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1162 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8315 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/segments/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.237773 masakari-dashboard-9.0.0/masakaridashboard/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.237773 masakari-dashboard-9.0.0/masakaridashboard/static/masakaridashboard/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.257773 masakari-dashboard-9.0.0/masakaridashboard/static/masakaridashboard/css/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/static/masakaridashboard/css/style.css
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.261773 masakari-dashboard-9.0.0/masakaridashboard/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/test/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/test/helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/test/settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.261773 masakari-dashboard-9.0.0/masakaridashboard/test/test_data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/test/test_data/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3487 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/test/test_data/masakari_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/test/test_data/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1122 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/test/uuidsentinel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/masakaridashboard/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.237773 masakari-dashboard-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.261773 masakari-dashboard-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/notes/blueprint-enable-to-segment-efdff66078dab752.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/notes/bug-1944679-0df043f17a8bbaff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/notes/drop-masakariclient-dep-054a456a5bf2b941.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/notes/drop-py-2-7-a5322c1cb7c74c61.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/notes/fix-cacert-023407ba61a4bb7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/notes/yamlify-policy-169e72bc8abd93a1.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:06:50.265773 masakari-dashboard-9.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9292 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2023-10-04 11:06:50.265773 masakari-dashboard-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3060 2023-10-04 11:06:22.000000 masakari-dashboard-9.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.443986 masakari-dashboard-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1158 2023-09-15 13:59:25.000000 masakari-dashboard-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2804 2023-09-15 13:59:25.000000 masakari-dashboard-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3480 2023-09-15 13:59:26.443986 masakari-dashboard-9.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2196 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.419984 masakari-dashboard-9.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5619 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.423984 masakari-dashboard-9.0.0.0rc1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10330 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.423984 masakari-dashboard-9.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2392 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/manage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.423984 masakari-dashboard-9.0.0.0rc1/masakari_dashboard.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3480 2023-09-15 13:59:25.000000 masakari-dashboard-9.0.0.0rc1/masakari_dashboard.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4041 2023-09-15 13:59:25.000000 masakari-dashboard-9.0.0.0rc1/masakari_dashboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-09-15 13:59:25.000000 masakari-dashboard-9.0.0.0rc1/masakari_dashboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-09-15 13:59:25.000000 masakari-dashboard-9.0.0.0rc1/masakari_dashboard.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-09-15 13:59:25.000000 masakari-dashboard-9.0.0.0rc1/masakari_dashboard.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2023-09-15 13:59:25.000000 masakari-dashboard-9.0.0.0rc1/masakari_dashboard.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2023-09-15 13:59:25.000000 masakari-dashboard-9.0.0.0rc1/masakari_dashboard.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.423984 masakari-dashboard-9.0.0.0rc1/masakaridashboard/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.423984 masakari-dashboard-9.0.0.0rc1/masakaridashboard/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6515 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/api/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.423984 masakari-dashboard-9.0.0.0rc1/masakaridashboard/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/conf/masakari_policy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1972 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/dashboard.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.427985 masakari-dashboard-9.0.0.0rc1/masakaridashboard/default/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/default/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/default/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.415984 masakari-dashboard-9.0.0.0rc1/masakaridashboard/default/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.427985 masakari-dashboard-9.0.0.0rc1/masakaridashboard/default/templates/default/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/default/templates/default/base.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/default/templates/default/table.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3010 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/handle_errors.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.427985 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2648 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3287 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.415984 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.427985 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/templates/hosts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/templates/hosts/_detail_overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/templates/hosts/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1190 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/templates/hosts/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/templates/hosts/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/templates/hosts/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6271 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4857 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.431985 masakari-dashboard-9.0.0.0rc1/masakaridashboard/local/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/local/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.431985 masakari-dashboard-9.0.0.0rc1/masakaridashboard/local/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/local/enabled/_50_masakaridashboard.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/local/enabled/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.431985 masakari-dashboard-9.0.0.0rc1/masakaridashboard/local/local_settings.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/local/local_settings.d/_50_masakari.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.431985 masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2493 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2787 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.415984 masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.431985 masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/templates/notifications/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/templates/notifications/_detail_overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/templates/notifications/_progress_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/templates/notifications/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5710 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      880 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4205 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.435985 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7238 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3614 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1773 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.415984 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.435985 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/templates/segments/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      580 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/templates/segments/_addhost.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1084 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/templates/segments/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/templates/segments/_detail_overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/templates/segments/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/templates/segments/addhost.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/templates/segments/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/templates/segments/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/templates/segments/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9764 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1162 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8315 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.415984 masakari-dashboard-9.0.0.0rc1/masakaridashboard/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.415984 masakari-dashboard-9.0.0.0rc1/masakaridashboard/static/masakaridashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.435985 masakari-dashboard-9.0.0.0rc1/masakaridashboard/static/masakaridashboard/css/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/static/masakaridashboard/css/style.css
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.439985 masakari-dashboard-9.0.0.0rc1/masakaridashboard/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/test/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/test/helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/test/settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.439985 masakari-dashboard-9.0.0.0rc1/masakaridashboard/test/test_data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/test/test_data/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3487 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/test/test_data/masakari_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/test/test_data/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1122 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/test/uuidsentinel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/masakaridashboard/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.415984 masakari-dashboard-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.439985 masakari-dashboard-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/notes/blueprint-enable-to-segment-efdff66078dab752.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/notes/bug-1944679-0df043f17a8bbaff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/notes/drop-masakariclient-dep-054a456a5bf2b941.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/notes/drop-py-2-7-a5322c1cb7c74c61.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/notes/fix-cacert-023407ba61a4bb7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/notes/yamlify-policy-169e72bc8abd93a1.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 13:59:26.443986 masakari-dashboard-9.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9292 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2023-09-15 13:59:26.443986 masakari-dashboard-9.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3060 2023-09-15 13:58:30.000000 masakari-dashboard-9.0.0.0rc1/tox.ini
```

### Comparing `masakari-dashboard-9.0.0/AUTHORS` & `masakari-dashboard-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/CONTRIBUTING.rst` & `masakari-dashboard-9.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/ChangeLog` & `masakari-dashboard-9.0.0.0rc1/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * remove duplicated code
 
 8.0.0
 -----
 
 * Update tox.ini for tox4
```

### Comparing `masakari-dashboard-9.0.0/LICENSE` & `masakari-dashboard-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/PKG-INFO` & `masakari-dashboard-9.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: masakari-dashboard
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Horizon plugin for masakari
 Home-page: https://opendev.org/openstack/masakari-dashboard
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===============================
         Masakari dashboard
```

### Comparing `masakari-dashboard-9.0.0/README.rst` & `masakari-dashboard-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/doc/Makefile` & `masakari-dashboard-9.0.0.0rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/doc/requirements.txt` & `masakari-dashboard-9.0.0.0rc1/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/doc/source/conf.py` & `masakari-dashboard-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/doc/source/contributor/contributing.rst` & `masakari-dashboard-9.0.0.0rc1/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/doc/source/index.rst` & `masakari-dashboard-9.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/manage.py` & `masakari-dashboard-9.0.0.0rc1/manage.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakari_dashboard.egg-info/PKG-INFO` & `masakari-dashboard-9.0.0.0rc1/masakari_dashboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: masakari-dashboard
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Horizon plugin for masakari
 Home-page: https://opendev.org/openstack/masakari-dashboard
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===============================
         Masakari dashboard
```

### Comparing `masakari-dashboard-9.0.0/masakari_dashboard.egg-info/SOURCES.txt` & `masakari-dashboard-9.0.0.0rc1/masakari_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/api/api.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/api/api.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/dashboard.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/default/panel.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/default/panel.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/handle_errors.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/handle_errors.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/hosts/forms.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/forms.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/hosts/panel.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/panel.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/hosts/tables.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/tables.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/hosts/tabs.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/tabs.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/hosts/templates/hosts/_detail_overview.html` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/templates/hosts/_detail_overview.html`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/hosts/templates/hosts/detail.html` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/templates/hosts/detail.html`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/hosts/tests.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/tests.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/hosts/urls.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/urls.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/hosts/views.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/hosts/views.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/local/enabled/_50_masakaridashboard.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/local/enabled/_50_masakaridashboard.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/local/local_settings.d/_50_masakari.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/local/local_settings.d/_50_masakari.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/notifications/panel.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/panel.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/notifications/tables.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/tables.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/notifications/tabs.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/tabs.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/notifications/templates/notifications/_detail_overview.html` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/templates/notifications/_detail_overview.html`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/notifications/tests.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/tests.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/notifications/urls.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/urls.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/notifications/views.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/notifications/views.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/segments/forms.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/forms.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/segments/panel.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/panel.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/segments/tables.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/tables.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/segments/tabs.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/tabs.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/segments/templates/segments/_addhost.html` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/templates/segments/_addhost.html`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/segments/templates/segments/_create.html` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/templates/segments/_create.html`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/segments/templates/segments/_detail_overview.html` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/templates/segments/_detail_overview.html`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/segments/tests.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/tests.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/segments/urls.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/urls.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/segments/views.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/segments/views.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/static/masakaridashboard/css/style.css` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/static/masakaridashboard/css/style.css`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/test/helpers.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/test/helpers.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/test/settings.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/test/settings.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/test/test_data/masakari_data.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/test/test_data/masakari_data.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/test/test_data/utils.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/test/test_data/utils.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/test/uuidsentinel.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/test/uuidsentinel.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/masakaridashboard/version.py` & `masakari-dashboard-9.0.0.0rc1/masakaridashboard/version.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/releasenotes/source/conf.py` & `masakari-dashboard-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/requirements.txt` & `masakari-dashboard-9.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/setup.cfg` & `masakari-dashboard-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/setup.py` & `masakari-dashboard-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/test-requirements.txt` & `masakari-dashboard-9.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `masakari-dashboard-9.0.0/tox.ini` & `masakari-dashboard-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

