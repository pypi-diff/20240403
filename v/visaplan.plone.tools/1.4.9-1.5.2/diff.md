# Comparing `tmp/visaplan.plone.tools-1.4.9.tar.gz` & `tmp/visaplan.plone.tools-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/visaplan.plone.tools-1.4.9.tar", last modified: Mon Dec 13 12:03:32 2021, max compression
+gzip compressed data, was "dist/visaplan.plone.tools-1.5.2.tar", last modified: Thu Mar 21 11:25:53 2024, max compression
```

## Comparing `visaplan.plone.tools-1.4.9.tar` & `visaplan.plone.tools-1.5.2.tar`

### file list

```diff
@@ -1,98 +1,115 @@
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/docs/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/LICENSE.GPL
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      669 2019-11-06 14:05:55.000000 visaplan.plone.tools-1.4.9/docs/LICENSE.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      615 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/Makefile
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5494 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/conf.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      103 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/conf.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      501 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/index.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      822 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/make.bat
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      102 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/modules.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      106 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/setup.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      233 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/visaplan.plone.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      181 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/visaplan.plone.tools.functions.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      258 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/visaplan.plone.tools.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      209 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/visaplan.rst
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/Extensions/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      476 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/Extensions/install.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3074 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    19711 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_args.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2416 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_attr.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8765 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_decorator.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1680 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_exc.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    12742 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_get_object.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4632 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_gs.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     7747 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_make_folder.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1224 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_misc.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    22901 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_o_tools.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4425 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_query.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    13482 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_reindex.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8117 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_rename.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5543 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_roles.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1563 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_switch.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    32525 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_tree.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1651 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_types.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    10604 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_uid.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3153 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_watch.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    24264 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_workflow.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       45 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1137 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/check-blobs-delete-selected.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2143 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/check-blobs.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      884 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    13282 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/fixblobs.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1557 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at0.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      921 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at1.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    13055 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at2.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      916 2021-11-29 09:44:56.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at3.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3023 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at4.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3740 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at5.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3108 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_dx4.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3601 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_dx5.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1583 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_have.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      753 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/attools.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8290 2021-11-29 09:44:56.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/brains.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    14072 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/cfg.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      202 2021-11-29 09:44:57.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    18026 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/context.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      882 2021-01-20 13:47:52.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/decorators.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      346 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/dxtools.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    30708 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/forms.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3171 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/functions.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    23246 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/groups.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1692 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/indexes.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     7265 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/log.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3539 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/mock.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1802 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/mock_cfg.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      817 2021-11-29 09:44:56.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/profiles.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    11970 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/search.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      832 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setuphandlers.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    12730 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/zcmlgen.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2019-11-06 14:14:59.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2019-11-06 14:14:59.000000 visaplan.plone.tools-1.4.9/src/visaplan/__init__.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    21741 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2923 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/entry_points.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       24 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/namespace_packages.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2019-03-25 17:32:23.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/not-zip-safe
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       68 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/requires.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/top_level.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    11351 2021-12-13 12:02:22.000000 visaplan.plone.tools-1.4.9/CHANGES.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/CONTRIBUTORS.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      183 2020-01-14 11:15:58.000000 visaplan.plone.tools-1.4.9/MANIFEST.in
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3742 2021-11-29 09:44:57.000000 visaplan.plone.tools-1.4.9/README.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      218 2021-12-13 12:02:16.000000 visaplan.plone.tools-1.4.9/TODO.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        6 2021-12-06 14:47:42.000000 visaplan.plone.tools-1.4.9/VERSION
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     9342 2020-09-04 22:52:51.000000 visaplan.plone.tools-1.4.9/long-description.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1404 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/setup.cfg
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     6854 2021-12-13 12:01:11.000000 visaplan.plone.tools-1.4.9/setup.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    15408 2021-12-13 12:00:01.000000 visaplan.plone.tools-1.4.9/test.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    21741 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/PKG-INFO
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/docs/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/LICENSE.GPL
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      669 2019-11-06 14:05:55.000000 visaplan.plone.tools-1.5.2/docs/LICENSE.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      615 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/Makefile
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5494 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/conf.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      103 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/conf.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      501 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/index.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      822 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/make.bat
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      102 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/modules.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      106 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/setup.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      233 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/visaplan.plone.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      181 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/visaplan.plone.tools.functions.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      258 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/visaplan.plone.tools.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      209 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/docs/visaplan.rst
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      759 2023-11-29 09:56:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      839 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_data.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8596 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_group.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3413 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_group_pio.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8675 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_helpers.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      687 2022-01-20 18:12:16.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_imports.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8339 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_membership.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5968 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_user.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3418 2023-11-14 00:16:32.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/groups/_user_pio.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/infofact/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5483 2022-01-20 18:17:48.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/infofact/_group.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3215 2022-01-20 14:33:44.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/infofact/_membership.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3431 2022-01-20 14:32:17.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/infofact/_user.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3114 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    19711 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_args.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2416 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_attr.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    12467 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_decorator.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1668 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_exc.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    12815 2024-02-09 10:40:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_get_object.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4632 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_gs.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     7747 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_make_folder.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1224 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_misc.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    22871 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_o_tools.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4622 2023-11-29 09:56:09.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_query.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    13552 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_reindex.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8117 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_rename.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5543 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_roles.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1563 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_switch.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    32598 2024-02-09 10:40:18.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_tree.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1651 2022-01-20 18:12:16.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_types.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    10604 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_uid.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3153 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_watch.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    24264 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_workflow.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       45 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1137 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/check-blobs-delete-selected.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2143 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/check-blobs.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      884 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    13282 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/fixblobs.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1557 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at0.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      921 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at1.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    13055 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at2.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      916 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at3.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3023 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at4.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3909 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at5.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      539 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at6.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3108 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_dx4.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3601 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_dx5.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1275 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_have.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      760 2023-11-29 09:56:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_idxnames.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1317 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/attools.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8290 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/brains.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    15313 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/cfg.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      202 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    18151 2024-03-21 11:22:18.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/context.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    18047 2024-01-22 12:38:47.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/context.py.orig
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1859 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/decorators.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      346 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/dxtools.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5190 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/env.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    30839 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/forms.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5041 2023-11-29 09:56:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/functions.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1692 2022-01-20 18:12:16.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/indexes.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    10338 2024-02-09 10:40:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/lock.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     7325 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/log.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3539 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/mock.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1799 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/mock_cfg.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      817 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/profiles.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    11691 2024-02-09 10:35:17.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/search.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4919 2023-11-29 09:56:09.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/seo.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1452 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setuphandlers.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      291 2022-12-06 12:33:06.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/strings.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    12714 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/zcmlgen.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2019-11-06 14:14:59.000000 visaplan.plone.tools-1.5.2/src/visaplan/plone/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2019-11-06 14:14:59.000000 visaplan.plone.tools-1.5.2/src/visaplan/__init__.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    28324 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/PKG-INFO
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3607 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/entry_points.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       24 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/namespace_packages.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2019-03-25 17:32:23.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/not-zip-safe
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      116 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/requires.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2024-03-21 11:25:52.000000 visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/top_level.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    15722 2024-03-21 11:24:19.000000 visaplan.plone.tools-1.5.2/CHANGES.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.5.2/CONTRIBUTORS.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      183 2020-01-14 11:15:58.000000 visaplan.plone.tools-1.5.2/MANIFEST.in
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3933 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/README.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      218 2023-11-14 00:16:00.000000 visaplan.plone.tools-1.5.2/TODO.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        6 2024-02-26 10:42:52.000000 visaplan.plone.tools-1.5.2/VERSION
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     9342 2020-09-04 22:52:51.000000 visaplan.plone.tools-1.5.2/long-description.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1597 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/setup.cfg
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     7604 2024-03-21 11:20:35.000000 visaplan.plone.tools-1.5.2/setup.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    28324 2024-03-21 11:25:53.000000 visaplan.plone.tools-1.5.2/PKG-INFO
```

### Comparing `visaplan.plone.tools-1.4.9/docs/LICENSE.GPL` & `visaplan.plone.tools-1.5.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/docs/LICENSE.rst` & `visaplan.plone.tools-1.5.2/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/docs/Makefile` & `visaplan.plone.tools-1.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/docs/conf.py` & `visaplan.plone.tools-1.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/docs/make.bat` & `visaplan.plone.tools-1.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/__init__.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 __all__ = [
         ## _args (Helferlein für **kwargs):
         'extract_object_and_brain', # --> (o, brain)
         'extract_object_or_brain',  # --> (o, brain=None)
         'extract_brain_or_object',  # --> (brain, o=None)
         ## _attr:
         'make_attribute_setter',
-        ## _decorator:
+        ## _decorator.py:
         'step',
+        'importStep',
         'StepAborted',
         ## _get_object:
         'make_object_getter',
         ## _make_folder:
         'make_subfolder_creator',
         ## _query:
         'make_query_extractor',
         'iterate_query',
         'getAllLanguages',
-        ## _reindex:
+        ## _reindex.py:
         'make_reindexer',
         'reindex_all',
         ## _rename:
         # 'make_mover',  (noch nicht implementiert)
         'make_renamer',
         'ACCEPT_ANY',
         ## _roles:
@@ -57,15 +58,15 @@
 # Local imports:
 from visaplan.plone.tools.setup._args import (
     extract_brain_or_object,
     extract_object_and_brain,
     extract_object_or_brain,
     )
 from visaplan.plone.tools.setup._attr import make_attribute_setter
-from visaplan.plone.tools.setup._decorator import StepAborted, step
+from visaplan.plone.tools.setup._decorator import StepAborted, importStep, step
 from visaplan.plone.tools.setup._get_object import make_object_getter
 from visaplan.plone.tools.setup._gs import load_and_cook, safe_context_id
 from visaplan.plone.tools.setup._make_folder import make_subfolder_creator
 from visaplan.plone.tools.setup._query import (
     getAllLanguages,
     iterate_query,
     make_query_extractor,
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_args.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_args.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_attr.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_attr.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_exc.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_exc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*- äöü vim: sw=4 sts=4 et tw=79
 # Python compatibility:
 from __future__ import absolute_import
 
-# Setup tools:
-import pkg_resources
+from importlib_metadata import PackageNotFoundError, version
 
 try:
-    pkg_resources.get_distribution('Products.LinguaPlone')
-except pkg_resources.DistributionNotFound:
+    version('Products.LinguaPlone')
+except PackageNotFoundError:
     class AlreadyTranslated(Exception):
         """
         Dummy exception; Products.LinguaPlone is not installed
         """
 else:
     # Zope:
     from Products.LinguaPlone.I18NBaseObject import AlreadyTranslated
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_get_object.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_get_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     )
 
 if HAS_SUBPORTALS:
     # Local imports:
     from visaplan.plone.tools.setup._o_tools import handle_subportal
 
 # Local imports:
+from .._idxnames import getExcludeFromNav
 from visaplan.plone.tools.setup._reindex import make_reindexer
 
 # Logging / Debugging:
 import logging
 from pdb import set_trace
 
 __all__ = [
@@ -132,15 +133,15 @@
     if set_canonical is None:
         set_canonical = set_language
     set_subportal = pop('set_subportal', None)
     subportal     = pop('subportal', None)
     return_tuple  = pop('return_tuple', False)
 
     if set_menu is not None:
-        idxs.append('getExcludeFromNav')
+        idxs.append(getExcludeFromNav)  # changed to 'exclude_from_nav'
     if set_title:
         idxs.extend([
             'Title',
             'getTitleIndex',  # ??
             'sortable_title',
             'SearchableText',    # contains the title
             'getEfectiveIndex',  # contains lower-cased title after numeric time
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_gs.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_gs.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_make_folder.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_make_folder.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_misc.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_misc.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_o_tools.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_o_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from __future__ import absolute_import
 
 from six import string_types as six_string_types
 from six.moves import map
 
 # Standard library:
 from collections import defaultdict
-from pprint import pprint
 
 # Zope:
 from Products.CMFCore.utils import getToolByName
 
 # Local imports:
 from visaplan.plone.tools._have import HAS_SUBPORTALS, HAS_VPSEARCH
 from visaplan.plone.tools.setup._args import (
@@ -306,15 +305,15 @@
             if canonical and canonical != o:
                 _NFO('Setting canonical to %(canonical)r', locals())
                 try:
                     o.addTranslationReference(canonical)
                 except AlreadyTranslated as e:
                     _ERR('%(o)r is already translated!', locals())
                     _ERR(str(CantAddTranslationReference(o, canonical)), {})
-                    if 0: pprint({
+                    if 0: pp({
                         'o': o, 'canonical': canonical,
                         'identical?': canonical is o,
                         })
                     set_trace()
                     nochmal = 0
                     if nochmal:
                         o.addTranslationReference(canonical)
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_query.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from __future__ import absolute_import
 
 from six import string_types as six_string_types
 
 # Zope:
 from Products.CMFCore.utils import getToolByName
 
+# Local imports:
+from visaplan.plone.tools._idxnames import getExcludeFromSearch
+
 # Logging / Debugging:
 import logging
 
 __all__ = [
         'make_query_extractor',
         'iterate_query',
         'getAllLanguages',
@@ -29,20 +32,21 @@
         """
         query = {}
         if do_pop:
             pop = dic.pop
         else:
             pop = dic.get
 
-        if 'getExcludeFromSearch' not in dic:
-            query['getExcludeFromSearch'] = False
+        if getExcludeFromSearch not in dic:
+            query[getExcludeFromSearch] = False  # WIP: change index name
         else:
-            val = pop('getExcludeFromSearch')
+            val = pop(getExcludeFromSearch)
             if val is not None:
-                query['getExcludeFromSearch'] = int(val)
+                # or bool(val)? what values do we expect (or support)?
+                query[getExcludeFromSearch] = int(val)  # WIP: change index name
         # optionale Argumente ohne Vorgabewert:
         for name in [
             'portal_type',
             'getCustomSearch',
             'path',
             ]:
             if name in dic:
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_reindex.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_reindex.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,22 +17,21 @@
 metadata attribute, you might want to use collective.metadataversion,
 which as well allows you to adjust this subset.
 Because of the slightly changed focus, the function there is named differently
 as well: .utils.make_metadata_updater.
 """
 
 # Python compatibility:
-from __future__ import absolute_import
+from __future__ import absolute_import, print_function
 
-# Setup tools:
-import pkg_resources
+from importlib_metadata import PackageNotFoundError, version
 
 try:
-    pkg_resources.get_distribution('collective.metadataversion')
-except pkg_resources.DistributionNotFound:
+    version('collective.metadataversion')
+except PackageNotFoundError:
     HAVE_METADATAVERSION = 0
 else:
     HAVE_METADATAVERSION = 1
 
 # Standard library:
 from traceback import extract_stack
 
@@ -61,14 +60,17 @@
         ]
 
 
 if HAVE_METADATAVERSION:
     # Zope:
     from zope.component import getUtility
 
+    # Plone:
+    from plone.registry.interfaces import IRegistry
+
     # 3rd party:
     from collective.metadataversion.config import DEFAULT_IDXS, FULL_IDXS_KEY
 
     def get_default_idxs():
         """
         We have collective.metadataversion
         """
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_rename.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_rename.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_roles.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_roles.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_switch.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_switch.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_tree.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # visaplan:
 from visaplan.tools.batches import batch_tuples
 from visaplan.tools.classes import StackOfDicts
 from visaplan.tools.minifuncs import gimme_False
 from visaplan.tools.sequences import unique_union
 
 # Local imports:
+from .._idxnames import getExcludeFromNav
 from visaplan.plone.tools._have import HAS_SUBPORTALS, HAS_VPSEARCH
 from visaplan.plone.tools.setup._args import (
     _extract_move_args,
     apply_move_order_options,
     extract_layout_switch,
     normalize_menu_switch,
     setdefault_move_args,
@@ -260,15 +261,15 @@
         logger.info('Will create all specified language variants')
     else:
         logger.info("Won't create any folders")
     portal = opt['portal']
     catalog = getToolByName(portal, 'portal_catalog')
     # ----------------------------- ] ... _clone_tree_inner: options ]
     idxs = [
-        'getExcludeFromNav',
+        getExcludeFromNav,  # changed to 'exclude_from_nav'
         'Language',
         # UNITRACC-spezifisch; visaplan.plone.subportals:
         'get_sub_portal',
         ]
 
     new_folder = make_subfolder_creator(logger=opt['logger'],
                                         parent=portal,
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_types.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_types.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_uid.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_uid.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_watch.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_watch.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_workflow.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/setup/_workflow.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/check-blobs-delete-selected.pt` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/check-blobs-delete-selected.pt`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/check-blobs.pt` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/check-blobs.pt`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/configure.zcml` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/configure.zcml`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/fixblobs.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/views/fixblobs.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at0.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at0.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at1.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at1.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at2.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at2.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at3.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at3.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at4.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at4.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     - ignore_empty (default: True) --
         If a field exists but is empty (or contains a non-string value),
         try the next one;
         with ignore_empty=False,
         any value of the first existing field would be used.
 
-    - decode (default: visaplan.plone.coding.safe_decode) --
+    - decode (default: visaplan.tools.coding.safe_decode) --
         a function to decode a bytes string to unicode.
         Specify a falsy value to suppress decoding.
 
     If the field contains text/plain (i.e., the content doesn't start with
     '<'), it is converted to HTML, using a simple function, which
 
     - creates paragraphs for each line (or sequence of lines), delimited by
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at5.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_dx5.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 # visaplan:
 from visaplan.tools.coding import safe_decode
 from visaplan.tools.html import from_plain_text
 
 # Local imports:
 from ._at3 import getter_name
+from ._at5 import is_nonempty_string
 
 
 def generate_all_texts(context, *fieldnames, **kwargs):
     """
     Generate all (existing) text fields as (fieldname, value) tuples
 
     Keyword options:
@@ -50,32 +51,34 @@
     if 'schema' in kwargs:
         schema = kwargs.pop('schema')
     elif fieldnames and not isinstance(fieldnames[0], six_string_types):
         fieldnames = list(fieldnames)
         schema = fieldnames.pop(0)
     else:
         schema = context.Schema()
+    if schema is not None:
+        raise ValueError('Sorry; using a dedicated schema here (%(schema)r)'
+                         'is not yet supported'
+                         % locals())
 
     if kwargs:
         raise TypeError('Unsupported keyword option(s): %s' % (
                         ', '.join(sorted(set(kwargs))),
                         ))
     if not fieldnames:
         fieldnames = [
                 'title',
                 'subject',
                 'description',
                 'text',
                 ]
     for fieldname in fieldnames:
-        field = schema.get(fieldname)
-        if field:
-            val = field.get(context)
-        else:
-            # e.g. for ATDocument: text not in schema, but getText exists!
+        try:
+            val = getattr(context, fieldname)
+        except AttributeError:
             gname = getter_name(fieldname)
             try:
                 getter = getattr(context, gname)
             except AttributeError:
                 continue
             else:
                 val = getter()
@@ -99,29 +102,14 @@
             continue
         if val.startswith(u'<'):
             soup = BeautifulSoup(val, 'lxml')
             val = soup.text
         yield fieldname, val
 
 
-def is_nonempty_string(val):
-    """
-    >>> is_nonempty_string(u'')
-    False
-    >>> is_nonempty_string(u'123')
-    True
-    >>> is_nonempty_string(123)
-    False
-    """
-    if isinstance(val, six_string_types):
-        return bool(val)
-    else:
-        return False
-
-
 def get_all_texts(context, *fieldnames, **kwargs):
     """
     Get all (existing) texts fields, joined to one unicode string
     """
     res = []
     for fieldname, value in generate_all_texts(context,
                                                *fieldnames, **kwargs):
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_dx4.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_dx4.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_dx5.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/_at5.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- vim: tw=79 cc=+1 sw=4 sts=4 et si
 """
-visaplan.plone.tools: attools: Archetypes-related tools (_at4)
+visaplan.plone.tools: attools: Archetypes-related tools (_at5)
 """
 
 # Python compatibility:
 from __future__ import absolute_import
 
 from six import string_types as six_string_types
 from six import text_type as six_text_type
@@ -13,16 +13,21 @@
 from bs4 import BeautifulSoup
 
 # visaplan:
 from visaplan.tools.coding import safe_decode
 from visaplan.tools.html import from_plain_text
 
 # Local imports:
-from ._at3 import getter_name
-from ._at5 import is_nonempty_string
+from ._at3 import getter_name  # ./_at3.py
+
+__all__ = [
+    'generate_all_texts',  # yield (name, val) tuples
+  # 'is_nonempty_string',  # copied to visaplan.tools v1.3.10+
+    'get_all_texts',
+    ]
 
 
 def generate_all_texts(context, *fieldnames, **kwargs):
     """
     Generate all (existing) text fields as (fieldname, value) tuples
 
     Keyword options:
@@ -31,15 +36,15 @@
         If a field exists but is empty (or contains a non-string value),
         try the next one;
         with ignore_empty=False,
         any value of the first existing field would be used.
 
     - decode (default: visaplan.plone.coding.safe_decode) --
         a function to decode a bytes string to unicode.
-        Specify a falsy value to supporess decoding.
+        Specify a falsy value to suppress decoding.
 
     If the field contains text/html (i.e., the content starts with
     '<'), it is converted to text/plain.
     """
     ignore_empty = kwargs.pop('ignore_empty', 1)
     if 'decode' not in kwargs:
         decode = safe_decode
@@ -51,34 +56,32 @@
     if 'schema' in kwargs:
         schema = kwargs.pop('schema')
     elif fieldnames and not isinstance(fieldnames[0], six_string_types):
         fieldnames = list(fieldnames)
         schema = fieldnames.pop(0)
     else:
         schema = context.Schema()
-    if schema is not None:
-        raise ValueError('Sorry; using a dedicated schema here (%(schema)r)'
-                         'is not yet supported'
-                         % locals())
 
     if kwargs:
         raise TypeError('Unsupported keyword option(s): %s' % (
                         ', '.join(sorted(set(kwargs))),
                         ))
     if not fieldnames:
         fieldnames = [
                 'title',
                 'subject',
                 'description',
                 'text',
                 ]
     for fieldname in fieldnames:
-        try:
-            val = getattr(context, fieldname)
-        except AttributeError:
+        field = schema.get(fieldname)
+        if field:
+            val = field.get(context)
+        else:
+            # e.g. for ATDocument: text not in schema, but getText exists!
             gname = getter_name(fieldname)
             try:
                 getter = getattr(context, gname)
             except AttributeError:
                 continue
             else:
                 val = getter()
@@ -102,14 +105,29 @@
             continue
         if val.startswith(u'<'):
             soup = BeautifulSoup(val, 'lxml')
             val = soup.text
         yield fieldname, val
 
 
+def is_nonempty_string(val):
+    """
+    >>> is_nonempty_string(u'')
+    False
+    >>> is_nonempty_string(u'123')
+    True
+    >>> is_nonempty_string(123)
+    False
+    """
+    if isinstance(val, six_string_types):
+        return bool(val)
+    else:
+        return False
+
+
 def get_all_texts(context, *fieldnames, **kwargs):
     """
     Get all (existing) texts fields, joined to one unicode string
     """
     res = []
     for fieldname, value in generate_all_texts(context,
                                                *fieldnames, **kwargs):
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/brains.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/brains.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/cfg.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 (kopiert nach ../../../parts/instance/etc/zope.conf, führender Leerraum wird
 entfernt)
 
 ACHTUNG - Der Defaultwert für get_debug_active muß ein String sein; z. B.:
 
     from Globals import DevelopmentMode
-    from Products.unitracc.tools.cfg import get_debug_active
+    from visaplan.plone.tools.cfg import get_debug_active
     debug_active = get_debug_active('tree', str(DevelopmentMode))
 
 Siehe auch:
 
 - visaplan.tools.dicts.getOption
 
 sowie die als Factory (zur Konversion der Strings zu den benötigten Datentypen)
@@ -216,17 +216,23 @@
 
     Die Unterstützung des Aufrufs aus Fremdpaketen ist noch etwas umständlich:
     >>> split_filename('/.../src/visaplan.UnitraccShop/src/visaplan/UnitraccShop/__init__.py',
     ...                name='visaplan.UnitraccShop',
     ...                prefix='')
     ('visaplan.UnitraccShop', 'visaplan.UnitraccShop')
 
+    >>> split_filename('/opt/zope/common/eggs/visaplan.plone.tools-1.5.0-py2.7.egg/visaplan/plone/tools/cfg.py')
+    ('visaplan.plone.tools', 'visaplan.plone.tools:cfg')
+
     Der folgende Aufruf zeitigt noch nicht das gewünschte Ergebnis:
-    >-> split_filename('.../src/Products.unitracc/src/Products/unitracc/browser/viewpreview/browser.pyc')
+    >>> split_filename('.../src/Products.unitracc/src/Products/unitracc/browser/viewpreview/browser.pyc')
+    ... # doctest: +SKIP
     ('Products.unitracc', 'Products.unitracc@@viewpreview (DEV)')
+    ... sondern:
+    ('Products.unitracc', 'Products.unitracc:browser.viewpreview.browser (DEV)')
     """
     if name:
         if prefix is None:
             prefix = 'unitracc@@'
         if suffix is None:
             suffix = ''
         return (name,
@@ -266,15 +272,29 @@
         _prefix = _Pn + '@@'
         _name = _dn
         _suffix = ':'+_fn_base
     elif _pn.startswith('adapter'):
         _prefix = _Pn + '->'
         _name = _dn
         _suffix = ':'+_fn_base
+    elif 'Products' in lst2[:-1]:
+        # "historic" components etc. from our monolith:
+        pi = lst2.index('Products')
+        return (_fn_base+'_oder_so',
+                ':'.join(lst2[pi+1:] + [_fn_base]),
+                )
     else:
+        ohwell = '.'.join(lst2) or 'oh well'
+        return (ohwell, ohwell)
+        raw = None
+        pp(_fn_base=_fn_base, _dn=_dn, lst2=lst2, raw=raw)
+        set_trace()
+        res = None
+        return res
+
         try:
             pi = lst2.index('Products')
             return (_fn_base+'_oder_so',
                     ':'.join(lst2[pi+1:] + [_fn_base]),
                     )
         except ValueError as e:
             print(str(e))
@@ -371,15 +391,16 @@
 
     Fallback-Wert für Pfade ohne src- eder egg-Komponente (kein Paket erkannt):
 
     >>> split_srcfilename('/some/strange/unexpected/path.py')
     (None, '.../strange/unexpected/path.py', True)
 
     Der folgende Aufruf zeitigt noch nicht das gewünschte Ergebnis:
-    >-> split_srcfilename('.../src/Products.unitracc/src/Products/unitracc/browser/viewpreview/utils.pyc')
+    >>> split_srcfilename('.../src/Products.unitracc/src/Products/unitracc/browser/viewpreview/utils.pyc')
+    ...   # doctest: +SKIP
     """
     if isinstance(fn, six_string_types):
         fn_list = fn.split(sep)
     else:
         fn_list = list(fn)
     i = 0
     src_positions = []
@@ -415,10 +436,25 @@
             sep.join(['...']
                      +fn_list[-3:]
                      ),
             True)
 
 
 if __name__ == '__main__':
+  if 0:
+      s = '/opt/zope/common/eggs/visaplan.plone.tools-1.5.0-py2.7.egg/visaplan/plone/tools/cfg.py'
+      s = '.../src/Products.unitracc/src/Products/unitracc/browser/viewpreview/browser.pyc'
+      # Logging / Debugging:
+      from pdb import set_trace
+      from visaplan.tools.debug import pp
+      pp(s)
+      set_trace()
+      res = split_srcfilename(s)
+      print(res)
+  else:
     # Standard library:
     import doctest
     doctest.testmod()
+
+# Logging / Debugging:
+from pdb import set_trace
+from visaplan.tools.debug import pp
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/context.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/context.py.orig`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
            'getMessenger',  # accepts a decoder argument
            'getbrain',
            'make_brainGetter',
            'parents',
            'parent_brains',
            'get_parent',
            'getPath',
+           'get_hostname',
            'get_published_templateid',
            ]
 
 
 def getActiveLanguage(context):
     """
     Gib den Code der aktiven Sprache zurück;
@@ -89,15 +90,15 @@
     """
     request = context.REQUEST
     cookies = request.cookies
     if cookies:
         la = cookies.get('I18N_LANGUAGE')
         if la:
             return la
-    la = context.REQUEST.get('LANGUAGE')
+    la = request.get('LANGUAGE')
     if not la:
         pl = getToolByName(context, 'portal_languages')
         la = pl.getDefaultLanguage()
     return la
 
 
 def getSupportedLanguageTuples(context):
@@ -413,23 +414,25 @@
         res = tool(*args, **kwargs)
         print('...' + ci + '.')
         return res
 
     decorated.__doc__ = '%(toolname)s tool (decorated)' % locals()
     return decorated
 
+
 def message(context, message, messageType='info', mapping=None):
     """
     Ersetzt den gleichnamigen Tomcom-Adapter
     """
     pu = getToolByName(context, 'plone_utils')
     pu.addPortalMessage(pmf(safe_decode(message),
                             mapping=mapping),
                         messageType)
 
+
 def getMessenger(context, decode=safe_decode):
     """
     Return a 'message' function which doesn't require
     (nor accept) a context argument
     """
     pu = getToolByName(context, 'plone_utils')
     apm = pu.addPortalMessage
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/forms.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,29 @@
 """\
 Tools für Formulare
 """
 
 # Python compatibility:
 from __future__ import absolute_import, print_function
 
+from importlib_metadata import PackageNotFoundError, version
 from six import string_types as six_string_types
 from six import text_type as six_text_type
 from six.moves.urllib.parse import urlencode, urlsplit, urlunsplit
 
-# Setup tools:
-import pkg_resources
-
 try:
-    pkg_resources.get_distribution('beautifulsoup4')
-except pkg_resources.DistributionNotFound:
+    version('beautifulsoup4')
+except PackageNotFoundError:
     HAS_BEAUTIFULSOUP = False
 else:
     HAS_BEAUTIFULSOUP = True
 
 try:
-    pkg_resources.get_distribution('visaplan.plone.infohubs')
-except pkg_resources.DistributionNotFound:
+    version('visaplan.plone.infohubs')
+except PackageNotFoundError:
     HAS_INFOHUBS = False
 else:
     HAS_INFOHUBS = True
 
 
 if HAS_INFOHUBS:
     # visaplan:
@@ -56,21 +54,21 @@
 except ImportError:
     if __name__ == '__main__':
         print('Some tests will fail due to import problem')
     else:
         raise
     UIDCHARS_UNICODE = frozenset(u'0123456789abcdef')
     def is_uid_shaped(s, onerror='raise'):
-        if isinstance(s, str):
+        if isinstance(s, six_text_type):
+            pass
+        elif isinstance(s, bytes):
             try:
                 s = s.decode('ascii')
             except UnicodeDecodeError:
                 return False
-        elif isinstance(s, six_text_type):
-            pass
         elif onerror == 'raise':
             raise ValueError('String expected: %(s)r'
                              % locals())
         else:
             return False
         return len(s) == 32 and UIDCHARS_UNICODE.issuperset(s)
     def as_new_list(val, splitfunc=None):
@@ -705,14 +703,18 @@
     Das Limit kann explizit angegeben oder auch aufgehoben werden:
     >>> uid_or_number('10001', limit=None)['number']
     10001
 
     Wenn eine Zahl übergeben wurde, gibt es keine solche Beschränkung:
     >>> uid_or_number(10001)['number']
     10001
+
+    We might use this as well to prefix our lesson ids in course xml:
+    >>> sorted(uid_or_number('lesson-5').items())
+    [('number', 5), ('prefix', 'lesson-'), ('uid', None)]
     """
     res = {'uid':    None,
            'number': None,
            'prefix': '',
            }
     if val is None:
         return res
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/indexes.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/indexes.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/log.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
 # Logging / Debugging:
 import logging
 from visaplan.tools.debug import arginfo, pretty_funcname
 
 __all__ = ['getLogSupport',
            'make_textlogger',
+           'locked_open',  # a context manager
            ]
 
 TIMEFORMAT_VERBOSE = u'%Y-%m-%d %T %Z (%A) '
 TIMEFORMAT_LASTCHARS = u' |-\t'
 _DEVMODE_STRING = str(DevelopmentMode)
 
 def getLogSupport(name=None,
@@ -66,15 +67,15 @@
     if 'stack_limit' not in kwargs:
         kwargs['stack_limit'] = 3
     name, label = split_filename(fn, name,  # stack_limit=stack_limit,
                                  **kwargs)
     logger = logging.getLogger(label)
     if default is None:
         default = defaultFromDevMode and _DEVMODE_STRING or 'False'
-    elif not isinstance(default, str):
+    elif not isinstance(default, six_string_types):
         raise ValueError('default must be a string! (%(default)r)'
                          % locals())
     tmp = get_debug_active(name,
                            default)
     if DevelopmentMode:
         debug_active = tmp
     else:
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/mock.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/mock.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/mock_cfg.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/mock_cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 (kopiert nach ../../../parts/instance/etc/zope.conf, führender Leerraum wird
 entfernt)
 
 ACHTUNG - Der Defaultwert für get_debug_active muß ein String sein; z. B.:
 
     from Globals import DevelopmentMode
-    from Products.unitracc.tools.cfg import get_debug_active
+    from visaplan.plone.tools.cfg import get_debug_active
     debug_active = get_debug_active('tree', str(DevelopmentMode))
 
 """
 
 # Python compatibility:
 from __future__ import absolute_import
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/profiles.zcml` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/profiles.zcml`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/search.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 
 def make_querystring_normalizer(decode=safe_decode):
     r"""
     Factory to create a `normalizeQueryString` function,
     injecting the default decoding function;
     by default, the safe_decode function from visaplan.tools is used,
-    which (or course) recognizes unicode strings and decodes UTF8 and Latin-1.
+    which (of course) recognizes unicode strings and decodes UTF8 and Latin-1.
 
     You may want to replace this `decode` argument by your own function,
     e.g. to
 
     - raise an exception if a non-unicode string is given,
       or
     - log calls which use non-unicode strings (to help during development)
@@ -364,21 +364,10 @@
                              for tup in language_tool.listSupportedLanguages()
                              ]
         values.update(all_languages)
     return sorted(values)
 
 
 if __name__ == "__main__":
-  if 0:
-      # Standard library:
-      from pprint import pprint
-
-      # Logging / Debugging:
-      from pdb import set_trace
-      set_trace()
-      mqs = make_querystring_mangle(None, mangle_umlauts)
-      lst = mqs(u'entkoppelte Förderschnecke ')
-      pprint(lst)
-  else:
     # Standard library:
     import doctest
     doctest.testmod()
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/zcmlgen.py` & `visaplan.plone.tools-1.5.2/src/visaplan/plone/tools/zcmlgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,16 +208,15 @@
         # are common to both
         if [difference
             for difference in difflines
             if not difference.startswith('  ')  # unchanged lines
             and difference not in ('+ ', '- ')  # empty lines added/removed
             ]:
             print('\n'.join(difflines))
-            if sys.stdout.isatty():
-                set_trace()
+            if sys.stdout.isatty(): set_trace()
             return False
         return True
 
 
 class ResourceGenerator(BasicGenerator):
     """
     implementiert die fehlenden Methoden der BasicGenerator-Klasse
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/PKG-INFO` & `visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visaplan.plone.tools
-Version: 1.4.9
+Version: 1.5.2
 Summary: General tools for Plone sites
 Home-page: UNKNOWN
 Author: Tobias Herp
 Author-email: tobias.herp@visaplan.com
 License: GPL version 2
 Project-URL: Source, https://github.com/visaplan/plone.tools
 Project-URL: Documentation, https://pypi.org/project/visaplan.plone.tools
@@ -117,14 +117,20 @@
           - ``@returns_json``:
         
             Wraps the function call and returns the JSON_-encoded result,
             including HTTP headers.
         
             Uses simplejson_ if available.
         
+            **NOT** to be used for functions which simply provide JSON_ data for
+            insertion in page templates!
+        
+            Otherwise, the browser might try to parse your HTML page as JSON
+            and fail.
+        
         Documentation
         -------------
         
         Sorry, we don't have real user documentation yet.
         
         Most functions are documented by doctests, anyway;
         it helps to understand some German.
@@ -190,17 +196,250 @@
         
         Contributors
         ============
         
         - Tobias Herp, tobias.herp@visaplan.com
         
         
+        .. vim: sw=2 sts=2 tw=79 cc=+1
+        
         Changelog
         =========
         
+        1.6.0 (estimated)
+        -----------------
+        
+        - Removal of all profile and zcml code
+        
+        
+        1.5.2 (2024-03-21)
+        ------------------
+        
+        New Features:
+        
+        - .decorators: new decorator ``headless_json``
+        
+        - .setup: new decorator ``importStep()``; usage::
+          
+            @importStep('profiles/default/my.checked-marker.txt')
+            def setup_various(context):
+                # jump right in!
+        
+        Profile changes:
+        
+        - We try pretty hard to prevent people from activating this package!
+          *NOTE:* Removal of any profile and ZCML code is scheduled for release 1.6.
+        
+        [tobiasherp]
+        
+        
+        1.5.1 (2023-12-21)
+        ------------------
+        
+        Bugfixes:
+        
+        - For some unexpected filenames, .cfg.split_filename didn't return a 2-tuple of strings
+          (but a single string instead) which caused potentially show-stopping ValueErrors.
+        
+        [tobiasherp]
+        
+        
+        1.5.0 (2023-11-28)
+        ------------------
+        
+        Miscellaneous:
+        
+        - Code maintenance only
+        
+        [tobiasherp]
+        
+        
+        1.4.19 (2023-05-31)
+        -------------------
+        
+        New Features:
+        
+        - New module `.lock`:
+        
+          - `ConvenientLock` context manager, wrapping zc.lockfile.LockFile
+          - `lockfile_kwargs()` function, taking the zc.lockfile_ version into account:
+        
+        - In the `.env` module, querying the environment:
+        
+          - `var_directory()` function, using ``VAR_ROOT`` and ``CLIENT_HOME``
+          - `lockfiles_directory()` function,
+            using ``LOCKFILES_DIR`` and the `var_directory()` function
+        
+        Requirements:
+        
+        - The `.lock` module is built on top of the zc.lockfile_ package.
+          To make use of it, you may
+        
+          - install zc.lockfile_ yourself
+            (release 1.2.0+ is supported *(1.2.1+ recommended)* but not required),
+            or
+          - use the ``lock`` extra.
+        
+          *Note:* Configure and create a ``LOCKFILES_DIR``,
+          or create a ``lock`` subdir in your instance's ``var`` directory!
+        
+        [tobiasherp]
+        
+        
+        1.4.18.1 (2023-05-03)
+        ---------------------
+        
+        Bugfixes:
+        
+        - When checking the version of the visaplan.plone.search package,
+          compare correctly, following `PEP 440`_.
+        
+        Requirements:
+        
+        - packaging_
+        
+        [tobiasherp]
+        
+        
+        1.4.18 (2023-05-02)
+        -------------------
+        
+        Improvements:
+        
+        - As we use the traditional index `getExcludeFromNav`, we import the
+          name of that index from visaplan.plone.search now, if available;
+        - The default is still ``getExcludeFromNav``.
+        
+        Requirements:
+        
+        - importlib_metadata_
+        - If we have visaplan.plone.search, we need 1.7+
+        
+        Hints:
+        
+        - The default value for the `getExcludeFromNav` index name
+          will change in a future release.
+        
+        [tobiasherp]
+        
+        
+        1.4.17 (2023-04-05)
+        -------------------
+        
+        New features: 
+        
+        - function .attools.can_be_html(field)
+        
+        [tobiasherp]
+        
+        
+        1.4.16 (2023-03-24)
+        -------------------
+        
+        New features: 
+        
+        - New function `short_hostname` in .functions
+        
+        [tobiasherp]
+        
+        
+        1.4.15 (2023-03-08)
+        -------------------
+        
+        Bugfixes:
+        
+        - Py3K support fixes for
+        
+          - .functions.is_uid_shaped
+          - .log.getLogSupport
+        
+        New features: 
+        
+        - New (still tiny) module .seo for SEO support;
+          for now, focused on structured data.
+          Functions:
+        
+          - `parse_title`, returning a dict
+        
+        [tobiasherp]
+        
+        
+        1.4.14 (2022-04-22)
+        -------------------
+        
+        Bugfixes:
+        
+        - Missing imports fixed for
+        
+          - .groups.is_member_of__factory
+          - .setup.get_default_idxs
+        
+        [tobiasherp]
+        
+        
+        1.4.13 (2022-03-04)
+        -------------------
+        
+        Bugfixes:
+        
+        - Fixed a bug in .groups.groupinfo_factory(pretty);
+          for this to work, we need visaplan.plone.groups.
+        
+        Improvements:
+        
+        - The label of the default logger of the ``@@step`` decorator
+          now includes the name of the worker, e.g. ``instance`` or ``client``
+        
+        New features: 
+        
+        - New `.env` module, providing the `worker_name()`
+        
+        [tobiasherp]
+        
+        
+        1.4.12 (2022-02-15)
+        -------------------
+        
+        Bugfixes:
+        
+        - Fixed a bug in .groups.groupinfo_factory(pretty);
+          for this to work, we need visaplan.plone.groups.
+        
+        [tobiasherp]
+        
+        
+        1.4.11 (2022-02-05)
+        -------------------
+        
+        Bugfixes:
+        
+        - Fixed a regression for .groups.groupinfo_factory
+        
+        [tobiasherp]
+        
+        
+        1.4.10 (2022-02-03)
+        -------------------
+        
+        Improvements:
+        
+        - Converted the .groups module in a subpackage
+        
+        New features: 
+        
+        - New option `missing=False` for
+        
+          - .groups.groupinfo_factory
+        
+          If `True`, the resulting function creates an `existing` key,
+          and for missing groups, the `group_title` is `None`;
+          otherwise, an empty dict is returned in such cases.
+        
+        [tobiasherp]
+        
         
         1.4.9 (2021-12-13)
         ------------------
         
         Improvements:
         
         - If collective.metadataversion_ is installed, use the configured default set of
@@ -276,30 +515,31 @@
         
           We keep the the ``uninstall`` profile *for now;*
           it will be removed in an near-future version.
         
           So, *don't "install"* this package (Quick-Installer, Plone add-ons);
           just use it in Python_ code!
         
-          We keep the ``configure.zcml`` file and the autoinclude entry point, though;
-          we can image to use e.g. the Plone registry for some settings.
+          We keep the ``configure.zcml`` file and the autoinclude entry point
+          for now, though;
+          we can imagine to use e.g. the Plone registry for some settings.
         
         [tobiasherp]
         
         
         1.4.4 (2021-08-31)
         ------------------
         
         Bugfixes:
         
-        - .setup.make_object_getter() didn't update the Language index when the language was changed
+        - `.setup.make_object_getter()` didn't update the Language index when the language was changed
         
         Improvements:
         
-        - .setup.make_object_getter() now additionally updates the following indexes
+        - `.setup.make_object_getter()` now additionally updates the following indexes
           when the .title attribute is changed:
         
           - sortable_title
           - SearchableText
           - getEffectiveIndex
         
         [tobiasherp]
@@ -675,28 +915,34 @@
         
         - Initial release.
           [tobiasherp]
         
         .. _BeautifulSoup: https://pypi.org/project/beautifulsoup4/
         .. _collective.metadataversion: https://pypi.org/project/collective.metadataversion
         .. _five.grok: https://pypi.org/project/five.grok
+        .. _importlib_metadata: https://pypi.org/project/importlib-metadata/
         .. _`metadata_version`: https://community.plone.org/t/metadata-column-metadata-version-for-conditional-metadata-refresh/14194/3
+        .. _packaging: https://pypi.org/project/packaging/
+        .. _`PEP 440`: https://peps.python.org/pep-0440/
         .. _Products.Archetypes: https://pypi.org/project/Products.Archetypes
         .. _Python: https://www.python.org
         .. _simplejson: https://pypi.org/project/simplejson
         .. _visaplan.kitchen: https://pypi.org/project/visaplan.kitchen
         .. _visaplan.plone.infohubs: https://pypi.org/project/visaplan.plone.infohubs
         .. _visaplan.tools: https://pypi.org/project/visaplan.tools
+        .. _zc.lockfile: https://pypi.org/project/zc.lockfile
         
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 4.3
 Classifier: Framework :: Zope2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: German
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Description-Content-Type: text/x-rst
 Provides-Extra: test
+Provides-Extra: lock
```

### Comparing `visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/SOURCES.txt` & `visaplan.plone.tools-1.5.2/src/visaplan.plone.tools.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 MANIFEST.in
 README.rst
 TODO.rst
 VERSION
 long-description.rst
 setup.cfg
 setup.py
-test.rst
 docs/LICENSE.GPL
 docs/LICENSE.rst
 docs/Makefile
 docs/conf.py
 docs/conf.rst
 docs/index.rst
 docs/make.bat
@@ -34,36 +33,53 @@
 src/visaplan/plone/tools/__init__.py
 src/visaplan/plone/tools/_at0.py
 src/visaplan/plone/tools/_at1.py
 src/visaplan/plone/tools/_at2.py
 src/visaplan/plone/tools/_at3.py
 src/visaplan/plone/tools/_at4.py
 src/visaplan/plone/tools/_at5.py
+src/visaplan/plone/tools/_at6.py
 src/visaplan/plone/tools/_dx4.py
 src/visaplan/plone/tools/_dx5.py
 src/visaplan/plone/tools/_have.py
+src/visaplan/plone/tools/_idxnames.py
 src/visaplan/plone/tools/attools.py
 src/visaplan/plone/tools/brains.py
 src/visaplan/plone/tools/cfg.py
 src/visaplan/plone/tools/configure.zcml
 src/visaplan/plone/tools/context.py
+src/visaplan/plone/tools/context.py.orig
 src/visaplan/plone/tools/decorators.py
 src/visaplan/plone/tools/dxtools.py
+src/visaplan/plone/tools/env.py
 src/visaplan/plone/tools/forms.py
 src/visaplan/plone/tools/functions.py
-src/visaplan/plone/tools/groups.py
 src/visaplan/plone/tools/indexes.py
+src/visaplan/plone/tools/lock.py
 src/visaplan/plone/tools/log.py
 src/visaplan/plone/tools/mock.py
 src/visaplan/plone/tools/mock_cfg.py
 src/visaplan/plone/tools/profiles.zcml
 src/visaplan/plone/tools/search.py
+src/visaplan/plone/tools/seo.py
 src/visaplan/plone/tools/setuphandlers.py
+src/visaplan/plone/tools/strings.py
 src/visaplan/plone/tools/zcmlgen.py
-src/visaplan/plone/tools/Extensions/install.py
+src/visaplan/plone/tools/groups/__init__.py
+src/visaplan/plone/tools/groups/_data.py
+src/visaplan/plone/tools/groups/_group.py
+src/visaplan/plone/tools/groups/_group_pio.py
+src/visaplan/plone/tools/groups/_helpers.py
+src/visaplan/plone/tools/groups/_imports.py
+src/visaplan/plone/tools/groups/_membership.py
+src/visaplan/plone/tools/groups/_user.py
+src/visaplan/plone/tools/groups/_user_pio.py
+src/visaplan/plone/tools/infofact/_group.py
+src/visaplan/plone/tools/infofact/_membership.py
+src/visaplan/plone/tools/infofact/_user.py
 src/visaplan/plone/tools/setup/__init__.py
 src/visaplan/plone/tools/setup/_args.py
 src/visaplan/plone/tools/setup/_attr.py
 src/visaplan/plone/tools/setup/_decorator.py
 src/visaplan/plone/tools/setup/_exc.py
 src/visaplan/plone/tools/setup/_get_object.py
 src/visaplan/plone/tools/setup/_gs.py
```

### Comparing `visaplan.plone.tools-1.4.9/CHANGES.rst` & `visaplan.plone.tools-1.5.2/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,243 @@
+.. vim: sw=2 sts=2 tw=79 cc=+1
+
 Changelog
 =========
 
+1.6.0 (estimated)
+-----------------
+
+- Removal of all profile and zcml code
+
+
+1.5.2 (2024-03-21)
+------------------
+
+New Features:
+
+- .decorators: new decorator ``headless_json``
+
+- .setup: new decorator ``importStep()``; usage::
+  
+    @importStep('profiles/default/my.checked-marker.txt')
+    def setup_various(context):
+        # jump right in!
+
+Profile changes:
+
+- We try pretty hard to prevent people from activating this package!
+  *NOTE:* Removal of any profile and ZCML code is scheduled for release 1.6.
+
+[tobiasherp]
+
+
+1.5.1 (2023-12-21)
+------------------
+
+Bugfixes:
+
+- For some unexpected filenames, .cfg.split_filename didn't return a 2-tuple of strings
+  (but a single string instead) which caused potentially show-stopping ValueErrors.
+
+[tobiasherp]
+
+
+1.5.0 (2023-11-28)
+------------------
+
+Miscellaneous:
+
+- Code maintenance only
+
+[tobiasherp]
+
+
+1.4.19 (2023-05-31)
+-------------------
+
+New Features:
+
+- New module `.lock`:
+
+  - `ConvenientLock` context manager, wrapping zc.lockfile.LockFile
+  - `lockfile_kwargs()` function, taking the zc.lockfile_ version into account:
+
+- In the `.env` module, querying the environment:
+
+  - `var_directory()` function, using ``VAR_ROOT`` and ``CLIENT_HOME``
+  - `lockfiles_directory()` function,
+    using ``LOCKFILES_DIR`` and the `var_directory()` function
+
+Requirements:
+
+- The `.lock` module is built on top of the zc.lockfile_ package.
+  To make use of it, you may
+
+  - install zc.lockfile_ yourself
+    (release 1.2.0+ is supported *(1.2.1+ recommended)* but not required),
+    or
+  - use the ``lock`` extra.
+
+  *Note:* Configure and create a ``LOCKFILES_DIR``,
+  or create a ``lock`` subdir in your instance's ``var`` directory!
+
+[tobiasherp]
+
+
+1.4.18.1 (2023-05-03)
+---------------------
+
+Bugfixes:
+
+- When checking the version of the visaplan.plone.search package,
+  compare correctly, following `PEP 440`_.
+
+Requirements:
+
+- packaging_
+
+[tobiasherp]
+
+
+1.4.18 (2023-05-02)
+-------------------
+
+Improvements:
+
+- As we use the traditional index `getExcludeFromNav`, we import the
+  name of that index from visaplan.plone.search now, if available;
+- The default is still ``getExcludeFromNav``.
+
+Requirements:
+
+- importlib_metadata_
+- If we have visaplan.plone.search, we need 1.7+
+
+Hints:
+
+- The default value for the `getExcludeFromNav` index name
+  will change in a future release.
+
+[tobiasherp]
+
+
+1.4.17 (2023-04-05)
+-------------------
+
+New features: 
+
+- function .attools.can_be_html(field)
+
+[tobiasherp]
+
+
+1.4.16 (2023-03-24)
+-------------------
+
+New features: 
+
+- New function `short_hostname` in .functions
+
+[tobiasherp]
+
+
+1.4.15 (2023-03-08)
+-------------------
+
+Bugfixes:
+
+- Py3K support fixes for
+
+  - .functions.is_uid_shaped
+  - .log.getLogSupport
+
+New features: 
+
+- New (still tiny) module .seo for SEO support;
+  for now, focused on structured data.
+  Functions:
+
+  - `parse_title`, returning a dict
+
+[tobiasherp]
+
+
+1.4.14 (2022-04-22)
+-------------------
+
+Bugfixes:
+
+- Missing imports fixed for
+
+  - .groups.is_member_of__factory
+  - .setup.get_default_idxs
+
+[tobiasherp]
+
+
+1.4.13 (2022-03-04)
+-------------------
+
+Bugfixes:
+
+- Fixed a bug in .groups.groupinfo_factory(pretty);
+  for this to work, we need visaplan.plone.groups.
+
+Improvements:
+
+- The label of the default logger of the ``@@step`` decorator
+  now includes the name of the worker, e.g. ``instance`` or ``client``
+
+New features: 
+
+- New `.env` module, providing the `worker_name()`
+
+[tobiasherp]
+
+
+1.4.12 (2022-02-15)
+-------------------
+
+Bugfixes:
+
+- Fixed a bug in .groups.groupinfo_factory(pretty);
+  for this to work, we need visaplan.plone.groups.
+
+[tobiasherp]
+
+
+1.4.11 (2022-02-05)
+-------------------
+
+Bugfixes:
+
+- Fixed a regression for .groups.groupinfo_factory
+
+[tobiasherp]
+
+
+1.4.10 (2022-02-03)
+-------------------
+
+Improvements:
+
+- Converted the .groups module in a subpackage
+
+New features: 
+
+- New option `missing=False` for
+
+  - .groups.groupinfo_factory
+
+  If `True`, the resulting function creates an `existing` key,
+  and for missing groups, the `group_title` is `None`;
+  otherwise, an empty dict is returned in such cases.
+
+[tobiasherp]
+
 
 1.4.9 (2021-12-13)
 ------------------
 
 Improvements:
 
 - If collective.metadataversion_ is installed, use the configured default set of
@@ -80,30 +313,31 @@
 
   We keep the the ``uninstall`` profile *for now;*
   it will be removed in an near-future version.
 
   So, *don't "install"* this package (Quick-Installer, Plone add-ons);
   just use it in Python_ code!
 
-  We keep the ``configure.zcml`` file and the autoinclude entry point, though;
-  we can image to use e.g. the Plone registry for some settings.
+  We keep the ``configure.zcml`` file and the autoinclude entry point
+  for now, though;
+  we can imagine to use e.g. the Plone registry for some settings.
 
 [tobiasherp]
 
 
 1.4.4 (2021-08-31)
 ------------------
 
 Bugfixes:
 
-- .setup.make_object_getter() didn't update the Language index when the language was changed
+- `.setup.make_object_getter()` didn't update the Language index when the language was changed
 
 Improvements:
 
-- .setup.make_object_getter() now additionally updates the following indexes
+- `.setup.make_object_getter()` now additionally updates the following indexes
   when the .title attribute is changed:
 
   - sortable_title
   - SearchableText
   - getEffectiveIndex
 
 [tobiasherp]
@@ -479,14 +713,18 @@
 
 - Initial release.
   [tobiasherp]
 
 .. _BeautifulSoup: https://pypi.org/project/beautifulsoup4/
 .. _collective.metadataversion: https://pypi.org/project/collective.metadataversion
 .. _five.grok: https://pypi.org/project/five.grok
+.. _importlib_metadata: https://pypi.org/project/importlib-metadata/
 .. _`metadata_version`: https://community.plone.org/t/metadata-column-metadata-version-for-conditional-metadata-refresh/14194/3
+.. _packaging: https://pypi.org/project/packaging/
+.. _`PEP 440`: https://peps.python.org/pep-0440/
 .. _Products.Archetypes: https://pypi.org/project/Products.Archetypes
 .. _Python: https://www.python.org
 .. _simplejson: https://pypi.org/project/simplejson
 .. _visaplan.kitchen: https://pypi.org/project/visaplan.kitchen
 .. _visaplan.plone.infohubs: https://pypi.org/project/visaplan.plone.infohubs
 .. _visaplan.tools: https://pypi.org/project/visaplan.tools
+.. _zc.lockfile: https://pypi.org/project/zc.lockfile
```

### Comparing `visaplan.plone.tools-1.4.9/README.rst` & `visaplan.plone.tools-1.5.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -106,14 +106,20 @@
   - ``@returns_json``:
 
     Wraps the function call and returns the JSON_-encoded result,
     including HTTP headers.
 
     Uses simplejson_ if available.
 
+    **NOT** to be used for functions which simply provide JSON_ data for
+    insertion in page templates!
+
+    Otherwise, the browser might try to parse your HTML page as JSON
+    and fail.
+
 Documentation
 -------------
 
 Sorry, we don't have real user documentation yet.
 
 Most functions are documented by doctests, anyway;
 it helps to understand some German.
```

### Comparing `visaplan.plone.tools-1.4.9/long-description.rst` & `visaplan.plone.tools-1.5.2/long-description.rst`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.9/setup.cfg` & `visaplan.plone.tools-1.5.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [nosetests]
 with-doctest = 1
 
 [isort]
 line_length = 79
-known_compatibility = six,future
+known_compatibility = six,future,importlib_metadata,importlib_resources
 import_heading_future = Python compatibility:
 import_heading_compatibility = Python compatibility:
 known_devel = logging,pdb,visaplan.plone.tools.log,visaplan.tools.debug
 import_heading_devel = Logging / Debugging:
 known_visaplan = Products.unitracc,visaplan
 import_heading_visaplan = visaplan:
-known_zope = AccessControl,Acquisition,App,archetypes,DateTime,five,Globals,OFS,Products,transaction,z3c,zExceptions,ZODB,zope,Zope,ZPublisher,ZServer,ZTUtils,Missing
+known_zope = AccessControl,Acquisition,App,archetypes,BTrees,DateTime,five,Globals,OFS,Products,transaction,z3c,zc,zExceptions,ZODB,zope,Zope,ZPublisher,ZServer,ZTUtils,Missing
 import_heading_zope = Zope:
-known_setup = distutils,pkg_resources,setuptools
+known_setup = distutils,pkg_resources,setuptools,packaging
 known_stdlibold = ConfigParser,cStringIO,StringIO,thread,urlparse
 import_heading_setup = Setup tools:
 known_plone = plone,Products.CMFPlone
 import_heading_plone = Plone:
 import_heading_stdlib = Standard library:
 import_heading_stdlibold = Standard library (Python 2):
 import_heading_thirdparty = 3rd party:
 import_heading_localfolder = Local imports:
-sections = FUTURE,COMPATIBILITY,SETUP,STDLIB,STDLIBOLD,ZOPE,PLONE,THIRDPARTY,VISAPLAN,FIRSTPARTY,LOCALFOLDER,DEVEL
+known_pdfreactor = pdfreactor
+import_heading_pdfreactor = PDFreactor (by RealObjects; Plone integration by visaplan GmbH):
+sections = FUTURE,COMPATIBILITY,SETUP,STDLIB,STDLIBOLD,ZOPE,PLONE,THIRDPARTY,PDFREACTOR,VISAPLAN,FIRSTPARTY,LOCALFOLDER,DEVEL
 dedup_headings = True
 multi_line_output = 8
 include_trailing_comma = True
 
 [check-manifest]
 ignore = 
 	*.cfg
```

### Comparing `visaplan.plone.tools-1.4.9/setup.py` & `visaplan.plone.tools-1.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 from __future__ import absolute_import, print_function
 
 # Setup tools:
 from setuptools import find_packages, setup
 
 # Standard library:
 from os.path import isfile
+from sys import version_info, argv
 
 package_name = 'visaplan.plone.tools'
+installing = set(argv[1:]).intersection(['install', 'd''evelop'])
 
 # -------------------------------------------- [ get the version ... [
 def read_version(fn, sfn):
     main = open(fn).read().strip()
     if sfn is not None and isfile(sfn):
         suffix = valid_suffix(open(sfn).read().strip())
     else:
@@ -23,15 +25,15 @@
 def valid_suffix(suffix):
     """
     Enforce our suffix convention
     """
     suffix = suffix.strip()
     if not suffix:
         return suffix
-    allowed = set('dev.0123456789rcpost')
+    allowed = set('edv.0123456789rcpost')
     disallowed = set(suffix).difference(allowed)
     if disallowed:
         disallowed = ''.join(sorted(disallowed))
         raise ValueError('Version suffix contains disallowed characters'
                          ' (%(disallowed)s)'
                          % locals())
     chunks = suffix.split('.')
@@ -54,14 +56,15 @@
             raise ValueError('Chunk %(chunk)r of version suffix %(suffix)r'
                              ' starts with a digit'
                              % locals())
         char = chunk[-1]
         if char not in '0123456789':
             raise ValueError('Chunk %(chunk)r of version suffix %(suffix)r'
                              ' doesn\'t end with a digit'
+                             ' (normalization would append a "0")'
                              % locals())
     return suffix  # ... valid_suffix
     # ... get the version ...
     # ... get the version ...
 VERSION = read_version('VERSION',
                        'VERSION_SUFFIX')
 # -------------------------------------------- ] ... get the version ]
@@ -111,20 +114,25 @@
     if pop_user:
         assert 'pick_user' not in kwargs
         assert 'user' not in kwargs
         user = pkg_list.pop(0)
         package = '.'.join(pkg_list)
     else:
         pick_user = pop('pick_user', 'user' not in kwargs)
+        given_user = pop('user', None)
         if pick_user:
             user = pkg_list[0]
-            if 'user' in kwargs:
-                assert pop('user') == user
+            if given_user is not None and given_user != user:
+                raise ValueError('given user %(given_user)r mismatches '
+                                 'user picked from package %(user)r!'
+                                 % locals())
+        elif given_user is not None:
+            user = given_user
         else:
-            user = pop('user')
+            raise ValueError('no user given nor picked!')
     if pop('travis', False):  # reqires github to be trueish
         res.update({  # CHECKME: is there a de-facto standard key for this?
             'Tests': 'https://travis-ci.org/%(user)s/%(package)s' % locals()
             })
     base = 'https://github.com/%(user)s/%(package)s' % locals()
     res.update({
         'Source': base,
@@ -145,14 +153,15 @@
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
         'Framework :: Zope2',
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "Natural Language :: German",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     # keywords='Python Plone',
     author='Tobias Herp',
@@ -165,26 +174,32 @@
         'visaplan.plone',
         ],
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'setuptools',
+        'importlib_metadata',
+        'packaging' if version_info.major >= 3 or not installing
+        else 'packaging <21.0',
         'six',
         'Products.CMFCore', # getToolByName
         # -*- Extra requirements: -*-
         'visaplan.tools >=1.3.1',  # list_of_strings improved
-        # 'visaplan.plone.infohubs >=1.1.1.dev1',  # .hubs2 module
+        # 'visaplan.plone.infohubs >=1.1.1', ".hubs2 module" (prob. earlier)
         # ... further requirements removed
     ],
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     """,
     extras_require={
+        'lock': [
+            'zc.locking',  # required by the .lock module
+            ],
         'test': [
             'nose2',
             #'plone.app.testing',
             # plone.app.robotframework 1.2.0 requires plone.testing 4.0.11; 
             # plone.app.robotframework 1.3+ drops Plone 4.3 compatibility:
             #'plone.testing',
             #'plone.app.robotframework[debug]',
```

### Comparing `visaplan.plone.tools-1.4.9/PKG-INFO` & `visaplan.plone.tools-1.5.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visaplan.plone.tools
-Version: 1.4.9
+Version: 1.5.2
 Summary: General tools for Plone sites
 Home-page: UNKNOWN
 Author: Tobias Herp
 Author-email: tobias.herp@visaplan.com
 License: GPL version 2
 Project-URL: Source, https://github.com/visaplan/plone.tools
 Project-URL: Documentation, https://pypi.org/project/visaplan.plone.tools
@@ -117,14 +117,20 @@
           - ``@returns_json``:
         
             Wraps the function call and returns the JSON_-encoded result,
             including HTTP headers.
         
             Uses simplejson_ if available.
         
+            **NOT** to be used for functions which simply provide JSON_ data for
+            insertion in page templates!
+        
+            Otherwise, the browser might try to parse your HTML page as JSON
+            and fail.
+        
         Documentation
         -------------
         
         Sorry, we don't have real user documentation yet.
         
         Most functions are documented by doctests, anyway;
         it helps to understand some German.
@@ -190,17 +196,250 @@
         
         Contributors
         ============
         
         - Tobias Herp, tobias.herp@visaplan.com
         
         
+        .. vim: sw=2 sts=2 tw=79 cc=+1
+        
         Changelog
         =========
         
+        1.6.0 (estimated)
+        -----------------
+        
+        - Removal of all profile and zcml code
+        
+        
+        1.5.2 (2024-03-21)
+        ------------------
+        
+        New Features:
+        
+        - .decorators: new decorator ``headless_json``
+        
+        - .setup: new decorator ``importStep()``; usage::
+          
+            @importStep('profiles/default/my.checked-marker.txt')
+            def setup_various(context):
+                # jump right in!
+        
+        Profile changes:
+        
+        - We try pretty hard to prevent people from activating this package!
+          *NOTE:* Removal of any profile and ZCML code is scheduled for release 1.6.
+        
+        [tobiasherp]
+        
+        
+        1.5.1 (2023-12-21)
+        ------------------
+        
+        Bugfixes:
+        
+        - For some unexpected filenames, .cfg.split_filename didn't return a 2-tuple of strings
+          (but a single string instead) which caused potentially show-stopping ValueErrors.
+        
+        [tobiasherp]
+        
+        
+        1.5.0 (2023-11-28)
+        ------------------
+        
+        Miscellaneous:
+        
+        - Code maintenance only
+        
+        [tobiasherp]
+        
+        
+        1.4.19 (2023-05-31)
+        -------------------
+        
+        New Features:
+        
+        - New module `.lock`:
+        
+          - `ConvenientLock` context manager, wrapping zc.lockfile.LockFile
+          - `lockfile_kwargs()` function, taking the zc.lockfile_ version into account:
+        
+        - In the `.env` module, querying the environment:
+        
+          - `var_directory()` function, using ``VAR_ROOT`` and ``CLIENT_HOME``
+          - `lockfiles_directory()` function,
+            using ``LOCKFILES_DIR`` and the `var_directory()` function
+        
+        Requirements:
+        
+        - The `.lock` module is built on top of the zc.lockfile_ package.
+          To make use of it, you may
+        
+          - install zc.lockfile_ yourself
+            (release 1.2.0+ is supported *(1.2.1+ recommended)* but not required),
+            or
+          - use the ``lock`` extra.
+        
+          *Note:* Configure and create a ``LOCKFILES_DIR``,
+          or create a ``lock`` subdir in your instance's ``var`` directory!
+        
+        [tobiasherp]
+        
+        
+        1.4.18.1 (2023-05-03)
+        ---------------------
+        
+        Bugfixes:
+        
+        - When checking the version of the visaplan.plone.search package,
+          compare correctly, following `PEP 440`_.
+        
+        Requirements:
+        
+        - packaging_
+        
+        [tobiasherp]
+        
+        
+        1.4.18 (2023-05-02)
+        -------------------
+        
+        Improvements:
+        
+        - As we use the traditional index `getExcludeFromNav`, we import the
+          name of that index from visaplan.plone.search now, if available;
+        - The default is still ``getExcludeFromNav``.
+        
+        Requirements:
+        
+        - importlib_metadata_
+        - If we have visaplan.plone.search, we need 1.7+
+        
+        Hints:
+        
+        - The default value for the `getExcludeFromNav` index name
+          will change in a future release.
+        
+        [tobiasherp]
+        
+        
+        1.4.17 (2023-04-05)
+        -------------------
+        
+        New features: 
+        
+        - function .attools.can_be_html(field)
+        
+        [tobiasherp]
+        
+        
+        1.4.16 (2023-03-24)
+        -------------------
+        
+        New features: 
+        
+        - New function `short_hostname` in .functions
+        
+        [tobiasherp]
+        
+        
+        1.4.15 (2023-03-08)
+        -------------------
+        
+        Bugfixes:
+        
+        - Py3K support fixes for
+        
+          - .functions.is_uid_shaped
+          - .log.getLogSupport
+        
+        New features: 
+        
+        - New (still tiny) module .seo for SEO support;
+          for now, focused on structured data.
+          Functions:
+        
+          - `parse_title`, returning a dict
+        
+        [tobiasherp]
+        
+        
+        1.4.14 (2022-04-22)
+        -------------------
+        
+        Bugfixes:
+        
+        - Missing imports fixed for
+        
+          - .groups.is_member_of__factory
+          - .setup.get_default_idxs
+        
+        [tobiasherp]
+        
+        
+        1.4.13 (2022-03-04)
+        -------------------
+        
+        Bugfixes:
+        
+        - Fixed a bug in .groups.groupinfo_factory(pretty);
+          for this to work, we need visaplan.plone.groups.
+        
+        Improvements:
+        
+        - The label of the default logger of the ``@@step`` decorator
+          now includes the name of the worker, e.g. ``instance`` or ``client``
+        
+        New features: 
+        
+        - New `.env` module, providing the `worker_name()`
+        
+        [tobiasherp]
+        
+        
+        1.4.12 (2022-02-15)
+        -------------------
+        
+        Bugfixes:
+        
+        - Fixed a bug in .groups.groupinfo_factory(pretty);
+          for this to work, we need visaplan.plone.groups.
+        
+        [tobiasherp]
+        
+        
+        1.4.11 (2022-02-05)
+        -------------------
+        
+        Bugfixes:
+        
+        - Fixed a regression for .groups.groupinfo_factory
+        
+        [tobiasherp]
+        
+        
+        1.4.10 (2022-02-03)
+        -------------------
+        
+        Improvements:
+        
+        - Converted the .groups module in a subpackage
+        
+        New features: 
+        
+        - New option `missing=False` for
+        
+          - .groups.groupinfo_factory
+        
+          If `True`, the resulting function creates an `existing` key,
+          and for missing groups, the `group_title` is `None`;
+          otherwise, an empty dict is returned in such cases.
+        
+        [tobiasherp]
+        
         
         1.4.9 (2021-12-13)
         ------------------
         
         Improvements:
         
         - If collective.metadataversion_ is installed, use the configured default set of
@@ -276,30 +515,31 @@
         
           We keep the the ``uninstall`` profile *for now;*
           it will be removed in an near-future version.
         
           So, *don't "install"* this package (Quick-Installer, Plone add-ons);
           just use it in Python_ code!
         
-          We keep the ``configure.zcml`` file and the autoinclude entry point, though;
-          we can image to use e.g. the Plone registry for some settings.
+          We keep the ``configure.zcml`` file and the autoinclude entry point
+          for now, though;
+          we can imagine to use e.g. the Plone registry for some settings.
         
         [tobiasherp]
         
         
         1.4.4 (2021-08-31)
         ------------------
         
         Bugfixes:
         
-        - .setup.make_object_getter() didn't update the Language index when the language was changed
+        - `.setup.make_object_getter()` didn't update the Language index when the language was changed
         
         Improvements:
         
-        - .setup.make_object_getter() now additionally updates the following indexes
+        - `.setup.make_object_getter()` now additionally updates the following indexes
           when the .title attribute is changed:
         
           - sortable_title
           - SearchableText
           - getEffectiveIndex
         
         [tobiasherp]
@@ -675,28 +915,34 @@
         
         - Initial release.
           [tobiasherp]
         
         .. _BeautifulSoup: https://pypi.org/project/beautifulsoup4/
         .. _collective.metadataversion: https://pypi.org/project/collective.metadataversion
         .. _five.grok: https://pypi.org/project/five.grok
+        .. _importlib_metadata: https://pypi.org/project/importlib-metadata/
         .. _`metadata_version`: https://community.plone.org/t/metadata-column-metadata-version-for-conditional-metadata-refresh/14194/3
+        .. _packaging: https://pypi.org/project/packaging/
+        .. _`PEP 440`: https://peps.python.org/pep-0440/
         .. _Products.Archetypes: https://pypi.org/project/Products.Archetypes
         .. _Python: https://www.python.org
         .. _simplejson: https://pypi.org/project/simplejson
         .. _visaplan.kitchen: https://pypi.org/project/visaplan.kitchen
         .. _visaplan.plone.infohubs: https://pypi.org/project/visaplan.plone.infohubs
         .. _visaplan.tools: https://pypi.org/project/visaplan.tools
+        .. _zc.lockfile: https://pypi.org/project/zc.lockfile
         
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 4.3
 Classifier: Framework :: Zope2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: German
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Description-Content-Type: text/x-rst
 Provides-Extra: test
+Provides-Extra: lock
```

