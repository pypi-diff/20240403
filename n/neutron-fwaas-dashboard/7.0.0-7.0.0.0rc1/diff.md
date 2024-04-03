# Comparing `tmp/neutron-fwaas-dashboard-7.0.0.tar.gz` & `tmp/neutron-fwaas-dashboard-7.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neutron-fwaas-dashboard-7.0.0.tar", last modified: Wed Apr  3 11:52:26 2024, max compression
+gzip compressed data, was "neutron-fwaas-dashboard-7.0.0.0rc1.tar", last modified: Thu Mar 14 07:08:52 2024, max compression
```

## Comparing `neutron-fwaas-dashboard-7.0.0.tar` & `neutron-fwaas-dashboard-7.0.0.0rc1.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.922448 neutron-fwaas-dashboard-7.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1023 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1188 2024-04-03 11:52:26.000000 neutron-fwaas-dashboard-7.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7954 2024-04-03 11:52:26.000000 neutron-fwaas-dashboard-7.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      470 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1480 2024-04-03 11:52:26.922448 neutron-fwaas-dashboard-7.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/babel-django.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/babel-djangojs.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.906448 neutron-fwaas-dashboard-7.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      965 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/devstack/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2563 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.898448 neutron-fwaas-dashboard-7.0.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.906448 neutron-fwaas-dashboard-7.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7053 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.906448 neutron-fwaas-dashboard-7.0.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.906448 neutron-fwaas-dashboard-7.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/doc/source/contributor/devstack-plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      996 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1373 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.906448 neutron-fwaas-dashboard-7.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3141 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.906448 neutron-fwaas-dashboard-7.0.0/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/etc/neutron-fwaas-policy.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      847 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/manage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.906448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.910448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11340 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/api/fwaas_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.910448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.910448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.910448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18766 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15725 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5590 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.914448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_addport.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_firewallgroup_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_insert_rule_to_policy.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_policy_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_remove_rule_from_policy.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_removeport.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_rule_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_update_port_help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_update_ports.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_update_rule_help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_update_rules.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_updatefirewall.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_updatepolicy.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_updaterule.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/addfirewallgroup.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/addpolicy.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/addport.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/addrule.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/details_tabs.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/insert_rule_to_policy.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/remove_rule_from_policy.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/removeport.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3139 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/table_select.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/updatefirewall.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/updatepolicy.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/updaterule.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32306 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2691 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16837 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8556 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/widgets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15441 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/workflows.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.914448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/enabled/_7010_project_firewalls_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/enabled/_7012_project_firewalls_v2_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/enabled/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.914448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/local_settings.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      677 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/local_settings.d/_7000_neutron_fwaas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.914448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.914448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18488 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.914448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16820 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/en_GB/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.914448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14080 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.914448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17490 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/id/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.914448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19958 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/ja/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.914448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22410 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/ko_KR/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.918448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12163 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.918448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24090 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/zh_Hans/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.918448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16530 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/zh_Hans/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/static/neutron_fwaas_dashboard/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.918448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/static/neutron_fwaas_dashboard/js/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/static/neutron_fwaas_dashboard/js/horizon.firewalls_v2.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.918448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/static/neutron_fwaas_dashboard/scss/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/static/neutron_fwaas_dashboard/scss/firewalls.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.918448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.918448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/api_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/api_tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31028 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/api_tests/test_fwaas_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/helpers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.918448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/integration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/integration/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/integration/horizon.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.918448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/integration/pages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/integration/pages/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.918448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/integration/pages/project/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/integration/pages/project/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.918448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/integration/pages/project/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/integration/pages/project/network/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/integration/pages/project/network/firewallgroupspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      966 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/integration/test_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1867 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.918448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/test_data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/test_data/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5381 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/test_data/fwaas_v2_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/test_data/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.910448 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1480 2024-04-03 11:52:26.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7621 2024-04-03 11:52:26.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:52:26.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:52:26.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-04-03 11:52:26.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-04-03 11:52:26.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2024-04-03 11:52:26.000000 neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.918448 neutron-fwaas-dashboard-7.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/notes/add-remove-router-policy-a3145bce0ce3cd92.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/notes/deprecate-neutron-fwaas-as-stadium-project-af51b5bcab1cb25f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/notes/drop-fwaas-v1-d10b108e8cf970fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/notes/drop-py-2-7-aeac41c824c80d4a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/notes/drop-python-3-6-and-3-7-b1cf8738aaab988f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/notes/fwaas-v2-dashboard-cd148bd824c5827f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/notes/shared-policy-fix-db8ca3cd327540d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/notes/split-out-from-horizon-4807f953d5dc0799.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.922448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/2023.2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6753 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.906448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/cs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.922448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/cs/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.922448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6020 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.922448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7416 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.922448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.922448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.922448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5099 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.922448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2922 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.922448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1045 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.922448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.902448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.922448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9111 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.906448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:26.922448 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2024-04-03 11:52:26.926448 neutron-fwaas-dashboard-7.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2698 2024-04-03 11:51:38.000000 neutron-fwaas-dashboard-7.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1023 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1188 2024-03-14 07:08:52.000000 neutron-fwaas-dashboard-7.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7964 2024-03-14 07:08:52.000000 neutron-fwaas-dashboard-7.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      470 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1485 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/babel-django.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/babel-djangojs.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.170004 neutron-fwaas-dashboard-7.0.0.0rc1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      965 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/devstack/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2563 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.170004 neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7053 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.170004 neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.170004 neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/contributor/devstack-plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      996 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1373 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.170004 neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3141 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.170004 neutron-fwaas-dashboard-7.0.0.0rc1/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/etc/neutron-fwaas-policy.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      847 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/manage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.170004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.170004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11340 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/api/fwaas_v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.170004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.170004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.170004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18766 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1575 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15725 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5590 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_addport.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_firewallgroup_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_insert_rule_to_policy.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_policy_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_remove_rule_from_policy.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_removeport.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_rule_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_update_port_help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_update_ports.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_update_rule_help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_update_rules.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_updatefirewall.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_updatepolicy.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_updaterule.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/addfirewallgroup.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/addpolicy.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/addport.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/addrule.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/details_tabs.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/insert_rule_to_policy.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/remove_rule_from_policy.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/removeport.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3139 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/table_select.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/updatefirewall.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/updatepolicy.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/updaterule.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32306 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2691 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16837 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8556 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/widgets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15441 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/workflows.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/enabled/_7010_project_firewalls_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/enabled/_7012_project_firewalls_v2_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/enabled/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/local_settings.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      677 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/local_settings.d/_7000_neutron_fwaas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18488 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16820 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/en_GB/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14080 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17490 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/id/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19958 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/ja/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22410 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/ko_KR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12163 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24090 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/zh_Hans/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16530 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/zh_Hans/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/static/neutron_fwaas_dashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/static/neutron_fwaas_dashboard/js/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/static/neutron_fwaas_dashboard/js/horizon.firewalls_v2.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/static/neutron_fwaas_dashboard/scss/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/static/neutron_fwaas_dashboard/scss/firewalls.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/api_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/api_tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31028 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/api_tests/test_fwaas_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/integration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/integration/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/integration/horizon.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/integration/pages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/integration/pages/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/integration/pages/project/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/integration/pages/project/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.174004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/integration/pages/project/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/integration/pages/project/network/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/integration/pages/project/network/firewallgroupspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      966 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/integration/test_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1867 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/test_data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/test_data/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5381 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/test_data/fwaas_v2_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/test_data/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.170004 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1485 2024-03-14 07:08:52.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7621 2024-03-14 07:08:52.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-14 07:08:52.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-14 07:08:52.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-14 07:08:52.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-03-14 07:08:52.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2024-03-14 07:08:52.000000 neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/notes/add-remove-router-policy-a3145bce0ce3cd92.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/notes/deprecate-neutron-fwaas-as-stadium-project-af51b5bcab1cb25f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/notes/drop-fwaas-v1-d10b108e8cf970fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/notes/drop-py-2-7-aeac41c824c80d4a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/notes/drop-python-3-6-and-3-7-b1cf8738aaab988f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/notes/fwaas-v2-dashboard-cd148bd824c5827f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/notes/shared-policy-fix-db8ca3cd327540d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/notes/split-out-from-horizon-4807f953d5dc0799.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6753 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/cs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/cs/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6020 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7416 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      773 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5099 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2922 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1045 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9111 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.166004 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2024-03-14 07:08:52.178005 neutron-fwaas-dashboard-7.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2698 2024-03-14 07:08:24.000000 neutron-fwaas-dashboard-7.0.0.0rc1/tox.ini
```

### Comparing `neutron-fwaas-dashboard-7.0.0/.zuul.yaml` & `neutron-fwaas-dashboard-7.0.0.0rc1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/AUTHORS` & `neutron-fwaas-dashboard-7.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/CONTRIBUTING.rst` & `neutron-fwaas-dashboard-7.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/ChangeLog` & `neutron-fwaas-dashboard-7.0.0.0rc1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-7.0.0
------
+7.0.0.0rc1
+----------
 
 * Add py3.11 support in testing runtime
 * Update master for stable/2023.2
 
 6.0.0
 -----
```

### Comparing `neutron-fwaas-dashboard-7.0.0/LICENSE` & `neutron-fwaas-dashboard-7.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/PKG-INFO` & `neutron-fwaas-dashboard-7.0.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: neutron-fwaas-dashboard
-Version: 7.0.0
+Version: 7.0.0.0rc1
 Summary: Neutron FWaaS Dashboard
 Home-page: https://docs.openstack.org/neutron-fwaas-dashboard/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =======================
         Neutron FWaaS Dashboard
```

### Comparing `neutron-fwaas-dashboard-7.0.0/devstack/README.rst` & `neutron-fwaas-dashboard-7.0.0.0rc1/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/devstack/plugin.sh` & `neutron-fwaas-dashboard-7.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/doc/source/conf.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/doc/source/configuration/index.rst` & `neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/doc/source/contributor/index.rst` & `neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/doc/source/index.rst` & `neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/doc/source/install/index.rst` & `neutron-fwaas-dashboard-7.0.0.0rc1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/etc/neutron-fwaas-policy.json` & `neutron-fwaas-dashboard-7.0.0.0rc1/etc/neutron-fwaas-policy.json`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/manage.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/manage.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/api/fwaas_v2.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/api/fwaas_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/forms.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/forms.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/panel.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/panel.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/tables.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/tables.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/tabs.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/tabs.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_firewallgroup_details.html` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_firewallgroup_details.html`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_policy_details.html` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_policy_details.html`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_rule_details.html` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_rule_details.html`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_update_ports.html` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_update_ports.html`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_update_rules.html` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/_update_rules.html`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/table_select.html` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/templates/firewalls_v2/table_select.html`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/tests.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/tests.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/urls.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/urls.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/views.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/views.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/widgets.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/widgets.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/workflows.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/dashboards/project/firewalls_v2/workflows.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/enabled/_7010_project_firewalls_common.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/enabled/_7010_project_firewalls_common.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/enabled/_7012_project_firewalls_v2_panel.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/enabled/_7012_project_firewalls_v2_panel.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/local_settings.d/_7000_neutron_fwaas.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/local_settings.d/_7000_neutron_fwaas.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/de/LC_MESSAGES/django.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/en_GB/LC_MESSAGES/django.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/fr/LC_MESSAGES/django.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/id/LC_MESSAGES/django.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/ja/LC_MESSAGES/django.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/ko_KR/LC_MESSAGES/django.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/pt_BR/LC_MESSAGES/django.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/ru/LC_MESSAGES/django.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/locale/zh_Hans/LC_MESSAGES/django.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/static/neutron_fwaas_dashboard/js/horizon.firewalls_v2.js` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/static/neutron_fwaas_dashboard/js/horizon.firewalls_v2.js`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/static/neutron_fwaas_dashboard/scss/firewalls.scss` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/static/neutron_fwaas_dashboard/scss/firewalls.scss`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/api_tests/test_fwaas_v2.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/api_tests/test_fwaas_v2.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/helpers.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/helpers.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/integration/pages/project/network/firewallgroupspage.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/integration/pages/project/network/firewallgroupspage.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/integration/test_basic.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/settings.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/settings.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/test_data/fwaas_v2_data.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/test_data/fwaas_v2_data.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/test/test_data/utils.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/test/test_data/utils.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard/version.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard/version.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard.egg-info/PKG-INFO` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: neutron-fwaas-dashboard
-Version: 7.0.0
+Version: 7.0.0.0rc1
 Summary: Neutron FWaaS Dashboard
 Home-page: https://docs.openstack.org/neutron-fwaas-dashboard/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =======================
         Neutron FWaaS Dashboard
```

### Comparing `neutron-fwaas-dashboard-7.0.0/neutron_fwaas_dashboard.egg-info/SOURCES.txt` & `neutron-fwaas-dashboard-7.0.0.0rc1/neutron_fwaas_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/releasenotes/notes/deprecate-neutron-fwaas-as-stadium-project-af51b5bcab1cb25f.yaml` & `neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/notes/deprecate-neutron-fwaas-as-stadium-project-af51b5bcab1cb25f.yaml`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/releasenotes/notes/split-out-from-horizon-4807f953d5dc0799.yaml` & `neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/notes/split-out-from-horizon-4807f953d5dc0799.yaml`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/releasenotes/source/conf.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/cs/LC_MESSAGES/releasenotes.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/cs/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po` & `neutron-fwaas-dashboard-7.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/requirements.txt` & `neutron-fwaas-dashboard-7.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/setup.cfg` & `neutron-fwaas-dashboard-7.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/setup.py` & `neutron-fwaas-dashboard-7.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/test-requirements.txt` & `neutron-fwaas-dashboard-7.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `neutron-fwaas-dashboard-7.0.0/tox.ini` & `neutron-fwaas-dashboard-7.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

