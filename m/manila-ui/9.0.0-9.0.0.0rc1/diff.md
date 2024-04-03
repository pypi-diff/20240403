# Comparing `tmp/manila-ui-9.0.0.tar.gz` & `tmp/manila-ui-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manila-ui-9.0.0.tar", last modified: Wed Mar 22 12:23:36 2023, max compression
+gzip compressed data, was "manila-ui-9.0.0.0rc1.tar", last modified: Fri Mar  3 11:18:03 2023, max compression
```

## Comparing `manila-ui-9.0.0.tar` & `manila-ui-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,683 +1,683 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.866940 manila-ui-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-22 12:23:08.000000 manila-ui-9.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-03-22 12:23:08.000000 manila-ui-9.0.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2023-03-22 12:23:08.000000 manila-ui-9.0.0/.testr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4517 2023-03-22 12:23:08.000000 manila-ui-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3173 2023-03-22 12:23:36.000000 manila-ui-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-03-22 12:23:08.000000 manila-ui-9.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20968 2023-03-22 12:23:36.000000 manila-ui-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-03-22 12:23:08.000000 manila-ui-9.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-03-22 12:23:08.000000 manila-ui-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1720 2023-03-22 12:23:36.866940 manila-ui-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2023-03-22 12:23:08.000000 manila-ui-9.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-03-22 12:23:08.000000 manila-ui-9.0.0/babel-django.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-03-22 12:23:08.000000 manila-ui-9.0.0/babel-djangojs.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2023-03-22 12:23:08.000000 manila-ui-9.0.0/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2023-03-22 12:23:08.000000 manila-ui-9.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.758941 manila-ui-9.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1965 2023-03-22 12:23:08.000000 manila-ui-9.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-03-22 12:23:08.000000 manila-ui-9.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.758941 manila-ui-9.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-03-22 12:23:08.000000 manila-ui-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.758941 manila-ui-9.0.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.758941 manila-ui-9.0.0/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4434 2023-03-22 12:23:08.000000 manila-ui-9.0.0/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3520 2023-03-22 12:23:08.000000 manila-ui-9.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.758941 manila-ui-9.0.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1157 2023-03-22 12:23:08.000000 manila-ui-9.0.0/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.758941 manila-ui-9.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2228 2023-03-22 12:23:08.000000 manila-ui-9.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5929 2023-03-22 12:23:08.000000 manila-ui-9.0.0/doc/source/contributor/development-environment.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2023-03-22 12:23:08.000000 manila-ui-9.0.0/doc/source/contributor/features.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-03-22 12:23:08.000000 manila-ui-9.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2023-03-22 12:23:08.000000 manila-ui-9.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.758941 manila-ui-9.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2023-03-22 12:23:08.000000 manila-ui-9.0.0/doc/source/install/installation.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.758941 manila-ui-9.0.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7499 2023-03-22 12:23:08.000000 manila-ui-9.0.0/doc/source/user/index.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      826 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.762941 manila-ui-9.0.0/manila_ui/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.762941 manila-ui-9.0.0/manila_ui/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22767 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/api/manila.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/api/network.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.762941 manila-ui-9.0.0/manila_ui/conf/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.766940 manila-ui-9.0.0/manila_ui/conf/default_policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    64229 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/conf/default_policies/manila.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    70209 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/conf/manila_policy.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.766940 manila-ui-9.0.0/manila_ui/dashboards/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.766940 manila-ui-9.0.0/manila_ui/dashboards/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.766940 manila-ui-9.0.0/manila_ui/dashboards/admin/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/defaults/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1822 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/defaults/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1506 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/defaults/tabs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3802 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/defaults/workflows.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.766940 manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2415 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.734941 manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.770940 manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/templates/security_services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1120 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/templates/security_services/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/templates/security_services/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/templates/security_services/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2084 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.770940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1999 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4545 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1210 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.734941 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.770940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/templates/share_group_snapshots/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/templates/share_group_snapshots/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/templates/share_group_snapshots/_reset_status.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/templates/share_group_snapshots/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/templates/share_group_snapshots/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/templates/share_group_snapshots/reset_status.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1254 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5713 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.774940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5663 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3753 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.738941 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.774940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1727 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/_manage_access.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/manage_access.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4936 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4622 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/workflows.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.778940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1948 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3867 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1119 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.738941 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.778940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/templates/share_groups/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3357 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/templates/share_groups/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/templates/share_groups/_reset_status.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/templates/share_groups/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/templates/share_groups/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/templates/share_groups/reset_status.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1202 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5238 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.782940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3227 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1123 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.738941 manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.782940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/templates/share_instances/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2019 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/templates/share_instances/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/templates/share_instances/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/templates/share_instances/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3248 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.782940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.738941 manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.782940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/templates/share_networks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1732 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/templates/share_networks/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/templates/share_networks/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/templates/share_networks/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2815 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.786940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3956 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.738941 manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.786940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/templates/share_servers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/templates/share_servers/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/templates/share_servers/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/templates/share_servers/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3527 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.786940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4109 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.738941 manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.790940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/templates/share_snapshots/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2151 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/templates/share_snapshots/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/templates/share_snapshots/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/templates/share_snapshots/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2396 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.790940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6755 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      927 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3815 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.738941 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.794940 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/templates/share_types/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/templates/share_types/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1702 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/templates/share_types/_manage_access.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/templates/share_types/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/templates/share_types/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/templates/share_types/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/templates/share_types/manage_access.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/templates/share_types/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1180 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5299 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4396 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/workflows.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.794940 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13316 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      880 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.794940 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/replicas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/replicas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3907 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/replicas/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5148 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/replicas/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/replicas/tabs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6041 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/replicas/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5550 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1045 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.738941 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.798940 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3950 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/_manage_share.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/_migration_cancel.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/_migration_complete.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/_migration_get_progress.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/_migration_start.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/_unmanage_share.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/manage_share.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/migration_cancel.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/migration_complete.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/migration_get_progress.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/migration_start.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.802940 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/replicas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1480 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/replicas/_detail_overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/replicas/_reset_replica_state.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/replicas/_reset_replica_status.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/replicas/_resync_replica.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/replicas/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/replicas/manage_replicas.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/replicas/reset_replica_state.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/replicas/reset_replica_status.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/replicas/resync_replica.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/unmanage_share.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2833 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10174 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/shares/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.802940 manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1524 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      890 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.738941 manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.802940 manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/templates/user_messages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      881 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/templates/user_messages/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/templates/user_messages/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/templates/user_messages/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/admin/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.802940 manila-ui-9.0.0/manila_ui/dashboards/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/identity/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.802940 manila-ui-9.0.0/manila_ui/dashboards/identity/projects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/identity/projects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2962 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/identity/projects/workflows.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.802940 manila-ui-9.0.0/manila_ui/dashboards/project/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      758 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.806940 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5373 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2984 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.738941 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.806940 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/templates/security_services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1771 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/templates/security_services/_add.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/templates/security_services/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1120 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/templates/security_services/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/templates/security_services/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/templates/security_services/add.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/templates/security_services/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/templates/security_services/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/templates/security_services/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/templates/security_services/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6802 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/security_services/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.806940 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2946 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5708 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.738941 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.810940 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6826 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.810940 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11528 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5047 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.742941 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.810940 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/templates/share_groups/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/templates/share_groups/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2960 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/templates/share_groups/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/templates/share_groups/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/templates/share_groups/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/templates/share_groups/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/templates/share_groups/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/templates/share_groups/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1309 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5840 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.814940 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5667 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4676 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1028 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.742941 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.814940 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/templates/share_networks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/templates/share_networks/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2034 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/templates/share_networks/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/templates/share_networks/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/templates/share_networks/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/templates/share_networks/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/templates/share_networks/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/templates/share_networks/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1191 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6442 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6044 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/workflows.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.814940 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3776 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10214 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1081 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.742941 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.818940 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2147 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1278 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/_limits.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/_rule_add.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/manage_rules.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/rule_add.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1608 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9463 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.818940 manila-ui-9.0.0/manila_ui/dashboards/project/shares/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2332 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22327 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.822940 manila-ui-9.0.0/manila_ui/dashboards/project/shares/replicas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/replicas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2924 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/replicas/forms.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6198 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/replicas/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/replicas/tabs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6990 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/replicas/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15895 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.742941 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.826940 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4002 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2351 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/_limits.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/_manage_rules.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/_resize.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/_resize_limits.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/_revert.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/_rule_add.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/_update_metadata.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/_update_rule_metadata.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/manage_rules.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.826940 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/replicas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/replicas/_create_replica.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/replicas/_detail_overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/replicas/_set_replica_as_active.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/replicas/create_replica.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/replicas/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/replicas/manage_replicas.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/replicas/set_replica_as_active.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/resize.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/revert.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/rule_add.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/update_metadata.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/update_rule_metadata.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2827 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15628 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/shares/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.826940 manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3147 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1105 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.742941 manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.830940 manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/templates/user_messages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      881 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/templates/user_messages/_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/templates/user_messages/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/templates/user_messages/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2770 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4428 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/dashboards/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1933 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/features.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.830940 manila-ui-9.0.0/manila_ui/local/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.834940 manila-ui-9.0.0/manila_ui/local/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1394 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_80_manila_admin_add_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1038 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_80_manila_project_add_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9010_manila_admin_add_shares_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9010_manila_project_add_shares_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9020_manila_admin_add_share_snapshots_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9020_manila_project_add_share_snapshots_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9030_manila_admin_add_share_types_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9040_manila_admin_add_share_networks_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9040_manila_project_add_share_networks_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9050_manila_admin_add_security_services_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9050_manila_project_add_security_services_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      725 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9060_manila_admin_add_share_servers_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9070_manila_admin_add_share_instances_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9080_manila_admin_add_share_groups_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9080_manila_project_add_share_groups_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9085_manila_admin_add_share_group_snapshots_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      915 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9085_manila_project_add_share_group_snapshots_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9090_manila_admin_add_share_group_types_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9095_manila_admin_add_user_messages_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/_9095_manila_project_add_user_messages_panel_to_share_panel_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/enabled/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.834940 manila-ui-9.0.0/manila_ui/local/local_settings.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/local/local_settings.d/_90_manila_shares.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.742941 manila-ui-9.0.0/manila_ui/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.742941 manila-ui-9.0.0/manila_ui/locale/cs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.834940 manila-ui-9.0.0/manila_ui/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19745 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/locale/cs/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.742941 manila-ui-9.0.0/manila_ui/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.834940 manila-ui-9.0.0/manila_ui/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52747 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.742941 manila-ui-9.0.0/manila_ui/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.834940 manila-ui-9.0.0/manila_ui/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51593 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/locale/en_GB/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.742941 manila-ui-9.0.0/manila_ui/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.834940 manila-ui-9.0.0/manila_ui/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24493 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.742941 manila-ui-9.0.0/manila_ui/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.834940 manila-ui-9.0.0/manila_ui/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49877 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.742941 manila-ui-9.0.0/manila_ui/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.834940 manila-ui-9.0.0/manila_ui/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52058 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/locale/ko_KR/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.742941 manila-ui-9.0.0/manila_ui/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.834940 manila-ui-9.0.0/manila_ui/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51267 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.742941 manila-ui-9.0.0/manila_ui/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.834940 manila-ui-9.0.0/manila_ui/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31580 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.746940 manila-ui-9.0.0/manila_ui/locale/tr_TR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.834940 manila-ui-9.0.0/manila_ui/locale/tr_TR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39805 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/locale/tr_TR/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.838940 manila-ui-9.0.0/manila_ui/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.838940 manila-ui-9.0.0/manila_ui/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42967 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/api/test_manila.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.838940 manila-ui-9.0.0/manila_ui/tests/dashboards/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.838940 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.838940 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/security_services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/security_services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4014 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/security_services/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.838940 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_group_snapshots/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_group_snapshots/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8080 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_group_snapshots/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.838940 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_group_types/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_group_types/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4432 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_group_types/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.838940 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_groups/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_groups/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8218 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_groups/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.838940 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_instances/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_instances/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5112 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_instances/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.842940 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_networks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_networks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7783 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_networks/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.842940 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_servers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_servers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5404 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_servers/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.842940 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_snapshots/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_snapshots/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6758 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_snapshots/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.842940 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_types/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_types/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11152 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_types/test_forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3958 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_types/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.842940 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/shares/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/shares/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.842940 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/shares/replicas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/shares/replicas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14821 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/shares/replicas/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4248 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/shares/test_forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10547 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/shares/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.842940 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/user_messages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/user_messages/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4524 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/admin/user_messages/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.842940 manila-ui-9.0.0/manila_ui/tests/dashboards/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/identity/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.842940 manila-ui-9.0.0/manila_ui/tests/dashboards/identity/projects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/identity/projects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2851 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/identity/projects/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.842940 manila-ui-9.0.0/manila_ui/tests/dashboards/project/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.846940 manila-ui-9.0.0/manila_ui/tests/dashboards/project/security_services/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/security_services/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6809 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/security_services/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.846940 manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_group_snapshots/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_group_snapshots/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11871 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_group_snapshots/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.846940 manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_groups/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_groups/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16553 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_groups/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.846940 manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_networks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_networks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10156 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_networks/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.846940 manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_snapshots/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_snapshots/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2617 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_snapshots/test_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13146 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_snapshots/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.846940 manila-ui-9.0.0/manila_ui/tests/dashboards/project/shares/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/shares/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.846940 manila-ui-9.0.0/manila_ui/tests/dashboards/project/shares/replicas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/shares/replicas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13242 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/shares/replicas/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32370 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/shares/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20613 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/test_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.846940 manila-ui-9.0.0/manila_ui/tests/dashboards/project/user_messages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/user_messages/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4058 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/project/user_messages/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3482 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/dashboards/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/helpers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.850940 manila-ui-9.0.0/manila_ui/tests/integration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/horizon.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.850940 manila-ui-9.0.0/manila_ui/tests/integration/pages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.850940 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.850940 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/messagespage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/securityservicespage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharegroupsnapshotspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharegroupspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharegroupssnapshotspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharegrouptypespage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/shareinstancespage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharenetworkspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/shareserverspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharesnapshotspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharespage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharetypespage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.850940 manila-ui-9.0.0/manila_ui/tests/integration/pages/project/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/project/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.854940 manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/messagespage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/securityservicespage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/sharegroupsnapshotspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/sharegroupspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/sharenetworkspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/sharesnapshotspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/sharespage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4675 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/integration/test_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.854940 manila-ui-9.0.0/manila_ui/tests/test_data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/test_data/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/test_data/keystone_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/test_data/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/urls.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.854940 manila-ui-9.0.0/manila_ui/tests/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1469 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/tests/utils/tests.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.854940 manila-ui-9.0.0/manila_ui/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/manila_ui/utils/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.762941 manila-ui-9.0.0/manila_ui.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1720 2023-03-22 12:23:36.000000 manila-ui-9.0.0/manila_ui.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31040 2023-03-22 12:23:36.000000 manila-ui-9.0.0/manila_ui.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-22 12:23:36.000000 manila-ui-9.0.0/manila_ui.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-22 12:23:36.000000 manila-ui-9.0.0/manila_ui.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-22 12:23:36.000000 manila-ui-9.0.0/manila_ui.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-03-22 12:23:36.000000 manila-ui-9.0.0/manila_ui.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2023-03-22 12:23:36.000000 manila-ui-9.0.0/manila_ui.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.750941 manila-ui-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.862940 manila-ui-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/add-create-share-type-with-description-d57f4c734d107554.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/add-is-default-field-to-share-group-types-list-e0ed183e2e8df9ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/add-is-default-field-to-share-types-list-a76fed8ebe7eef03.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/add-maprfs-protocol-5d7f4b4c47da8fab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/add-revert-share-to-snapshot-support-cba6227cef75c1a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/add-share-access-rules-66a86a45a1f4a9c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      563 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/add-share-panel-group-to-admin-dashboard-ef6a02243c0e776c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/add-share-panel-group-to-project-dashboard-722ab48392588728.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/add-support-for-microversion-2-34-share-groups-fields-f447cd6563e377c1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/allow-access-to-ipv6-clients-2.38-154d308ec87bfb73.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bp-manila-mountable-snapshots-93a732ad0dc95ade.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bp-ocata-migration-improvements-e0ecccbe95e3c265.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bp-ui-user-messages-6ff935cabc516be0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bp-update-share-type-name-or-description-cc5357feee2a3b61.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1498433-42796ef1e266f4d3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1619244-1cc15914050d9a64.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1664370-drop-host-field-in-project-view-tables-20b7a67023d57d35.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1679960-fix-quota-names-overlapping-4277d45cd0110489.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1685655-drop-snapshot-support-param-a4e7c7ee068c8bc9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1685657-fix-create-share-from-snapshot-form-7f5993c1100ce9b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1702396-add-share-servers-to-share-network-details-1cff66010817f1a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1702396-fix-cannot-get-share-network-details-83e2882df1714506.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1783232-fix-quotas-retrieval-for-shares-and-snapshots-tables-63a1fc877029eac8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1787016-fix-share-replica-details-eecdc8b43f2a6008.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1823078-upgrade-api-to-v2.33-82871432659a8285.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1842119-fix-get-quotas-for-update-quotas-share-7f229e4e011004cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1931641-fix-handling-share-type-name-with-hyphens-8a9f16af36da5852.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1967312-fix-shares-panel-8b5da4eee68ba6c4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-1968925-fix-replica-creation-190321bf9fefe179.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-2004165-fix-type-listing-when-rbac-enabled-c01f363dfa574b9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/bug-873434-fix-set-as-active-button-visibility-e7cc416d66ab360b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/drop-python2-support-8f7cbc2c3a758777.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/field-encoder-update-7141766f0b5f8ecb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/filter-share-type-by-extra-spec-2.43-39710ce64f8be239.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/policy-in-code-support-23744e26a7f6e284.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/python-manilaclient-yoga-ef2c44b205fa216b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/raise-python-manilaclient-version-9caa15ec2c94968d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/remove-nova-net-plugin-4fdc0d944d93644f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/security-service-ou-field-2.44-c288a880b9b0fa68.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/share-shrinking-c1d46fc1c3ce29b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/notes/start-using-reno-49da440f5e237dda.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.866940 manila-ui-9.0.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.866940 manila-ui-9.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.866940 manila-ui-9.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8964 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.750941 manila-ui-9.0.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.750941 manila-ui-9.0.0/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.866940 manila-ui-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7323 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.750941 manila-ui-9.0.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.866940 manila-ui-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16452 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.750941 manila-ui-9.0.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.866940 manila-ui-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.750941 manila-ui-9.0.0/releasenotes/source/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.866940 manila-ui-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5840 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.750941 manila-ui-9.0.0/releasenotes/source/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.866940 manila-ui-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.750941 manila-ui-9.0.0/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.866940 manila-ui-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2080 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.750941 manila-ui-9.0.0/releasenotes/source/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.866940 manila-ui-9.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5774 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.750941 manila-ui-9.0.0/releasenotes/source/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.866940 manila-ui-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1878 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-22 12:23:08.000000 manila-ui-9.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2023-03-22 12:23:08.000000 manila-ui-9.0.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    16399 2023-03-22 12:23:08.000000 manila-ui-9.0.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2023-03-22 12:23:36.870940 manila-ui-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-03-22 12:23:08.000000 manila-ui-9.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2023-03-22 12:23:08.000000 manila-ui-9.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:23:36.866940 manila-ui-9.0.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2395 2023-03-22 12:23:08.000000 manila-ui-9.0.0/tools/cover.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2023-03-22 12:23:08.000000 manila-ui-9.0.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2473 2023-03-22 12:23:08.000000 manila-ui-9.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.479685 manila-ui-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/.testr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4517 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3173 2023-03-03 11:18:03.000000 manila-ui-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20978 2023-03-03 11:18:03.000000 manila-ui-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1725 2023-03-03 11:18:03.479685 manila-ui-9.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/babel-django.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/babel-djangojs.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.415670 manila-ui-9.0.0.0rc1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1965 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.415670 manila-ui-9.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.415670 manila-ui-9.0.0.0rc1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.415670 manila-ui-9.0.0.0rc1/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4434 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3520 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.415670 manila-ui-9.0.0.0rc1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1157 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.415670 manila-ui-9.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2228 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5929 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/doc/source/contributor/development-environment.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/doc/source/contributor/features.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.415670 manila-ui-9.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/doc/source/install/installation.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.415670 manila-ui-9.0.0.0rc1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7499 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/doc/source/user/index.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      826 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.415670 manila-ui-9.0.0.0rc1/manila_ui/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.415670 manila-ui-9.0.0.0rc1/manila_ui/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22767 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/api/manila.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/api/network.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.415670 manila-ui-9.0.0.0rc1/manila_ui/conf/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.419671 manila-ui-9.0.0.0rc1/manila_ui/conf/default_policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    64229 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/conf/default_policies/manila.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    70209 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/conf/manila_policy.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.419671 manila-ui-9.0.0.0rc1/manila_ui/dashboards/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.419671 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.419671 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/defaults/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1822 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/defaults/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1506 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/defaults/tabs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3802 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/defaults/workflows.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.419671 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2415 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.395666 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.419671 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/templates/security_services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1120 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/templates/security_services/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/templates/security_services/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/templates/security_services/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2084 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.419671 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1999 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4545 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1210 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.395666 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.419671 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/templates/share_group_snapshots/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/templates/share_group_snapshots/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/templates/share_group_snapshots/_reset_status.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/templates/share_group_snapshots/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/templates/share_group_snapshots/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/templates/share_group_snapshots/reset_status.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1254 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5713 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.423672 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5663 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3753 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.395666 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.423672 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1727 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/_manage_access.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/manage_access.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4936 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4622 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/workflows.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.423672 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1948 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3867 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1119 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.399667 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.423672 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/templates/share_groups/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3357 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/templates/share_groups/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/templates/share_groups/_reset_status.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/templates/share_groups/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/templates/share_groups/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/templates/share_groups/reset_status.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1202 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5238 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.423672 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3227 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1123 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.399667 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.427673 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/templates/share_instances/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2019 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/templates/share_instances/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/templates/share_instances/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/templates/share_instances/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3248 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.427673 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.399667 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.427673 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/templates/share_networks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1732 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/templates/share_networks/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/templates/share_networks/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/templates/share_networks/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2815 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.427673 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3956 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.399667 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.427673 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/templates/share_servers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/templates/share_servers/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/templates/share_servers/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/templates/share_servers/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3527 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.427673 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4109 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.399667 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.427673 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/templates/share_snapshots/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2151 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/templates/share_snapshots/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/templates/share_snapshots/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/templates/share_snapshots/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2396 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.431674 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6755 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      927 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3815 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.399667 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.431674 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/templates/share_types/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/templates/share_types/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1702 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/templates/share_types/_manage_access.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/templates/share_types/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/templates/share_types/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/templates/share_types/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/templates/share_types/manage_access.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/templates/share_types/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1180 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5299 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4396 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/workflows.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.431674 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13316 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      880 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.431674 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/replicas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/replicas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3907 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/replicas/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5148 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/replicas/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/replicas/tabs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6041 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/replicas/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5550 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1045 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.435675 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3950 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/_manage_share.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/_migration_cancel.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/_migration_complete.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/_migration_get_progress.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/_migration_start.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/_unmanage_share.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/manage_share.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/migration_cancel.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/migration_complete.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/migration_get_progress.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/migration_start.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.435675 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/replicas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1480 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/replicas/_detail_overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/replicas/_reset_replica_state.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/replicas/_reset_replica_status.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/replicas/_resync_replica.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/replicas/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/replicas/manage_replicas.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/replicas/reset_replica_state.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/replicas/reset_replica_status.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/replicas/resync_replica.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/unmanage_share.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2833 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10174 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.435675 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1524 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      890 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.435675 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/templates/user_messages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      881 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/templates/user_messages/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/templates/user_messages/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/templates/user_messages/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.435675 manila-ui-9.0.0.0rc1/manila_ui/dashboards/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/identity/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.435675 manila-ui-9.0.0.0rc1/manila_ui/dashboards/identity/projects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/identity/projects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2962 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/identity/projects/workflows.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.435675 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      758 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.439676 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5373 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2984 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.439676 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/templates/security_services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1771 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/templates/security_services/_add.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/templates/security_services/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1120 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/templates/security_services/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/templates/security_services/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/templates/security_services/add.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/templates/security_services/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/templates/security_services/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/templates/security_services/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/templates/security_services/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6802 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.439676 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2946 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5708 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.439676 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6826 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.443677 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11528 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5047 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.443677 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/templates/share_groups/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/templates/share_groups/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2960 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/templates/share_groups/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/templates/share_groups/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/templates/share_groups/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/templates/share_groups/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/templates/share_groups/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/templates/share_groups/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1309 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5840 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.443677 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5667 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4676 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1028 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.443677 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/templates/share_networks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/templates/share_networks/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2034 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/templates/share_networks/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/templates/share_networks/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/templates/share_networks/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/templates/share_networks/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/templates/share_networks/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/templates/share_networks/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1191 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6442 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6044 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/workflows.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.447678 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3776 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10214 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1081 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.447678 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2147 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1278 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/_limits.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/_rule_add.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/manage_rules.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/rule_add.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1608 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9463 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.447678 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2332 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22327 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.447678 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/replicas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/replicas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2924 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/replicas/forms.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6198 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/replicas/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/replicas/tabs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6990 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/replicas/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15895 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.451679 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4002 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2351 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/_limits.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/_manage_rules.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/_resize.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/_resize_limits.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/_revert.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/_rule_add.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/_update_metadata.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/_update_rule_metadata.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/manage_rules.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.451679 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/replicas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/replicas/_create_replica.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/replicas/_detail_overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/replicas/_set_replica_as_active.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/replicas/create_replica.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/replicas/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/replicas/manage_replicas.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/replicas/set_replica_as_active.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/resize.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/revert.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/rule_add.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/update_metadata.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/update_rule_metadata.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2827 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15628 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.451679 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3147 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1105 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.455680 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/templates/user_messages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      881 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/templates/user_messages/_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/templates/user_messages/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/templates/user_messages/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2770 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4428 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/dashboards/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1933 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/features.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.455680 manila-ui-9.0.0.0rc1/manila_ui/local/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.455680 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1394 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_80_manila_admin_add_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1038 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_80_manila_project_add_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9010_manila_admin_add_shares_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9010_manila_project_add_shares_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9020_manila_admin_add_share_snapshots_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9020_manila_project_add_share_snapshots_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9030_manila_admin_add_share_types_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9040_manila_admin_add_share_networks_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9040_manila_project_add_share_networks_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9050_manila_admin_add_security_services_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9050_manila_project_add_security_services_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      725 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9060_manila_admin_add_share_servers_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9070_manila_admin_add_share_instances_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9080_manila_admin_add_share_groups_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      867 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9080_manila_project_add_share_groups_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9085_manila_admin_add_share_group_snapshots_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      915 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9085_manila_project_add_share_group_snapshots_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9090_manila_admin_add_share_group_types_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9095_manila_admin_add_user_messages_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9095_manila_project_add_user_messages_panel_to_share_panel_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/enabled/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.455680 manila-ui-9.0.0.0rc1/manila_ui/local/local_settings.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/local/local_settings.d/_90_manila_shares.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.407669 manila-ui-9.0.0.0rc1/manila_ui/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/locale/cs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.455680 manila-ui-9.0.0.0rc1/manila_ui/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19745 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.455680 manila-ui-9.0.0.0rc1/manila_ui/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52747 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.455680 manila-ui-9.0.0.0rc1/manila_ui/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51593 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/locale/en_GB/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.455680 manila-ui-9.0.0.0rc1/manila_ui/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24493 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.455680 manila-ui-9.0.0.0rc1/manila_ui/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49877 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52058 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/locale/ko_KR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51267 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.403668 manila-ui-9.0.0.0rc1/manila_ui/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31580 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.407669 manila-ui-9.0.0.0rc1/manila_ui/locale/tr_TR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/locale/tr_TR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    39805 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/locale/tr_TR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42967 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/api/test_manila.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/security_services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/security_services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4014 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/security_services/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_group_snapshots/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_group_snapshots/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8080 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_group_snapshots/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_group_types/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_group_types/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4432 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_group_types/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_groups/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_groups/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8218 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_groups/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_instances/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_instances/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5112 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_instances/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_networks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_networks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7783 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_networks/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_servers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_servers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5404 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_servers/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.459680 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_snapshots/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_snapshots/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6758 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_snapshots/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_types/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_types/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11152 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_types/test_forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3958 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_types/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/shares/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/shares/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/shares/replicas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/shares/replicas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14821 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/shares/replicas/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4248 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/shares/test_forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10547 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/shares/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/user_messages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/user_messages/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4524 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/user_messages/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/identity/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/identity/projects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/identity/projects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2851 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/identity/projects/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/security_services/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/security_services/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6809 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/security_services/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_group_snapshots/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_group_snapshots/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11871 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_group_snapshots/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_groups/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_groups/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16553 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_groups/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_networks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_networks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10156 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_networks/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_snapshots/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_snapshots/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2617 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_snapshots/test_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13146 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_snapshots/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/shares/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/shares/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/shares/replicas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/shares/replicas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13242 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/shares/replicas/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32370 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/shares/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20613 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/test_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.463681 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/user_messages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/user_messages/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4058 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/user_messages/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3482 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.467682 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/horizon.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.467682 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.467682 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.467682 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/messagespage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/securityservicespage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharegroupsnapshotspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharegroupspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharegroupssnapshotspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharegrouptypespage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/shareinstancespage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharenetworkspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/shareserverspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharesnapshotspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharespage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharetypespage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.467682 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.467682 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/messagespage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/securityservicespage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/sharegroupsnapshotspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/sharegroupspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/sharenetworkspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/sharesnapshotspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/sharespage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4675 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/integration/test_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.467682 manila-ui-9.0.0.0rc1/manila_ui/tests/test_data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/test_data/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/test_data/keystone_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/test_data/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.467682 manila-ui-9.0.0.0rc1/manila_ui/tests/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1469 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/tests/utils/tests.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.471683 manila-ui-9.0.0.0rc1/manila_ui/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/manila_ui/utils/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.415670 manila-ui-9.0.0.0rc1/manila_ui.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1725 2023-03-03 11:18:03.000000 manila-ui-9.0.0.0rc1/manila_ui.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31040 2023-03-03 11:18:03.000000 manila-ui-9.0.0.0rc1/manila_ui.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-03 11:18:03.000000 manila-ui-9.0.0.0rc1/manila_ui.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-03 11:18:03.000000 manila-ui-9.0.0.0rc1/manila_ui.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-03 11:18:03.000000 manila-ui-9.0.0.0rc1/manila_ui.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-03-03 11:18:03.000000 manila-ui-9.0.0.0rc1/manila_ui.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2023-03-03 11:18:03.000000 manila-ui-9.0.0.0rc1/manila_ui.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.407669 manila-ui-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.475684 manila-ui-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/add-create-share-type-with-description-d57f4c734d107554.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/add-is-default-field-to-share-group-types-list-e0ed183e2e8df9ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/add-is-default-field-to-share-types-list-a76fed8ebe7eef03.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/add-maprfs-protocol-5d7f4b4c47da8fab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/add-revert-share-to-snapshot-support-cba6227cef75c1a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/add-share-access-rules-66a86a45a1f4a9c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      563 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/add-share-panel-group-to-admin-dashboard-ef6a02243c0e776c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/add-share-panel-group-to-project-dashboard-722ab48392588728.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/add-support-for-microversion-2-34-share-groups-fields-f447cd6563e377c1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/allow-access-to-ipv6-clients-2.38-154d308ec87bfb73.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bp-manila-mountable-snapshots-93a732ad0dc95ade.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bp-ocata-migration-improvements-e0ecccbe95e3c265.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bp-ui-user-messages-6ff935cabc516be0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bp-update-share-type-name-or-description-cc5357feee2a3b61.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1498433-42796ef1e266f4d3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1619244-1cc15914050d9a64.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1664370-drop-host-field-in-project-view-tables-20b7a67023d57d35.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1679960-fix-quota-names-overlapping-4277d45cd0110489.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1685655-drop-snapshot-support-param-a4e7c7ee068c8bc9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1685657-fix-create-share-from-snapshot-form-7f5993c1100ce9b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1702396-add-share-servers-to-share-network-details-1cff66010817f1a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1702396-fix-cannot-get-share-network-details-83e2882df1714506.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1783232-fix-quotas-retrieval-for-shares-and-snapshots-tables-63a1fc877029eac8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1787016-fix-share-replica-details-eecdc8b43f2a6008.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1823078-upgrade-api-to-v2.33-82871432659a8285.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1842119-fix-get-quotas-for-update-quotas-share-7f229e4e011004cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1931641-fix-handling-share-type-name-with-hyphens-8a9f16af36da5852.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1967312-fix-shares-panel-8b5da4eee68ba6c4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-1968925-fix-replica-creation-190321bf9fefe179.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-2004165-fix-type-listing-when-rbac-enabled-c01f363dfa574b9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/bug-873434-fix-set-as-active-button-visibility-e7cc416d66ab360b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/drop-python2-support-8f7cbc2c3a758777.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/field-encoder-update-7141766f0b5f8ecb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/filter-share-type-by-extra-spec-2.43-39710ce64f8be239.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/policy-in-code-support-23744e26a7f6e284.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/python-manilaclient-yoga-ef2c44b205fa216b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/raise-python-manilaclient-version-9caa15ec2c94968d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/remove-nova-net-plugin-4fdc0d944d93644f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/security-service-ou-field-2.44-c288a880b9b0fa68.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/share-shrinking-c1d46fc1c3ce29b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/notes/start-using-reno-49da440f5e237dda.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.475684 manila-ui-9.0.0.0rc1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.475684 manila-ui-9.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.475684 manila-ui-9.0.0.0rc1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8964 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.411670 manila-ui-9.0.0.0rc1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.407669 manila-ui-9.0.0.0rc1/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.475684 manila-ui-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7323 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.407669 manila-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.475684 manila-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16452 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.407669 manila-ui-9.0.0.0rc1/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.475684 manila-ui-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.407669 manila-ui-9.0.0.0rc1/releasenotes/source/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.479685 manila-ui-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5840 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.407669 manila-ui-9.0.0.0rc1/releasenotes/source/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.479685 manila-ui-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.411670 manila-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.479685 manila-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2080 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.411670 manila-ui-9.0.0.0rc1/releasenotes/source/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.479685 manila-ui-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5774 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.411670 manila-ui-9.0.0.0rc1/releasenotes/source/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.479685 manila-ui-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1878 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    16399 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2023-03-03 11:18:03.479685 manila-ui-9.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-03 11:18:03.479685 manila-ui-9.0.0.0rc1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2395 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/tools/cover.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2473 2023-03-03 11:17:25.000000 manila-ui-9.0.0.0rc1/tox.ini
```

### Comparing `manila-ui-9.0.0/.zuul.yaml` & `manila-ui-9.0.0.0rc1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/AUTHORS` & `manila-ui-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/CONTRIBUTING.rst` & `manila-ui-9.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/ChangeLog` & `manila-ui-9.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * Fix "Set as Active" button's display for replicas
 * Fix coverage job from running with tox4
 * Imported Translations from Zanata
 * Support capital letter in share type name
 * Fix getting len() attr from boolean values
 * Add update share-type name description and/or public access
```

### Comparing `manila-ui-9.0.0/LICENSE` & `manila-ui-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/PKG-INFO` & `manila-ui-9.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: manila-ui
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Manila Management Dashboard
 Home-page: https://docs.openstack.org/manila-ui/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Team and repository tags
         ------------------------
```

### Comparing `manila-ui-9.0.0/README.rst` & `manila-ui-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/bindep.txt` & `manila-ui-9.0.0.0rc1/bindep.txt`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/devstack/plugin.sh` & `manila-ui-9.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/doc/source/admin/index.rst` & `manila-ui-9.0.0.0rc1/doc/source/admin/index.rst`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/doc/source/conf.py` & `manila-ui-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/doc/source/configuration/index.rst` & `manila-ui-9.0.0.0rc1/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/doc/source/contributor/contributing.rst` & `manila-ui-9.0.0.0rc1/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/doc/source/contributor/development-environment.rst` & `manila-ui-9.0.0.0rc1/doc/source/contributor/development-environment.rst`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/doc/source/contributor/features.rst` & `manila-ui-9.0.0.0rc1/doc/source/contributor/features.rst`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/doc/source/index.rst` & `manila-ui-9.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/doc/source/install/installation.rst` & `manila-ui-9.0.0.0rc1/doc/source/install/installation.rst`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/doc/source/user/index.rst` & `manila-ui-9.0.0.0rc1/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manage.py` & `manila-ui-9.0.0.0rc1/manage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/__init__.py` & `manila-ui-9.0.0.0rc1/manila_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/api/manila.py` & `manila-ui-9.0.0.0rc1/manila_ui/api/manila.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/api/network.py` & `manila-ui-9.0.0.0rc1/manila_ui/api/network.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/conf/default_policies/manila.yaml` & `manila-ui-9.0.0.0rc1/manila_ui/conf/default_policies/manila.yaml`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/conf/manila_policy.yaml` & `manila-ui-9.0.0.0rc1/manila_ui/conf/manila_policy.yaml`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/defaults/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/defaults/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/defaults/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/defaults/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/defaults/workflows.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/defaults/workflows.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/templates/security_services/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/templates/security_services/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/security_services/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/security_services/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/templates/share_group_snapshots/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/templates/share_group_snapshots/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_snapshots/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_snapshots/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/_manage_access.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/_manage_access.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/_update.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/templates/share_group_types/_update.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_group_types/workflows.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_group_types/workflows.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/templates/share_groups/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/templates/share_groups/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_groups/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_groups/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/templates/share_instances/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/templates/share_instances/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_instances/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_instances/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/templates/share_networks/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/templates/share_networks/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_networks/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_networks/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/templates/share_servers/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/templates/share_servers/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_servers/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_servers/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/templates/share_snapshots/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/templates/share_snapshots/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_snapshots/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_snapshots/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/templates/share_types/_create.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/templates/share_types/_create.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/templates/share_types/_manage_access.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/templates/share_types/_manage_access.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/templates/share_types/_update.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/templates/share_types/_update.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/share_types/workflows.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/share_types/workflows.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/shares/forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/shares/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/shares/replicas/forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/replicas/forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/shares/replicas/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/replicas/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/shares/replicas/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/replicas/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/shares/replicas/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/replicas/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/shares/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/shares/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/shares/templates/shares/replicas/_detail_overview.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/templates/shares/replicas/_detail_overview.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/shares/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/shares/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/shares/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/templates/user_messages/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/templates/user_messages/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/user_messages/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/user_messages/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/admin/utils.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/admin/utils.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/identity/projects/workflows.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/identity/projects/workflows.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/__init__.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/config.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/config.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/security_services/forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/security_services/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/security_services/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/security_services/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/security_services/templates/security_services/_add.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/templates/security_services/_add.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/security_services/templates/security_services/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/templates/security_services/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/security_services/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/security_services/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/security_services/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/templates/share_group_snapshots/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_group_snapshots/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_group_snapshots/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/templates/share_groups/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/templates/share_groups/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_groups/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_groups/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/templates/share_networks/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/templates/share_networks/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/templates/share_networks/_update.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/templates/share_networks/_update.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_networks/workflows.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_networks/workflows.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/_limits.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/templates/share_snapshots/_limits.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/share_snapshots/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/share_snapshots/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/__init__.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/replicas/forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/replicas/forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/replicas/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/replicas/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/replicas/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/replicas/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/replicas/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/replicas/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/_limits.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/_limits.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/_resize_limits.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/_resize_limits.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/templates/shares/replicas/_detail_overview.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/templates/shares/replicas/_detail_overview.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/shares/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/shares/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/panel.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/panel.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/tabs.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/tabs.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/templates/user_messages/_detail.html` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/templates/user_messages/_detail.html`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/project/user_messages/views.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/project/user_messages/views.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/dashboards/utils.py` & `manila-ui-9.0.0.0rc1/manila_ui/dashboards/utils.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/exceptions.py` & `manila-ui-9.0.0.0rc1/manila_ui/exceptions.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/features.py` & `manila-ui-9.0.0.0rc1/manila_ui/features.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_80_manila_admin_add_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_80_manila_admin_add_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_80_manila_project_add_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_80_manila_project_add_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9010_manila_admin_add_shares_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9010_manila_admin_add_shares_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9010_manila_project_add_shares_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9010_manila_project_add_shares_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9020_manila_admin_add_share_snapshots_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9020_manila_admin_add_share_snapshots_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9020_manila_project_add_share_snapshots_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9020_manila_project_add_share_snapshots_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9030_manila_admin_add_share_types_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9030_manila_admin_add_share_types_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9040_manila_admin_add_share_networks_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9040_manila_admin_add_share_networks_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9040_manila_project_add_share_networks_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9040_manila_project_add_share_networks_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9050_manila_admin_add_security_services_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9050_manila_admin_add_security_services_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9050_manila_project_add_security_services_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9050_manila_project_add_security_services_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9060_manila_admin_add_share_servers_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9060_manila_admin_add_share_servers_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9070_manila_admin_add_share_instances_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9070_manila_admin_add_share_instances_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9080_manila_admin_add_share_groups_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9080_manila_admin_add_share_groups_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9080_manila_project_add_share_groups_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9080_manila_project_add_share_groups_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9085_manila_admin_add_share_group_snapshots_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9085_manila_admin_add_share_group_snapshots_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9085_manila_project_add_share_group_snapshots_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9085_manila_project_add_share_group_snapshots_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9090_manila_admin_add_share_group_types_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9090_manila_admin_add_share_group_types_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9095_manila_admin_add_user_messages_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9095_manila_admin_add_user_messages_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/enabled/_9095_manila_project_add_user_messages_panel_to_share_panel_group.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/enabled/_9095_manila_project_add_user_messages_panel_to_share_panel_group.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/local/local_settings.d/_90_manila_shares.py` & `manila-ui-9.0.0.0rc1/manila_ui/local/local_settings.d/_90_manila_shares.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/locale/cs/LC_MESSAGES/django.po` & `manila-ui-9.0.0.0rc1/manila_ui/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/locale/de/LC_MESSAGES/django.po` & `manila-ui-9.0.0.0rc1/manila_ui/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/locale/en_GB/LC_MESSAGES/django.po` & `manila-ui-9.0.0.0rc1/manila_ui/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/locale/fr/LC_MESSAGES/django.po` & `manila-ui-9.0.0.0rc1/manila_ui/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/locale/id/LC_MESSAGES/django.po` & `manila-ui-9.0.0.0rc1/manila_ui/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/locale/ko_KR/LC_MESSAGES/django.po` & `manila-ui-9.0.0.0rc1/manila_ui/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/locale/pt_BR/LC_MESSAGES/django.po` & `manila-ui-9.0.0.0rc1/manila_ui/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/locale/ru/LC_MESSAGES/django.po` & `manila-ui-9.0.0.0rc1/manila_ui/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/locale/tr_TR/LC_MESSAGES/django.po` & `manila-ui-9.0.0.0rc1/manila_ui/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/api/test_manila.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/api/test_manila.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/admin/security_services/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/security_services/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_group_snapshots/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_group_snapshots/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_group_types/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_group_types/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_groups/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_groups/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_instances/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_instances/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_networks/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_networks/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_servers/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_servers/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_snapshots/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_snapshots/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_types/test_forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_types/test_forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/admin/share_types/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/share_types/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/admin/shares/replicas/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/shares/replicas/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/admin/shares/test_forms.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/shares/test_forms.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/admin/shares/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/shares/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/admin/user_messages/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/admin/user_messages/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/identity/projects/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/identity/projects/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/project/security_services/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/security_services/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_group_snapshots/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_group_snapshots/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_groups/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_groups/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_networks/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_networks/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_snapshots/test_tables.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_snapshots/test_tables.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/project/share_snapshots/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/share_snapshots/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/project/shares/replicas/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/shares/replicas/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/project/shares/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/shares/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/project/test_data.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/test_data.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/project/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/project/user_messages/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/project/user_messages/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/dashboards/test_utils.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/dashboards/test_utils.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/helpers.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/messagespage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/messagespage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/securityservicespage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/securityservicespage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharegroupsnapshotspage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharegroupsnapshotspage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharegroupspage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharegroupspage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharegroupssnapshotspage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharegroupssnapshotspage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharegrouptypespage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharegrouptypespage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/shareinstancespage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/shareinstancespage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharenetworkspage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharenetworkspage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/shareserverspage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/shareserverspage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharesnapshotspage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharesnapshotspage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharespage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharespage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/admin/share/sharetypespage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/admin/share/sharetypespage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/messagespage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/messagespage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/securityservicespage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/securityservicespage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/sharegroupsnapshotspage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/sharegroupsnapshotspage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/sharegroupspage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/sharegroupspage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/sharenetworkspage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/sharenetworkspage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/sharesnapshotspage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/sharesnapshotspage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/pages/project/share/sharespage.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/pages/project/share/sharespage.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/integration/test_basic.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/settings.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/settings.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/test_data/keystone_data.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/test_data/keystone_data.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/test_data/utils.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/test_data/utils.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/urls.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/urls.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui/tests/utils/tests.py` & `manila-ui-9.0.0.0rc1/manila_ui/tests/utils/tests.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/manila_ui.egg-info/PKG-INFO` & `manila-ui-9.0.0.0rc1/manila_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: manila-ui
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Manila Management Dashboard
 Home-page: https://docs.openstack.org/manila-ui/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Team and repository tags
         ------------------------
```

### Comparing `manila-ui-9.0.0/manila_ui.egg-info/SOURCES.txt` & `manila-ui-9.0.0.0rc1/manila_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/releasenotes/notes/add-share-panel-group-to-admin-dashboard-ef6a02243c0e776c.yaml` & `manila-ui-9.0.0.0rc1/releasenotes/notes/add-share-panel-group-to-admin-dashboard-ef6a02243c0e776c.yaml`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/releasenotes/notes/add-share-panel-group-to-project-dashboard-722ab48392588728.yaml` & `manila-ui-9.0.0.0rc1/releasenotes/notes/add-share-panel-group-to-project-dashboard-722ab48392588728.yaml`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/releasenotes/source/conf.py` & `manila-ui-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `manila-ui-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `manila-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `manila-ui-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po` & `manila-ui-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po` & `manila-ui-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `manila-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po` & `manila-ui-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po` & `manila-ui-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/requirements.txt` & `manila-ui-9.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/run_tests.sh` & `manila-ui-9.0.0.0rc1/run_tests.sh`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/setup.cfg` & `manila-ui-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/setup.py` & `manila-ui-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/test-requirements.txt` & `manila-ui-9.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/tools/cover.sh` & `manila-ui-9.0.0.0rc1/tools/cover.sh`

 * *Files identical despite different names*

### Comparing `manila-ui-9.0.0/tox.ini` & `manila-ui-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

