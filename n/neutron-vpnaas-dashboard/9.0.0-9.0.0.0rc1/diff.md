# Comparing `tmp/neutron-vpnaas-dashboard-9.0.0.tar.gz` & `tmp/neutron-vpnaas-dashboard-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutron-vpnaas-dashboard-9.0.0.tar", last modified: Wed Oct  4 11:15:51 2023, max compression
+gzip compressed data, was "neutron-vpnaas-dashboard-9.0.0.0rc1.tar", last modified: Thu Sep 14 01:41:49 2023, max compression
```

## Comparing `neutron-vpnaas-dashboard-9.0.0.tar` & `neutron-vpnaas-dashboard-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.609139 neutron-vpnaas-dashboard-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2023-10-04 11:15:51.000000 neutron-vpnaas-dashboard-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6626 2023-10-04 11:15:51.000000 neutron-vpnaas-dashboard-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1519 2023-10-04 11:15:51.609139 neutron-vpnaas-dashboard-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/babel-django.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/babel-djangojs.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.569189 neutron-vpnaas-dashboard-9.0.0/deliverables/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.585169 neutron-vpnaas-dashboard-9.0.0/deliverables/pike/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/deliverables/pike/neutron-vpnaas-dashboard.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.585169 neutron-vpnaas-dashboard-9.0.0/deliverables/queens/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/deliverables/queens/neutron-vpnaas-dashboard.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.585169 neutron-vpnaas-dashboard-9.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/devstack/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2131 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.585169 neutron-vpnaas-dashboard-9.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.585169 neutron-vpnaas-dashboard-9.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6826 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.585169 neutron-vpnaas-dashboard-9.0.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.585169 neutron-vpnaas-dashboard-9.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/doc/source/contributor/devstack-plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.585169 neutron-vpnaas-dashboard-9.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2485 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/doc/source/install/index.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      848 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/manage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.589164 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.589164 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17650 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/api/vpn.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.589164 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.589164 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.593159 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15480 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1640 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19174 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10351 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.573184 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.597154 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_add_endpoint_group_help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1044 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_add_ike_policy_help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1038 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_add_ipsec_policy_help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_add_vpn_service_help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_endpointgroup_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_ikepolicy_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_ipsecpolicy_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3010 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_ipsecsiteconnection_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_update_endpointgroup.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_update_ikepolicy.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_update_ipsecpolicy.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_update_ipsecsiteconnection.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_update_vpnservice.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_vpn_ips.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1929 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_vpnservice_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/update_endpointgroup.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/update_ikepolicy.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/update_ipsecpolicy.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/update_ipsecsiteconnection.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/update_vpnservice.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43886 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2849 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18275 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28156 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/workflows.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.597154 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/enabled/_7100_project_vpn_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/enabled/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.597154 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.573184 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.597154 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24778 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.573184 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.597154 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23388 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/en_GB/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.573184 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.597154 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22850 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.573184 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.597154 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25663 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/ja/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.573184 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.601149 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24551 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/ko_KR/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.573184 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.601149 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8887 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.573184 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.601149 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32028 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.573184 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/tr_TR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.601149 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/tr_TR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8452 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/tr_TR/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.573184 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/zh_Hans/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.601149 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21573 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/zh_Hans/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.601149 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.601149 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/api_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/api_tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17524 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/api_tests/test_vpnaas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1844 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.601149 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/test_data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/test_data/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1001 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/test_data/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9818 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/test_data/vpnaas_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.589164 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1519 2023-10-04 11:15:51.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6193 2023-10-04 11:15:51.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-10-04 11:15:51.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-10-04 11:15:51.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-10-04 11:15:51.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-10-04 11:15:51.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2023-10-04 11:15:51.000000 neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.577179 neutron-vpnaas-dashboard-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.605144 neutron-vpnaas-dashboard-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/notes/add-aggressive-negotiation-mode-ad665f5cfda2e08b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/notes/add-more-formats-to-ipsec-site-connection-e105363b9125b1ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/notes/auth-algorithm-fbfe0831ab8dc346.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/notes/django2-support-ef2f2bd52a8bb63f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/notes/drop-py-2-7-bfbdac2889ac051a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/notes/drop-python-3-6-and-3-7-39c229fcb744870f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/notes/endpoint-group-3bb4083130952d17.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/notes/split-out-from-horizon-4807f953d5dc0799.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.609139 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6759 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.577179 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.577179 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/cs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.609139 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/cs/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.577179 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.609139 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4509 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.577179 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.609139 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5014 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.577179 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.609139 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.577179 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.609139 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.577179 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.609139 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3528 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.577179 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.609139 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1062 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.577179 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.609139 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1606 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.577179 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.609139 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.577179 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.609139 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5141 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.577179 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:15:51.609139 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2023-10-04 11:15:51.613134 neutron-vpnaas-dashboard-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2595 2023-10-04 11:15:19.000000 neutron-vpnaas-dashboard-9.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.009537 neutron-vpnaas-dashboard-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2023-09-14 01:41:48.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6636 2023-09-14 01:41:48.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1524 2023-09-14 01:41:49.009537 neutron-vpnaas-dashboard-9.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/babel-django.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/babel-djangojs.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.981538 neutron-vpnaas-dashboard-9.0.0.0rc1/deliverables/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.989538 neutron-vpnaas-dashboard-9.0.0.0rc1/deliverables/pike/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/deliverables/pike/neutron-vpnaas-dashboard.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.989538 neutron-vpnaas-dashboard-9.0.0.0rc1/deliverables/queens/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/deliverables/queens/neutron-vpnaas-dashboard.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.989538 neutron-vpnaas-dashboard-9.0.0.0rc1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/devstack/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2131 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.989538 neutron-vpnaas-dashboard-9.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.989538 neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6826 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.989538 neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.989538 neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/contributor/devstack-plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.989538 neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2485 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/install/index.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      848 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/manage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.993538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.993538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17650 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/api/vpn.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.993538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.993538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.993538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15480 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1640 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19174 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10351 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.981538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.997538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_add_endpoint_group_help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1044 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_add_ike_policy_help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1038 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_add_ipsec_policy_help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_add_vpn_service_help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_endpointgroup_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_ikepolicy_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_ipsecpolicy_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3010 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_ipsecsiteconnection_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_update_endpointgroup.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_update_ikepolicy.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_update_ipsecpolicy.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_update_ipsecsiteconnection.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_update_vpnservice.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_vpn_ips.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1929 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_vpnservice_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/update_endpointgroup.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/update_ikepolicy.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/update_ipsecpolicy.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/update_ipsecsiteconnection.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/update_vpnservice.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43886 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2849 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18275 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28156 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/workflows.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.997538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/enabled/_7100_project_vpn_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/enabled/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.001537 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.981538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.001537 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24778 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.981538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.001537 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23388 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/en_GB/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.981538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.001537 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22850 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.981538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.001537 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25663 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.981538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.001537 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24551 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/ko_KR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.001537 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8887 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.001537 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32028 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/tr_TR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.001537 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/tr_TR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8452 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/tr_TR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/zh_Hans/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.001537 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21573 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/zh_Hans/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.001537 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.001537 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/api_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/api_tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17524 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/api_tests/test_vpnaas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1844 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.001537 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/test_data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/test_data/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1001 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/test_data/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9818 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/test_data/vpnaas_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.993538 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1524 2023-09-14 01:41:48.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6193 2023-09-14 01:41:48.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-09-14 01:41:48.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-09-14 01:41:48.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-09-14 01:41:48.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-09-14 01:41:48.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2023-09-14 01:41:48.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.005537 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/notes/add-aggressive-negotiation-mode-ad665f5cfda2e08b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/notes/add-more-formats-to-ipsec-site-connection-e105363b9125b1ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/notes/auth-algorithm-fbfe0831ab8dc346.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/notes/django2-support-ef2f2bd52a8bb63f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/notes/drop-py-2-7-bfbdac2889ac051a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/notes/drop-python-3-6-and-3-7-39c229fcb744870f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/notes/endpoint-group-3bb4083130952d17.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/notes/split-out-from-horizon-4807f953d5dc0799.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.005537 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6759 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/cs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.005537 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/cs/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.009537 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4509 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.009537 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5014 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.009537 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.009537 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.009537 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3528 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.009537 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1062 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.009537 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1606 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.009537 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.009537 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5141 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:48.985538 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-14 01:41:49.009537 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2023-09-14 01:41:49.009537 neutron-vpnaas-dashboard-9.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2595 2023-09-14 01:41:24.000000 neutron-vpnaas-dashboard-9.0.0.0rc1/tox.ini
```

### Comparing `neutron-vpnaas-dashboard-9.0.0/AUTHORS` & `neutron-vpnaas-dashboard-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/CONTRIBUTING.rst` & `neutron-vpnaas-dashboard-9.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/ChangeLog` & `neutron-vpnaas-dashboard-9.0.0.0rc1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * setup.cfg: Replace dashes with underscores
 * Imported Translations from Zanata
 * Update master for stable/2023.1
 
 8.0.0
 -----
```

### Comparing `neutron-vpnaas-dashboard-9.0.0/LICENSE` & `neutron-vpnaas-dashboard-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/PKG-INFO` & `neutron-vpnaas-dashboard-9.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: neutron-vpnaas-dashboard
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Neutron VPNaaS Dashboard
 Home-page: https://docs.openstack.org/neutron-vpnaas-dashboard/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Neutron VPNaaS Dashboard
```

### Comparing `neutron-vpnaas-dashboard-9.0.0/README.rst` & `neutron-vpnaas-dashboard-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/deliverables/pike/neutron-vpnaas-dashboard.yaml` & `neutron-vpnaas-dashboard-9.0.0.0rc1/deliverables/pike/neutron-vpnaas-dashboard.yaml`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/devstack/README.rst` & `neutron-vpnaas-dashboard-9.0.0.0rc1/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/devstack/plugin.sh` & `neutron-vpnaas-dashboard-9.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/doc/source/conf.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/doc/source/configuration/index.rst` & `neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/doc/source/contributor/index.rst` & `neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/doc/source/index.rst` & `neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/doc/source/install/index.rst` & `neutron-vpnaas-dashboard-9.0.0.0rc1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/manage.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/manage.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/api/vpn.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/api/vpn.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/forms.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/forms.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/panel.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/panel.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/tables.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/tables.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/tabs.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/tabs.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_add_ike_policy_help.html` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_add_ike_policy_help.html`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_add_ipsec_policy_help.html` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_add_ipsec_policy_help.html`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_add_vpn_service_help.html` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_add_vpn_service_help.html`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_endpointgroup_details.html` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_endpointgroup_details.html`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_ikepolicy_details.html` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_ikepolicy_details.html`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_ipsecpolicy_details.html` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_ipsecpolicy_details.html`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_ipsecsiteconnection_details.html` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_ipsecsiteconnection_details.html`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_vpnservice_details.html` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/templates/vpn/_vpnservice_details.html`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/tests.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/tests.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/urls.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/urls.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/views.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/views.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/dashboards/project/vpn/workflows.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/dashboards/project/vpn/workflows.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/enabled/_7100_project_vpn_panel.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/enabled/_7100_project_vpn_panel.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/de/LC_MESSAGES/django.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/en_GB/LC_MESSAGES/django.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/id/LC_MESSAGES/django.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/ja/LC_MESSAGES/django.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/ko_KR/LC_MESSAGES/django.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/pt_BR/LC_MESSAGES/django.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/ru/LC_MESSAGES/django.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/tr_TR/LC_MESSAGES/django.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/locale/zh_Hans/LC_MESSAGES/django.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/api_tests/test_vpnaas.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/api_tests/test_vpnaas.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/helpers.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/helpers.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/settings.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/settings.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/test_data/utils.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/test_data/utils.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/test/test_data/vpnaas_data.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/test/test_data/vpnaas_data.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard/version.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard/version.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard.egg-info/PKG-INFO` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: neutron-vpnaas-dashboard
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Neutron VPNaaS Dashboard
 Home-page: https://docs.openstack.org/neutron-vpnaas-dashboard/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Neutron VPNaaS Dashboard
```

### Comparing `neutron-vpnaas-dashboard-9.0.0/neutron_vpnaas_dashboard.egg-info/SOURCES.txt` & `neutron-vpnaas-dashboard-9.0.0.0rc1/neutron_vpnaas_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/releasenotes/source/conf.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/cs/LC_MESSAGES/releasenotes.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/cs/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po` & `neutron-vpnaas-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/requirements.txt` & `neutron-vpnaas-dashboard-9.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/setup.cfg` & `neutron-vpnaas-dashboard-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/setup.py` & `neutron-vpnaas-dashboard-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `neutron-vpnaas-dashboard-9.0.0/tox.ini` & `neutron-vpnaas-dashboard-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

