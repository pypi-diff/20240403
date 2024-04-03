# Comparing `tmp/fstd2nc-0.20231105.2.tar.gz` & `tmp/fstd2nc-0.20240401.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fstd2nc-0.20231105.2.tar", last modified: Tue Feb 20 18:43:36 2024, max compression
+gzip compressed data, was "dist/fstd2nc-0.20240401.0.tar", last modified: Wed Apr  3 16:45:21 2024, max compression
```

## Comparing `fstd2nc-0.20231105.2.tar` & `fstd2nc-0.20240401.0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-02-20 18:43:36.722464 fstd2nc-0.20231105.2/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1809 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/.gitignore
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35147 2022-04-13 02:52:23.000000 fstd2nc-0.20231105.2/COPYING
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7651 2022-04-13 02:52:23.000000 fstd2nc-0.20231105.2/COPYING.LESSER
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    29176 2024-02-19 19:45:46.000000 fstd2nc-0.20231105.2/Changelog
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      114 2022-04-13 02:52:23.000000 fstd2nc-0.20231105.2/Makefile
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14074 2024-02-20 18:43:36.722124 fstd2nc-0.20231105.2/PKG-INFO
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13327 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/README.md
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14595 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/README_fr.md
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-02-20 18:43:36.379134 fstd2nc-0.20231105.2/cccbuffer/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      777 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/cccbuffer/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      182 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/cccbuffer/__main__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1022 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/cccbuffer/_xarray_hook.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      149 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/cccbuffer/cccdump.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-02-20 18:43:36.381707 fstd2nc-0.20231105.2/cccbuffer/mixins/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        0 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/cccbuffer/mixins/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3913 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/cccbuffer/mixins/ccc.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1193 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/cccbuffer/mixins/char.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2289 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/cccbuffer/mixins/grid.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4359 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/cccbuffer/mixins/levels.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3047 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/cccbuffer/mixins/superlabels.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6112 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/cccbuffer/mixins/times.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-02-20 18:43:36.383294 fstd2nc-0.20231105.2/conda.recipe/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      658 2024-02-19 19:45:46.000000 fstd2nc-0.20231105.2/conda.recipe/README.md
--rwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)       67 2024-02-19 19:45:46.000000 fstd2nc-0.20231105.2/conda.recipe/build.sh
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      512 2024-02-19 19:48:04.000000 fstd2nc-0.20231105.2/conda.recipe/meta.yaml
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-02-20 18:43:36.385306 fstd2nc-0.20231105.2/debian/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      143 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/debian/changelog
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        2 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/debian/compat
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      624 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/debian/control
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1103 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/debian/copyright
--rwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)      607 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/debian/rules
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-02-20 18:43:36.385694 fstd2nc-0.20231105.2/debian/source/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       12 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/debian/source/format
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-02-20 18:43:36.387039 fstd2nc-0.20231105.2/fstd2nc/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3788 2024-02-19 19:45:46.000000 fstd2nc-0.20231105.2/fstd2nc/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9892 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/__main__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7146 2024-02-19 19:45:46.000000 fstd2nc-0.20231105.2/fstd2nc/_xarray_hook.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14755 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/extra.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-02-20 18:43:36.391377 fstd2nc-0.20231105.2/fstd2nc/locale/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1526 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/locale/Makefile
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      974 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/locale/README.md
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-02-20 18:43:36.371501 fstd2nc-0.20231105.2/fstd2nc/locale/fr_CA/
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-02-20 18:43:36.391817 fstd2nc-0.20231105.2/fstd2nc/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    25402 2024-02-20 18:43:09.000000 fstd2nc-0.20231105.2/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    27270 2024-02-20 18:43:09.000000 fstd2nc-0.20231105.2/fstd2nc/locale/fr_CA.po
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-02-20 18:43:36.720940 fstd2nc-0.20231105.2/fstd2nc/mixins/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    42803 2024-02-19 19:45:46.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/__init__.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6457 2024-02-19 19:45:46.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/accum.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1871 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/ascii.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20498 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/compat.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    11830 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/dates.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3138 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/diaghacks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3220 2024-02-19 19:45:46.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/ensembles.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    34086 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/extern.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3581 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/filter.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    11699 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/fstd.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    23130 2024-01-24 19:13:40.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/gridhacks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8236 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/masks.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4249 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/mesh.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1786 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/misc.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20973 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/netcdf.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1735 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/pruneaxes.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4790 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/removestuff.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2610 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/select.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    23171 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/series.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8075 2024-02-19 19:45:46.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/sfc_codes.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7876 2024-02-19 19:45:46.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/vardict.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    41836 2024-02-19 19:45:46.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/vcoords.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    61231 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/mixins/xycoords.py
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2583 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/fstd2nc/stdout.py
-drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-02-20 18:43:36.388919 fstd2nc-0.20231105.2/fstd2nc.egg-info/
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14074 2024-02-20 18:43:35.000000 fstd2nc-0.20231105.2/fstd2nc.egg-info/PKG-INFO
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1554 2024-02-20 18:43:36.387749 fstd2nc-0.20231105.2/fstd2nc.egg-info/SOURCES.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        1 2024-02-20 18:43:35.000000 fstd2nc-0.20231105.2/fstd2nc.egg-info/dependency_links.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      289 2024-02-20 18:43:35.000000 fstd2nc-0.20231105.2/fstd2nc.egg-info/entry_points.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      218 2024-02-20 18:43:35.000000 fstd2nc-0.20231105.2/fstd2nc.egg-info/requires.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       18 2024-02-20 18:43:35.000000 fstd2nc-0.20231105.2/fstd2nc.egg-info/top_level.txt
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       59 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/pyproject.toml
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1370 2022-04-13 02:52:23.000000 fstd2nc-0.20231105.2/sample_meta.ini
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       38 2024-02-20 18:43:36.722540 fstd2nc-0.20231105.2/setup.cfg
--rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2664 2024-01-22 23:23:00.000000 fstd2nc-0.20231105.2/setup.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.169491 fstd2nc-0.20240401.0/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1809 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/.gitignore
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    35147 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.0/COPYING
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7651 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.0/COPYING.LESSER
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    29844 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/Changelog
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      114 2024-03-25 14:07:01.000000 fstd2nc-0.20240401.0/Makefile
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14236 2024-04-03 16:45:21.169094 fstd2nc-0.20240401.0/PKG-INFO
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    13489 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/README.md
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14775 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/README_fr.md
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.033633 fstd2nc-0.20240401.0/cccbuffer/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      777 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      182 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/__main__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1022 2024-03-27 16:22:27.000000 fstd2nc-0.20240401.0/cccbuffer/_xarray_hook.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      149 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/cccdump.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.035944 fstd2nc-0.20240401.0/cccbuffer/mixins/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        0 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/mixins/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3913 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/mixins/ccc.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1193 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/mixins/char.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2289 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/mixins/grid.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4359 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/mixins/levels.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3047 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/mixins/superlabels.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6112 2024-03-27 16:22:28.000000 fstd2nc-0.20240401.0/cccbuffer/mixins/times.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.037112 fstd2nc-0.20240401.0/conda.recipe/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      658 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/conda.recipe/README.md
+-rwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)       67 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/conda.recipe/build.sh
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      512 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/conda.recipe/meta.yaml
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.079387 fstd2nc-0.20240401.0/debian/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      143 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/debian/changelog
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        2 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/debian/compat
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      624 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/debian/control
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1103 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/debian/copyright
+-rwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)      607 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/debian/rules
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.079746 fstd2nc-0.20240401.0/debian/source/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       12 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/debian/source/format
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.081146 fstd2nc-0.20240401.0/fstd2nc/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3833 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     9889 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/__main__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     7146 2024-03-27 16:22:57.000000 fstd2nc-0.20240401.0/fstd2nc/_xarray_hook.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20044 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/extra.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.083519 fstd2nc-0.20240401.0/fstd2nc/locale/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1526 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/fstd2nc/locale/Makefile
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      974 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/fstd2nc/locale/README.md
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.028507 fstd2nc-0.20240401.0/fstd2nc/locale/fr_CA/
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.083893 fstd2nc-0.20240401.0/fstd2nc/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    25691 2024-04-03 16:44:59.000000 fstd2nc-0.20240401.0/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    27563 2024-04-03 16:44:59.000000 fstd2nc-0.20240401.0/fstd2nc/locale/fr_CA.po
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.168632 fstd2nc-0.20240401.0/fstd2nc/mixins/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    42803 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/__init__.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     6457 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/accum.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1871 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/ascii.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20498 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/compat.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    11830 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/dates.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3138 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/diaghacks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3220 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/ensembles.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    34534 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/extern.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3581 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/filter.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    12004 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/fstd.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    23130 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/gridhacks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8248 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/masks.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4249 2024-04-03 15:12:55.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/mesh.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1786 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/misc.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    20973 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/netcdf.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1735 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/pruneaxes.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     4790 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/removestuff.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2610 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/select.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    23171 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/series.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8075 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/sfc_codes.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     8783 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/vardict.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    41836 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/vcoords.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     3058 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/xmeta.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    61231 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/mixins/xycoords.py
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2583 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/fstd2nc/stdout.py
+drwxr-xr-x   0 min000   (67229) eccc_ccmr (66073)        0 2024-04-03 16:45:21.082876 fstd2nc-0.20240401.0/fstd2nc.egg-info/
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)    14236 2024-04-03 16:45:20.000000 fstd2nc-0.20240401.0/fstd2nc.egg-info/PKG-INFO
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1578 2024-04-03 16:45:20.000000 fstd2nc-0.20240401.0/fstd2nc.egg-info/SOURCES.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)        1 2024-04-03 16:45:20.000000 fstd2nc-0.20240401.0/fstd2nc.egg-info/dependency_links.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      289 2024-04-03 16:45:20.000000 fstd2nc-0.20240401.0/fstd2nc.egg-info/entry_points.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)      218 2024-04-03 16:45:20.000000 fstd2nc-0.20240401.0/fstd2nc.egg-info/requires.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       18 2024-04-03 16:45:20.000000 fstd2nc-0.20240401.0/fstd2nc.egg-info/top_level.txt
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       59 2024-03-25 14:09:07.000000 fstd2nc-0.20240401.0/pyproject.toml
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     1370 2022-04-13 02:52:23.000000 fstd2nc-0.20240401.0/sample_meta.ini
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)       38 2024-04-03 16:45:21.169656 fstd2nc-0.20240401.0/setup.cfg
+-rw-r--r--   0 min000   (67229) eccc_ccmr (66073)     2664 2024-04-03 15:12:56.000000 fstd2nc-0.20240401.0/setup.py
```

### Comparing `fstd2nc-0.20231105.2/.gitignore` & `fstd2nc-0.20240401.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/COPYING` & `fstd2nc-0.20240401.0/COPYING`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/COPYING.LESSER` & `fstd2nc-0.20240401.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/Changelog` & `fstd2nc-0.20240401.0/Changelog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Version 0.20240401.0 (Apr 3, 2023)
+	* Some support for new RSF file container and fst24 data format.
+	* Fixed bug in fstpy bridge - nk no longer stored in Buffer.
+	* Fixed check for operational dictionary when opdict=True is used in
+	  Python interface.
+	* Added _CRS attribute to xarray interface.
+	* Fixed bug when using dask distributed - the keys were not integers,
+	  but rather numpy integers, which apparently was a problem.
+	* Some support for mask typvar '!@'.
+	* Fix potential bug if used in future librmn release 20.1 - the
+	  call signature for armn_compress now requires an extra 'swap_stream'
+	  argument to control byte swapping of the decoded values.
+
 Version 0.20231105.2 (Feb 19, 2023)
 	* Fixed a bug in open_index() when the index contains pickled data.
 	* Fix some bugs in vertical bounds (when --bounds is used).
 	* Added some more fields to the list of accumulated quantities.
 	* Fix a bug when using .from_fstpy() followed by .to_xarray() on
 	  a single record.
```

### Comparing `fstd2nc-0.20231105.2/PKG-INFO` & `fstd2nc-0.20240401.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstd2nc
-Version: 0.20231105.2
+Version: 0.20240401.0
 Summary: Converts RPN standard files (from Environment Canada) to netCDF files.
 Home-page: https://github.com/neishm/fstd2nc
 Author: Mike Neish
 License: LGPL-3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -30,14 +30,18 @@
 Installing
 ==========
 
 The easiest way to install is using [pip](https://pip.pypa.io/en/stable):
 ```
 pip install fstd2nc
 ```
+Or, from conda:
+```
+conda install fortiers::fstd2nc
+```
 
 
 Basic Usage
 ===========
 
 From the command-line
 ---------------------
@@ -147,14 +151,16 @@
                         coordinates. Note that axes will only be excluded if
                         they have a length of 1.
   --yin                 Select first subgrid from a supergrid.
   --yang                Select second subgrid from a supergrid.
   --crop-to-smallest-grid
                         Crop grids to the smaller (inner core) domain for LAM
                         outputs.
+  --extended-metadata   Add extended metadata to the variables (fst24 data
+                        only).
   --metadata-file METADATA_FILE
                         Use metadata from the specified file. You can repeat
                         this option multiple times to build metadata from
                         different sources.
   --rename OLDNAME=NEWNAME,...
                         Apply the specified name changes to the variables.
   --conventions CONVENTIONS
```

### Comparing `fstd2nc-0.20231105.2/README.md` & `fstd2nc-0.20240401.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 Installing
 ==========
 
 The easiest way to install is using [pip](https://pip.pypa.io/en/stable):
 ```
 pip install fstd2nc
 ```
+Or, from conda:
+```
+conda install fortiers::fstd2nc
+```
 
 
 Basic Usage
 ===========
 
 From the command-line
 ---------------------
@@ -125,14 +129,16 @@
                         coordinates. Note that axes will only be excluded if
                         they have a length of 1.
   --yin                 Select first subgrid from a supergrid.
   --yang                Select second subgrid from a supergrid.
   --crop-to-smallest-grid
                         Crop grids to the smaller (inner core) domain for LAM
                         outputs.
+  --extended-metadata   Add extended metadata to the variables (fst24 data
+                        only).
   --metadata-file METADATA_FILE
                         Use metadata from the specified file. You can repeat
                         this option multiple times to build metadata from
                         different sources.
   --rename OLDNAME=NEWNAME,...
                         Apply the specified name changes to the variables.
   --conventions CONVENTIONS
```

### Comparing `fstd2nc-0.20231105.2/README_fr.md` & `fstd2nc-0.20240401.0/README_fr.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 Installation
 ==========
 
 La façon plus simple d'installer est d'utiliser [pip](https://pip.pypa.io/en/stable):
 ```
 pip install fstd2nc
 ```
+Ou, de conda:
+```
+conda install fortiers::fstd2nc
+```
 
 
 Utilisation de base
 ===========
 
 À partir de la ligne de commande
 ---------------------
@@ -137,14 +141,16 @@
   --yin                 Sélectionner la première sous-grille d'une super
                         grille.
   --yang                Sélectionner la deuxième sous-grille d'une super
                         grille.
   --crop-to-smallest-grid
                         Couper les grilles au domaine plus petit (noyau
                         interne) pours les sorties LAM.
+  --extended-metadata   Ajouter des métadonnées étendues aux variables
+                        (données fst24 seulement).
   --metadata-file METADATA_FILE
                         Utiliser les métadonnées du fichier spécifié.
   --rename OLDNAME=NEWNAME,...
                         Appliquer les changes de nom spécifiés aux variables.
   --conventions CONVENTIONS
                         Définir l'attribut "Conventions" pour le fichier
                         netCDF. Le défaut est "CF-1.6". Notez que cela n'a
```

### Comparing `fstd2nc-0.20231105.2/cccbuffer/__init__.py` & `fstd2nc-0.20240401.0/cccbuffer/__init__.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/cccbuffer/_xarray_hook.py` & `fstd2nc-0.20240401.0/cccbuffer/_xarray_hook.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/cccbuffer/mixins/ccc.py` & `fstd2nc-0.20240401.0/cccbuffer/mixins/ccc.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/cccbuffer/mixins/char.py` & `fstd2nc-0.20240401.0/cccbuffer/mixins/char.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/cccbuffer/mixins/grid.py` & `fstd2nc-0.20240401.0/cccbuffer/mixins/grid.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/cccbuffer/mixins/levels.py` & `fstd2nc-0.20240401.0/cccbuffer/mixins/levels.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/cccbuffer/mixins/superlabels.py` & `fstd2nc-0.20240401.0/cccbuffer/mixins/superlabels.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/cccbuffer/mixins/times.py` & `fstd2nc-0.20240401.0/cccbuffer/mixins/times.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/conda.recipe/README.md` & `fstd2nc-0.20240401.0/conda.recipe/README.md`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/conda.recipe/meta.yaml` & `fstd2nc-0.20240401.0/conda.recipe/meta.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 package:
   name: fstd2nc
-  version: 0.20231105.2
+  version: 0.20240401.0
 
 
 requirements:
   build:
     - python
     - numpy  >1.15.3
     - netcdf4
```

### Comparing `fstd2nc-0.20231105.2/debian/control` & `fstd2nc-0.20240401.0/debian/control`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/debian/copyright` & `fstd2nc-0.20240401.0/debian/copyright`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/debian/rules` & `fstd2nc-0.20240401.0/debian/rules`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/fstd2nc/__init__.py` & `fstd2nc-0.20240401.0/fstd2nc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -19,15 +19,15 @@
 ###############################################################################
 
 
 """
 Functionality for converting between FSTD and netCDF files.
 """
 
-__version__ = "0.20231105.2"
+__version__ = "0.20240401.0"
 
 
 # Check for bundled rpnpy package.
 # Fall back to this one if no standard rpnpy package available.
 try:
   # Importing the module will set up the appropriate search paths.
   import fstd2nc_deps
@@ -61,20 +61,21 @@
 from fstd2nc.mixins.xycoords import XYCoords
 from fstd2nc.mixins.mesh import Mesh
 from fstd2nc.mixins.misc import NoNK
 from fstd2nc.mixins.filter import FilterRecords
 from fstd2nc.mixins.removestuff import RemoveStuff
 from fstd2nc.mixins.gridhacks import GridHacks, Interp, YinYang, Crop
 from fstd2nc.mixins.pruneaxes import PruneAxes
+from fstd2nc.mixins.xmeta import XMeta
 from fstd2nc.mixins.netcdf import netCDF_Atts, netCDF_IO
 from fstd2nc.mixins.compat import FSTD_Compat
 from fstd2nc.mixins.extern import ExternInput, ExternOutput
 from fstd2nc.mixins.diaghacks import DiagHacks
 
-class Buffer (DiagHacks,ExternOutput,FSTD_Compat,netCDF_IO,netCDF_Atts,PruneAxes,Crop,YinYang,Interp,GridHacks,RemoveStuff,FilterRecords,NoNK,Mesh,XYCoords,VCoords,Sfc_Codes,VarDict,Series,Ensembles,Accum,Dates,Masks,ASCII,SelectVars,ExternInput,FSTD):
+class Buffer (DiagHacks,ExternOutput,FSTD_Compat,netCDF_IO,netCDF_Atts,XMeta,PruneAxes,Crop,YinYang,Interp,GridHacks,RemoveStuff,FilterRecords,NoNK,Mesh,XYCoords,VCoords,Sfc_Codes,VarDict,Series,Ensembles,Accum,Dates,Masks,ASCII,SelectVars,ExternInput,FSTD):
   """
   High-level interface for FSTD data, to treat it as multi-dimensional arrays.
   Contains logic for dealing with most of the common FSTD file conventions.
   """
   def __init__ (self, filename, *args, **kwargs):
     super(Buffer,self).__init__(filename, *args,**kwargs)
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/__main__.py` & `fstd2nc-0.20240401.0/fstd2nc/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -60,15 +60,15 @@
   try:
     buf = buffer_type(infile, **args)
   except FSTDError:
     error (_("problem opening one or more input files."))
 
   # Get the metadata in a netCDF-like structure.
   buf._makevars()
-  print ("fstd98 %s {"%basename(infile))
+  print ("fst %s {"%basename(infile))
   print ("dimensions:")
   for axis in buf._iter_axes():
     print ("\t%s = %d ;"%(axis.name,len(axis)))
   print ("variables:")
   for var in buf._iter_objects():
     if not hasattr(var,'axes'): continue # Skip dimensions
     if hasattr(var,'dtype'):
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/_xarray_hook.py` & `fstd2nc-0.20240401.0/fstd2nc/_xarray_hook.py`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/fstd2nc/locale/Makefile` & `fstd2nc-0.20240401.0/fstd2nc/locale/Makefile`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/fstd2nc/locale/README.md` & `fstd2nc-0.20240401.0/fstd2nc/locale/README.md`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo` & `fstd2nc-0.20240401.0/fstd2nc/locale/fr_CA/LC_MESSAGES/fstd2nc.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: fstd2nc\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:09+0000\n"
+"POT-Creation-Date: 2024-03-27 15:44+0000\n"
 "PO-Revision-Date: 2022-11-25 17:40+0000\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: fr_CA\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=ISO-8859-1\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -33,14 +33,18 @@
 
 msgid ".__call__() not defined"
 msgstr ".__call__() non défini"
 
 msgid "Aborted by user."
 msgstr "Annulé par l'utilisateur."
 
+msgid "Add extended metadata to the variables (fst24 data only)."
+msgstr ""
+"Ajouter des métadonnées étendues aux variables (données fst24 seulement)."
+
 msgid ""
 "Adds a compatibility layer to the netCDF output file, so it can also "
 "function as a valid FSTD file.  EXPERIMENTAL."
 msgstr ""
 "Ajoute une couche de compatibilité au fichier de sortie netCDF, qu'il puisse "
 "également fonctionner comme un fichier FSTD valide.  EXPÉRIMENTAL."
 
@@ -61,14 +65,17 @@
 "plusieurs dates d'origine.  Assayez relancer avec l'option --dateo."
 
 msgid "Cannot read from %s - file may be missing or damaged."
 msgstr ""
 "Impossible de lire à partir de %s - le fichier est peut-être manquant ou "
 "endommagé."
 
+msgid "Cartopy not found.  Unable to add _CRS attribute."
+msgstr "Cartopy non trouvée Impossible d'ajouter l'attribut _CRS."
+
 msgid ""
 "Collect different etikets for the same variable together into an "
 "\"ensemble\" axis."
 msgstr ""
 "Rassembler différentes etikets pour la même variable ensemble dans une axe "
 "\"ensemble\"."
 
@@ -643,15 +650,15 @@
 
 msgid "an RPN standard file"
 msgstr "un fichier standard RPN"
 
 msgid "argument \"-\" with mode %r"
 msgstr "argument \"-\" avec le mode %r"
 
-msgid "can't open '%s': %s"
+msgid "can't open '%(filename)s': %(error)s"
 msgstr "impossible d'ouvrir '%s': %s"
 
 msgid "cannot have multiple subparser arguments"
 msgstr "impossible d'avoir plusiers arguments de sous-analyseur"
 
 msgid "cannot merge actions - two groups are named %r"
 msgstr "impossible de fusionner les actions - deux groupes sont nommés %r"
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/locale/fr_CA.po` & `fstd2nc-0.20240401.0/fstd2nc/locale/fr_CA.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file is distributed under the same license as the fstd2nc package.
 # Automatically generated, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: fstd2nc\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-08 18:09+0000\n"
+"POT-Creation-Date: 2024-03-27 15:44+0000\n"
 "PO-Revision-Date: 2022-11-25 17:40+0000\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: fr_CA\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=ISO-8859-1\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -114,14 +114,17 @@
 #, python-format
 msgid "Refusing to overwrite existing file '%s'."
 msgstr "Refus de remplacer le fichier existant '%s'."
 
 msgid "Aborted by user."
 msgstr "Annulé par l'utilisateur."
 
+msgid "Add extended metadata to the variables (fst24 data only)."
+msgstr "Ajouter des métadonnées étendues aux variables (données fst24 seulement)."
+
 msgid "NAME,NAME,..."
 msgstr "NOM,NOM,..."
 
 msgid ""
 "Exclude some axes, attributes,  or derived variables from the output.  For "
 "instance, excluding 'leadtime,reftime' can help for netCDF tools that don't "
 "recognize leadtime and reftime as valid coordinates.  Note that axes will "
@@ -515,14 +518,17 @@
 msgid ""
 "Dates out of bounds for pandas routines.  Using alternative (slower) "
 "routines."
 msgstr ""
 "Dates hors limites pour les routines des pandas. Utiliser des routines "
 "alternatives (plus lentes)."
 
+msgid "Cartopy not found.  Unable to add _CRS attribute."
+msgstr "Cartopy non trouvée Impossible d'ajouter l'attribut _CRS."
+
 #, python-format
 msgid "'batch' size (%d) does not divide evenly into number of files (%s)"
 msgstr ""
 "Taille 'batch' (%d) ne se divise pas uniformément en nombre de fichiers (%s)"
 
 msgid "Indexing the files"
 msgstr "Indexer les fichiers"
@@ -726,15 +732,15 @@
 msgstr "Analyseur inconnue %(parser_name)r (choix: %(choices)s)"
 
 #, python-format
 msgid "argument \"-\" with mode %r"
 msgstr "argument \"-\" avec le mode %r"
 
 #, python-format
-msgid "can't open '%s': %s"
+msgid "can't open '%(filename)s': %(error)s"
 msgstr "impossible d'ouvrir '%s': %s"
 
 #, python-format
 msgid "cannot merge actions - two groups are named %r"
 msgstr "impossible de fusionner les actions - deux groupes sont nommés %r"
 
 msgid "'required' is an invalid argument for positionals"
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/__init__.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/accum.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/accum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/ascii.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/ascii.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/compat.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/dates.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/dates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/diaghacks.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/diaghacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/ensembles.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/ensembles.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/extern.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/extern.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -443,15 +443,15 @@
       graphs = zip([self._dasked_read]*nchunks, *args)
       array = np.empty(nchunks, dtype=object)
       array[:] = list(graphs)
       shape = tuple(len(c) for c in var.chunks)
       array = array.reshape(shape)
 
       # Create dask array from this info.
-      chunk_indices = [np.cumsum((0,)+c)[:-1] for c in var.chunks]
+      chunk_indices = [list(map(int,np.cumsum((0,)+c)[:-1])) for c in var.chunks]
       # Loop over all indices, generate dask graph.
       dsk = dict()
       for ind, chunk_coord, chunk_shape in zip(np.ndindex(array.shape), product(*chunk_indices), product(*var.chunks)):
         # Unique key for this graph member.
         key = (name,) + chunk_coord
         # Add this record as a chunk in the dask Array.
         graph = array[ind]
@@ -471,14 +471,15 @@
   def to_xarray (self, fused=False):
     """
     Create an xarray interface for the RPN data.
     Requires the xarray and dask packages.
     """
     from collections import OrderedDict
     import xarray as xr
+    from fstd2nc.extra import get_crs
     out = OrderedDict()
     for var in self._iter_dask(fused=fused):
       if not hasattr(var,'array'): continue
       out[var.name] = xr.DataArray(data=var.array, dims=var.dims, name=var.name, attrs=var.atts)
       # Preserve chunking information for writing to netCDF4.
       if hasattr(var.array,'chunks'):
         chunk_shape = [c[0] for c in var.array.chunks]
@@ -495,14 +496,22 @@
     out.encoding['unlimited_dims'] = ('time',)
 
     # Remove coordinates from encoding, so that xarray can determine the
     # appropriate values upon writing to netCDF4.
     for var in out.variables:
       out[var].encoding.pop('coordinates',None)
 
+    # Add CRS information (used by some Python modules).
+    try:
+      crs = get_crs(out)
+    except ModuleNotFoundError:
+      warn(_('Cartopy not found.  Unable to add _CRS attribute.'))
+    else:
+      if crs is not None:
+        out.attrs['_CRS'] = crs.to_wkt()
     return out
 
   def to_xarray_list (self, fused=False):
     """
     Similar to the to_xarray method, but returns a list of xarray Datasets,
     one for each variable, instead of a single Dataset object.
     Could be useful for case where the dimension names are non-unique, to avoid
@@ -722,27 +731,29 @@
     """
     import pandas as pd
     import numpy as np
     from fstd2nc.extra import decode
     from dask import delayed
     import dask.array as da
     # Put all the header info into a dictionary.
-    fields = ['nomvar', 'typvar', 'etiket', 'ni', 'nj', 'nk', 'ip1', 'ip2', 'ip3', 'deet', 'npas', 'datyp', 'nbits', 'grtyp', 'ig1', 'ig2', 'ig3', 'ig4', 'datev']
+    fields = ['nomvar', 'typvar', 'etiket', 'ni', 'nj', 'ip1', 'ip2', 'ip3', 'deet', 'npas', 'datyp', 'nbits', 'grtyp', 'ig1', 'ig2', 'ig3', 'ig4', 'datev']
     table = dict()
     # Create a mask to exclude deleted / overwritten / unselected records.
     # Include all meta (coordinate) records in the output.
     mask = self._headers['selected'] | self._headers['ismeta']
     for field in fields:
       col = self._headers[field][mask]
       # Convert byte arrays to strings, which is what fstpy expects.
       if col.dtype.str.startswith('|S'):
         col = np.asarray(col,dtype=col.dtype.str.replace('|S','<U'))
       table[field] = col
     # Convert to pandas table.
     table = pd.DataFrame.from_dict(table)
+    # Add other things which aren't stored in the headers.
+    table['nk'] = 1  # This was removed from fstd2nc header table to save space.
     # Generate dask objects.
     # NOTE: using raw (records for this, no transformations / masking applied).
     if 'file_id' in self._headers and 'address' in self._headers and 'length' in self._headers:
       filenames = np.array(self._files+[None])
       filenames = filenames[self._headers['file_id']]
       arrays = map(delayed(_read_block), filenames, self._headers['address'], self._headers['length'])
       arrays = map(delayed(decode), arrays)
@@ -795,15 +806,15 @@
     table : pandas DataFrame
         The table of records from fstpy.
     """
     import numpy as np
     if hasattr(table,'to_pandas'):
       table = table.to_pandas()
     # Construct the record header info from the table.
-    fields = ['nomvar', 'typvar', 'etiket', 'ni', 'nj', 'nk', 'ip1', 'ip2', 'ip3', 'deet', 'npas', 'datyp', 'nbits', 'grtyp', 'ig1', 'ig2', 'ig3', 'ig4', 'datev']
+    fields = ['nomvar', 'typvar', 'etiket', 'ni', 'nj', 'ip1', 'ip2', 'ip3', 'deet', 'npas', 'datyp', 'nbits', 'grtyp', 'ig1', 'ig2', 'ig3', 'ig4', 'datev']
     headers = {}
     for col in fields:
       headers[col] = table[col].values.copy()
     # Pad out string variables with spaces.
     headers['nomvar'] = np.asarray(headers['nomvar'], dtype='|S4')
     headers['typvar'] = np.asarray(headers['nomvar'], dtype='|S2')
     headers['etiket'] = np.asarray(headers['etiket'], dtype='|S12')
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/filter.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/fstd.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/fstd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -127,15 +127,15 @@
         variable on different etikets.
     """
     import numpy as np
 
     # Note: name should always be the first attribute
     self._var_id = ('name','ni','nj') + self._var_id
     self._human_var_id = ('%(name)s', '%(ni)sx%(nj)s') + self._human_var_id
-    self._ignore_atts = ('swa','lng','dltf','ubc','xtra1','xtra2','xtra3','i','j','k','nk','ismeta','d') + self._ignore_atts
+    self._ignore_atts = ('swa','lng','meta_length','dltf','ubc','xtra1','xtra2','xtra3','i','j','k','nk','ismeta','d') + self._ignore_atts
 
     ignore_typvar = kwargs.pop('ignore_typvar',False)
     ignore_etiket = kwargs.pop('ignore_etiket',False)
 
     if not ignore_typvar:
       # Insert typvar value just after nomvar.
       self._var_id = self._var_id[0:1] + ('typvar',) + self._var_id[1:]
@@ -166,30 +166,34 @@
     self._headers['j'] = self._headers['nj']
     self._headers['i'] = self._headers['ni']
 
     # Add some standard fields needed for the Buffer.
     self._headers['name'] = self._headers['nomvar']
     # These two fields may not exist for externally-sourced data
     # (such as from fstpy)
-    if 'swa' in self._headers:
+    if 'address' not in self._headers and 'swa' in self._headers:
       self._headers['address'] = np.array(self._headers['swa'],int)*8-8
       del self._headers['swa']
-    if 'lng' in self._headers:
+    if 'length' not in self._headers and 'lng' in self._headers:
       self._headers['length'] = np.array(self._headers['lng'],'int32')*4
       del self._headers['lng']
+    # Metadata length is a fixed size for fst98.
+    if 'meta_length' not in self._headers:
+      self._headers['meta_length'] = np.full(self._nrecs,18,dtype='uint16')
     self._headers['dtype'] = np.empty(self._nrecs, dtype='|S2')
     self._headers['dtype'][:] = np.array(fast_dtype_fst2numpy(self._headers['datyp'],self._headers['nbits']))
     self._headers['selected'] = (self._headers['dltf']==0) & (self._headers['ismeta'] == False)
 
   # How to decode the data from a raw binary array.
-  @staticmethod
-  def _decode (data):
+  @classmethod
+  def _decode (cls,data):
     from fstd2nc.extra import decode
-    nbits = int(data[0x0b])
-    datyp = int(data[0x13])
+    prm = cls._decode_headers(data[:72])
+    nbits = int(prm['nbits'][0])
+    datyp = int(prm['datyp'][0])
     dtype = dtype_fst2numpy(datyp, nbits)
     out = decode(data).view(dtype)
     return out
 
   # Shortcuts to header decoding functions.
   # Put into the class so they can potentially be overridden for other formats.
   @staticmethod
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/gridhacks.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/gridhacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/masks.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/masks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -79,15 +79,15 @@
     ip3 = self._headers['ip3']
     dltf = self._headers['dltf']
     uses_mask = np.array(typvar,dtype='|S2').view('|S1').reshape(-1,2)[:,1] == b'@'
     if not np.any(uses_mask): return
 
     # Remove all mask records from the table, they should not become variables
     # themselves.
-    is_mask = (self._headers['typvar'] == b'@@')
+    is_mask = np.isin(self._headers['typvar'],(b'@@',b'!@'))
     self._headers['selected'][is_mask] = False
 
     nrecs = len(self._headers['name'])
 
     # Figure out how to pair up the data and mask.
     # Requires O(n log n) time, which is better than O(n^2) for naive lookup
     # on each record.
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/mesh.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/misc.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/netcdf.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/netcdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/pruneaxes.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/pruneaxes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/removestuff.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/removestuff.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/select.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/select.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/series.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/sfc_codes.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/sfc_codes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/vardict.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/vardict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -65,22 +65,46 @@
     opdict : bool, optional
         Similar to above, but use the standard CMC-RPN operational dictionary.
     """
     from os import environ
     from fstd2nc.mixins import _var_type, _axis_type, _dim_type
     from collections import OrderedDict
     from xml.etree import ElementTree as ET
+    from os.path import exists
 
+    opdict = kwargs.pop('opdict',False)
     vardicts = kwargs.pop('vardict',None) or []
-    if kwargs.pop('opdict',False):
+
+    ### copied and modified from _check_args
+    if opdict:
+      if 'CMCCONST' in environ:
+        f = environ['CMCCONST']+'/opdict/ops.variable_dictionary.xml'
+        if not exists(f):
+          error(_("Unable to find $CMCCONST/opdict/ops.variable_dictionary.xml"))
+      elif 'AFSISIO' in environ:
+        f = environ['AFSISIO']+'/datafiles/constants/opdict/ops.variable_dictionary.xml'
+        if not exists(f):
+          error(_("Unable to find $AFSISIO/datafiles/constants/opdict/ops.variable_dictionary.xml"))
+      else:
+        error(_("Neither $CMCCONST nor $AFSISIO defined.  Can't find operational dictionary."))
+
+    if vardicts is not None:
+      for f in vardicts:
+        if not exists(f):
+          error(_("Unable to find '%s'")%f)
+    ###
+
+    # Add operational dictionary to list of dictionaries to use.
+    if opdict:
       if 'CMCCONST' in environ:
         f = environ['CMCCONST']+'/opdict/ops.variable_dictionary.xml'
+        vardicts.append(f)
       elif 'AFSISIO' in environ:
         f = environ['AFSISIO']+'/datafiles/constants/opdict/ops.variable_dictionary.xml'
-      vardicts.append(f)
+        vardicts.append(f)
 
     super(VarDict,self).__init__(*args, **kwargs)
 
     metadata = OrderedDict()
     ip1_axis = OrderedDict()
     ip3_axis = OrderedDict()
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/vcoords.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/vcoords.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/mixins/xycoords.py` & `fstd2nc-0.20240401.0/fstd2nc/mixins/xycoords.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc/stdout.py` & `fstd2nc-0.20240401.0/fstd2nc/stdout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc.egg-info/PKG-INFO` & `fstd2nc-0.20240401.0/fstd2nc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fstd2nc
-Version: 0.20231105.2
+Version: 0.20240401.0
 Summary: Converts RPN standard files (from Environment Canada) to netCDF files.
 Home-page: https://github.com/neishm/fstd2nc
 Author: Mike Neish
 License: LGPL-3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -30,14 +30,18 @@
 Installing
 ==========
 
 The easiest way to install is using [pip](https://pip.pypa.io/en/stable):
 ```
 pip install fstd2nc
 ```
+Or, from conda:
+```
+conda install fortiers::fstd2nc
+```
 
 
 Basic Usage
 ===========
 
 From the command-line
 ---------------------
@@ -147,14 +151,16 @@
                         coordinates. Note that axes will only be excluded if
                         they have a length of 1.
   --yin                 Select first subgrid from a supergrid.
   --yang                Select second subgrid from a supergrid.
   --crop-to-smallest-grid
                         Crop grids to the smaller (inner core) domain for LAM
                         outputs.
+  --extended-metadata   Add extended metadata to the variables (fst24 data
+                        only).
   --metadata-file METADATA_FILE
                         Use metadata from the specified file. You can repeat
                         this option multiple times to build metadata from
                         different sources.
   --rename OLDNAME=NEWNAME,...
                         Apply the specified name changes to the variables.
   --conventions CONVENTIONS
```

### Comparing `fstd2nc-0.20231105.2/fstd2nc.egg-info/SOURCES.txt` & `fstd2nc-0.20240401.0/fstd2nc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -61,8 +61,9 @@
 fstd2nc/mixins/pruneaxes.py
 fstd2nc/mixins/removestuff.py
 fstd2nc/mixins/select.py
 fstd2nc/mixins/series.py
 fstd2nc/mixins/sfc_codes.py
 fstd2nc/mixins/vardict.py
 fstd2nc/mixins/vcoords.py
+fstd2nc/mixins/xmeta.py
 fstd2nc/mixins/xycoords.py
```

### Comparing `fstd2nc-0.20231105.2/sample_meta.ini` & `fstd2nc-0.20240401.0/sample_meta.ini`

 * *Files identical despite different names*

### Comparing `fstd2nc-0.20231105.2/setup.py` & `fstd2nc-0.20240401.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################################################################
-# Copyright 2017-2023 - Climate Research Division
+# Copyright 2017-2024 - Climate Research Division
 #                       Environment and Climate Change Canada
 #
 # This file is part of the "fstd2nc" package.
 #
 # "fstd2nc" is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Lesser General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
@@ -40,17 +40,17 @@
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
     'Programming Language :: Python',
     'Topic :: Scientific/Engineering :: Atmospheric Science',
   ],
   packages = find_packages(),
   setup_requires = ['pip >= 8.1'],
-  install_requires = ['numpy >= 1.13.0, != 1.15.3','netcdf4','fstd2nc-deps >= 0.20200304.0','progress'],
+  install_requires = ['numpy >= 1.13.0, != 1.15.3','netcdf4','fstd2nc-deps >= 0.20200304.0'],
   extras_require = {
-    'manyfiles': ['pandas'],
+    'manyfiles': ['pandas','progress'],
     'array': ['xarray>=0.10.3','dask','toolz'],
     'iris': ['iris>=2.0','xarray>=0.10.3','dask','toolz'],
     'pygeode': ['pygeode>=1.2.2','xarray>=0.10.3','dask','toolz'],
   },
   package_data = {
     'fstd2nc': ['locale/*/LC_MESSAGES/fstd2nc.mo'],
   },
```

