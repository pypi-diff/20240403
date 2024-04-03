# Comparing `tmp/vitrage-dashboard-6.0.0.tar.gz` & `tmp/vitrage-dashboard-6.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vitrage-dashboard-6.0.0.tar", last modified: Wed Apr  3 11:52:56 2024, max compression
+gzip compressed data, was "vitrage-dashboard-6.0.0.0rc1.tar", last modified: Thu Mar 14 12:07:24 2024, max compression
```

## Comparing `vitrage-dashboard-6.0.0.tar` & `vitrage-dashboard-6.0.0.0rc1.tar`

### file list

```diff
@@ -1,309 +1,309 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.950979 vitrage-dashboard-6.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/.jshintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2630 2024-04-03 11:52:56.000000 vitrage-dashboard-6.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10753 2024-04-03 11:52:56.000000 vitrage-dashboard-6.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3260 2024-04-03 11:52:56.950979 vitrage-dashboard-6.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1745 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.914979 vitrage-dashboard-6.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1741 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.914979 vitrage-dashboard-6.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.914979 vitrage-dashboard-6.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3043 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.914979 vitrage-dashboard-6.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/doc/source/contributor/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/doc/source/contributor/readme.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/doc/source/contributor/usage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5685 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/karma.conf.js
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      844 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/package.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.906979 vitrage-dashboard-6.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.918979 vitrage-dashboard-6.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/notes/add-del-template-b6592a2787e26239.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/notes/alarm-banner-7aa616e3f8e69171.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/notes/drop-py-2-7-53892de5b1c6cf5b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/notes/entities-graph-filtered-by-heat-stacks-4643b7bcf6737631.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/notes/highlight-fc02111debe1e3f5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/notes/pin-all-eca759914ddd1429.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/notes/reorganize-vendorized-static-files-dbe3cfdd7bc61243.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/notes/search-entities-e0f9e21afd03815a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/notes/sunburst-enhancements-dd6126beed02ccb4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/notes/template-view-4f10a05c52680f75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/notes/template_panel_in_admin_section-133f1b0cc228fedc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/notes/vitrage-admin-menu-5fa73358a8559a37.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.922979 vitrage-dashboard-6.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.922979 vitrage-dashboard-6.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.922979 vitrage-dashboard-6.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1299 2024-04-03 11:52:56.950979 vitrage-dashboard-6.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3198 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/test-shim.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.922979 vitrage-dashboard-6.0.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/tools/executable_files.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/tools/find_executables.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2278 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.922979 vitrage-dashboard-6.0.0/vitrage_dashboard/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.922979 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_alarms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_alarms/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_alarms/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.906979 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_alarms/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.926979 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_alarms/templates/adminalarms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_alarms/templates/adminalarms/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_alarms/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1069 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_alarms/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.926979 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_dashboard/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_dashboard/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_dashboard/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.906979 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_dashboard/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.926979 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_dashboard/templates/admintopology/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_dashboard/templates/admintopology/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_dashboard/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_dashboard/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.926979 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_entities/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_entities/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_entities/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.906979 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_entities/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.926979 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_entities/templates/adminentities/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_entities/templates/adminentities/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_entities/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_entities/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.926979 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_templates/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_templates/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.906979 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_templates/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.926979 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_templates/templates/admintemplates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_templates/templates/admintemplates/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_templates/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1057 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/admin_templates/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.926979 vitrage-dashboard-6.0.0/vitrage_dashboard/alarms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/alarms/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/alarms/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.906979 vitrage-dashboard-6.0.0/vitrage_dashboard/alarms/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.926979 vitrage-dashboard-6.0.0/vitrage_dashboard/alarms/templates/alarms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/alarms/templates/alarms/banner.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/alarms/templates/alarms/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/alarms/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1506 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/alarms/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.930979 vitrage-dashboard-6.0.0/vitrage_dashboard/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6072 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/api/vitrage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7151 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/api/vitrage_rest_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.930979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.906979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.906979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/app/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.906979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/app/core/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.930979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/app/core/openstack-service-api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3946 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/app/core/openstack-service-api/vitrage.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1864 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/app/core/openstack-service-api/vitrage.service.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.906979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.930979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.930979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/alarmList/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6048 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/alarmList/alarmList.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6387 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/alarmList/alarmList.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/alarmList/alarmList.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.934979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3492 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/all.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16716 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_gray_off.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16830 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_gray_on.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13408 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_green_off.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16832 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_green_on.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9206 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_orange_off.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8997 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_orange_on.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9206 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_red_off.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8997 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_red_on.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9206 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_yellow_off.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8997 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_yellow_on.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3642 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/cluster.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3605 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/host.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1555 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/spinner.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3631 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/vm.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3625 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/zone.png
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.906979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.934979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/addTemplate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5251 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/addTemplate/addTemplateContainer.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2286 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/addTemplate/addTemplateContainer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/addTemplate/addTemplateContainer.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.934979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/alarms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1401 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/alarms/alarms.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2346 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/alarms/alarms.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/alarms/alarms.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.934979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/information/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/information/information.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/information/information.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/information/information.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.934979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rcaContainer.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rcaContainer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rcaContainer.scss
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12346 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rootCauseAnalysisGraph.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rootCauseAnalysisGraph.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      984 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rootCauseAnalysisGraph.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.934979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/stacks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/stacks/stacks.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/stacks/stacks.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/stacks/stacks.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.938979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6502 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst/sunburst.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst/sunburst.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst/sunburst.scss
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst/sunburst.test.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.938979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst-minimap/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst-minimap/sunburst-minimap.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst-minimap/sunburst-minimap.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.938979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/template/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1181 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/template/templateContainer.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6816 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/template/templateContainer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/template/templateContainer.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.938979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/templateAdd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/templateAdd/templateAddOptions.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.938979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/vms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/vms/vms.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/vms/vms.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/vms/vms.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.938979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14354 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/entities.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1118 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/entities.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/entities.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.938979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/graph/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25462 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/graph/entities-graph.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/graph/entities-graph.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1501 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/graph/entities-graph.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.938979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/info/entities-info.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/info/entities-info.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/info/entities-info.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.938979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/toolbox/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/toolbox/entities-toolbox.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1379 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/toolbox/entities-toolbox.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/toolbox/entities-toolbox.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.942979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/filters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/filters/titleCase.filter.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/filters/vitrageDate.filter.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.906979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.942979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.942979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/compute/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/compute/compute.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2696 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/compute/compute.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/compute/compute.scss
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/main.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/main.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/main.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.942979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/network/network.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/network/network.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/network/network.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.942979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/storage/storage.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/storage/storage.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/storage/storage.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.942979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/services/modal.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/services/time.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3686 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/services/vitrage_topology.service.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.942979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/templateList/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3946 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/templateList/templateList.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2693 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/templateList/templateList.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/templateList/templateList.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.942979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/topology/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13305 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/topology/graph.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14527 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/topology/graph.sample.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/vitrage.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/vitrage.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.910979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.942979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/templates/topology/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/templates/topology/index.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.946979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.946979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/horizon.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.946979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/pages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/pages/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.946979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/pages/project/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/pages/project/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.946979 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/alarmspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/entitygraphpage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/templatespage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/topologypage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/test_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/settings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/test_vitragedashboard.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1066 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.946979 vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1054 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4000_project_vitrage_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1176 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4010_project_topology_vitrage_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4020_project_alarms_vitrage_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4030_project_entities_vitrage_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4040_project_template_vitrage_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4100_admin_vitrage_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4110_admin_topology_vitrage_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4120_admin_alarms_vitrage_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4130_admin_entities_vitrage_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1276 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4140_admin_template_vitrage_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.950979 vitrage-dashboard-6.0.0/vitrage_dashboard/entities/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/entities/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/entities/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.910979 vitrage-dashboard-6.0.0/vitrage_dashboard/entities/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.950979 vitrage-dashboard-6.0.0/vitrage_dashboard/entities/templates/entities/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/entities/templates/entities/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/entities/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1066 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/entities/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.950979 vitrage-dashboard-6.0.0/vitrage_dashboard/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/templates/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/templates/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.910979 vitrage-dashboard-6.0.0/vitrage_dashboard/templates/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.950979 vitrage-dashboard-6.0.0/vitrage_dashboard/templates/templates/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/templates/templates/templates/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/templates/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/templates/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1067 2024-04-03 11:52:14.000000 vitrage-dashboard-6.0.0/vitrage_dashboard/templates/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:56.922979 vitrage-dashboard-6.0.0/vitrage_dashboard.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3260 2024-04-03 11:52:56.000000 vitrage-dashboard-6.0.0/vitrage_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13366 2024-04-03 11:52:56.000000 vitrage-dashboard-6.0.0/vitrage_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:52:56.000000 vitrage-dashboard-6.0.0/vitrage_dashboard.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:52:56.000000 vitrage-dashboard-6.0.0/vitrage_dashboard.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-04-03 11:52:56.000000 vitrage-dashboard-6.0.0/vitrage_dashboard.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2024-04-03 11:52:56.000000 vitrage-dashboard-6.0.0/vitrage_dashboard.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2024-04-03 11:52:56.000000 vitrage-dashboard-6.0.0/vitrage_dashboard.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.928205 vitrage-dashboard-6.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/.jshintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2630 2024-03-14 12:07:24.000000 vitrage-dashboard-6.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10763 2024-03-14 12:07:24.000000 vitrage-dashboard-6.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3265 2024-03-14 12:07:24.928205 vitrage-dashboard-6.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1745 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.880204 vitrage-dashboard-6.0.0.0rc1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1741 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.880204 vitrage-dashboard-6.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.880204 vitrage-dashboard-6.0.0.0rc1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3043 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.880204 vitrage-dashboard-6.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/doc/source/contributor/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/doc/source/contributor/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/doc/source/contributor/usage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5685 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/karma.conf.js
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      844 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/package.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.864204 vitrage-dashboard-6.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.884204 vitrage-dashboard-6.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/notes/add-del-template-b6592a2787e26239.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/notes/alarm-banner-7aa616e3f8e69171.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/notes/drop-py-2-7-53892de5b1c6cf5b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/notes/entities-graph-filtered-by-heat-stacks-4643b7bcf6737631.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/notes/highlight-fc02111debe1e3f5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/notes/pin-all-eca759914ddd1429.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/notes/reorganize-vendorized-static-files-dbe3cfdd7bc61243.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/notes/search-entities-e0f9e21afd03815a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/notes/sunburst-enhancements-dd6126beed02ccb4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/notes/template-view-4f10a05c52680f75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/notes/template_panel_in_admin_section-133f1b0cc228fedc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/notes/vitrage-admin-menu-5fa73358a8559a37.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.888204 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.888204 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.888204 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1299 2024-03-14 12:07:24.932205 vitrage-dashboard-6.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3198 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/test-shim.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.888204 vitrage-dashboard-6.0.0.0rc1/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/tools/executable_files.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/tools/find_executables.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2278 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.888204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.892204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_alarms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_alarms/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_alarms/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.868203 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_alarms/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.892204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_alarms/templates/adminalarms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_alarms/templates/adminalarms/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_alarms/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1069 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_alarms/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.892204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_dashboard/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_dashboard/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_dashboard/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.868203 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_dashboard/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.892204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_dashboard/templates/admintopology/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_dashboard/templates/admintopology/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_dashboard/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_dashboard/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.892204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_entities/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_entities/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_entities/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.868203 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_entities/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.892204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_entities/templates/adminentities/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_entities/templates/adminentities/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_entities/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_entities/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.896204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_templates/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_templates/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.868203 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_templates/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.896204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_templates/templates/admintemplates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_templates/templates/admintemplates/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_templates/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1057 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_templates/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.896204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/alarms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/alarms/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/alarms/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.868203 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/alarms/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.896204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/alarms/templates/alarms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/alarms/templates/alarms/banner.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/alarms/templates/alarms/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/alarms/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1506 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/alarms/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.896204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6072 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/api/vitrage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7151 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/api/vitrage_rest_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.900204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.868203 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.868203 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/app/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.868203 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/app/core/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.900204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/app/core/openstack-service-api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3946 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/app/core/openstack-service-api/vitrage.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1864 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/app/core/openstack-service-api/vitrage.service.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.868203 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.900204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.900204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/alarmList/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6048 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/alarmList/alarmList.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6387 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/alarmList/alarmList.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/alarmList/alarmList.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.904204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3492 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/all.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16716 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_gray_off.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16830 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_gray_on.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13408 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_green_off.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16832 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_green_on.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9206 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_orange_off.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8997 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_orange_on.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9206 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_red_off.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8997 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_red_on.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9206 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_yellow_off.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8997 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_yellow_on.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3642 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/cluster.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3605 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/host.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1555 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/spinner.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3631 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/vm.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3625 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/zone.png
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.872204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.904204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/addTemplate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5251 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/addTemplate/addTemplateContainer.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2286 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/addTemplate/addTemplateContainer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/addTemplate/addTemplateContainer.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.904204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/alarms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1401 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/alarms/alarms.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2346 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/alarms/alarms.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/alarms/alarms.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.908204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/information/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/information/information.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/information/information.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/information/information.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.908204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rcaContainer.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rcaContainer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rcaContainer.scss
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12346 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rootCauseAnalysisGraph.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rootCauseAnalysisGraph.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      984 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rootCauseAnalysisGraph.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.908204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/stacks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/stacks/stacks.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/stacks/stacks.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/stacks/stacks.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.908204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6502 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst/sunburst.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst/sunburst.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst/sunburst.scss
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst/sunburst.test.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.912205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst-minimap/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst-minimap/sunburst-minimap.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst-minimap/sunburst-minimap.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.912205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/template/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1181 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/template/templateContainer.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6816 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/template/templateContainer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/template/templateContainer.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.912205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/templateAdd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/templateAdd/templateAddOptions.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.912205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/vms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/vms/vms.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/vms/vms.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/vms/vms.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.912205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14354 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/entities.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1118 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/entities.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/entities.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.912205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/graph/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25462 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/graph/entities-graph.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/graph/entities-graph.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1501 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/graph/entities-graph.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.916205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/info/entities-info.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/info/entities-info.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/info/entities-info.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.916205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/toolbox/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/toolbox/entities-toolbox.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1379 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/toolbox/entities-toolbox.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/toolbox/entities-toolbox.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.916205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/filters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/filters/titleCase.filter.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/filters/vitrageDate.filter.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.872204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.916205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.916205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/compute/compute.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2696 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/compute/compute.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/compute/compute.scss
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/main.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/main.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/main.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.916205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/network/network.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/network/network.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/network/network.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.920205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/storage/storage.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/storage/storage.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/storage/storage.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.920205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/services/modal.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/services/time.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3686 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/services/vitrage_topology.service.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.920205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/templateList/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3946 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/templateList/templateList.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2693 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/templateList/templateList.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/templateList/templateList.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.920205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/topology/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13305 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/topology/graph.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14527 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/topology/graph.sample.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/vitrage.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/vitrage.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.872204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.920205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/templates/topology/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/templates/topology/index.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.920205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.924205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/horizon.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.924205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/pages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/pages/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.924205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/pages/project/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/pages/project/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.924205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/alarmspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/entitygraphpage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/templatespage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/topologypage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/test_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/settings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/test_vitragedashboard.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1066 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.928205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1054 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4000_project_vitrage_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1176 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4010_project_topology_vitrage_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4020_project_alarms_vitrage_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4030_project_entities_vitrage_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4040_project_template_vitrage_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1058 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4100_admin_vitrage_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4110_admin_topology_vitrage_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4120_admin_alarms_vitrage_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4130_admin_entities_vitrage_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1276 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4140_admin_template_vitrage_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.928205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/entities/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/entities/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/entities/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.872204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/entities/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.928205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/entities/templates/entities/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/entities/templates/entities/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/entities/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1066 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/entities/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.928205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/templates/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/templates/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.872204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/templates/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.928205 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/templates/templates/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/templates/templates/templates/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/templates/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/templates/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1067 2024-03-14 12:06:52.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/templates/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 12:07:24.892204 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3265 2024-03-14 12:07:24.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13366 2024-03-14 12:07:24.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-14 12:07:24.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-14 12:07:24.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-14 12:07:24.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2024-03-14 12:07:24.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2024-03-14 12:07:24.000000 vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard.egg-info/top_level.txt
```

### Comparing `vitrage-dashboard-6.0.0/.jshintrc` & `vitrage-dashboard-6.0.0.0rc1/.jshintrc`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/.zuul.yaml` & `vitrage-dashboard-6.0.0.0rc1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/AUTHORS` & `vitrage-dashboard-6.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/CONTRIBUTING.rst` & `vitrage-dashboard-6.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/ChangeLog` & `vitrage-dashboard-6.0.0.0rc1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-6.0.0
------
+6.0.0.0rc1
+----------
 
 * reno: Update master for unmaintained/xena
 * reno: Update master for unmaintained/wallaby
 * reno: Update master for unmaintained/victoria
 * reno: Update master for unmaintained/yoga
 * Update python classifier in setup.cfg
 * Update master for stable/2023.2
```

### Comparing `vitrage-dashboard-6.0.0/LICENSE` & `vitrage-dashboard-6.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/MANIFEST.in` & `vitrage-dashboard-6.0.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/PKG-INFO` & `vitrage-dashboard-6.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: vitrage-dashboard
-Version: 6.0.0
+Version: 6.0.0.0rc1
 Summary: Vitrage Horizon plugin
 Home-page: https://docs.openstack.org/vitrage-dashboard/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =================
         Vitrage Dashboard
```

### Comparing `vitrage-dashboard-6.0.0/README.rst` & `vitrage-dashboard-6.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/devstack/plugin.sh` & `vitrage-dashboard-6.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/doc/source/conf.py` & `vitrage-dashboard-6.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/doc/source/index.rst` & `vitrage-dashboard-6.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/karma.conf.js` & `vitrage-dashboard-6.0.0.0rc1/karma.conf.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/manage.py` & `vitrage-dashboard-6.0.0.0rc1/manage.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/package.json` & `vitrage-dashboard-6.0.0.0rc1/package.json`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/releasenotes/source/conf.py` & `vitrage-dashboard-6.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/requirements.txt` & `vitrage-dashboard-6.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/setup.cfg` & `vitrage-dashboard-6.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/setup.py` & `vitrage-dashboard-6.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/test-shim.js` & `vitrage-dashboard-6.0.0.0rc1/test-shim.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/tox.ini` & `vitrage-dashboard-6.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_alarms/__init__.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_alarms/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_alarms/panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_alarms/panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_alarms/urls.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_alarms/urls.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_alarms/views.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_alarms/views.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_dashboard/__init__.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_dashboard/panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_dashboard/panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_dashboard/templates/admintopology/index.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_dashboard/templates/admintopology/index.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_dashboard/urls.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_dashboard/urls.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_dashboard/views.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_dashboard/views.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_entities/__init__.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_entities/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_entities/panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_entities/panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_entities/templates/adminentities/index.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_entities/templates/adminentities/index.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_entities/urls.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_entities/urls.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_entities/views.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_entities/views.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_templates/__init__.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_templates/panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_templates/panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_templates/urls.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_templates/urls.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/admin_templates/views.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/admin_templates/views.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/alarms/__init__.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/alarms/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/alarms/panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/alarms/panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/alarms/templates/alarms/banner.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/alarms/templates/alarms/banner.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/alarms/urls.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/alarms/urls.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/alarms/views.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/alarms/views.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/api/vitrage.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/api/vitrage.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/api/vitrage_rest_api.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/api/vitrage_rest_api.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/__init__.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/app/core/openstack-service-api/vitrage.service.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/app/core/openstack-service-api/vitrage.service.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/app/core/openstack-service-api/vitrage.service.spec.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/app/core/openstack-service-api/vitrage.service.spec.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/alarmList/alarmList.controller.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/alarmList/alarmList.controller.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/alarmList/alarmList.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/alarmList/alarmList.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/alarmList/alarmList.scss` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/alarmList/alarmList.scss`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/all.png` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/all.png`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_gray_off.svg` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_gray_off.svg`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_gray_on.svg` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_gray_on.svg`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_green_off.svg` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_green_off.svg`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_green_on.svg` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_green_on.svg`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_orange_off.svg` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_orange_off.svg`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_orange_on.svg` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_orange_on.svg`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_red_off.svg` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_red_off.svg`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_red_on.svg` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_red_on.svg`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_yellow_off.svg` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_yellow_off.svg`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_yellow_on.svg` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/bell_yellow_on.svg`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/cluster.png` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/cluster.png`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/host.png` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/host.png`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/spinner.gif` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/spinner.gif`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/vm.png` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/vm.png`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/assets/zone.png` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/assets/zone.png`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/addTemplate/addTemplateContainer.controller.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/addTemplate/addTemplateContainer.controller.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/addTemplate/addTemplateContainer.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/addTemplate/addTemplateContainer.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/alarms/alarms.directive.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/alarms/alarms.directive.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/alarms/alarms.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/alarms/alarms.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/alarms/alarms.scss` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/alarms/alarms.scss`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/information/information.directive.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/information/information.directive.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/information/information.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/information/information.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/information/information.scss` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/information/information.scss`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rcaContainer.controller.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rcaContainer.controller.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rootCauseAnalysisGraph.directive.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rootCauseAnalysisGraph.directive.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rootCauseAnalysisGraph.scss` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/rca/rootCauseAnalysisGraph.scss`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst/sunburst.directive.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst/sunburst.directive.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst-minimap/sunburst-minimap.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/sunburst-minimap/sunburst-minimap.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/template/templateContainer.controller.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/template/templateContainer.controller.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/template/templateContainer.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/template/templateContainer.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/template/templateContainer.scss` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/template/templateContainer.scss`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/components/templateAdd/templateAddOptions.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/components/templateAdd/templateAddOptions.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/entities.controller.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/entities.controller.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/entities.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/entities.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/graph/entities-graph.directive.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/graph/entities-graph.directive.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/graph/entities-graph.scss` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/graph/entities-graph.scss`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/info/entities-info.directive.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/info/entities-info.directive.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/info/entities-info.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/info/entities-info.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/info/entities-info.scss` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/info/entities-info.scss`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/toolbox/entities-toolbox.directive.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/toolbox/entities-toolbox.directive.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/toolbox/entities-toolbox.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/toolbox/entities-toolbox.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/entities/toolbox/entities-toolbox.scss` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/entities/toolbox/entities-toolbox.scss`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/compute/compute.directive.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/compute/compute.directive.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/compute/compute.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/compute/compute.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/compute/compute.scss` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/compute/compute.scss`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/main.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/main.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/network/network.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/network/network.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/storage/storage.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/layout/main/storage/storage.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/services/modal.service.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/services/modal.service.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/services/time.service.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/services/time.service.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/services/vitrage_topology.service.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/services/vitrage_topology.service.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/templateList/templateList.controller.js` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/templateList/templateList.controller.js`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/templateList/templateList.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/templateList/templateList.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/topology/graph.json` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/topology/graph.json`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/topology/graph.sample.json` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/topology/graph.sample.json`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/static/dashboard/project/vitrage.scss` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/static/dashboard/project/vitrage.scss`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/templates/topology/index.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/templates/topology/index.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/base.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/alarmspage.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/alarmspage.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/entitygraphpage.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/entitygraphpage.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/templatespage.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/templatespage.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/topologypage.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/pages/project/vitrage/topologypage.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/integration/test_basic.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/settings.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/settings.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/tests/test_vitragedashboard.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/tests/test_vitragedashboard.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/urls.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/urls.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/dashboard/views.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/dashboard/views.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4000_project_vitrage_panel_group.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4000_project_vitrage_panel_group.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4010_project_topology_vitrage_panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4010_project_topology_vitrage_panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4020_project_alarms_vitrage_panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4020_project_alarms_vitrage_panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4030_project_entities_vitrage_panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4030_project_entities_vitrage_panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4040_project_template_vitrage_panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4040_project_template_vitrage_panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4100_admin_vitrage_panel_group.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4100_admin_vitrage_panel_group.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4110_admin_topology_vitrage_panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4110_admin_topology_vitrage_panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4120_admin_alarms_vitrage_panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4120_admin_alarms_vitrage_panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4130_admin_entities_vitrage_panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4130_admin_entities_vitrage_panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/enabled/_4140_admin_template_vitrage_panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/enabled/_4140_admin_template_vitrage_panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/entities/__init__.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/entities/panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/entities/panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/entities/templates/entities/index.html` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/entities/templates/entities/index.html`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/entities/urls.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/entities/urls.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/entities/views.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/entities/views.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/templates/__init__.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/templates/panel.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/templates/panel.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/templates/urls.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/templates/urls.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/templates/version.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/templates/version.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard/templates/views.py` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard/templates/views.py`

 * *Files identical despite different names*

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard.egg-info/PKG-INFO` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: vitrage-dashboard
-Version: 6.0.0
+Version: 6.0.0.0rc1
 Summary: Vitrage Horizon plugin
 Home-page: https://docs.openstack.org/vitrage-dashboard/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =================
         Vitrage Dashboard
```

### Comparing `vitrage-dashboard-6.0.0/vitrage_dashboard.egg-info/SOURCES.txt` & `vitrage-dashboard-6.0.0.0rc1/vitrage_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

