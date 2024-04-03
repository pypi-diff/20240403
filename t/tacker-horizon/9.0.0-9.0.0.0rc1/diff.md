# Comparing `tmp/tacker-horizon-9.0.0.tar.gz` & `tmp/tacker-horizon-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tacker-horizon-9.0.0.tar", last modified: Wed Apr  3 11:52:07 2024, max compression
+gzip compressed data, was "tacker-horizon-9.0.0.0rc1.tar", last modified: Fri Mar 15 14:25:39 2024, max compression
```

## Comparing `tacker-horizon-9.0.0.tar` & `tacker-horizon-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,360 +1,360 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.498303 tacker-horizon-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7659 2024-04-03 11:52:07.000000 tacker-horizon-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26009 2024-04-03 11:52:07.000000 tacker-horizon-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2024-04-03 11:52:07.498303 tacker-horizon-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1642 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/babel-django.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/babel-djangojs.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.446302 tacker-horizon-9.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.446302 tacker-horizon-9.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.446302 tacker-horizon-9.0.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.446302 tacker-horizon-9.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.446302 tacker-horizon-9.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.446302 tacker-horizon-9.0.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/doc/source/user/index.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      831 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/manage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.434301 tacker-horizon-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.446302 tacker-horizon-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/releasenotes/notes/drop-py-2-7-55250f584936f88e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/releasenotes/notes/support-nfv-orchestration-api-v2-a0ec6da7c67e6d4f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2024-04-03 11:52:07.498303 tacker-horizon-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.446302 tacker-horizon-9.0.0/tacker_horizon/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.450302 tacker-horizon-9.0.0/tacker_horizon/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/enabled/_80_nfv.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/enabled/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.450302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.450302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19130 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/api/tacker.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.450302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.450302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1881 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/dashboard.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.454302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2080 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2294 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3622 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.434301 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.454302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/templates/lccnsubscription/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/templates/lccnsubscription/_create_lccn_subscription.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/templates/lccnsubscription/create_lccn_subscription.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/templates/lccnsubscription/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/templates/lccnsubscription/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/templates/lccnsubscription/lccnsubsc_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3369 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.454302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4190 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2026 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3848 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.438302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.458302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/templates/nscatalog/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/templates/nscatalog/_onboardns.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/templates/nscatalog/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/templates/nscatalog/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/templates/nscatalog/onboardns.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/templates/nscatalog/template.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3883 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.458302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6796 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3754 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.438302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.458302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/templates/nsmanager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/templates/nsmanager/_deploy_ns.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/templates/nsmanager/deploy_ns.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/templates/nsmanager/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/templates/nsmanager/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3502 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.438302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.438302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.438302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/nfv/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.458302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/nfv/css/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/nfv/css/nfv.css
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.458302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/nfv/js/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/nfv/js/nfv.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2019 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/nfv/js/nfv.vim.reg.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.438302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.458302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/templates/nfv/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/templates/nfv/base.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1705 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.462302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5911 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2452 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4918 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.438302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.462302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/templates/vim/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/templates/vim/_registervim.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/templates/vim/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/templates/vim/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/templates/vim/registervim.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      976 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3115 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.462302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4308 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2206 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4327 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.438302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.462302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/templates/vnfcatalog/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/templates/vnfcatalog/_onboardvnf.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/templates/vnfcatalog/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/templates/vnfcatalog/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/templates/vnfcatalog/onboardvnf.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/templates/vnfcatalog/template.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3978 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.466302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4214 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      822 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2077 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2793 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.438302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.466302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/templates/vnffgcatalog/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/templates/vnffgcatalog/_onboardvnffg.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/templates/vnffgcatalog/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/templates/vnffgcatalog/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/templates/vnffgcatalog/onboardvnffg.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/templates/vnffgcatalog/template.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3955 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.466302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3740 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      822 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8377 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2895 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.438302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.470302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/_deploy_vnffg.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/deploy_vnffg.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/vdu_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/vnffg_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4298 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.470302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1830 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3945 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.438302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.470302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/vnffmalarm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/vnffmalarm/_update_alarm.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1616 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/vnffmalarm/alarm_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/vnffmalarm/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/vnffmalarm/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/vnffmalarm/update_alarm.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3295 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.474303 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2193 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3720 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.438302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.474303 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/templates/vnffmsubscription/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/templates/vnffmsubscription/_create_subscription.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/templates/vnffmsubscription/create_subscription.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/templates/vnffmsubscription/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/templates/vnffmsubscription/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/templates/vnffmsubscription/subscription_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1028 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3704 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.474303 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15218 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4253 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4693 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.438302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.478303 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_change_connectivity.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_change_vnfpkg.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_create_vnf_identifier.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_heal_vnf.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_instantiate_vnf.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_scale_vnf.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_terminate_vnf.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_update_vnf.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/change_connectivity.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/change_vnfpkg.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/create_vnf_identifier.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/heal_vnf.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/instantiate_vnf.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/scale_vnf.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/terminate_vnf.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/update_vnf.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1074 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/vnflcm_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1836 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7659 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.478303 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3324 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.438302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.482303 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/templates/vnflcmopocc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/templates/vnflcmopocc/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/templates/vnflcmopocc/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1421 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/templates/vnflcmopocc/vnflcmopocc_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2654 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.482303 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9592 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10453 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4358 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.442302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.482303 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/_deploy_vnf.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/deploy_vnf.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1636 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/vdu_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      965 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4270 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.482303 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7251 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3994 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4146 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.442302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.486303 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/_update_vnfpkg.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/_upload_vnfpkg.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/update_vnfpkg.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/upload_vnfpkg.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/vnfpkg_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4415 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.486303 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3396 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3885 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.442302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.486303 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/_create_pmjob.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/_update_pmjob.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/create_pmjob.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1563 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/pmjob_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/report_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/update_pmjob.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1238 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6574 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.490303 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3504 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2464 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3749 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.442302 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.490303 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/_create_pmthreshold.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/_update_pmthreshold.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/create_pmthreshold.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/pmthreshold_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/update_pmthreshold.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4733 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.490303 tacker-horizon-9.0.0/tacker_horizon/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.490303 tacker-horizon-9.0.0/tacker_horizon/test/integration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      504 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/horizon.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.490303 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.490303 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.494303 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/nscatalogpage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/nsmanagerpage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/vimmanagementpage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/vnffgcatalogpage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/vnffgmanagerpage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.494303 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnf_management/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnf_management/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnf_management/vnfcatalogpage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnf_management/vnfmanagerpage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.494303 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnffm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnffm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnffm/vnffmalarmpage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnffm/vnffmsubscriptionpage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.494303 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnflcm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnflcm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      879 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnflcm/lccnsubscriptionpage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnflcm/vnflcmopoccpage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnflcm/vnflcmpage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.494303 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnfpackages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnfpackages/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      864 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnfpackages/vnfpackagespage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.494303 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnfpm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnfpm/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      852 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnfpm/vnfpmjobpage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnfpm/vnfpmthresholdpage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4158 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/integration/test_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1425 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/settings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tacker_horizon/test/urls.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.450302 tacker-horizon-9.0.0/tacker_horizon.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2024-04-03 11:52:07.000000 tacker-horizon-9.0.0/tacker_horizon.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20126 2024-04-03 11:52:07.000000 tacker-horizon-9.0.0/tacker_horizon.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:52:07.000000 tacker-horizon-9.0.0/tacker_horizon.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2024-04-03 11:52:07.000000 tacker-horizon-9.0.0/tacker_horizon.egg-info/namespace_packages.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:52:07.000000 tacker-horizon-9.0.0/tacker_horizon.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-04-03 11:52:07.000000 tacker-horizon-9.0.0/tacker_horizon.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-04-03 11:52:07.000000 tacker-horizon-9.0.0/tacker_horizon.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2024-04-03 11:52:07.000000 tacker-horizon-9.0.0/tacker_horizon.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.494303 tacker-horizon-9.0.0/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/test/README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:07.498303 tacker-horizon-9.0.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tools/executable_files.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      580 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tools/find_executables.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2024-04-03 11:51:42.000000 tacker-horizon-9.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:39.007152 tacker-horizon-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7659 2024-03-15 14:25:38.000000 tacker-horizon-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26019 2024-03-15 14:25:38.000000 tacker-horizon-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2024-03-15 14:25:39.007152 tacker-horizon-9.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1642 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/babel-django.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/babel-djangojs.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.959152 tacker-horizon-9.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.959152 tacker-horizon-9.0.0.0rc1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.959152 tacker-horizon-9.0.0.0rc1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.959152 tacker-horizon-9.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.959152 tacker-horizon-9.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.963152 tacker-horizon-9.0.0.0rc1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/doc/source/user/index.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      831 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/manage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.951152 tacker-horizon-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.963152 tacker-horizon-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/releasenotes/notes/drop-py-2-7-55250f584936f88e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/releasenotes/notes/support-nfv-orchestration-api-v2-a0ec6da7c67e6d4f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2024-03-15 14:25:39.007152 tacker-horizon-9.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.963152 tacker-horizon-9.0.0.0rc1/tacker_horizon/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.963152 tacker-horizon-9.0.0.0rc1/tacker_horizon/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/enabled/_80_nfv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/enabled/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.963152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.963152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19130 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/api/tacker.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.963152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.963152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1881 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/dashboard.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.967152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2080 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2294 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3622 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.951152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.967152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/templates/lccnsubscription/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/templates/lccnsubscription/_create_lccn_subscription.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/templates/lccnsubscription/create_lccn_subscription.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/templates/lccnsubscription/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/templates/lccnsubscription/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/templates/lccnsubscription/lccnsubsc_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3369 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.967152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4190 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2026 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3848 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.951152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.967152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/templates/nscatalog/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/templates/nscatalog/_onboardns.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/templates/nscatalog/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/templates/nscatalog/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/templates/nscatalog/onboardns.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/templates/nscatalog/template.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3883 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.971152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6796 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3754 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.951152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.971152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/templates/nsmanager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/templates/nsmanager/_deploy_ns.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/templates/nsmanager/deploy_ns.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/templates/nsmanager/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/templates/nsmanager/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3502 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.951152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.951152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.951152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/nfv/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.971152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/nfv/css/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/nfv/css/nfv.css
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.971152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/nfv/js/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       37 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/nfv/js/nfv.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2019 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/nfv/js/nfv.vim.reg.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.951152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.971152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/templates/nfv/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/templates/nfv/base.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1705 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.971152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5911 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2452 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4918 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.955152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.971152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/templates/vim/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/templates/vim/_registervim.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/templates/vim/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/templates/vim/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/templates/vim/registervim.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      976 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3115 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.975152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4308 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2206 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4327 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.955152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.975152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/templates/vnfcatalog/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/templates/vnfcatalog/_onboardvnf.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/templates/vnfcatalog/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/templates/vnfcatalog/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/templates/vnfcatalog/onboardvnf.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/templates/vnfcatalog/template.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3978 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.975152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4214 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      822 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2077 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2793 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.955152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.975152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/templates/vnffgcatalog/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/templates/vnffgcatalog/_onboardvnffg.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/templates/vnffgcatalog/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/templates/vnffgcatalog/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/templates/vnffgcatalog/onboardvnffg.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/templates/vnffgcatalog/template.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3955 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.979152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3740 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      822 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8377 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2895 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.955152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.979152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/_deploy_vnffg.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/deploy_vnffg.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/vdu_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/vnffg_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4298 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.979152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1830 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3945 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.955152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.979152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/vnffmalarm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/vnffmalarm/_update_alarm.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1616 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/vnffmalarm/alarm_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/vnffmalarm/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/vnffmalarm/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/vnffmalarm/update_alarm.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3295 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.983152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2193 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3720 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.955152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.983152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/templates/vnffmsubscription/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/templates/vnffmsubscription/_create_subscription.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/templates/vnffmsubscription/create_subscription.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/templates/vnffmsubscription/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/templates/vnffmsubscription/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/templates/vnffmsubscription/subscription_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1028 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3704 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.983152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15218 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4253 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4693 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.955152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.987152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_change_connectivity.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_change_vnfpkg.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_create_vnf_identifier.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_heal_vnf.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_instantiate_vnf.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_scale_vnf.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_terminate_vnf.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/_update_vnf.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/change_connectivity.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/change_vnfpkg.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/create_vnf_identifier.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/heal_vnf.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/instantiate_vnf.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/scale_vnf.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/terminate_vnf.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/update_vnf.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1074 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/vnflcm_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1836 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7659 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.987152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3324 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.955152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.987152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/templates/vnflcmopocc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/templates/vnflcmopocc/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/templates/vnflcmopocc/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1421 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/templates/vnflcmopocc/vnflcmopocc_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2654 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.991152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9592 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10453 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4358 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.955152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.991152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/_deploy_vnf.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/deploy_vnf.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1636 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/vdu_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      965 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4270 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.991152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7251 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3994 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4146 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.955152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.991152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/_update_vnfpkg.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/_upload_vnfpkg.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/update_vnfpkg.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/upload_vnfpkg.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/vnfpkg_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4415 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.995152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3396 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3885 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.955152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.995152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/_create_pmjob.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/_update_pmjob.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/create_pmjob.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1563 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/pmjob_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/report_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/update_pmjob.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1238 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6574 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.999152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3504 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2464 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3749 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.955152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.999152 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/_create_pmthreshold.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/_update_pmthreshold.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/create_pmthreshold.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/pmthreshold_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/update_pmthreshold.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4733 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.999152 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:39.003152 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      504 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/horizon.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:39.003152 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:39.003152 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:39.003152 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/nscatalogpage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/nsmanagerpage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/vimmanagementpage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/vnffgcatalogpage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/vnffgmanagerpage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:39.003152 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnf_management/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnf_management/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnf_management/vnfcatalogpage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnf_management/vnfmanagerpage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:39.003152 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnffm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnffm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnffm/vnffmalarmpage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnffm/vnffmsubscriptionpage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:39.007152 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnflcm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnflcm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      879 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnflcm/lccnsubscriptionpage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnflcm/vnflcmopoccpage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnflcm/vnflcmpage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:39.007152 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnfpackages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnfpackages/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      864 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnfpackages/vnfpackagespage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:39.007152 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnfpm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnfpm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      852 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnfpm/vnfpmjobpage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      870 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnfpm/vnfpmthresholdpage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4158 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/test_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1425 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/settings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon/test/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:38.963152 tacker-horizon-9.0.0.0rc1/tacker_horizon.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2024-03-15 14:25:38.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20126 2024-03-15 14:25:38.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 14:25:38.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2024-03-15 14:25:38.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 14:25:38.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-15 14:25:38.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-03-15 14:25:38.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2024-03-15 14:25:38.000000 tacker-horizon-9.0.0.0rc1/tacker_horizon.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:39.007152 tacker-horizon-9.0.0.0rc1/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/test/README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:25:39.007152 tacker-horizon-9.0.0.0rc1/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tools/executable_files.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      580 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tools/find_executables.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2024-03-15 14:24:54.000000 tacker-horizon-9.0.0.0rc1/tox.ini
```

### Comparing `tacker-horizon-9.0.0/.zuul.yaml` & `tacker-horizon-9.0.0.0rc1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/AUTHORS` & `tacker-horizon-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/CONTRIBUTING.rst` & `tacker-horizon-9.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/ChangeLog` & `tacker-horizon-9.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * Support NFV Orchestration API v2.0
 
 8.0.0
 -----
 
 * Update metadata in setup.cfg
```

### Comparing `tacker-horizon-9.0.0/HACKING.rst` & `tacker-horizon-9.0.0.0rc1/HACKING.rst`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/LICENSE` & `tacker-horizon-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/PKG-INFO` & `tacker-horizon-9.0.0.0rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tacker-horizon
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Tacker extension for Horizon
 Home-page: https://docs.openstack.org/tacker-horizon/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Tacker extension for Horizon
 Platform: UNKNOWN
```

### Comparing `tacker-horizon-9.0.0/README.rst` & `tacker-horizon-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/doc/source/conf.py` & `tacker-horizon-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/doc/source/contributor/index.rst` & `tacker-horizon-9.0.0.0rc1/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/doc/source/index.rst` & `tacker-horizon-9.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/doc/source/install/index.rst` & `tacker-horizon-9.0.0.0rc1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/manage.py` & `tacker-horizon-9.0.0.0rc1/manage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/requirements.txt` & `tacker-horizon-9.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/setup.cfg` & `tacker-horizon-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/setup.py` & `tacker-horizon-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/__init__.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/__init__.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/enabled/_80_nfv.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/enabled/_80_nfv.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/api/__init__.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/api/tacker.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/api/tacker.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/dashboard.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/dashboard.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/forms.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/forms.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/lccnsubscription/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/forms.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/forms.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nscatalog/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/forms.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/forms.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/templates/nsmanager/_deploy_ns.html` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/templates/nsmanager/_deploy_ns.html`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/nsmanager/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/nfv/js/nfv.vim.reg.js` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/static/dashboard/nfv/js/nfv.vim.reg.js`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/utils.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/utils.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/forms.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/forms.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vim/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/forms.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/forms.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfcatalog/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/forms.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/forms.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgcatalog/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/forms.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/forms.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/vdu_details.html` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/vdu_details.html`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/vnffg_details.html` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/templates/vnffgmanager/vnffg_details.html`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffgmanager/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/forms.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/forms.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/vnffmalarm/alarm_detail.html` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/templates/vnffmalarm/alarm_detail.html`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmalarm/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/forms.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/forms.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnffmsubscription/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/forms.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/forms.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/vnflcm_detail.html` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/templates/vnflcm/vnflcm_detail.html`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcm/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/templates/vnflcmopocc/vnflcmopocc_detail.html` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/templates/vnflcmopocc/vnflcmopocc_detail.html`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnflcmopocc/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/forms.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/forms.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/_deploy_vnf.html` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/_deploy_vnf.html`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/vdu_details.html` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/templates/vnfmanager/vdu_details.html`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfmanager/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/forms.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/forms.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/vnfpkg_detail.html` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/templates/vnfpackages/vnfpkg_detail.html`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpackages/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/forms.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/forms.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/pmjob_detail.html` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/pmjob_detail.html`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/report_detail.html` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/templates/vnfpmjob/report_detail.html`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmjob/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/forms.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/forms.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/panel.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/panel.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/tables.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/tables.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/tabs.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/tabs.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/pmthreshold_detail.html` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/templates/vnfpmthreshold/pmthreshold_detail.html`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/views.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/openstack_dashboard/dashboards/nfv/vnfpmthreshold/views.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/base.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/base.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/nscatalogpage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/nscatalogpage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/nsmanagerpage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/nsmanagerpage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/vimmanagementpage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/vimmanagementpage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/vnffgcatalogpage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/vnffgcatalogpage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/vnffgmanagerpage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/nfv_orchestration/vnffgmanagerpage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnf_management/vnfcatalogpage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnf_management/vnfcatalogpage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnf_management/vnfmanagerpage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnf_management/vnfmanagerpage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnffm/vnffmalarmpage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnffm/vnffmalarmpage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnffm/vnffmsubscriptionpage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnffm/vnffmsubscriptionpage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnflcm/lccnsubscriptionpage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnflcm/lccnsubscriptionpage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnflcm/vnflcmopoccpage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnflcm/vnflcmopoccpage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnflcm/vnflcmpage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnflcm/vnflcmpage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnfpackages/vnfpackagespage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnfpackages/vnfpackagespage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnfpm/vnfpmjobpage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnfpm/vnfpmjobpage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/pages/nfv/vnfpm/vnfpmthresholdpage.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/pages/nfv/vnfpm/vnfpmthresholdpage.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/integration/test_basic.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/settings.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/settings.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon/test/urls.py` & `tacker-horizon-9.0.0.0rc1/tacker_horizon/test/urls.py`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tacker_horizon.egg-info/PKG-INFO` & `tacker-horizon-9.0.0.0rc1/tacker_horizon.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tacker-horizon
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Tacker extension for Horizon
 Home-page: https://docs.openstack.org/tacker-horizon/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Tacker extension for Horizon
 Platform: UNKNOWN
```

### Comparing `tacker-horizon-9.0.0/tacker_horizon.egg-info/SOURCES.txt` & `tacker-horizon-9.0.0.0rc1/tacker_horizon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/test-requirements.txt` & `tacker-horizon-9.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tools/find_executables.sh` & `tacker-horizon-9.0.0.0rc1/tools/find_executables.sh`

 * *Files identical despite different names*

### Comparing `tacker-horizon-9.0.0/tox.ini` & `tacker-horizon-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

