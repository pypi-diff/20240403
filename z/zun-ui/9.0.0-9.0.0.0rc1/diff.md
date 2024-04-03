# Comparing `tmp/zun-ui-9.0.0.tar.gz` & `tmp/zun-ui-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zun-ui-9.0.0.tar", last modified: Wed Mar 30 12:00:25 2022, max compression
+gzip compressed data, was "zun-ui-9.0.0.0rc1.tar", last modified: Tue Mar  8 12:48:41 2022, max compression
```

## Comparing `zun-ui-9.0.0.tar` & `zun-ui-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,287 +1,287 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.524554 zun-ui-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1587 2022-03-30 11:59:52.000000 zun-ui-9.0.0/.eslintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2022-03-30 11:59:52.000000 zun-ui-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2022-03-30 12:00:25.000000 zun-ui-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11851 2022-03-30 12:00:25.000000 zun-ui-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-03-30 11:59:52.000000 zun-ui-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2022-03-30 12:00:25.524554 zun-ui-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2022-03-30 11:59:52.000000 zun-ui-9.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2022-03-30 11:59:52.000000 zun-ui-9.0.0/_0330_cloud_shell_settings.py.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2022-03-30 11:59:52.000000 zun-ui-9.0.0/babel-django.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2022-03-30 11:59:52.000000 zun-ui-9.0.0/babel-djangojs.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2022-03-30 11:59:52.000000 zun-ui-9.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.504554 zun-ui-9.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2022-03-30 11:59:52.000000 zun-ui-9.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2022-03-30 11:59:52.000000 zun-ui-9.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.504554 zun-ui-9.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2022-03-30 11:59:52.000000 zun-ui-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.504554 zun-ui-9.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10135 2022-03-30 11:59:52.000000 zun-ui-9.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.504554 zun-ui-9.0.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      581 2022-03-30 11:59:52.000000 zun-ui-9.0.0/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.504554 zun-ui-9.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2022-03-30 11:59:52.000000 zun-ui-9.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2022-03-30 11:59:52.000000 zun-ui-9.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.504554 zun-ui-9.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2022-03-30 11:59:52.000000 zun-ui-9.0.0/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2567 2022-03-30 11:59:52.000000 zun-ui-9.0.0/lower-constraints.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      822 2022-03-30 11:59:52.000000 zun-ui-9.0.0/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2022-03-30 11:59:52.000000 zun-ui-9.0.0/package.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.508554 zun-ui-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/notes/add-reno-d6cc570f7a86e445.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/notes/bug-1763250-5035b39df953d25d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/notes/drop-py-2-7-e15513672c769acb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/notes/manage-security-groups-c17e4a0febe6dd4c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1897 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/notes/pike-322fc171cfab0443.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2750 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/notes/queens-1a10c0660636d2e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2475 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/notes/rocky-62e140c8a5971922.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/notes/stein-0b3ffcd0aba9eb45.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.508554 zun-ui-9.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8786 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.508554 zun-ui-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5165 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.508554 zun-ui-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20077 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/releasenotes/source/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.508554 zun-ui-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20025 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/releasenotes/source/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.508554 zun-ui-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22842 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.508554 zun-ui-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1380 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-03-30 11:59:52.000000 zun-ui-9.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2022-03-30 11:59:52.000000 zun-ui-9.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2022-03-30 12:00:25.524554 zun-ui-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-03-30 11:59:52.000000 zun-ui-9.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2022-03-30 11:59:52.000000 zun-ui-9.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2635 2022-03-30 11:59:52.000000 zun-ui-9.0.0/test-shim.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.508554 zun-ui-9.0.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2389 2022-03-30 11:59:52.000000 zun-ui-9.0.0/tools/install_venv.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5920 2022-03-30 11:59:52.000000 zun-ui-9.0.0/tools/install_venv_common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2022-03-30 11:59:52.000000 zun-ui-9.0.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3448 2022-03-30 11:59:52.000000 zun-ui-9.0.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.508554 zun-ui-9.0.0/zun_ui/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.512554 zun-ui-9.0.0/zun_ui/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10160 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/api/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8995 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/api/rest_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.512554 zun-ui-9.0.0/zun_ui/content/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.512554 zun-ui-9.0.0/zun_ui/content/cloud_shell/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/cloud_shell/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/cloud_shell/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.512554 zun-ui-9.0.0/zun_ui/content/container/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.512554 zun-ui-9.0.0/zun_ui/content/container/capsules/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/capsules/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/capsules/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/capsules/urls.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.512554 zun-ui-9.0.0/zun_ui/content/container/containers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/containers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/containers/admin_urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/containers/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/containers/tests.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/containers/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/containers/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.512554 zun-ui-9.0.0/zun_ui/content/container/hosts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/hosts/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      725 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/hosts/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/hosts/urls.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.512554 zun-ui-9.0.0/zun_ui/content/container/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/images/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/images/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/content/container/images/urls.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.512554 zun-ui-9.0.0/zun_ui/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/enabled/_0330_cloud_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/enabled/_1330_project_container_panelgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/enabled/_1331_project_container_containers_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      957 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/enabled/_1332_project_container_capsules_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/enabled/_2330_admin_container_panelgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/enabled/_2331_admin_container_images_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      946 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/enabled/_2332_admin_container_hosts_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      969 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/enabled/_2333_admin_container_containers_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/enabled/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5586 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/karma.conf.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/zun_ui/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/zun_ui/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.512554 zun-ui-9.0.0/zun_ui/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35731 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/locale/de/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/zun_ui/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.512554 zun-ui-9.0.0/zun_ui/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/locale/en_GB/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32906 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/locale/en_GB/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/zun_ui/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.516554 zun-ui-9.0.0/zun_ui/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/locale/id/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32370 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/locale/id/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/zun_ui/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.516554 zun-ui-9.0.0/zun_ui/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/locale/ja/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37487 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/locale/ja/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/zun_ui/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.516554 zun-ui-9.0.0/zun_ui/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/locale/ko_KR/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34510 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/locale/ko_KR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/zun_ui/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.516554 zun-ui-9.0.0/zun_ui/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/locale/ru/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46075 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/locale/ru/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/zun_ui/locale/tr_TR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.516554 zun-ui-9.0.0/zun_ui/locale/tr_TR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/locale/tr_TR/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.500554 zun-ui-9.0.0/zun_ui/locale/zh_Hans/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.516554 zun-ui-9.0.0/zun_ui/locale/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/models.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.504554 zun-ui-9.0.0/zun_ui/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.516554 zun-ui-9.0.0/zun_ui/static/cloud-shell/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5641 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/cloud-shell/cloud-shell.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/cloud-shell/cloud-shell.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/cloud-shell/cloud-shell.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/cloud-shell/cloud-shell.scss
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1523 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/cloud-shell/cloud-shell.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2407 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/cloud-shell/resizer.directive.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.504554 zun-ui-9.0.0/zun_ui/static/dashboard/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.516554 zun-ui-9.0.0/zun_ui/static/dashboard/container/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.516554 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.516554 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2569 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions/create.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5349 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions/delete.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions/refresh.service.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.516554 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions/workflow/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions/workflow/load-template.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions/workflow/load-template.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2088 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions/workflow/workflow.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2418 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5110 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/capsules.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2600 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/capsules.service.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.516554 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1547 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/details/details.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1045 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/details/overview.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1723 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/details/overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/drawer.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/panel.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/container.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/container.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/container.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.516554 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.520554 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5851 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/create.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5665 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/delete-force.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5797 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/delete-stop.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5924 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/delete.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5606 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/execute.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/kill.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3847 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/kill.service.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.520554 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1780 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/delete-security-group.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8740 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/manage-security-groups.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1526 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/manage-security-groups.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4747 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/manage-security-groups.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2524 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/pause.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4359 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/rebuild.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1887 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/refresh.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3870 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/restart.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2502 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/start.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3831 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/stop.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2546 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/unpause.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5406 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/update.service.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.520554 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/info.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/labels.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/misc.help.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.520554 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1761 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/delete-volume.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4417 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/mounts.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      399 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/mounts.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2218 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/mounts.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.520554 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/networks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2736 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/networks/networks.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1309 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/networks/networks.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7808 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/networks/networks.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.520554 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/ports/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2128 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/ports/ports.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      934 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/ports/ports.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6766 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/ports/ports.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.520554 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/scheduler-hints/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1873 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/scheduler-hints/scheduler-hints.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/scheduler-hints/scheduler-hints.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/scheduler-hints/scheduler-hints.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.520554 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-group-details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2112 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-groups.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      965 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-groups.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4055 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-groups.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/spec.help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24947 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/workflow.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5830 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7994 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/containers.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/containers.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/containers.scss
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2960 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/containers.service.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.524554 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1652 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/console.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/console.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2038 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/details.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/drawer.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1286 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/logs.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/logs.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1003 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/overview.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1471 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/panel.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.524554 zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.524554 zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/details/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1508 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/details/details.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3023 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/details/overview.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2111 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/details/overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4462 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/hosts.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/hosts.scss
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2448 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/hosts.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/panel.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.524554 zun-ui-9.0.0/zun_ui/static/dashboard/container/images/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.524554 zun-ui-9.0.0/zun_ui/static/dashboard/container/images/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2511 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/images/actions/create.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5205 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/images/actions/delete.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2779 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/images/actions/workflow.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2132 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/images/actions.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/images/drawer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4542 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/images/images.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1768 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/images/images.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/images/panel.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9953 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/static/dashboard/container/zun.service.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.504554 zun-ui-9.0.0/zun_ui/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.524554 zun-ui-9.0.0/zun_ui/templates/cloud_shell/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/templates/cloud_shell/cloud_shell.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.524554 zun-ui-9.0.0/zun_ui/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/test/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1348 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/test/settings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2022-03-30 11:59:52.000000 zun-ui-9.0.0/zun_ui/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 12:00:25.512554 zun-ui-9.0.0/zun_ui.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2022-03-30 12:00:25.000000 zun-ui-9.0.0/zun_ui.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10835 2022-03-30 12:00:25.000000 zun-ui-9.0.0/zun_ui.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-30 12:00:25.000000 zun-ui-9.0.0/zun_ui.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-30 12:00:25.000000 zun-ui-9.0.0/zun_ui.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-03-30 12:00:25.000000 zun-ui-9.0.0/zun_ui.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2022-03-30 12:00:25.000000 zun-ui-9.0.0/zun_ui.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2022-03-30 12:00:25.000000 zun-ui-9.0.0/zun_ui.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.398195 zun-ui-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1587 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/.eslintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2022-03-08 12:48:41.000000 zun-ui-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11861 2022-03-08 12:48:41.000000 zun-ui-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2022-03-08 12:48:41.398195 zun-ui-9.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/_0330_cloud_shell_settings.py.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/babel-django.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/babel-djangojs.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10135 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      581 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2567 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/lower-constraints.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      822 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/package.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.374195 zun-ui-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/notes/add-reno-d6cc570f7a86e445.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/notes/bug-1763250-5035b39df953d25d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/notes/drop-py-2-7-e15513672c769acb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/notes/manage-security-groups-c17e4a0febe6dd4c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1897 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/notes/pike-322fc171cfab0443.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2750 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/notes/queens-1a10c0660636d2e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2475 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/notes/rocky-62e140c8a5971922.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/notes/stein-0b3ffcd0aba9eb45.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8786 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.374195 zun-ui-9.0.0.0rc1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.374195 zun-ui-9.0.0.0rc1/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5165 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.374195 zun-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20077 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.374195 zun-ui-9.0.0.0rc1/releasenotes/source/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20025 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.374195 zun-ui-9.0.0.0rc1/releasenotes/source/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22842 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.374195 zun-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1380 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2022-03-08 12:48:41.398195 zun-ui-9.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2635 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/test-shim.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2389 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/tools/install_venv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5920 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/tools/install_venv_common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3448 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/zun_ui/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.386195 zun-ui-9.0.0.0rc1/zun_ui/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10160 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/api/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8995 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/api/rest_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.386195 zun-ui-9.0.0.0rc1/zun_ui/content/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.386195 zun-ui-9.0.0.0rc1/zun_ui/content/cloud_shell/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/cloud_shell/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/cloud_shell/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.386195 zun-ui-9.0.0.0rc1/zun_ui/content/container/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.386195 zun-ui-9.0.0.0rc1/zun_ui/content/container/capsules/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/capsules/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/capsules/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/capsules/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.386195 zun-ui-9.0.0.0rc1/zun_ui/content/container/containers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/containers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/containers/admin_urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/containers/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/containers/tests.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/containers/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/containers/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.386195 zun-ui-9.0.0.0rc1/zun_ui/content/container/hosts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/hosts/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      725 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/hosts/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/hosts/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.386195 zun-ui-9.0.0.0rc1/zun_ui/content/container/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/images/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/images/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/content/container/images/urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.386195 zun-ui-9.0.0.0rc1/zun_ui/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/enabled/_0330_cloud_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/enabled/_1330_project_container_panelgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/enabled/_1331_project_container_containers_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      957 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/enabled/_1332_project_container_capsules_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/enabled/_2330_admin_container_panelgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/enabled/_2331_admin_container_images_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      946 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/enabled/_2332_admin_container_hosts_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      969 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/enabled/_2333_admin_container_containers_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/enabled/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5586 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/karma.conf.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.378195 zun-ui-9.0.0.0rc1/zun_ui/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.378195 zun-ui-9.0.0.0rc1/zun_ui/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.386195 zun-ui-9.0.0.0rc1/zun_ui/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35731 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/locale/de/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.378195 zun-ui-9.0.0.0rc1/zun_ui/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.386195 zun-ui-9.0.0.0rc1/zun_ui/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/locale/en_GB/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32906 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/locale/en_GB/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.378195 zun-ui-9.0.0.0rc1/zun_ui/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.386195 zun-ui-9.0.0.0rc1/zun_ui/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/locale/id/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32370 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/locale/id/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.378195 zun-ui-9.0.0.0rc1/zun_ui/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.386195 zun-ui-9.0.0.0rc1/zun_ui/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/locale/ja/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37487 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/locale/ja/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.378195 zun-ui-9.0.0.0rc1/zun_ui/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.386195 zun-ui-9.0.0.0rc1/zun_ui/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/locale/ko_KR/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34510 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/locale/ko_KR/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.378195 zun-ui-9.0.0.0rc1/zun_ui/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.390195 zun-ui-9.0.0.0rc1/zun_ui/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/locale/ru/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46075 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/locale/ru/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.378195 zun-ui-9.0.0.0rc1/zun_ui/locale/tr_TR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.390195 zun-ui-9.0.0.0rc1/zun_ui/locale/tr_TR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/locale/tr_TR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.378195 zun-ui-9.0.0.0rc1/zun_ui/locale/zh_Hans/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.390195 zun-ui-9.0.0.0rc1/zun_ui/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/models.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.378195 zun-ui-9.0.0.0rc1/zun_ui/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.390195 zun-ui-9.0.0.0rc1/zun_ui/static/cloud-shell/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5641 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/cloud-shell/cloud-shell.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/cloud-shell/cloud-shell.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/cloud-shell/cloud-shell.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/cloud-shell/cloud-shell.scss
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1523 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/cloud-shell/cloud-shell.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2407 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/cloud-shell/resizer.directive.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.378195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.390195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.390195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.390195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2569 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions/create.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5349 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions/delete.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions/refresh.service.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.390195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions/workflow/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions/workflow/load-template.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions/workflow/load-template.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2088 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions/workflow/workflow.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2418 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5110 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/capsules.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2600 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/capsules.service.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.390195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1547 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/details/details.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1045 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/details/overview.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1723 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/details/overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1107 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/drawer.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/drawer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/panel.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1413 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/container.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/container.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/container.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.390195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.394195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5851 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/create.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5665 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/delete-force.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5797 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/delete-stop.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5924 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/delete.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5606 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/execute.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/kill.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3847 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/kill.service.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.394195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1780 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/delete-security-group.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8740 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/manage-security-groups.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1526 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/manage-security-groups.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4747 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/manage-security-groups.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2524 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/pause.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4359 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/rebuild.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1887 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/refresh.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3870 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/restart.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2502 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/start.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3831 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/stop.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2546 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/unpause.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5406 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/update.service.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.394195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/info.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/labels.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/misc.help.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.394195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1761 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/delete-volume.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4417 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/mounts.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      399 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/mounts.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2218 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/mounts.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.394195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/networks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2736 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/networks/networks.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1309 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/networks/networks.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7808 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/networks/networks.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.394195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/ports/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2128 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/ports/ports.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      934 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/ports/ports.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6766 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/ports/ports.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.394195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/scheduler-hints/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1873 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/scheduler-hints/scheduler-hints.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/scheduler-hints/scheduler-hints.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/scheduler-hints/scheduler-hints.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.394195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-group-details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2112 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-groups.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      965 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-groups.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4055 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-groups.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/spec.help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24947 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/workflow.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5830 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7994 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/containers.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/containers.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/containers.scss
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2960 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/containers.service.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.394195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1652 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/console.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/console.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2038 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/details.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/drawer.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/drawer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1286 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/logs.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/logs.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1003 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/overview.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1471 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/panel.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.394195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.394195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/details/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1508 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/details/details.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3023 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/details/overview.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2111 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/details/overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/drawer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4462 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/hosts.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/hosts.scss
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2448 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/hosts.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/panel.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.398195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.398195 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2511 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/actions/create.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5205 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/actions/delete.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2779 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/actions/workflow.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2132 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/actions.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/drawer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4542 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/images.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1768 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/images.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/panel.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9953 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/zun.service.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.378195 zun-ui-9.0.0.0rc1/zun_ui/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.398195 zun-ui-9.0.0.0rc1/zun_ui/templates/cloud_shell/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/templates/cloud_shell/cloud_shell.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.398195 zun-ui-9.0.0.0rc1/zun_ui/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/test/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1348 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/test/settings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2022-03-08 12:48:06.000000 zun-ui-9.0.0.0rc1/zun_ui/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-08 12:48:41.382195 zun-ui-9.0.0.0rc1/zun_ui.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2022-03-08 12:48:41.000000 zun-ui-9.0.0.0rc1/zun_ui.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10835 2022-03-08 12:48:41.000000 zun-ui-9.0.0.0rc1/zun_ui.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-08 12:48:41.000000 zun-ui-9.0.0.0rc1/zun_ui.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-08 12:48:41.000000 zun-ui-9.0.0.0rc1/zun_ui.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-03-08 12:48:41.000000 zun-ui-9.0.0.0rc1/zun_ui.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2022-03-08 12:48:41.000000 zun-ui-9.0.0.0rc1/zun_ui.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2022-03-08 12:48:41.000000 zun-ui-9.0.0.0rc1/zun_ui.egg-info/top_level.txt
```

### Comparing `zun-ui-9.0.0/.eslintrc` & `zun-ui-9.0.0.0rc1/.eslintrc`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/AUTHORS` & `zun-ui-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/ChangeLog` & `zun-ui-9.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * Updating python testing classifier as per Yoga testing runtime
 * Add Python3 yoga unit tests
 * Update master for stable/xena
 
 8.0.0
 -----
```

### Comparing `zun-ui-9.0.0/LICENSE` & `zun-ui-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/PKG-INFO` & `zun-ui-9.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: zun-ui
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Zun User Interface
 Home-page: https://docs.openstack.org/zun-ui/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==========
         zun-ui
```

### Comparing `zun-ui-9.0.0/devstack/plugin.sh` & `zun-ui-9.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/doc/requirements.txt` & `zun-ui-9.0.0.0rc1/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/doc/source/conf.py` & `zun-ui-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/doc/source/configuration/index.rst` & `zun-ui-9.0.0.0rc1/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/doc/source/install/index.rst` & `zun-ui-9.0.0.0rc1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/lower-constraints.txt` & `zun-ui-9.0.0.0rc1/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/manage.py` & `zun-ui-9.0.0.0rc1/manage.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/package.json` & `zun-ui-9.0.0.0rc1/package.json`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/releasenotes/notes/pike-322fc171cfab0443.yaml` & `zun-ui-9.0.0.0rc1/releasenotes/notes/pike-322fc171cfab0443.yaml`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/releasenotes/notes/queens-1a10c0660636d2e0.yaml` & `zun-ui-9.0.0.0rc1/releasenotes/notes/queens-1a10c0660636d2e0.yaml`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/releasenotes/notes/rocky-62e140c8a5971922.yaml` & `zun-ui-9.0.0.0rc1/releasenotes/notes/rocky-62e140c8a5971922.yaml`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/releasenotes/notes/stein-0b3ffcd0aba9eb45.yaml` & `zun-ui-9.0.0.0rc1/releasenotes/notes/stein-0b3ffcd0aba9eb45.yaml`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/releasenotes/source/conf.py` & `zun-ui-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `zun-ui-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `zun-ui-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po` & `zun-ui-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po` & `zun-ui-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `zun-ui-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/requirements.txt` & `zun-ui-9.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/setup.cfg` & `zun-ui-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/setup.py` & `zun-ui-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/test-requirements.txt` & `zun-ui-9.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/test-shim.js` & `zun-ui-9.0.0.0rc1/test-shim.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/tools/install_venv.py` & `zun-ui-9.0.0.0rc1/tools/install_venv.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/tools/install_venv_common.py` & `zun-ui-9.0.0.0rc1/tools/install_venv_common.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/tox.ini` & `zun-ui-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/api/client.py` & `zun-ui-9.0.0.0rc1/zun_ui/api/client.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/api/rest_api.py` & `zun-ui-9.0.0.0rc1/zun_ui/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/content/cloud_shell/views.py` & `zun-ui-9.0.0.0rc1/zun_ui/content/cloud_shell/views.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/content/container/__init__.py` & `zun-ui-9.0.0.0rc1/zun_ui/content/container/__init__.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/content/container/capsules/panel.py` & `zun-ui-9.0.0.0rc1/zun_ui/content/container/capsules/panel.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/content/container/capsules/urls.py` & `zun-ui-9.0.0.0rc1/zun_ui/content/container/capsules/urls.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/content/container/containers/admin_urls.py` & `zun-ui-9.0.0.0rc1/zun_ui/content/container/containers/admin_urls.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/content/container/containers/panel.py` & `zun-ui-9.0.0.0rc1/zun_ui/content/container/containers/panel.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/content/container/containers/tests.py` & `zun-ui-9.0.0.0rc1/zun_ui/content/container/containers/tests.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/content/container/containers/urls.py` & `zun-ui-9.0.0.0rc1/zun_ui/content/container/containers/urls.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/content/container/containers/views.py` & `zun-ui-9.0.0.0rc1/zun_ui/content/container/containers/views.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/content/container/hosts/panel.py` & `zun-ui-9.0.0.0rc1/zun_ui/content/container/hosts/panel.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/content/container/hosts/urls.py` & `zun-ui-9.0.0.0rc1/zun_ui/content/container/hosts/urls.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/content/container/images/panel.py` & `zun-ui-9.0.0.0rc1/zun_ui/content/container/images/panel.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/content/container/images/urls.py` & `zun-ui-9.0.0.0rc1/zun_ui/content/container/images/urls.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/enabled/_0330_cloud_shell.py` & `zun-ui-9.0.0.0rc1/zun_ui/enabled/_0330_cloud_shell.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/enabled/_1330_project_container_panelgroup.py` & `zun-ui-9.0.0.0rc1/zun_ui/enabled/_1330_project_container_panelgroup.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/enabled/_1331_project_container_containers_panel.py` & `zun-ui-9.0.0.0rc1/zun_ui/enabled/_1331_project_container_containers_panel.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/enabled/_1332_project_container_capsules_panel.py` & `zun-ui-9.0.0.0rc1/zun_ui/enabled/_1332_project_container_capsules_panel.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/enabled/_2330_admin_container_panelgroup.py` & `zun-ui-9.0.0.0rc1/zun_ui/enabled/_2330_admin_container_panelgroup.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/enabled/_2331_admin_container_images_panel.py` & `zun-ui-9.0.0.0rc1/zun_ui/enabled/_2331_admin_container_images_panel.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/enabled/_2332_admin_container_hosts_panel.py` & `zun-ui-9.0.0.0rc1/zun_ui/enabled/_2332_admin_container_hosts_panel.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/enabled/_2333_admin_container_containers_panel.py` & `zun-ui-9.0.0.0rc1/zun_ui/enabled/_2333_admin_container_containers_panel.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/karma.conf.js` & `zun-ui-9.0.0.0rc1/zun_ui/karma.conf.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/locale/de/LC_MESSAGES/django.po` & `zun-ui-9.0.0.0rc1/zun_ui/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/locale/de/LC_MESSAGES/djangojs.po` & `zun-ui-9.0.0.0rc1/zun_ui/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/locale/en_GB/LC_MESSAGES/django.po` & `zun-ui-9.0.0.0rc1/zun_ui/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/locale/en_GB/LC_MESSAGES/djangojs.po` & `zun-ui-9.0.0.0rc1/zun_ui/locale/en_GB/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/locale/id/LC_MESSAGES/django.po` & `zun-ui-9.0.0.0rc1/zun_ui/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/locale/id/LC_MESSAGES/djangojs.po` & `zun-ui-9.0.0.0rc1/zun_ui/locale/id/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/locale/ja/LC_MESSAGES/django.po` & `zun-ui-9.0.0.0rc1/zun_ui/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/locale/ja/LC_MESSAGES/djangojs.po` & `zun-ui-9.0.0.0rc1/zun_ui/locale/ja/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/locale/ko_KR/LC_MESSAGES/django.po` & `zun-ui-9.0.0.0rc1/zun_ui/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/locale/ko_KR/LC_MESSAGES/djangojs.po` & `zun-ui-9.0.0.0rc1/zun_ui/locale/ko_KR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/locale/ru/LC_MESSAGES/django.po` & `zun-ui-9.0.0.0rc1/zun_ui/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/locale/ru/LC_MESSAGES/djangojs.po` & `zun-ui-9.0.0.0rc1/zun_ui/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/locale/tr_TR/LC_MESSAGES/django.po` & `zun-ui-9.0.0.0rc1/zun_ui/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/locale/zh_Hans/LC_MESSAGES/django.po` & `zun-ui-9.0.0.0rc1/zun_ui/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/cloud-shell/cloud-shell.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/cloud-shell/cloud-shell.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/cloud-shell/cloud-shell.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/cloud-shell/cloud-shell.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/cloud-shell/cloud-shell.module.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/cloud-shell/cloud-shell.module.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/cloud-shell/cloud-shell.scss` & `zun-ui-9.0.0.0rc1/zun_ui/static/cloud-shell/cloud-shell.scss`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/cloud-shell/cloud-shell.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/cloud-shell/cloud-shell.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/cloud-shell/resizer.directive.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/cloud-shell/resizer.directive.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions/create.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions/create.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions/delete.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions/delete.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions/refresh.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions/refresh.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions/workflow/load-template.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions/workflow/load-template.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions/workflow/workflow.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions/workflow/workflow.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/actions.module.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/actions.module.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/capsules.module.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/capsules.module.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/capsules.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/capsules.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/details/details.module.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/details/details.module.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/details/overview.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/details/overview.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/details/overview.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/details/overview.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/capsules/drawer.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/capsules/drawer.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/container.module.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/container.module.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/container.module.spec.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/container.module.spec.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/create.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/create.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/delete-force.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/delete-force.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/delete-stop.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/delete-stop.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/delete.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/delete.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/execute.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/execute.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/kill.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/kill.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/delete-security-group.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/delete-security-group.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/manage-security-groups.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/manage-security-groups.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/manage-security-groups.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/manage-security-groups.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/manage-security-groups.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/manage-security-groups/manage-security-groups.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/pause.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/pause.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/rebuild.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/rebuild.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/refresh.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/refresh.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/restart.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/restart.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/start.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/start.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/stop.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/stop.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/unpause.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/unpause.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/update.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/update.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/info.help.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/info.help.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/delete-volume.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/delete-volume.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/mounts.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/mounts.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/mounts.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/mounts/mounts.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/networks/networks.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/networks/networks.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/networks/networks.help.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/networks/networks.help.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/networks/networks.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/networks/networks.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/ports/ports.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/ports/ports.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/ports/ports.help.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/ports/ports.help.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/ports/ports.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/ports/ports.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/scheduler-hints/scheduler-hints.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/scheduler-hints/scheduler-hints.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-group-details.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-group-details.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-groups.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-groups.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-groups.help.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-groups.help.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-groups.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/security-groups/security-groups.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/spec.help.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/spec.help.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions/workflow/workflow.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions/workflow/workflow.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/actions.module.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/actions.module.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/containers.module.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/containers.module.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/containers.module.spec.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/containers.module.spec.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/containers.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/containers.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/console.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/console.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/details.module.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/details.module.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/drawer.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/drawer.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/logs.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/logs.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/overview.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/overview.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/containers/details/overview.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/containers/details/overview.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/details/details.module.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/details/details.module.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/details/overview.controller.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/details/overview.controller.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/details/overview.html` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/details/overview.html`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/hosts.module.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/hosts.module.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/hosts.scss` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/hosts.scss`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/hosts/hosts.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/hosts/hosts.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/images/actions/create.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/actions/create.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/images/actions/delete.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/actions/delete.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/images/actions/workflow.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/actions/workflow.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/images/actions.module.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/actions.module.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/images/images.module.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/images.module.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/images/images.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/images/images.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/static/dashboard/container/zun.service.js` & `zun-ui-9.0.0.0rc1/zun_ui/static/dashboard/container/zun.service.js`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui/test/settings.py` & `zun-ui-9.0.0.0rc1/zun_ui/test/settings.py`

 * *Files identical despite different names*

### Comparing `zun-ui-9.0.0/zun_ui.egg-info/PKG-INFO` & `zun-ui-9.0.0.0rc1/zun_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: zun-ui
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Zun User Interface
 Home-page: https://docs.openstack.org/zun-ui/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==========
         zun-ui
```

### Comparing `zun-ui-9.0.0/zun_ui.egg-info/SOURCES.txt` & `zun-ui-9.0.0.0rc1/zun_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

