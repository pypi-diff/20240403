# Comparing `tmp/blazar-nova-5.0.0.tar.gz` & `tmp/blazar-nova-5.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blazar-nova-5.0.0.tar", last modified: Wed Apr  3 11:08:38 2024, max compression
+gzip compressed data, was "blazar-nova-5.0.0.0rc1.tar", last modified: Thu Mar 14 07:29:05 2024, max compression
```

## Comparing `blazar-nova-5.0.0.tar` & `blazar-nova-5.0.0.0rc1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.270465 blazar-nova-5.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1408 2024-04-03 11:08:38.000000 blazar-nova-5.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4510 2024-04-03 11:08:38.000000 blazar-nova-5.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2024-04-03 11:08:38.270465 blazar-nova-5.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.266464 blazar-nova-5.0.0/blazar_nova.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2024-04-03 11:08:38.000000 blazar-nova-5.0.0/blazar_nova.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2024-04-03 11:08:38.000000 blazar-nova-5.0.0/blazar_nova.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:08:38.000000 blazar-nova-5.0.0/blazar_nova.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:08:38.000000 blazar-nova-5.0.0/blazar_nova.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-04-03 11:08:38.000000 blazar-nova-5.0.0/blazar_nova.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-04-03 11:08:38.000000 blazar-nova-5.0.0/blazar_nova.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2024-04-03 11:08:38.000000 blazar-nova-5.0.0/blazar_nova.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.266464 blazar-nova-5.0.0/blazarnova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/blazarnova/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1320 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/blazarnova/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.266464 blazar-nova-5.0.0/blazarnova/scheduler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/blazarnova/scheduler/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.266464 blazar-nova-5.0.0/blazarnova/scheduler/filters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/blazarnova/scheduler/filters/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7018 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/blazarnova/scheduler/filters/blazar_filter.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.266464 blazar-nova-5.0.0/blazarnova/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/blazarnova/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.266464 blazar-nova-5.0.0/blazarnova/tests/scheduler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/blazarnova/tests/scheduler/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.266464 blazar-nova-5.0.0/blazarnova/tests/scheduler/filters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/blazarnova/tests/scheduler/filters/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13868 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/blazarnova/tests/scheduler/filters/test_blazar_filter.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.266464 blazar-nova-5.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.266464 blazar-nova-5.0.0/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/etc/nova.conf.example
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.266464 blazar-nova-5.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.266464 blazar-nova-5.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/releasenotes/notes/drop-python2-406d4474c1cf9cf9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/releasenotes/notes/preemptible-instances-7c3731586faa9b0d.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.270465 blazar-nova-5.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.270465 blazar-nova-5.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.270465 blazar-nova-5.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8566 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2024-04-03 11:08:38.270465 blazar-nova-5.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:38.270465 blazar-nova-5.0.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2231 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/tools/tox_install.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1299 2024-04-03 11:08:07.000000 blazar-nova-5.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.629872 blazar-nova-5.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1408 2024-03-14 07:29:05.000000 blazar-nova-5.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4520 2024-03-14 07:29:05.000000 blazar-nova-5.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2167 2024-03-14 07:29:05.629872 blazar-nova-5.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      854 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.621868 blazar-nova-5.0.0.0rc1/blazar_nova.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2167 2024-03-14 07:29:05.000000 blazar-nova-5.0.0.0rc1/blazar_nova.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2024-03-14 07:29:05.000000 blazar-nova-5.0.0.0rc1/blazar_nova.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-14 07:29:05.000000 blazar-nova-5.0.0.0rc1/blazar_nova.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-14 07:29:05.000000 blazar-nova-5.0.0.0rc1/blazar_nova.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-14 07:29:05.000000 blazar-nova-5.0.0.0rc1/blazar_nova.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-03-14 07:29:05.000000 blazar-nova-5.0.0.0rc1/blazar_nova.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2024-03-14 07:29:05.000000 blazar-nova-5.0.0.0rc1/blazar_nova.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.621868 blazar-nova-5.0.0.0rc1/blazarnova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/blazarnova/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1320 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/blazarnova/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.625870 blazar-nova-5.0.0.0rc1/blazarnova/scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/blazarnova/scheduler/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.625870 blazar-nova-5.0.0.0rc1/blazarnova/scheduler/filters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/blazarnova/scheduler/filters/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7018 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/blazarnova/scheduler/filters/blazar_filter.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.625870 blazar-nova-5.0.0.0rc1/blazarnova/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/blazarnova/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.625870 blazar-nova-5.0.0.0rc1/blazarnova/tests/scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/blazarnova/tests/scheduler/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.625870 blazar-nova-5.0.0.0rc1/blazarnova/tests/scheduler/filters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/blazarnova/tests/scheduler/filters/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13868 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/blazarnova/tests/scheduler/filters/test_blazar_filter.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.625870 blazar-nova-5.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.625870 blazar-nova-5.0.0.0rc1/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/etc/nova.conf.example
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.617867 blazar-nova-5.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.625870 blazar-nova-5.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/releasenotes/notes/drop-python2-406d4474c1cf9cf9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/releasenotes/notes/preemptible-instances-7c3731586faa9b0d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.629872 blazar-nova-5.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.629872 blazar-nova-5.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.629872 blazar-nova-5.0.0.0rc1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8566 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2024-03-14 07:29:05.629872 blazar-nova-5.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:05.629872 blazar-nova-5.0.0.0rc1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2231 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/tools/tox_install.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1299 2024-03-14 07:28:37.000000 blazar-nova-5.0.0.0rc1/tox.ini
```

### Comparing `blazar-nova-5.0.0/AUTHORS` & `blazar-nova-5.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `blazar-nova-5.0.0/ChangeLog` & `blazar-nova-5.0.0.0rc1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-5.0.0
------
+5.0.0.0rc1
+----------
 
 * reno: Update master for unmaintained/yoga
 * Update python classifier in setup.cfg
 * Use generic testing template
 * Update master for stable/2023.2
 
 4.0.0
```

### Comparing `blazar-nova-5.0.0/LICENSE` & `blazar-nova-5.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `blazar-nova-5.0.0/PKG-INFO` & `blazar-nova-5.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: blazar-nova
-Version: 5.0.0
+Version: 5.0.0.0rc1
 Summary: Nova related filters and extensions for Blazar
 Home-page: https://launchpad.net/blazar
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache Software License
 Description: ========================
         Team and repository tags
```

### Comparing `blazar-nova-5.0.0/README.rst` & `blazar-nova-5.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `blazar-nova-5.0.0/blazar_nova.egg-info/PKG-INFO` & `blazar-nova-5.0.0.0rc1/blazar_nova.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: blazar-nova
-Version: 5.0.0
+Version: 5.0.0.0rc1
 Summary: Nova related filters and extensions for Blazar
 Home-page: https://launchpad.net/blazar
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache Software License
 Description: ========================
         Team and repository tags
```

### Comparing `blazar-nova-5.0.0/blazar_nova.egg-info/SOURCES.txt` & `blazar-nova-5.0.0.0rc1/blazar_nova.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blazar-nova-5.0.0/blazarnova/i18n.py` & `blazar-nova-5.0.0.0rc1/blazarnova/i18n.py`

 * *Files identical despite different names*

### Comparing `blazar-nova-5.0.0/blazarnova/scheduler/filters/blazar_filter.py` & `blazar-nova-5.0.0.0rc1/blazarnova/scheduler/filters/blazar_filter.py`

 * *Files identical despite different names*

### Comparing `blazar-nova-5.0.0/blazarnova/tests/scheduler/filters/test_blazar_filter.py` & `blazar-nova-5.0.0.0rc1/blazarnova/tests/scheduler/filters/test_blazar_filter.py`

 * *Files identical despite different names*

### Comparing `blazar-nova-5.0.0/releasenotes/source/conf.py` & `blazar-nova-5.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `blazar-nova-5.0.0/requirements.txt` & `blazar-nova-5.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `blazar-nova-5.0.0/setup.cfg` & `blazar-nova-5.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `blazar-nova-5.0.0/setup.py` & `blazar-nova-5.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `blazar-nova-5.0.0/tools/tox_install.sh` & `blazar-nova-5.0.0.0rc1/tools/tox_install.sh`

 * *Files identical despite different names*

### Comparing `blazar-nova-5.0.0/tox.ini` & `blazar-nova-5.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

