# Comparing `tmp/watcher-dashboard-9.0.0.tar.gz` & `tmp/watcher-dashboard-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watcher-dashboard-9.0.0.tar", last modified: Wed Mar 22 12:48:12 2023, max compression
+gzip compressed data, was "watcher-dashboard-9.0.0.0rc1.tar", last modified: Tue Feb 28 13:43:36 2023, max compression
```

## Comparing `watcher-dashboard-9.0.0.tar` & `watcher-dashboard-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,245 +1,245 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2144 2023-03-22 12:48:12.000000 watcher-dashboard-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8029 2023-03-22 12:48:12.000000 watcher-dashboard-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2349 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2159 2023-03-22 12:48:12.611664 watcher-dashboard-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/babel-django.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/babel-djangojs.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.587662 watcher-dashboard-9.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/devstack/local.conf.example
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1803 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.591663 watcher-dashboard-9.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.591663 watcher-dashboard-9.0.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3987 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.591663 watcher-dashboard-9.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2102 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1810 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.591663 watcher-dashboard-9.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4503 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/doc/source/install/installation.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      833 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/manage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.583662 watcher-dashboard-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.591663 watcher-dashboard-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/notes/drop-py-2-7-198cca7f72d16655.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.591663 watcher-dashboard-9.0.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.591663 watcher-dashboard-9.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.591663 watcher-dashboard-9.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9206 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.583662 watcher-dashboard-9.0.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.583662 watcher-dashboard-9.0.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.591663 watcher-dashboard-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.583662 watcher-dashboard-9.0.0/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.591663 watcher-dashboard-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    18017 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1068 2023-03-22 12:48:12.611664 watcher-dashboard-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.591663 watcher-dashboard-9.0.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2396 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/tools/install_venv.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5919 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/tools/install_venv_common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      795 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/tools/register_plugin.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      506 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.595663 watcher-dashboard-9.0.0/watcher_dashboard/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.595663 watcher-dashboard-9.0.0/watcher_dashboard/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16321 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/api/watcher.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.595663 watcher-dashboard-9.0.0/watcher_dashboard/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/common/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.595663 watcher-dashboard-9.0.0/watcher_dashboard/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1138 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/conf/watcher_policy.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.595663 watcher-dashboard-9.0.0/watcher_dashboard/content/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.595663 watcher-dashboard-9.0.0/watcher_dashboard/content/action_plans/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/action_plans/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/action_plans/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7655 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/action_plans/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/action_plans/tabs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/action_plans/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5055 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/action_plans/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.595663 watcher-dashboard-9.0.0/watcher_dashboard/content/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/actions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/actions/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4519 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/actions/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/actions/tabs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      856 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/actions/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3724 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/actions/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.599663 watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4508 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3647 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/tabs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4428 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      943 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4844 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.599663 watcher-dashboard-9.0.0/watcher_dashboard/content/audits/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audits/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5060 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audits/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audits/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5378 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audits/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1005 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audits/tabs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audits/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4688 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/audits/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.599663 watcher-dashboard-9.0.0/watcher_dashboard/content/goals/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/goals/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/goals/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/goals/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/goals/tabs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2347 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/goals/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      852 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/goals/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4470 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/goals/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.599663 watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      730 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2314 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/tabs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2591 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3439 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.599663 watcher-dashboard-9.0.0/watcher_dashboard/local/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/local/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.599663 watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/_31000_goals_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/_31010_strategies_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1175 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/_31020_watcher_panelgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      946 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/_31030_audit_templates_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/_31040_audits_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/_31050_action_plans_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/_31060_actions_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.583662 watcher-dashboard-9.0.0/watcher_dashboard/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.583662 watcher-dashboard-9.0.0/watcher_dashboard/static/infra_optim/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.603664 watcher-dashboard-9.0.0/watcher_dashboard/static/infra_optim/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/static/infra_optim/images/chevron.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/static/infra_optim/images/power.png
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.603664 watcher-dashboard-9.0.0/watcher_dashboard/static/infra_optim/scss/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/static/infra_optim/scss/infra_optim.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.603664 watcher-dashboard-9.0.0/watcher_dashboard/static/infra_optim/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2386 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/static/infra_optim/tests/formset_table.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.587662 watcher-dashboard-9.0.0/watcher_dashboard/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.603664 watcher-dashboard-9.0.0/watcher_dashboard/templates/client_side/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/client_side/_modal_chart.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/client_side/templates.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.603664 watcher-dashboard-9.0.0/watcher_dashboard/templates/formset_table/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/formset_table/_row.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/formset_table/_table.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1559 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/formset_table/menu_formset.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.587662 watcher-dashboard-9.0.0/watcher_dashboard/templates/horizon/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.603664 watcher-dashboard-9.0.0/watcher_dashboard/templates/horizon/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/horizon/common/_items_count_domain_page_header.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.603664 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1656 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/_fullscreen_workflow.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/_fullscreen_workflow_base.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/_performance_chart.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2660 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/_performance_chart_box.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/_top_5_box.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/_top_5_chart.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/_workflow_base.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.603664 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/action_plans/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/action_plans/_details_overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/action_plans/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/action_plans/details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/action_plans/index.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.603664 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/actions/details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/actions/index.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.603664 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/actions_history/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/actions_history/details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/actions_history/index.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.603664 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/audit_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1544 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/audit_templates/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/audit_templates/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1438 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/audit_templates/details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/audit_templates/index.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/audits/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/audits/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/audits/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/audits/details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/audits/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/base.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/base_detail.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/goals/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1060 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/goals/details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/goals/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/header_actions.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/logs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/logs/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7122 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/qunit.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/strategies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/strategies/details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/strategies/index.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/watcher_dashboard/templatetags/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/templatetags/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/watcher_dashboard/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/watcher_dashboard/test/api_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/api_tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12822 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/api_tests/test_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/helpers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1805 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/horizon.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/pages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/pages/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/pages/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/pages/admin/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/pages/admin/optimization/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/pages/admin/optimization/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2886 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/pages/admin/optimization/auditspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4350 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/pages/admin/optimization/audittemplatespage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3194 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/tests/test_audit_template_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1979 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/selenium.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/watcher_dashboard/test/test_data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/test_data/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      903 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/test_data/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1950 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/test_data/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7748 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/test_data/watcher_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1839 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/test_formset_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/test/urls.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.607664 watcher-dashboard-9.0.0/watcher_dashboard/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3000 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/utils/errors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/utils/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3029 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/utils/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2023-03-22 12:47:47.000000 watcher-dashboard-9.0.0/watcher_dashboard/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:48:12.595663 watcher-dashboard-9.0.0/watcher_dashboard.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2159 2023-03-22 12:48:12.000000 watcher-dashboard-9.0.0/watcher_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8125 2023-03-22 12:48:12.000000 watcher-dashboard-9.0.0/watcher_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-22 12:48:12.000000 watcher-dashboard-9.0.0/watcher_dashboard.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-22 12:48:12.000000 watcher-dashboard-9.0.0/watcher_dashboard.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-22 12:48:12.000000 watcher-dashboard-9.0.0/watcher_dashboard.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-03-22 12:48:12.000000 watcher-dashboard-9.0.0/watcher_dashboard.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2023-03-22 12:48:12.000000 watcher-dashboard-9.0.0/watcher_dashboard.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.575460 watcher-dashboard-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2144 2023-02-28 13:43:36.000000 watcher-dashboard-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8039 2023-02-28 13:43:36.000000 watcher-dashboard-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2349 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2164 2023-02-28 13:43:36.575460 watcher-dashboard-9.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/babel-django.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/babel-djangojs.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.543458 watcher-dashboard-9.0.0.0rc1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/devstack/local.conf.example
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1803 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.543458 watcher-dashboard-9.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.543458 watcher-dashboard-9.0.0.0rc1/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3987 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.543458 watcher-dashboard-9.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2102 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1810 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.543458 watcher-dashboard-9.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4503 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/doc/source/install/installation.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      833 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/manage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.535457 watcher-dashboard-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.543458 watcher-dashboard-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/notes/drop-py-2-7-198cca7f72d16655.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.547458 watcher-dashboard-9.0.0.0rc1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.547458 watcher-dashboard-9.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.547458 watcher-dashboard-9.0.0.0rc1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9206 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.535457 watcher-dashboard-9.0.0.0rc1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.535457 watcher-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.547458 watcher-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.535457 watcher-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.547458 watcher-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    18017 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1068 2023-02-28 13:43:36.575460 watcher-dashboard-9.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.547458 watcher-dashboard-9.0.0.0rc1/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2396 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/tools/install_venv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5919 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/tools/install_venv_common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      795 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/tools/register_plugin.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      506 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.547458 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.551458 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16321 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/api/watcher.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.551458 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/common/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.551458 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1138 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/conf/watcher_policy.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.551458 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.551458 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/action_plans/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/action_plans/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      735 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/action_plans/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7655 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/action_plans/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/action_plans/tabs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/action_plans/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5055 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/action_plans/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.555459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/actions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/actions/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4519 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/actions/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/actions/tabs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      856 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/actions/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3724 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/actions/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.555459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4508 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3647 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/tabs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4428 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      943 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4844 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.555459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audits/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audits/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5060 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audits/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audits/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5378 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audits/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1005 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audits/tabs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audits/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4688 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audits/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.559459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/goals/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/goals/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/goals/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/goals/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/goals/tabs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2347 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/goals/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      852 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/goals/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4470 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/goals/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.559459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      730 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2314 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/tabs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2591 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3439 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.559459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.559459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/_31000_goals_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/_31010_strategies_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1175 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/_31020_watcher_panelgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      946 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/_31030_audit_templates_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/_31040_audits_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/_31050_action_plans_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/_31060_actions_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.535457 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.535457 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/static/infra_optim/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.559459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/static/infra_optim/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      348 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/static/infra_optim/images/chevron.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/static/infra_optim/images/power.png
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.563459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/static/infra_optim/scss/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/static/infra_optim/scss/infra_optim.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.563459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/static/infra_optim/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2386 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/static/infra_optim/tests/formset_table.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.539457 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.563459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/client_side/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/client_side/_modal_chart.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/client_side/templates.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.563459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/formset_table/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/formset_table/_row.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/formset_table/_table.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1559 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/formset_table/menu_formset.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.539457 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/horizon/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.563459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/horizon/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/horizon/common/_items_count_domain_page_header.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.563459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1656 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/_fullscreen_workflow.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/_fullscreen_workflow_base.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/_performance_chart.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2660 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/_performance_chart_box.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/_top_5_box.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/_top_5_chart.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/_workflow_base.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.567459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/action_plans/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/action_plans/_details_overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/action_plans/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/action_plans/details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/action_plans/index.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.567459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1293 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/actions/details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/actions/index.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.567459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/actions_history/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      945 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/actions_history/details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/actions_history/index.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.567459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/audit_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1544 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/audit_templates/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/audit_templates/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1438 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/audit_templates/details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/audit_templates/index.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.567459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/audits/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/audits/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/audits/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/audits/details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/audits/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/base.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/base_detail.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.567459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/goals/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1060 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/goals/details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/goals/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/header_actions.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.567459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/logs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/logs/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7122 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/qunit.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.567459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/strategies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/strategies/details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/strategies/index.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.567459 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templatetags/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templatetags/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.571460 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.571460 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/api_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/api_tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12822 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/api_tests/test_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.571460 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1805 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/horizon.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.571460 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/pages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/pages/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.571460 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/pages/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/pages/admin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.571460 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/pages/admin/optimization/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/pages/admin/optimization/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2886 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/pages/admin/optimization/auditspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4350 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/pages/admin/optimization/audittemplatespage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.571460 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3194 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/tests/test_audit_template_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1979 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/selenium.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.571460 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/test_data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/test_data/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      903 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/test_data/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1950 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/test_data/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7748 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/test_data/watcher_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1839 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/test_formset_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.571460 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3000 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/utils/errors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/utils/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3029 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/utils/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2023-02-28 13:43:08.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-28 13:43:36.551458 watcher-dashboard-9.0.0.0rc1/watcher_dashboard.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2164 2023-02-28 13:43:36.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8125 2023-02-28 13:43:36.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-28 13:43:36.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-28 13:43:36.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-28 13:43:36.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-02-28 13:43:36.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2023-02-28 13:43:36.000000 watcher-dashboard-9.0.0.0rc1/watcher_dashboard.egg-info/top_level.txt
```

### Comparing `watcher-dashboard-9.0.0/AUTHORS` & `watcher-dashboard-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/ChangeLog` & `watcher-dashboard-9.0.0.0rc1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * Adjust tox.ini for tox4
 * Replace deprecated inspect.getargspec
 * Switch to 2023.1 Python3 unit tests and generic template name
 * Update master for stable/zed
 
 8.0.0
```

### Comparing `watcher-dashboard-9.0.0/HACKING.rst` & `watcher-dashboard-9.0.0.0rc1/HACKING.rst`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/LICENSE` & `watcher-dashboard-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/PKG-INFO` & `watcher-dashboard-9.0.0.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: watcher-dashboard
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Watcher Management Dashboard
 Home-page: https://docs.openstack.org/watcher-dashboard/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `watcher-dashboard-9.0.0/README.rst` & `watcher-dashboard-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/devstack/plugin.sh` & `watcher-dashboard-9.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/doc/source/conf.py` & `watcher-dashboard-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/doc/source/contributor/contributing.rst` & `watcher-dashboard-9.0.0.0rc1/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/doc/source/index.rst` & `watcher-dashboard-9.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/doc/source/install/installation.rst` & `watcher-dashboard-9.0.0.0rc1/doc/source/install/installation.rst`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/manage.py` & `watcher-dashboard-9.0.0.0rc1/manage.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/releasenotes/source/conf.py` & `watcher-dashboard-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `watcher-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `watcher-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/run_tests.sh` & `watcher-dashboard-9.0.0.0rc1/run_tests.sh`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/setup.cfg` & `watcher-dashboard-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/setup.py` & `watcher-dashboard-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/test-requirements.txt` & `watcher-dashboard-9.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/tools/install_venv.py` & `watcher-dashboard-9.0.0.0rc1/tools/install_venv.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/tools/install_venv_common.py` & `watcher-dashboard-9.0.0.0rc1/tools/install_venv_common.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/tools/register_plugin.sh` & `watcher-dashboard-9.0.0.0rc1/tools/register_plugin.sh`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/tox.ini` & `watcher-dashboard-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/api/watcher.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/api/watcher.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/common/exceptions.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/conf/watcher_policy.json` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/conf/watcher_policy.json`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/action_plans/panel.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/action_plans/panel.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/action_plans/tables.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/action_plans/tables.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/action_plans/tabs.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/action_plans/tabs.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/action_plans/urls.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/action_plans/urls.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/action_plans/views.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/action_plans/views.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/actions/panel.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/actions/panel.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/actions/tables.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/actions/tables.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/actions/tabs.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/actions/tabs.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/actions/urls.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/actions/urls.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/actions/views.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/actions/views.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/forms.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/forms.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/panel.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/panel.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/tables.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/tables.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/tabs.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/tabs.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/tests.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/tests.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/urls.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/urls.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/audit_templates/views.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audit_templates/views.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/audits/forms.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audits/forms.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/audits/panel.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audits/panel.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/audits/tables.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audits/tables.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/audits/tabs.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audits/tabs.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/audits/urls.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audits/urls.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/audits/views.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/audits/views.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/goals/panel.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/goals/panel.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/goals/tables.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/goals/tables.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/goals/tabs.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/goals/tabs.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/goals/tests.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/goals/tests.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/goals/urls.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/goals/urls.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/goals/views.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/goals/views.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/panel.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/panel.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/tables.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/tables.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/tabs.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/tabs.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/tests.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/tests.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/urls.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/urls.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/content/strategies/views.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/content/strategies/views.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/_31000_goals_panel.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/_31000_goals_panel.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/_31010_strategies_panel.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/_31010_strategies_panel.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/_31020_watcher_panelgroup.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/_31020_watcher_panelgroup.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/_31030_audit_templates_panel.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/_31030_audit_templates_panel.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/_31040_audits_panel.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/_31040_audits_panel.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/_31050_action_plans_panel.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/_31050_action_plans_panel.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/local/enabled/_31060_actions_panel.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/local/enabled/_31060_actions_panel.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/static/infra_optim/images/power.png` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/static/infra_optim/images/power.png`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/static/infra_optim/tests/formset_table.js` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/static/infra_optim/tests/formset_table.js`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/client_side/_modal_chart.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/client_side/_modal_chart.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/formset_table/_row.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/formset_table/_row.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/formset_table/_table.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/formset_table/_table.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/formset_table/menu_formset.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/formset_table/menu_formset.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/_fullscreen_workflow.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/_fullscreen_workflow.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/_performance_chart_box.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/_performance_chart_box.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/_top_5_chart.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/_top_5_chart.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/action_plans/_details_overview.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/action_plans/_details_overview.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/actions/details.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/actions/details.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/actions_history/details.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/actions_history/details.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/actions_history/index.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/actions_history/index.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/audit_templates/_create.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/audit_templates/_create.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/audit_templates/details.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/audit_templates/details.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/audits/details.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/audits/details.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/goals/details.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/goals/details.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/qunit.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/qunit.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templates/infra_optim/strategies/details.html` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templates/infra_optim/strategies/details.html`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/templatetags/__init__.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/test/api_tests/test_watcher.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/api_tests/test_watcher.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/test/helpers.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/helpers.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/horizon.conf` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/horizon.conf`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/pages/admin/optimization/auditspage.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/pages/admin/optimization/auditspage.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/pages/admin/optimization/audittemplatespage.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/pages/admin/optimization/audittemplatespage.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/test/integration_tests/tests/test_audit_template_panel.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/integration_tests/tests/test_audit_template_panel.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/test/selenium.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/selenium.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/test/settings.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/settings.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/test/test_data/exceptions.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/test_data/exceptions.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/test/test_data/utils.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/test_data/utils.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/test/test_data/watcher_data.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/test_data/watcher_data.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/test/test_formset_table.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/test_formset_table.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/test/urls.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/test/urls.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/utils/errors.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/utils/errors.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/utils/tests.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/utils/tests.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/utils/utils.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/utils/utils.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard/version.py` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard/version.py`

 * *Files identical despite different names*

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard.egg-info/PKG-INFO` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: watcher-dashboard
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Watcher Management Dashboard
 Home-page: https://docs.openstack.org/watcher-dashboard/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `watcher-dashboard-9.0.0/watcher_dashboard.egg-info/SOURCES.txt` & `watcher-dashboard-9.0.0.0rc1/watcher_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

