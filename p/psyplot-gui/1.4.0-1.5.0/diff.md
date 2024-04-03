# Comparing `tmp/psyplot-gui-1.4.0.tar.gz` & `tmp/psyplot-gui-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyplot-gui-1.4.0.tar", last modified: Sat Oct  9 15:09:59 2021, max compression
+gzip compressed data, was "psyplot-gui-1.5.0.tar", last modified: Wed Apr  3 14:52:42 2024, max compression
```

## Comparing `psyplot-gui-1.4.0.tar` & `psyplot-gui-1.5.0.tar`

### file list

```diff
@@ -1,67 +1,140 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-10-09 15:09:59.678027 psyplot-gui-1.4.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/COPYING
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7652 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/COPYING.LESSER
--rw-r--r--   0 circleci  (3434) circleci  (3434)      279 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4748 2021-10-09 15:09:59.678027 psyplot-gui-1.4.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3414 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-10-09 15:09:59.678027 psyplot-gui-1.4.0/psyplot_gui/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18384 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      497 2021-10-09 15:09:59.678027 psyplot-gui-1.4.0/psyplot_gui/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5644 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/backend.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12428 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/common.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-10-09 15:09:59.670027 psyplot-gui-1.4.0/psyplot_gui/compat/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      970 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/compat/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5893 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/compat/qtcompat.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-10-09 15:09:59.670027 psyplot-gui-1.4.0/psyplot_gui/config/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     1807 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/config/__init__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     9831 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/config/rcsetup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13451 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/console.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28170 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/content_widget.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    37100 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/dataframeeditor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7032 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/dependencies.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26861 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/fmt_widget.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    41464 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/help_explorer.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-10-09 15:09:59.674027 psyplot-gui-1.4.0/psyplot_gui/icons/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1165 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/console-go.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      846 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/copy.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1627 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/docu_button.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10790 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/info.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16750 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/invalid.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      571 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/ipython_console.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      357 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/ipython_console_t.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      777 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/lock.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      307 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/lock_open.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)   109439 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/logo.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)   138236 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/logo.svg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1381 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/minus.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16872 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/minusminus.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1861 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/next.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4509 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/plus.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22468 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/plusplus.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1715 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/previous.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12413 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/rcParams.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4595 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/refresh.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6042 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/run_arrow.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12381 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/valid.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11037 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/warning.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13643 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/world.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28114 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/icons/world_red.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    44881 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/main.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    87524 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/plot_creator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24015 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/preferences.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-10-09 15:09:59.678027 psyplot-gui-1.4.0/psyplot_gui/sphinx_supp/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      988 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/sphinx_supp/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-10-09 15:09:59.678027 psyplot-gui-1.4.0/psyplot_gui/sphinx_supp/_static/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/sphinx_supp/_static/.gitignore
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     6214 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/sphinx_supp/conf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/psyplot_gui/sphinx_supp/psyplot.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-10-09 15:09:59.670027 psyplot-gui-1.4.0/psyplot_gui.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4748 2021-10-09 15:09:59.000000 psyplot-gui-1.4.0/psyplot_gui.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1621 2021-10-09 15:09:59.000000 psyplot-gui-1.4.0/psyplot_gui.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-10-09 15:09:59.000000 psyplot-gui-1.4.0/psyplot_gui.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-10-09 15:09:59.000000 psyplot-gui-1.4.0/psyplot_gui.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2021-10-09 15:09:59.000000 psyplot-gui-1.4.0/psyplot_gui.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2021-10-09 15:09:59.000000 psyplot-gui-1.4.0/psyplot_gui.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      213 2021-10-09 15:09:59.678027 psyplot-gui-1.4.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3827 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    69731 2021-10-09 15:03:52.000000 psyplot-gui-1.4.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:52:42.266748 psyplot-gui-1.5.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:52:42.246747 psyplot-gui-1.5.0/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    17023 2024-04-03 14:52:13.000000 psyplot-gui-1.5.0/LICENSES/CC-BY-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-04-03 14:52:13.000000 psyplot-gui-1.5.0/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)    42098 2024-04-03 14:52:13.000000 psyplot-gui-1.5.0/LICENSES/LGPL-3.0-only.txt
+-rw-rw-rw-   0 root         (0) root         (0)      444 2024-04-03 14:52:13.000000 psyplot-gui-1.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2713 2024-04-03 14:52:42.266748 psyplot-gui-1.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3183 2024-04-03 14:52:13.000000 psyplot-gui-1.5.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:52:42.250748 psyplot-gui-1.5.0/psyplot_gui/
+-rw-rw-rw-   0 root         (0) root         (0)    18116 2024-04-03 14:52:13.000000 psyplot-gui-1.5.0/psyplot_gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-03 14:52:42.266748 psyplot-gui-1.5.0/psyplot_gui/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5116 2024-04-03 14:52:13.000000 psyplot-gui-1.5.0/psyplot_gui/backend.py
+-rw-rw-rw-   0 root         (0) root         (0)    11918 2024-04-03 14:52:13.000000 psyplot-gui-1.5.0/psyplot_gui/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:52:42.250748 psyplot-gui-1.5.0/psyplot_gui/compat/
+-rwxrwxrwx   0 root         (0) root         (0)      277 2024-04-03 14:52:13.000000 psyplot-gui-1.5.0/psyplot_gui/compat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2024-04-03 14:52:13.000000 psyplot-gui-1.5.0/psyplot_gui/compat/qtcompat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:52:42.250748 psyplot-gui-1.5.0/psyplot_gui/config/
+-rwxrwxrwx   0 root         (0) root         (0)     1089 2024-04-03 14:52:13.000000 psyplot-gui-1.5.0/psyplot_gui/config/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9669 2024-04-03 14:52:13.000000 psyplot-gui-1.5.0/psyplot_gui/config/rcsetup.py
+-rw-rw-rw-   0 root         (0) root         (0)    13209 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/console.py
+-rw-rw-rw-   0 root         (0) root         (0)    27922 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/content_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)    36965 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/dataframeeditor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6452 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/dependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)    26736 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/fmt_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)    41875 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/help_explorer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:52:42.262748 psyplot-gui-1.5.0/psyplot_gui/icons/
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/console-go.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/console-go.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      500 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/console-go.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/console-go.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/copy.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/copy.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/copy.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/copy.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/docu_button.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/docu_button.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/docu_button.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/docu_button.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)     6699 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/info.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/info.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      499 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/info.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/info.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)     3518 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/invalid.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/invalid.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/invalid.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/invalid.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)      571 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/ipython_console.png
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/ipython_console.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/ipython_console_t.png
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/ipython_console_t.png.license
+-rw-rw-rw-   0 root         (0) root         (0)     4281 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/lock.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/lock.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/lock.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/lock.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)     4137 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/lock_open.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/lock_open.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/lock_open.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/lock_open.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)   109439 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/logo.png.license
+-rw-rw-rw-   0 root         (0) root         (0)   132697 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/logo.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/minus.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/minus.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/minus.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/minus.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/minusminus.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/minusminus.png.license
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/minusminus.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/minusminus.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)      722 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/next.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/next.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      400 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/next.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/next.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/plus.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/plus.png.license
+-rw-rw-rw-   0 root         (0) root         (0)     2434 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/plus.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/plus.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)    22468 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/plusplus.png
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/plusplus.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      710 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/previous.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/previous.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      397 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/previous.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/previous.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/rcParams.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/rcParams.png.license
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/rcParams.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/rcParams.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/refresh.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/refresh.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/refresh.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/refresh.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)    10654 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/run_arrow.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/run_arrow.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      521 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/run_arrow.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/run_arrow.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)     2574 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/valid.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/valid.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      427 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/valid.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/valid.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)     1800 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/warning.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/warning.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/warning.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/warning.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/world.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/world.png.license
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/world.svg
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/world.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)     5158 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/world_red.png
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/world_red.png.license
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/icons/world_red.svg.license
+-rw-rw-rw-   0 root         (0) root         (0)    45139 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    88788 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/plot_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)    23578 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/preferences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:52:42.262748 psyplot-gui-1.5.0/psyplot_gui/sphinx_supp/
+-rw-rw-rw-   0 root         (0) root         (0)      295 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/sphinx_supp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:52:42.262748 psyplot-gui-1.5.0/psyplot_gui/sphinx_supp/_static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/sphinx_supp/_static/.gitignore
+-rwxrwxrwx   0 root         (0) root         (0)     5333 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/sphinx_supp/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/psyplot_gui/sphinx_supp/psyplot.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:52:42.262748 psyplot-gui-1.5.0/psyplot_gui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2713 2024-04-03 14:52:42.000000 psyplot-gui-1.5.0/psyplot_gui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4070 2024-04-03 14:52:42.000000 psyplot-gui-1.5.0/psyplot_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 14:52:42.000000 psyplot-gui-1.5.0/psyplot_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 14:52:41.000000 psyplot-gui-1.5.0/psyplot_gui.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      392 2024-04-03 14:52:42.000000 psyplot-gui-1.5.0/psyplot_gui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-03 14:52:42.000000 psyplot-gui-1.5.0/psyplot_gui.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3225 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 14:52:42.266748 psyplot-gui-1.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      287 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 14:52:42.262748 psyplot-gui-1.5.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4678 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/tests/test_console.py
+-rw-rw-rw-   0 root         (0) root         (0)     9699 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/tests/test_dataframeeditor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/tests/test_dependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)     6446 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/tests/test_fmt_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     9887 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/tests/test_help_explorer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/tests/test_main.py
+-rw-rw-rw-   0 root         (0) root         (0)    16591 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/tests/test_plot_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)    11440 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/tests/test_preferences.py
+-rw-rw-rw-   0 root         (0) root         (0)    12461 2024-04-03 14:52:14.000000 psyplot-gui-1.5.0/tests/test_project_content.py
```

### Comparing `psyplot-gui-1.4.0/COPYING` & `psyplot-gui-1.5.0/LICENSES/LGPL-3.0-only.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,674 +1,304 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
+GNU LESSER GENERAL PUBLIC LICENSE
+Version 3, 29 June 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
 
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
+
+This version of the GNU Lesser General Public License incorporates the terms and conditions of version 3 of the GNU General Public License, supplemented by the additional permissions listed below.
+
+0. Additional Definitions.
+
+As used herein, "this License" refers to version 3 of the GNU Lesser General Public License, and the "GNU GPL" refers to version 3 of the GNU General Public License.
+
+"The Library" refers to a covered work governed by this License, other than an Application or a Combined Work as defined below.
+
+An "Application" is any work that makes use of an interface provided by the Library, but which is not otherwise based on the Library. Defining a subclass of a class defined by the Library is deemed a mode of using an interface provided by the Library.
+
+A "Combined Work" is a work produced by combining or linking an Application with the Library.  The particular version of the Library with which the Combined Work was made is also called the "Linked Version".
+
+The "Minimal Corresponding Source" for a Combined Work means the Corresponding Source for the Combined Work, excluding any source code for portions of the Combined Work that, considered in isolation, are based on the Application, and not on the Linked Version.
+
+The "Corresponding Application Code" for a Combined Work means the object code and/or source code for the Application, including any data and utility programs needed for reproducing the Combined Work from the Application, but excluding the System Libraries of the Combined Work.
+
+1. Exception to Section 3 of the GNU GPL.
+You may convey a covered work under sections 3 and 4 of this License without being bound by section 3 of the GNU GPL.
+
+2. Conveying Modified Versions.
+If you modify a copy of the Library, and, in your modifications, a facility refers to a function or data to be supplied by an Application that uses the facility (other than as an argument passed when the facility is invoked), then you may convey a copy of the modified version:
+
+     a) under this License, provided that you make a good faith effort to ensure that, in the event an Application does not supply the function or data, the facility still operates, and performs whatever part of its purpose remains meaningful, or
+
+     b) under the GNU GPL, with none of the additional permissions of this License applicable to that copy.
+
+3. Object Code Incorporating Material from Library Header Files.
+The object code form of an Application may incorporate material from a header file that is part of the Library.  You may convey such object code under terms of your choice, provided that, if the incorporated material is not limited to numerical parameters, data structure layouts and accessors, or small macros, inline functions and templates (ten or fewer lines in length), you do both of the following:
+
+     a) Give prominent notice with each copy of the object code that the Library is used in it and that the Library and its use are covered by this License.
+
+     b) Accompany the object code with a copy of the GNU GPL and this license document.
+
+4. Combined Works.
+You may convey a Combined Work under terms of your choice that, taken together, effectively do not restrict modification of the portions of the Library contained in the Combined Work and reverse engineering for debugging such modifications, if you also do each of the following:
+
+     a) Give prominent notice with each copy of the Combined Work that the Library is used in it and that the Library and its use are covered by this License.
+
+     b) Accompany the Combined Work with a copy of the GNU GPL and this license document.
+
+     c) For a Combined Work that displays copyright notices during execution, include the copyright notice for the Library among these notices, as well as a reference directing the user to the copies of the GNU GPL and this license document.
+
+     d) Do one of the following:
+
+           0) Convey the Minimal Corresponding Source under the terms of this License, and the Corresponding Application Code in a form suitable for, and under terms that permit, the user to recombine or relink the Application with a modified version of the Linked Version to produce a modified Combined Work, in the manner specified by section 6 of the GNU GPL for conveying Corresponding Source.
+
+          1) Use a suitable shared library mechanism for linking with the Library.  A suitable mechanism is one that (a) uses at run time a copy of the Library already present on the user's computer system, and (b) will operate properly with a modified version of the Library that is interface-compatible with the Linked Version.
+
+     e) Provide Installation Information, but only if you would otherwise be required to provide such information under section 6 of the GNU GPL, and only to the extent that such information is necessary to install and execute a modified version of the Combined Work produced by recombining or relinking the Application with a modified version of the Linked Version. (If you use option 4d0, the Installation Information must accompany the Minimal Corresponding Source and Corresponding Application Code. If you use option 4d1, you must provide the Installation Information in the manner specified by section 6 of the GNU GPL for conveying Corresponding Source.)
+
+5. Combined Libraries.
+You may place library facilities that are a work based on the Library side by side in a single library together with other library facilities that are not Applications and are not covered by this License, and convey such a combined library under terms of your choice, if you do both of the following:
+
+     a) Accompany the combined library with a copy of the same work based on the Library, uncombined with any other library facilities, conveyed under the terms of this License.
+
+     b) Give prominent notice with the combined library that part of it is a work based on the Library, and explaining where to find the accompanying uncombined form of the same work.
+
+6. Revised Versions of the GNU Lesser General Public License.
+The Free Software Foundation may publish revised and/or new versions of the GNU Lesser General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Library as you received it specifies that a certain numbered version of the GNU Lesser General Public License "or any later version" applies to it, you have the option of following the terms and conditions either of that published version or of any later version published by the Free Software Foundation. If the Library as you received it does not specify a version number of the GNU Lesser General Public License, you may choose any version of the GNU Lesser General Public License ever published by the Free Software Foundation.
+
+If the Library as you received it specifies that a proxy can decide whether future versions of the GNU Lesser General Public License shall
+apply, that proxy's public statement of acceptance of any version is permanent authorization for you to choose that version for the Library.
+
+GNU GENERAL PUBLIC LICENSE
+Version 3, 29 June 2007
+
+Copyright © 2007 Free Software Foundation, Inc. <http://fsf.org/>
+
+Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
+
+Preamble
+
+The GNU General Public License is a free, copyleft license for software and other kinds of works.
+
+The licenses for most software and other practical works are designed to take away your freedom to share and change the works. By contrast, the GNU General Public License is intended to guarantee your freedom to share and change all versions of a program--to make sure it remains free software for all its users. We, the Free Software Foundation, use the GNU General Public License for most of our software; it applies also to any other work released this way by its authors. You can apply it to your programs, too.
+
+When we speak of free software, we are referring to freedom, not price. Our General Public Licenses are designed to make sure that you have the freedom to distribute copies of free software (and charge for them if you wish), that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs, and that you know you can do these things.
+
+To protect your rights, we need to prevent others from denying you these rights or asking you to surrender the rights. Therefore, you have certain responsibilities if you distribute copies of the software, or if you modify it: responsibilities to respect the freedom of others.
+
+For example, if you distribute copies of such a program, whether gratis or for a fee, you must pass on to the recipients the same freedoms that you received. You must make sure that they, too, receive or can get the source code. And you must show them these terms so they know their rights.
+
+Developers that use the GNU GPL protect your rights with two steps: (1) assert copyright on the software, and (2) offer you this License giving you legal permission to copy, distribute and/or modify it.
+
+For the developers' and authors' protection, the GPL clearly explains that there is no warranty for this free software. For both users' and authors' sake, the GPL requires that modified versions be marked as changed, so that their problems will not be attributed erroneously to authors of previous versions.
+
+Some devices are designed to deny users access to install or run modified versions of the software inside them, although the manufacturer can do so. This is fundamentally incompatible with the aim of protecting users' freedom to change the software. The systematic pattern of such abuse occurs in the area of products for individuals to use, which is precisely where it is most unacceptable. Therefore, we have designed this version of the GPL to prohibit the practice for those products. If such problems arise substantially in other domains, we stand ready to extend this provision to those domains in future versions of the GPL, as needed to protect the freedom of users.
+
+Finally, every program is threatened constantly by software patents. States should not allow patents to restrict development and use of software on general-purpose computers, but in those that do, we wish to avoid the special danger that patents applied to a free program could make it effectively proprietary. To prevent this, the GPL assures that patents cannot be used to render the program non-free.
+
+The precise terms and conditions for copying, distribution and modification follow.
+
+TERMS AND CONDITIONS
+
+0. Definitions.
+
+“This License” refers to version 3 of the GNU General Public License.
+
+“Copyright” also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.
+
+“The Program” refers to any copyrightable work licensed under this License. Each licensee is addressed as “you”. “Licensees” and “recipients” may be individuals or organizations.
+
+To “modify” a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a “modified version” of the earlier work or a work “based on” the earlier work.
+
+A “covered work” means either the unmodified Program or a work based on the Program.
+
+To “propagate” a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
+
+To “convey” a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
+
+An interactive user interface displays “Appropriate Legal Notices” to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
+
+1. Source Code.
+The “source code” for a work means the preferred form of the work for making modifications to it. “Object code” means any non-source form of a work.
+
+A “Standard Interface” means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
+
+The “System Libraries” of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A “Major Component”, in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
+
+The “Corresponding Source” for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
+
+The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
+
+The Corresponding Source for a work in source code form is that same work.
+
+2. Basic Permissions.
+All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
+
+You may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
+
+3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
+
+When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
+
+4. Conveying Verbatim Copies.
+You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
+
+You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
+
+5. Conveying Modified Source Versions.
+You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
+
+     a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
+
+     b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to “keep intact all notices”.
+
+     c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
+
+     d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
+
+A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an “aggregate” if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
+
+6. Conveying Non-Source Forms.
+You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
+
+     a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
+
+     b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
+
+     c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
+
+     d) Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge. You need not require recipients to copy the Corresponding Source along with the object code. If the place to copy the object code is a network server, the Corresponding Source may be on a different server (operated by you or a third party) that supports equivalent copying facilities, provided you maintain clear directions next to the object code saying where to find the Corresponding Source. Regardless of what server hosts the Corresponding Source, you remain obligated to ensure that it is available for as long as needed to satisfy these requirements.
+
+     e) Convey the object code using peer-to-peer transmission, provided you inform other peers where the object code and Corresponding Source of the work are being offered to the general public at no charge under subsection 6d.
+
+A separable portion of the object code, whose source code is excluded from the Corresponding Source as a System Library, need not be included in conveying the object code work.
+
+A “User Product” is either (1) a “consumer product”, which means any tangible personal property which is normally used for personal, family, or household purposes, or (2) anything designed or sold for incorporation into a dwelling. In determining whether a product is a consumer product, doubtful cases shall be resolved in favor of coverage. For a particular product received by a particular user, “normally used” refers to a typical or common use of that class of product, regardless of the status of the particular user or of the way in which the particular user actually uses, or expects or is expected to use, the product. A product is a consumer product regardless of whether the product has substantial commercial, industrial or non-consumer uses, unless such uses represent the only significant mode of use of the product.
+
+“Installation Information” for a User Product means any methods, procedures, authorization keys, or other information required to install and execute modified versions of a covered work in that User Product from a modified version of its Corresponding Source. The information must suffice to ensure that the continued functioning of the modified object code is in no case prevented or interfered with solely because modification has been made.
+
+If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
+
+The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
+
+Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
+
+7. Additional Terms.
+“Additional permissions” are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
+
+When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
+
+Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
+
+     a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
+
+     b) Requiring preservation of specified reasonable legal notices or author attributions in that material or in the Appropriate Legal Notices displayed by works containing it; or
+
+     c) Prohibiting misrepresentation of the origin of that material, or requiring that modified versions of such material be marked in reasonable ways as different from the original version; or
+
+     d) Limiting the use for publicity purposes of names of licensors or authors of the material; or
+
+     e) Declining to grant rights under trademark law for use of some trade names, trademarks, or service marks; or
+
+     f) Requiring indemnification of licensors and authors of that material by anyone who conveys the material (or modified versions of it) with contractual assumptions of liability to the recipient, for any liability that these contractual assumptions directly impose on those licensors and authors.
+
+All other non-permissive additional terms are considered “further restrictions” within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
+
+Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
+
+8. Termination.
+You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
+
+However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
+
+Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
+
+9. Acceptance Not Required for Having Copies.
+You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
+
+10. Automatic Licensing of Downstream Recipients.
+Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
+
+An “entity transaction” is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
+
+You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
+
+11. Patents.
+A “contributor” is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's “contributor version”.
+
+A contributor's “essential patent claims” are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, “control” includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
+
+Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
+
+In the following three paragraphs, a “patent license” is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To “grant” such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
+
+If you convey a covered work, knowingly relying on a patent license, and the Corresponding Source of the work is not available for anyone to copy, free of charge and under the terms of this License, through a publicly available network server or other readily accessible means, then you must either (1) cause the Corresponding Source to be so available, or (2) arrange to deprive yourself of the benefit of the patent license for this particular work, or (3) arrange, in a manner consistent with the requirements of this License, to extend the patent license to downstream recipients. “Knowingly relying” means you have actual knowledge that, but for the patent license, your conveying the covered work in a country, or your recipient's use of the covered work in a country, would infringe one or more identifiable patents in that country that you have reason to believe are valid.
+
+If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
+
+A patent license is “discriminatory” if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
+
+12. No Surrender of Others' Freedom.
+If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
+
+13. Use with the GNU Affero General Public License.
+Notwithstanding any other provision of this License, you have permission to link or combine any covered work with a work licensed under version 3 of the GNU Affero General Public License into a single combined work, and to convey the resulting work. The terms of this License will continue to apply to the part which is the covered work, but the special requirements of the GNU Affero General Public License, section 13, concerning interaction through a network will apply to the combination as such.
+
+14. Revised Versions of this License.
+The Free Software Foundation may publish revised and/or new versions of the GNU General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the GNU General Public License “or any later version” applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of the GNU General Public License, you may choose any version ever published by the Free Software Foundation.
+
+If the Program specifies that a proxy can decide which future versions of the GNU General Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
+
+Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
+
+15. Disclaimer of Warranty.
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM “AS IS” WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+16. Limitation of Liability.
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
+
+17. Interpretation of Sections 15 and 16.
+If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
+
+END OF TERMS AND CONDITIONS
+
+How to Apply These Terms to Your New Programs
+
+If you develop a new program, and you want it to be of the greatest possible use to the public, the best way to achieve this is to make it free software which everyone can redistribute and change under these terms.
+
+To do so, attach the following notices to the program. It is safest to attach them to the start of each source file to most effectively state the exclusion of warranty; and each file should have at least the “copyright” line and a pointer to where the full notice is found.
+
+     <one line to give the program's name and a brief idea of what it does.>
+     Copyright (C) <year>  <name of author>
+
+     This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+
+     This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+
+     You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
+If the program does terminal interaction, make it output a short notice like this when it starts in an interactive mode:
+
+     <program>  Copyright (C) <year>  <name of author>
+     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+     This is free software, and you are welcome to redistribute it under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate parts of the General Public License. Of course, your program's commands might be different; for a GUI interface, you would use an “about box”.
+
+You should also get your employer (if you work as a programmer) or school, if any, to sign a “copyright disclaimer” for the program, if necessary. For more information on this, and how to apply and follow the GNU GPL, see <http://www.gnu.org/licenses/>.
 
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+The GNU General Public License does not permit incorporating your program into proprietary programs. If your program is a subroutine library, you may consider it more useful to permit linking proprietary applications with the library. If this is what you want to do, use the GNU Lesser General Public License instead of this License. But first, please read <http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `psyplot-gui-1.4.0/README.rst` & `psyplot-gui-1.5.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,24 @@
+.. SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 Graphical User Interface for the psyplot package
 ================================================
 
 .. start-badges
 
-.. list-table::
-    :stub-columns: 1
-    :widths: 10 90
-
-    * - docs
-      - |docs|
-    * - tests
-      - |circleci| |appveyor| |codecov|
-    * - package
-      - |version| |conda| |github| |zenodo|
-    * - implementations
-      - |supported-versions| |supported-implementations|
-
-.. |docs| image:: https://img.shields.io/github/deployments/psyplot/psyplot-gui/github-pages
-    :alt: Documentation
-    :target: http://psyplot.github.io/psyplot-gui/
-
-.. |circleci| image:: https://circleci.com/gh/psyplot/psyplot-gui/tree/master.svg?style=svg
-    :alt: CircleCI
-    :target: https://circleci.com/gh/psyplot/psyplot-gui/tree/master
-
-.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/bud4ov6lddrjvt88/branch/master?svg=true
-    :alt: AppVeyor
-    :target: https://ci.appveyor.com/project/psyplot/psyplot-gui-q726s
-
-.. |codecov| image:: https://codecov.io/gh/psyplot/psyplot-gui/branch/master/graph/badge.svg
-    :alt: Coverage
-    :target: https://codecov.io/gh/psyplot/psyplot-gui
-
-.. |version| image:: https://img.shields.io/pypi/v/psyplot-gui.svg?style=flat
-    :alt: PyPI Package latest release
-    :target: https://pypi.python.org/pypi/psyplot-gui
-
-.. |conda| image:: https://anaconda.org/conda-forge/psyplot-gui/badges/version.svg
-    :alt: conda
-    :target: https://anaconda.org/conda-forge/psyplot-gui
-
-.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/psyplot-gui.svg?style=flat
-    :alt: Supported versions
-    :target: https://pypi.python.org/pypi/psyplot-gui
-
-.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/psyplot-gui.svg?style=flat
-    :alt: Supported implementations
-    :target: https://pypi.python.org/pypi/psyplot-gui
-
-.. |zenodo| image:: https://zenodo.org/badge/55793611.svg
-    :alt: Zenodo
-    :target: https://zenodo.org/badge/latestdoi/55793611
-
-.. |github| image:: https://img.shields.io/github/release/psyplot/psyplot-gui.svg
-    :target: https://github.com/psyplot/psyplot-gui/releases/latest
-    :alt: Latest github release
+|CI|
+|Code coverage|
+|Latest Release|
+|PyPI version|
+|Code style: black|
+|Imports: isort|
+|PEP8|
+|REUSE status|
 
 
 .. end-badges
 
 Welcome! This package enhances the interactive visualization framework
 psyplot_ with a graphical user interface using PyQt_. See the homepage of the
 main project on examples on the possibilities with psyplot_.
@@ -68,25 +28,51 @@
 
 .. _PyQt: https://riverbankcomputing.com/software/pyqt/intro
 .. _psyplot: http://psyplot.github.io/
 
 
 Copyright
 ---------
-Copyright © 2021 Helmholtz-Zentrum Hereon, 2020-2021 Helmholtz-Zentrum
-Geesthacht, 2016-2021 University of Lausanne
+Copyright © 2024 Helmholtz-Zentrum Hereon, 2020-2021 Helmholtz-Zentrum
+Geesthacht, 2016-2024 University of Lausanne
+
+Code files in this repository are licensed under the
+LGPL-3.0-only, if not stated otherwise in the file.
+
+Documentation files in this repository are licensed under CC-BY-4.0, if not
+stated otherwise in the file.
 
-psyplot-gui is released under the GNU LGPL-3.O license.
-See COPYING and COPYING.LESSER in the root of the repository for full
-licensing details.
+Supplementary and configuration files in this repository are licensed
+under CC0-1.0, if not stated otherwise
+in the file.
+
+Please check the header of the individual files for more detailed
+information.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Lesser General Public License version 3.0 as
 published by the Free Software Foundation.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU LGPL-3.0 license for more details.
 
 You should have received a copy of the GNU LGPL-3.0 license
 along with this program.  If not, see https://www.gnu.org/licenses/.
+
+.. |CI| image:: https://codebase.helmholtz.cloud/psyplot/psyplot-gui/badges/master/pipeline.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psyplot-gui/-/pipelines?page=1&scope=all&ref=master
+.. |Code coverage| image:: https://codebase.helmholtz.cloud/psyplot/psyplot-gui/badges/master/coverage.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psyplot-gui/-/graphs/master/charts
+.. |Latest Release| image:: https://codebase.helmholtz.cloud/psyplot/psyplot-gui/-/badges/release.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psyplot-gui
+.. |PyPI version| image:: https://img.shields.io/pypi/v/psyplot-gui.svg
+   :target: https://pypi.python.org/pypi/psyplot-gui/
+.. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+.. |Imports: isort| image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+   :target: https://pycqa.github.io/isort/
+.. |PEP8| image:: https://img.shields.io/badge/code%20style-pep8-orange.svg
+   :target: https://www.python.org/dev/peps/pep-0008/
+.. |REUSE status| image:: https://api.reuse.software/badge/codebase.helmholtz.cloud/psyplot/psyplot-gui
+   :target: https://api.reuse.software/info/codebase.helmholtz.cloud/psyplot/psyplot-gui
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/__init__.py` & `psyplot-gui-1.5.0/psyplot_gui/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,128 +1,134 @@
-"""Core package for the psyplot graphical user interface"""
-
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import sys
+"""psyplot-gui
+
+Graphical user interface for the psyplot package
+"""
+
+from __future__ import annotations
+
+import argparse
+import atexit
+import datetime as dt
+import logging
 import os
 import os.path as osp
-import six
-import tempfile
-import yaml
+import pickle
 import socket
-import atexit
-import fasteners
+import sys
+import tempfile
 import time
-import pickle
-import datetime as dt
-import logging
-import argparse
-import xarray as xr
+from itertools import chain
+
+import fasteners
 import psyplot
+import six
+import xarray as xr
+import yaml
 from psyplot.__main__ import make_plot
-from psyplot_gui.config.rcsetup import rcParams
-import psyplot_gui.config as config
-from itertools import chain
 from psyplot.config.rcsetup import get_configdir, safe_list
 from psyplot.docstring import docstrings
+from psyplot.utils import get_default_value
 from psyplot.warning import warn
-from psyplot.compat.pycompat import map
 
+import psyplot_gui.config as config
+from psyplot_gui.config.rcsetup import rcParams
 
-from ._version import get_versions
-__version__ = get_versions()['version']
-del get_versions
-
+from . import _version
 
-from psyplot.compat.pycompat import get_default_value
+__version__ = _version.get_versions()["version"]
 
 __author__ = "Philipp S. Sommer"
-__copyright__ = """
-Copyright (C) 2021 Helmholtz-Zentrum Hereon
-Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-Copyright (C) 2016-2021 University of Lausanne
-"""
-__credits__ = ["Philipp S. Sommer"]
+__copyright__ = "2021-2024 Helmholtz-Zentrum hereon GmbH"
+__credits__ = [
+    "Philipp S. Sommer",
+]
 __license__ = "LGPL-3.0-only"
 
 __maintainer__ = "Philipp S. Sommer"
-__email__ = "psyplot@hereon.de"
+__email__ = "philipp.sommer@hereon.de"
 
 __status__ = "Production"
 
 logger = logging.getLogger(__name__)
 logger.debug(
     "%s: Initializing psyplot gui, version %s",
-    dt.datetime.now().isoformat(), __version__)
+    dt.datetime.now().isoformat(),
+    __version__,
+)
 logger.debug("psyplot version: %s", psyplot.__version__)
 logger.debug("Logging configuration file: %s", config.logcfg_path)
 logger.debug("Configuration file: %s", config.config_path)
 
 
 rcParams.HEADER += "\n\npsyplot gui version: " + __version__
 
 
 logger = logging.getLogger(__name__)
 
 
 def get_versions(requirements=True):
-    ret = {'version': __version__}
+    ret = {"version": __version__}
     if requirements:
-        req = ret['requirements'] = {}
+        req = ret["requirements"] = {}
         try:
             import qtconsole
         except Exception:
-            logger.error('Could not load qtconsole!', exc_info=True)
+            logger.error("Could not load qtconsole!", exc_info=True)
         else:
-            req['qtconsole'] = qtconsole.__version__
+            req["qtconsole"] = qtconsole.__version__
         try:
             from psyplot_gui.compat.qtcompat import PYQT_VERSION, QT_VERSION
         except Exception:
-            logger.error('Could not load qt and pyqt!', exc_info=True)
+            logger.error("Could not load qt and pyqt!", exc_info=True)
         else:
-            req['qt'] = QT_VERSION
-            req['pyqt'] = PYQT_VERSION
+            req["qt"] = QT_VERSION
+            req["pyqt"] = PYQT_VERSION
     return ret
 
 
-@docstrings.get_sections(base='psyplot_gui.start_app')
+@docstrings.get_sections(base="psyplot_gui.start_app")
 @docstrings.dedent
-def start_app(fnames=[], name=[], dims=None, plot_method=None,
-              output=None, project=None, engine=None, formatoptions=None,
-              tight=False, encoding=None, enable_post=False,
-              seaborn_style=None, output_project=None,
-              concat_dim=get_default_value(xr.open_mfdataset, 'concat_dim'),
-              chname={},
-              backend=False, new_instance=False, rc_file=None,
-              rc_gui_file=None, include_plugins=rcParams['plugins.include'],
-              exclude_plugins=rcParams['plugins.exclude'], offline=False,
-              pwd=None, script=None, command=None, exec_=True, use_all=False,
-              callback=None, preset=None,
-              opengl_implementation=None, webengineview=True):
+def start_app(
+    fnames=[],
+    name=[],
+    dims=None,
+    plot_method=None,
+    output=None,
+    project=None,
+    engine=None,
+    formatoptions=None,
+    tight=False,
+    encoding=None,
+    enable_post=False,
+    seaborn_style=None,
+    output_project=None,
+    concat_dim=get_default_value(xr.open_mfdataset, "concat_dim"),
+    chname={},
+    backend=False,
+    new_instance=False,
+    rc_file=None,
+    rc_gui_file=None,
+    include_plugins=rcParams["plugins.include"],
+    exclude_plugins=rcParams["plugins.exclude"],
+    offline=False,
+    pwd=None,
+    script=None,
+    command=None,
+    exec_=True,
+    use_all=False,
+    callback=None,
+    preset=None,
+    opengl_implementation=None,
+    webengineview=True,
+    decoder=None,
+):
     """
     Eventually start the QApplication or only make a plot
 
     Parameters
     ----------
     %(make_plot.parameters)s
     backend: None or str
@@ -182,71 +188,90 @@
     """
     if pwd is not None:
         os.chdir(pwd)
     if script is not None:
         script = osp.abspath(script)
 
     if project is not None and (name != [] or dims is not None):
-        warn('The `name` and `dims` parameter are ignored if the `project`'
-             ' parameter is set!')
+        warn(
+            "The `name` and `dims` parameter are ignored if the `project`"
+            " parameter is set!"
+        )
 
     # load rcParams from file
     if rc_gui_file is not None:
         rcParams.load_from_file(rc_gui_file)
 
     # set plugins
-    rcParams['plugins.include'] = include_plugins
-    rcParams['plugins.exclude'] = exclude_plugins
+    rcParams["plugins.include"] = include_plugins
+    rcParams["plugins.exclude"] = exclude_plugins
     if webengineview is not None:
-        rcParams['help_explorer.use_webengineview'] = webengineview
+        rcParams["help_explorer.use_webengineview"] = webengineview
 
     if offline:
-        rcParams['help_explorer.online'] = False
-        rcParams['help_explorer.use_intersphinx'] = False
+        rcParams["help_explorer.online"] = False
+        rcParams["help_explorer.use_intersphinx"] = False
 
     if dims is not None and not isinstance(dims, dict):
         dims = dict(chain(*map(six.iteritems, dims)))
 
     if output is not None:
         return make_plot(
-            fnames=fnames, name=name, dims=dims, plot_method=plot_method,
-            output=output, project=project, engine=engine,
-            formatoptions=formatoptions, tight=tight, rc_file=rc_file,
-            encoding=encoding, enable_post=enable_post,
-            seaborn_style=seaborn_style, output_project=output_project,
-            concat_dim=concat_dim, chname=chname, preset=preset)
+            fnames=fnames,
+            name=name,
+            dims=dims,
+            plot_method=plot_method,
+            output=output,
+            project=project,
+            engine=engine,
+            formatoptions=formatoptions,
+            tight=tight,
+            rc_file=rc_file,
+            encoding=encoding,
+            enable_post=enable_post,
+            seaborn_style=seaborn_style,
+            output_project=output_project,
+            concat_dim=concat_dim,
+            chname=chname,
+            preset=preset,
+            decoder=decoder,
+        )
     if use_all:
-        name = 'all'
+        name = "all"
     else:
         name = safe_list(name)
 
     if formatoptions is not None:
         if not isinstance(formatoptions, dict):
             # list of dicts
             for fmt in formatoptions[1:]:
                 formatoptions[0].update(fmt)
             formatoptions = formatoptions[0]
         if preset is not None:
             import psyplot.project as psy
+
             preset_data = psy.Project._load_preset(preset)
         else:
             preset_data = {}
         preset_data.update(formatoptions)
-        preset = tempfile.NamedTemporaryFile(prefix='psy_', suffix='.yml').name
-        with open(preset, 'w') as f:
+        preset = tempfile.NamedTemporaryFile(prefix="psy_", suffix=".yml").name
+        with open(preset, "w") as f:
             yaml.dump(preset_data, f)
 
     # make preset path absolute
-    if preset is not None and not isinstance(preset, dict) and \
-            osp.exists(preset):
+    if (
+        preset is not None
+        and not isinstance(preset, dict)
+        and osp.exists(preset)
+    ):
         preset = osp.abspath(preset)
 
     # Lock file creation
     if not new_instance:
-        lock_file = osp.join(get_configdir(), 'psyplot.lock')
+        lock_file = osp.join(get_configdir(), "psyplot.lock")
         lock = fasteners.InterProcessLock(lock_file)
 
         # Try to lock psyplot.lock. If it's *possible* to do it, then
         # there is no previous instance running and we can start a
         # new one. If *not*, then there is an instance already
         # running, which is locking that file
         lock_created = lock.acquire(False)
@@ -257,50 +282,76 @@
 
     if lock_created:
         # Start a new instance
         atexit.register(lock.release)
     elif not new_instance:
         if callback is None:
             if fnames or project:
-                callback = 'new_plot'
+                callback = "new_plot"
             elif pwd is not None:
-                callback = 'change_cwd'
+                callback = "change_cwd"
                 fnames = [pwd]
             elif script is not None:
-                callback = 'run_script'
+                callback = "run_script"
                 fnames = [script]
             elif command is not None:
-                callback = 'command'
+                callback = "command"
                 engine = command
         if callback:
             send_files_to_psyplot(
-                callback, fnames, project, engine, plot_method, name, dims,
-                encoding, enable_post, seaborn_style, concat_dim, chname,
-                preset)
+                callback,
+                fnames,
+                project,
+                engine,
+                plot_method,
+                name,
+                dims,
+                encoding,
+                enable_post,
+                seaborn_style,
+                concat_dim,
+                chname,
+                preset,
+                decoder,
+            )
         return
     elif new_instance:
-        rcParams['main.listen_to_port'] = False
+        rcParams["main.listen_to_port"] = False
     if backend is not False:
-        rcParams['backend'] = backend
+        rcParams["backend"] = backend
     from psyplot_gui.main import MainWindow
+
     fnames = _get_abs_names(fnames)
     if project is not None:
         project = _get_abs_names([project])[0]
     if exec_:
         from psyplot_gui.compat.qtcompat import QApplication
+
         app = QApplication(sys.argv)
 
     _set_opengl_implementation(opengl_implementation)
 
     if isinstance(new_instance, MainWindow):
         mainwindow = new_instance
     else:
-        mainwindow = MainWindow.run(fnames, project, engine, plot_method, name,
-                                    dims, encoding, enable_post, seaborn_style,
-                                    concat_dim, chname, preset)
+        mainwindow = MainWindow.run(
+            fnames,
+            project,
+            engine,
+            plot_method,
+            name,
+            dims,
+            encoding,
+            enable_post,
+            seaborn_style,
+            concat_dim,
+            chname,
+            preset,
+            decoder,
+        )
     if script is not None:
         mainwindow.console.run_script_in_shell(script)
     if command is not None:
         mainwindow.console.run_command_in_shell(command)
     if exec_:
         sys.excepthook = mainwindow.excepthook
         sys.exit(app.exec_())
@@ -311,25 +362,26 @@
 def send_files_to_psyplot(callback, fnames, project, *args):
     """
     Simple socket client used to send the args passed to the psyplot
     executable to an already running instance.
 
     This function has to most parts been taken from spyder
     """
-    port = rcParams['main.open_files_port']
+    port = rcParams["main.open_files_port"]
 
     # Wait ~50 secs for the server to be up
     # Taken from http://stackoverflow.com/a/4766598/438386
     for _x in range(200):
         fnames = _get_abs_names(fnames)
         if project is not None:
             project = _get_abs_names([project])[0]
         try:
-            client = socket.socket(socket.AF_INET, socket.SOCK_STREAM,
-                                   socket.IPPROTO_TCP)
+            client = socket.socket(
+                socket.AF_INET, socket.SOCK_STREAM, socket.IPPROTO_TCP
+            )
             client.connect(("127.0.0.1", port))
             client.send(pickle.dumps([callback, fnames, project] + list(args)))
             client.close()
         except socket.error:
             time.sleep(0.25)
             continue
         break
@@ -337,15 +389,15 @@
 
 def _get_abs_names(fnames):
     """Return the absolute paths of the given filenames"""
     if fnames is None:
         return
     for i, fname in enumerate(fnames):
         if fname:
-            fnames[i] = ','.join(map(osp.abspath, fname.split(',')))
+            fnames[i] = ",".join(map(osp.abspath, fname.split(",")))
     return fnames
 
 
 def get_parser(create=True):
     """Return a parser to make that can be used to make plots or open files
     from the command line
 
@@ -356,82 +408,111 @@
 
     See Also
     --------
     psyplot.main.get_parser
     psyplot.parser.FuncArgParser
     psyplot.main.main"""
     from psyplot.__main__ import get_parser
+
     parser = get_parser(create=False)
 
     parser.setup_args(start_app)
 
     gui_grp = parser.add_argument_group(
-        'Gui options',
-        'Options specific to the graphical user interface')
+        "Gui options", "Options specific to the graphical user interface"
+    )
 
     parser.update_arg(
-        'backend', short='b', const=None, nargs='?', metavar='backend',
+        "backend",
+        short="b",
+        const=None,
+        nargs="?",
+        metavar="backend",
         help="""
         The backend to use. By default, the ``'gui.backend'`` key in the
         :attr:`~psyplot_gui.config.rcsetup.rcParams` dictionary is used. If
         used without options, the default matplotlib backend is used.""",
-        group=gui_grp)
+        group=gui_grp,
+    )
 
-    parser.update_arg('new_instance', short='ni', group=gui_grp)
+    parser.update_arg("new_instance", short="ni", group=gui_grp)
 
-    parser.update_arg('rc_gui_file', short='rc-gui', group=gui_grp)
-    parser.pop_key('rc_gui_file', 'metavar')
-    parser.update_arg('include_plugins', short='inc', group=gui_grp,
-                      default=rcParams['plugins.include'])
-    parser.append2help('include_plugins', '. Default: %(default)s')
-    parser.update_arg('exclude_plugins', short='exc', group=gui_grp,
-                      default=rcParams['plugins.exclude'])
-    parser.append2help('exclude_plugins', '. Default: %(default)s')
-
-    parser.update_arg('offline', group=gui_grp)
-    parser.update_arg('pwd', group=gui_grp)
-    parser.update_arg('script', short='s', group=gui_grp)
-    parser.update_arg('command', short='c', group=gui_grp)
+    parser.update_arg("rc_gui_file", short="rc-gui", group=gui_grp)
+    parser.pop_key("rc_gui_file", "metavar")
+    parser.update_arg(
+        "include_plugins",
+        short="inc",
+        group=gui_grp,
+        default=rcParams["plugins.include"],
+    )
+    parser.append2help("include_plugins", ". Default: %(default)s")
+    parser.update_arg(
+        "exclude_plugins",
+        short="exc",
+        group=gui_grp,
+        default=rcParams["plugins.exclude"],
+    )
+    parser.append2help("exclude_plugins", ". Default: %(default)s")
+
+    parser.update_arg("offline", group=gui_grp)
+    parser.update_arg("pwd", group=gui_grp)
+    parser.update_arg("script", short="s", group=gui_grp)
+    parser.update_arg("command", short="c", group=gui_grp)
 
-    parser.update_arg('opengl_implementation', group=gui_grp, short='opengl',
-                      choices=['software', 'desktop', 'gles', 'automatic'])
+    parser.update_arg(
+        "opengl_implementation",
+        group=gui_grp,
+        short="opengl",
+        choices=["software", "desktop", "gles", "automatic"],
+    )
 
     # add an action to display the GUI plugins
-    info_grp = parser.unfinished_arguments['list_plugins'].get('group')
+    info_grp = parser.unfinished_arguments["list_plugins"].get("group")
     parser.update_arg(
-        'list_gui_plugins', short='lgp', long='list-gui-plugins',
-        action=ListGuiPluginsAction, if_existent=False,
-        help=("Print the names of the GUI plugins and exit. Note that the "
-              "displayed plugins are not affected by the `include-plugins` "
-              "and `exclude-plugins` options"))
+        "list_gui_plugins",
+        short="lgp",
+        long="list-gui-plugins",
+        action=ListGuiPluginsAction,
+        if_existent=False,
+        help=(
+            "Print the names of the GUI plugins and exit. Note that the "
+            "displayed plugins are not affected by the `include-plugins` "
+            "and `exclude-plugins` options"
+        ),
+    )
     if info_grp is not None:
-        parser.unfinished_arguments['list_gui_plugins']['group'] = info_grp
+        parser.unfinished_arguments["list_gui_plugins"]["group"] = info_grp
 
-    parser.pop_key('offline', 'short')
+    parser.pop_key("offline", "short")
 
-    parser.append2help('output_project',
-                       '. This option has only an effect if the `output` '
-                       ' option is set.')
+    parser.append2help(
+        "output_project",
+        ". This option has only an effect if the `output` " " option is set.",
+    )
 
-    parser.update_arg('use_all', short='a')
+    parser.update_arg("use_all", short="a")
 
-    parser.pop_arg('exec_')
-    parser.pop_arg('callback')
+    parser.pop_arg("exec_")
+    parser.pop_arg("callback")
 
-    parser.pop_key('webengineview', 'short')
-    parser.update_arg('webengineview', default=None, action='store_true',
-                      group=gui_grp)
+    parser.pop_key("webengineview", "short")
+    parser.update_arg(
+        "webengineview", default=None, action="store_true", group=gui_grp
+    )
 
-    parser.unfinished_arguments['no-webengineview'] = dict(
-        long='no-webengineview', default=None, action='store_false',
-        dest='webengineview',
+    parser.unfinished_arguments["no-webengineview"] = dict(
+        long="no-webengineview",
+        default=None,
+        action="store_false",
+        dest="webengineview",
         help="Do not use HTML rendering.",
-        group=gui_grp)
+        group=gui_grp,
+    )
 
-    if psyplot.__version__ < '1.0':
+    if psyplot.__version__ < "1.0":
         parser.set_main(start_app)
 
     parser.epilog += """
 
 If you omit the ``'-o'`` option, the file is opened in the graphical user
 interface and if you run::
 
@@ -453,30 +534,36 @@
         parser.create_arguments()
 
     return parser
 
 
 #: A boolean variable to check if the GUI is tested. This is set automatically
 #: true on CI services
-UNIT_TESTING = os.getenv('CI')
+UNIT_TESTING = os.getenv("CI")
 
 
 class ListGuiPluginsAction(argparse.Action):
-
-    def __init__(self, option_strings, dest=argparse.SUPPRESS, nargs=None,
-                 default=argparse.SUPPRESS, **kwargs):
+    def __init__(
+        self,
+        option_strings,
+        dest=argparse.SUPPRESS,
+        nargs=None,
+        default=argparse.SUPPRESS,
+        **kwargs,
+    ):
         if nargs is not None:
             raise ValueError("nargs not allowed")
-        kwargs['default'] = default
+        kwargs["default"] = default
         super(ListGuiPluginsAction, self).__init__(
-            option_strings, nargs=0, dest=dest,
-            **kwargs)
+            option_strings, nargs=0, dest=dest, **kwargs
+        )
 
     def __call__(self, parser, namespace, values, option_string=None):
         import yaml
+
         if not rcParams._plugins:
             list(rcParams._load_plugin_entrypoints())
         print(yaml.dump(rcParams._plugins, default_flow_style=False))
         sys.exit(0)
 
 
 def _set_opengl_implementation(option):
@@ -489,21 +576,22 @@
     See issue https://github.com/spyder-ide/spyder/issues/7447 for the details.
     """
     try:
         from PyQt5.QtQuick import QQuickWindow, QSGRendererInterface
     except Exception:
         QQuickWindow = QSGRendererInterface = None
     from PyQt5.QtCore import QCoreApplication, Qt
+
     if option is None:
-        option = rcParams['main.opengl']
-    if option == 'software':
+        option = rcParams["main.opengl"]
+    if option == "software":
         QCoreApplication.setAttribute(Qt.AA_UseSoftwareOpenGL)
         if QQuickWindow is not None:
             QQuickWindow.setSceneGraphBackend(QSGRendererInterface.Software)
-    elif option == 'desktop':
+    elif option == "desktop":
         QCoreApplication.setAttribute(Qt.AA_UseDesktopOpenGL)
         if QQuickWindow is not None:
             QQuickWindow.setSceneGraphBackend(QSGRendererInterface.OpenGL)
-    elif option == 'gles':
+    elif option == "gles":
         QCoreApplication.setAttribute(Qt.AA_UseOpenGLES)
         if QQuickWindow is not None:
             QQuickWindow.setSceneGraphBackend(QSGRendererInterface.OpenGL)
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/backend.py` & `psyplot-gui-1.5.0/psyplot_gui/backend.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 """Matplotlib backend to include matplotlib figures as dockwidgets in the
 psyplot gui
 
 This backend is based upon matplotlibs qt4agg and qt5agg backends."""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-from psyplot_gui.compat.qtcompat import (
-    QDockWidget, Qt, QWidget, QVBoxLayout, with_qt5)
-from psyplot_gui.common import DockMixin
 from matplotlib.backend_bases import FigureManagerBase
 from matplotlib.figure import Figure
+
+from psyplot_gui.common import DockMixin
+from psyplot_gui.compat.qtcompat import (
+    QDockWidget,
+    Qt,
+    QVBoxLayout,
+    QWidget,
+    with_qt5,
+)
+
 if with_qt5:
     from matplotlib.backends.backend_qt5agg import (
-        show, FigureManagerQT, FigureCanvasQTAgg)
+        FigureCanvasQTAgg,
+        FigureManagerQT,
+    )
 else:
     from matplotlib.backends.backend_qt4agg import (
-        show, FigureManagerQT, FigureCanvasQTAgg)
+        FigureCanvasQTAgg,
+        FigureManagerQT,
+    )
 
 
 class FiguresDock(QDockWidget):
-    """Reimplemented QDockWidget to remove the dock widget when closed
-    """
+    """Reimplemented QDockWidget to remove the dock widget when closed"""
 
     def close(self, *args, **kwargs):
         """
         Reimplemented to remove the dock widget from the mainwindow when closed
         """
         from psyplot_gui.main import mainwindow
+
         try:
             mainwindow.figures.remove(self)
         except Exception:
             pass
         try:
             mainwindow.removeDockWidget(self)
         except Exception:
@@ -65,15 +59,15 @@
     dock_cls = FiguresDock
 
 
 def new_figure_manager(num, *args, **kwargs):
     """
     Create a new figure manager instance
     """
-    FigureClass = kwargs.pop('FigureClass', Figure)
+    FigureClass = kwargs.pop("FigureClass", Figure)
     thisFig = FigureClass(*args, **kwargs)
     return new_figure_manager_given_figure(num, thisFig)
 
 
 def new_figure_manager_given_figure(num, figure):
     """
     Create a new figure manager instance for the given figure.
@@ -86,31 +80,37 @@
     """The canvas manager for the psyplot backend interacting with the
     mainwindow of the psyplot gui"""
 
     toolbar = None
 
     def __init__(self, canvas, num):
         from psyplot_gui.main import mainwindow
+
         self.main = mainwindow
         if mainwindow is None:
             return super(PsyplotCanvasManager, self).__init__(canvas, num)
         parent_widget = FigureWidget()
         parent_widget.vbox = vbox = QVBoxLayout()
         self.window = dock = parent_widget.to_dock(
-            mainwindow, title="Figure %d" % num, position=Qt.TopDockWidgetArea,
-            docktype=None)
+            mainwindow,
+            title="Figure %d" % num,
+            position=Qt.TopDockWidgetArea,
+            docktype=None,
+        )
         if mainwindow.figures:
             mainwindow.tabifyDockWidget(mainwindow.figures[-1], dock)
         mainwindow.figures.append(dock)
         FigureManagerBase.__init__(self, canvas, num)
         self.canvas = canvas
 
         self.window.setWindowTitle("Figure %d" % num)
 
-        self.toolbar = self._get_toolbar(canvas, parent_widget)
+        if hasattr(self, "_get_toolbar"):
+            # legacy solution for matplotlib < 3.6
+            self.toolbar = self._get_toolbar(canvas, parent_widget)
 
         # add text label to status bar
         self.statusbar_label = mainwindow.figures_label
 
         if self.toolbar is not None:
             vbox.addWidget(self.toolbar)
             self.toolbar.message.connect(self.statusbar_label.setText)
@@ -132,14 +132,15 @@
 
         self.main.show()
 
         def notify_axes_change(fig):
             # This will be called whenever the current axes is changed
             if self.toolbar is not None:
                 self.toolbar.update()
+
         self.canvas.figure.add_axobserver(notify_axes_change)
 
     def statusBar(self, *args, **kwargs):
         if self.main is None:
             return super(PsyplotCanvasManager, self).statusBar(*args, **kwargs)
         return self.main.statusBar(*args, **kwargs)
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/common.py` & `psyplot-gui-1.5.0/psyplot_gui/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 """Common functions used for the psyplot gui"""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import sys
-import six
 import inspect
+import logging
+import os.path as osp
+import sys
 import traceback as tb
 from functools import partial
-import os.path as osp
+
+import six
+
 from psyplot_gui.compat.qtcompat import (
-    QDockWidget, QRegExpValidator, QtCore, QErrorMessage, QDesktopWidget,
-    QToolButton, QInputDialog, QIcon, QAction)
-import logging
+    QAction,
+    QDesktopWidget,
+    QDockWidget,
+    QErrorMessage,
+    QIcon,
+    QInputDialog,
+    QRegExpValidator,
+    QtCore,
+    QToolButton,
+)
 
 if six.PY2:
     try:
         import CStringIO as io
     except ImportError:
         import StringIO as io
 else:
@@ -44,26 +37,27 @@
 
 
 def is_running_tests():
     """Check if there are any GUI tests running
 
     This function returns the :attr:`psyplot_gui.UNIT_TESTING` variable"""
     import psyplot_gui
+
     return psyplot_gui.UNIT_TESTING
 
 
 def get_module_path(modname):
     """Return module `modname` base path"""
 
     return osp.abspath(osp.dirname(sys.modules[modname].__file__))
 
 
 def get_icon(name):
     """Get the path to an icon in the icons directory"""
-    return osp.join(get_module_path('psyplot_gui'), 'icons', name)
+    return osp.join(get_module_path("psyplot_gui"), "icons", name)
 
 
 class DockMixin(object):
     """A mixin class to define psyplot_gui plugins
 
     Notes
     -----
@@ -92,29 +86,31 @@
 
     #: The instance of :class:`QDockWidget` of this plugin
     dock = None
 
     @property
     def is_shown(self):
         """Boolean that is True, if the dock widget is shown"""
-        return (self.dock is not None and
-                self.dock.toggleViewAction().isChecked())
-
-    def to_dock(self, main, title=None, position=None, docktype='pane', *args,
-                **kwargs):
+        return (
+            self.dock is not None and self.dock.toggleViewAction().isChecked()
+        )
+
+    def to_dock(
+        self, main, title=None, position=None, docktype="pane", *args, **kwargs
+    ):
         if title is None:
             title = self.title
         if title is None:
-            raise ValueError(
-                "No title specified for the %s widget" % (self))
+            raise ValueError("No title specified for the %s widget" % (self))
         if position is None:
             position = self.dock_position
         if position is None:
-            raise ValueError("No position specified for the %s widget (%s)" % (
-                title, self))
+            raise ValueError(
+                "No position specified for the %s widget (%s)" % (title, self)
+            )
         self.title = title
         self.dock_position = position
         if self.dock is None:
             self.dock = self.dock_cls(title, main)
             self.dock.setWidget(self)
             main.dockwidgets.append(self.dock)
             self.create_central_widget_action(main)
@@ -133,15 +129,14 @@
 
         Parameters
         ----------
         main: psyplot_gui.main.Mainwindow
             The main window where the dock is added"""
         main.addDockWidget(self.dock_position, self.dock, *args, **kwargs)
 
-
     def show_plugin(self):
         """Show the plugin widget"""
         a = self.dock.toggleViewAction()
         if not a.isChecked():
             a.trigger()
 
     def hide_plugin(self):
@@ -165,37 +160,40 @@
             self._set_central_action = action = QAction(self.title, main)
             action.setCheckable(True)
             action.triggered.connect(partial(main.set_central_widget, self))
             menu.addAction(action)
             group.addAction(action)
         return self._set_central_action
 
-    def create_view_action(self, main, docktype='pane'):
+    def create_view_action(self, main, docktype="pane"):
         if self._view_action is None:
             self._view_action = action = self.dock.toggleViewAction()
-            if docktype == 'pane':
+            if docktype == "pane":
                 main.panes_menu.addAction(action)
-            elif docktype == 'df':
+            elif docktype == "df":
                 main.dataframe_menu.addAction(action)
         return self._view_action
 
     def remove_plugin(self):
         """Remove this plugin and close it"""
         mainwindow = self.dock.parent() if self.dock else self.parent()
-        key = next((key for key, w in mainwindow.plugins.items()
-                    if w is self), None)
+        key = next(
+            (key for key, w in mainwindow.plugins.items() if w is self), None
+        )
         if mainwindow.centralWidget() is self:
             mainwindow.set_central_widget(
-                mainwindow.__class__.central_widget_key)
+                mainwindow.__class__.central_widget_key
+            )
         if self._view_action is not None:
             mainwindow.panes_menu.removeAction(self._view_action)
             mainwindow.dataframe_menu.removeAction(self._view_action)
         if self._set_central_action is not None:
             mainwindow.central_widgets_menu.removeAction(
-                self._set_central_action)
+                self._set_central_action
+            )
         if key is not None:
             del mainwindow.plugins[key]
         if self.dock is not None:
             mainwindow.removeDockWidget(self.dock)
             self.dock.close()
         self.close()
 
@@ -205,146 +203,160 @@
 
     #: The signal that is emitted when an object has been loaded. The first
     #: argument is the object name, the second the object itself
     object_loaded = QtCore.pyqtSignal(str, object)
 
     @property
     def instances2check_str(self):
-        return ', '.join('%s.%s' % (cls.__module__, cls.__name__)
-                         for cls in self._instances2check)
+        return ", ".join(
+            "%s.%s" % (cls.__module__, cls.__name__)
+            for cls in self._instances2check
+        )
 
     @property
     def potential_object_names(self):
         from ipykernel.inprocess.ipkernel import InProcessInteractiveShell
+
         shell = InProcessInteractiveShell.instance()
-        return sorted(name for name, obj in shell.user_global_ns.items()
-                      if not name.startswith('_') and self.check(obj))
+        return sorted(
+            name
+            for name, obj in shell.user_global_ns.items()
+            if not name.startswith("_") and self.check(obj)
+        )
 
     def __init__(self, instances=None, *args, **kwargs):
         """
         Parameters
         ----------
         instances: class or tuple of classes
             The classes that should be used for an instance check
         """
         super(LoadFromConsoleButton, self).__init__(*args, **kwargs)
-        self.setIcon(QIcon(get_icon('console-go.png')))
+        self.setIcon(QIcon(get_icon("console-go.png")))
         if instances is not None and inspect.isclass(instances):
-            instances = (instances, )
+            instances = (instances,)
         self._instances2check = instances
         self.error_msg = PyErrorMessage(self)
         self.clicked.connect(partial(self.get_from_shell, None))
 
     def check(self, obj):
-        return True if not self._instances2check else isinstance(
-            obj, self._instances2check)
+        return (
+            True
+            if not self._instances2check
+            else isinstance(obj, self._instances2check)
+        )
 
     def get_from_shell(self, oname=None):
         """Open an input dialog, receive an object and emit the
         :attr:`object_loaded` signal"""
         if oname is None:
             oname, ok = QInputDialog.getItem(
-                self, 'Select variable',
-                'Select a variable to import from the console',
-                self.potential_object_names)
+                self,
+                "Select variable",
+                "Select a variable to import from the console",
+                self.potential_object_names,
+            )
             if not ok:
                 return
-        if self.check(oname) and (self._instances2check or
-                                  not isinstance(oname, six.string_types)):
+        if self.check(oname) and (
+            self._instances2check or not isinstance(oname, six.string_types)
+        ):
             obj = oname
-            oname = 'object'
+            oname = "object"
         else:
             found, obj = self.get_obj(oname.strip())
             if found:
                 if not self.check(obj):
                     self.error_msg.showMessage(
-                        'Object must be an instance of %r, not %r' % (
+                        "Object must be an instance of %r, not %r"
+                        % (
                             self.instances2check_str,
-                            '%s.%s' % (type(obj).__module__,
-                                       type(obj).__name__)))
+                            "%s.%s"
+                            % (type(obj).__module__, type(obj).__name__),
+                        )
+                    )
                     return
             else:
                 if not oname.strip():
-                    msg = 'The variable name must not be empty!'
+                    msg = "The variable name must not be empty!"
                 else:
-                    msg = 'Could not find object ' + oname
+                    msg = "Could not find object " + oname
                 self.error_msg.showMessage(msg)
                 return
         self.object_loaded.emit(oname, obj)
 
     def get_obj(self, oname):
         """Load an object from the current shell"""
         from psyplot_gui.main import mainwindow
+
         return mainwindow.console.get_obj(oname)
 
 
 class ListValidator(QRegExpValidator):
     """A validator class to validate that a string consists of strings in a
     list of strings"""
 
-    def __init__(self, valid, sep=',', *args, **kwargs):
+    def __init__(self, valid, sep=",", *args, **kwargs):
         """
         Parameters
         ----------
         valid: list of str
             The possible choices
         sep: str, optional
             The separation pattern
         ``*args,**kwargs``
             Determined by PyQt5.QtGui.QValidator
         """
-        patt = QtCore.QRegExp('^((%s)(;;)?)+$' % '|'.join(valid))
+        patt = QtCore.QRegExp("^((%s)(;;)?)+$" % "|".join(valid))
         super(QRegExpValidator, self).__init__(patt, *args, **kwargs)
 
 
 class PyErrorMessage(QErrorMessage):
     """Widget designed to display python errors via the :meth:`showTraceback`
     method"""
 
     def showTraceback(self, header=None):
-
         if is_running_tests():
             raise
 
         s = io.StringIO()
         tb.print_exc(file=s)
-        last_tb = '<p>' + '<br>'.join(s.getvalue().splitlines()) + \
-            '</p>'
-        header = header + '\n' if header else ''
+        last_tb = "<p>" + "<br>".join(s.getvalue().splitlines()) + "</p>"
+        header = header + "\n" if header else ""
         self.showMessage(header + last_tb)
-        available_width = QDesktopWidget().availableGeometry().width() / 3.
-        available_height = QDesktopWidget().availableGeometry().height() / 3.
+        available_width = QDesktopWidget().availableGeometry().width() / 3.0
+        available_height = QDesktopWidget().availableGeometry().height() / 3.0
         width = self.sizeHint().width()
         height = self.sizeHint().height()
         # The message window should cover at least one third of the screen
         self.resize(max(available_width, width), max(available_height, height))
 
     def excepthook(self, type, value, traceback):
         s = io.StringIO()
         tb.print_exception(type, value, traceback, file=s)
-        last_tb = '<p>' + '<br>'.join(s.getvalue().splitlines()) + \
-            '</p>'
+        last_tb = "<p>" + "<br>".join(s.getvalue().splitlines()) + "</p>"
         header = value.message if six.PY2 else str(value)
-        self.showMessage(header + '\n' + last_tb)
-        available_width = QDesktopWidget().availableGeometry().width() / 3.
-        available_height = QDesktopWidget().availableGeometry().height() / 3.
+        self.showMessage(header + "\n" + last_tb)
+        available_width = QDesktopWidget().availableGeometry().width() / 3.0
+        available_height = QDesktopWidget().availableGeometry().height() / 3.0
         width = self.sizeHint().width()
         height = self.sizeHint().height()
         # The message window should cover at least one third of the screen
         self.resize(max(available_width, width), max(available_height, height))
 
 
 class StreamToLogger(object):
     """
     Fake file-like stream object that redirects writes to a logger instance.
     """
+
     def __init__(self, logger, log_level=logging.INFO):
         self.logger = logger
         self.log_level = log_level
-        self.linebuf = ''
+        self.linebuf = ""
 
     def write(self, buf):
         for line in buf.rstrip().splitlines():
             self.logger.log(self.log_level, line.rstrip())
 
     def flush(self):
         pass
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/compat/qtcompat.py` & `psyplot-gui-1.5.0/psyplot_gui/compat/qtcompat.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,120 @@
 """Compatibility module for the different versions of PyQt"""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
+
+import sys
 
 # make sure that the right pyqt version suitable for the IPython console is
 # loaded
 import six
-import sys
+
 from psyplot_gui.config.rcsetup import rcParams
 
 try:
-    from qtconsole.rich_jupyter_widget import RichJupyterWidget
+    from qtconsole.rich_jupyter_widget import RichJupyterWidget  # noqa: F401
 except ImportError:
     pass
 try:
-    import PyQt5
+    import PyQt5  # noqa: F401
 except ImportError:
-    from PyQt4.QtGui import (
-        QMainWindow, QDockWidget, QToolBox, QApplication, QListWidget,
-        QListWidgetItem, QHBoxLayout, QVBoxLayout, QAbstractItemView,
-        QWidget, QPushButton, QFrame, QSplitter, QTreeWidget, QTreeWidgetItem,
-        QSizePolicy, QLabel, QLineEdit, QIcon, QToolButton,
-        QComboBox as OrigQComboBox,
-        QKeyEvent, QSortFilterProxyModel, QStandardItem, QStandardItemModel,
-        QCompleter, QStatusBar, QPlainTextEdit, QTextEdit, QToolBar, QMenu,
-        QAction, QTextCursor, QMessageBox, QCheckBox, QFileDialog,
-        QListView, QDesktopWidget, QValidator, QStyledItemDelegate,
-        QTableWidget, QTableWidgetItem, QRegExpValidator, QGridLayout,
-        QIntValidator, QErrorMessage, QInputDialog, QTabWidget,
-        QDoubleValidator, QGraphicsScene, QGraphicsRectItem, QGraphicsView,
-        QKeySequence, QStyleOptionViewItem, QDialog, QDialogButtonBox,
-        QStackedWidget, QScrollArea, QTableView, QHeaderView, QActionGroup)
-    from PyQt4 import QtCore
-    from PyQt4.QtCore import Qt
-    from PyQt4.QtWebKit import QWebView as QWebEngineView
-    from PyQt4.QtTest import QTest
-    from PyQt4 import QtGui
-    from PyQt4.Qt import PYQT_VERSION_STR as PYQT_VERSION
-    from PyQt4.Qt import QT_VERSION_STR as QT_VERSION
+    from PyQt4 import QtCore, QtGui  # noqa: F401
+    from PyQt4.Qt import PYQT_VERSION_STR as PYQT_VERSION  # noqa: F401
+    from PyQt4.Qt import QT_VERSION_STR as QT_VERSION  # noqa: F401
+    from PyQt4.QtCore import Qt  # noqa: F401
+    from PyQt4.QtGui import (  # noqa: F401
+        QAbstractItemView,
+        QAction,
+        QActionGroup,
+        QApplication,
+        QCheckBox,
+    )
+    from PyQt4.QtGui import QComboBox as OrigQComboBox
+    from PyQt4.QtGui import (  # noqa: F401
+        QCompleter,
+        QDesktopWidget,
+        QDialog,
+        QDialogButtonBox,
+        QDockWidget,
+        QDoubleValidator,
+        QErrorMessage,
+        QFileDialog,
+        QFrame,
+        QGraphicsRectItem,
+        QGraphicsScene,
+        QGraphicsView,
+        QGridLayout,
+        QHBoxLayout,
+        QHeaderView,
+        QIcon,
+        QInputDialog,
+        QIntValidator,
+        QKeyEvent,
+        QKeySequence,
+        QLabel,
+        QLineEdit,
+        QListView,
+        QListWidget,
+        QListWidgetItem,
+        QMainWindow,
+        QMenu,
+        QMessageBox,
+        QPlainTextEdit,
+        QPushButton,
+        QRegExpValidator,
+        QScrollArea,
+        QSizePolicy,
+        QSortFilterProxyModel,
+        QSplitter,
+        QStackedWidget,
+        QStandardItem,
+        QStandardItemModel,
+        QStatusBar,
+        QStyledItemDelegate,
+        QStyleOptionViewItem,
+        QTableView,
+        QTableWidget,
+        QTableWidgetItem,
+        QTabWidget,
+        QTextCursor,
+        QTextEdit,
+        QToolBar,
+        QToolBox,
+        QToolButton,
+        QTreeWidget,
+        QTreeWidgetItem,
+        QValidator,
+        QVBoxLayout,
+        QWidget,
+    )
+    from PyQt4.QtTest import QTest  # noqa: F401
+    from PyQt4.QtWebKit import QWebView as QWebEngineView  # noqa: F401
+
     with_qt5 = False
     QSignalSpy = None
 
     try:
-        from PyQt4.QtCore import QString, QByteArray
+        from PyQt4.QtCore import QByteArray, QString
     except ImportError:
+
         def isstring(s):
             return isinstance(s, six.string_types)
+
     else:
+
         def isstring(s):
             return isinstance(
-                s, tuple(list(six.string_types) + [QString, QByteArray]))
+                s, tuple(list(six.string_types) + [QString, QByteArray])
+            )
 
     class QComboBox(OrigQComboBox):
-
         currentTextChanged = QtCore.pyqtSignal(str)
 
         def __init__(self, *args, **kwargs):
             OrigQComboBox.__init__(self, *args, **kwargs)
             self.currentIndexChanged.connect(self._emit_currentTextChanged)
 
         def _emit_currentTextChanged(self, i):
@@ -86,64 +124,119 @@
             idx = self.findText(s)
             if idx == -1:
                 self.addItem(s)
                 idx = self.findText(s)
             self.setCurrentIndex(idx)
 
 else:
-    from PyQt5.QtWidgets import (
-        QMainWindow, QDockWidget, QToolBox, QApplication, QListWidget,
-        QListWidgetItem, QHBoxLayout, QVBoxLayout, QAbstractItemView,
-        QWidget, QPushButton, QFrame, QSplitter, QTreeWidget, QTreeWidgetItem,
-        QSizePolicy, QLabel, QLineEdit, QToolButton, QComboBox, QCompleter,
-        QStatusBar, QPlainTextEdit, QTextEdit, QToolBar, QMenu,
-        QAction, QMessageBox, QCheckBox, QFileDialog, QListView,
-        QDesktopWidget, QStyledItemDelegate, QTableWidget, QTableWidgetItem,
-        QGridLayout, QErrorMessage, QInputDialog, QTabWidget,
-        QGraphicsScene, QGraphicsRectItem, QGraphicsView, QStyleOptionViewItem,
-        QDialog, QDialogButtonBox, QStackedWidget, QScrollArea,
-        QTableView, QHeaderView, QActionGroup)
-    from PyQt5.QtGui import (
-        QIcon, QKeyEvent, QStandardItem, QStandardItemModel, QTextCursor,
-        QValidator, QRegExpValidator, QIntValidator, QDoubleValidator,
-        QKeySequence)
     from PyQt5 import QtCore
-    from PyQt5.QtCore import Qt, QSortFilterProxyModel
-    if rcParams['help_explorer.use_webengineview']:
+    from PyQt5.QtCore import QSortFilterProxyModel, Qt  # noqa: F401
+    from PyQt5.QtGui import (  # noqa: F401
+        QDoubleValidator,
+        QIcon,
+        QIntValidator,
+        QKeyEvent,
+        QKeySequence,
+        QRegExpValidator,
+        QStandardItem,
+        QStandardItemModel,
+        QTextCursor,
+        QValidator,
+    )
+    from PyQt5.QtWidgets import (  # noqa: F401
+        QAbstractItemView,
+        QAction,
+        QActionGroup,
+        QApplication,
+        QCheckBox,
+        QComboBox,
+        QCompleter,
+        QDesktopWidget,
+        QDialog,
+        QDialogButtonBox,
+        QDockWidget,
+        QErrorMessage,
+        QFileDialog,
+        QFrame,
+        QGraphicsRectItem,
+        QGraphicsScene,
+        QGraphicsView,
+        QGridLayout,
+        QHBoxLayout,
+        QHeaderView,
+        QInputDialog,
+        QLabel,
+        QLineEdit,
+        QListView,
+        QListWidget,
+        QListWidgetItem,
+        QMainWindow,
+        QMenu,
+        QMessageBox,
+        QPlainTextEdit,
+        QPushButton,
+        QScrollArea,
+        QSizePolicy,
+        QSplitter,
+        QStackedWidget,
+        QStatusBar,
+        QStyledItemDelegate,
+        QStyleOptionViewItem,
+        QTableView,
+        QTableWidget,
+        QTableWidgetItem,
+        QTabWidget,
+        QTextEdit,
+        QToolBar,
+        QToolBox,
+        QToolButton,
+        QTreeWidget,
+        QTreeWidgetItem,
+        QVBoxLayout,
+        QWidget,
+    )
+
+    if rcParams["help_explorer.use_webengineview"]:
         try:
-            from PyQt5.QtWebEngineWidgets import QWebEngineView
+            from PyQt5.QtWebEngineWidgets import QWebEngineView  # noqa: F401
         except ImportError:
-            from PyQt5.QtWebKitWidgets import QWebView as QWebEngineView
+            from PyQt5.QtWebKitWidgets import (  # noqa: F401
+                QWebView as QWebEngineView,
+            )
     else:
         QWebEngineView = None
-    from PyQt5.QtTest import QTest, QSignalSpy
-    from PyQt5 import QtGui
-    from PyQt5.Qt import PYQT_VERSION_STR as PYQT_VERSION
-    from PyQt5.Qt import QT_VERSION_STR as QT_VERSION
+    from PyQt5 import QtGui  # noqa: F401
+    from PyQt5.Qt import PYQT_VERSION_STR as PYQT_VERSION  # noqa: F401
+    from PyQt5.Qt import QT_VERSION_STR as QT_VERSION  # noqa: F401
+    from PyQt5.QtTest import QSignalSpy, QTest  # noqa: F401
+
     with_qt5 = True
 
     def isstring(s):
         return isinstance(s, six.string_types)
 
 
 def asstring(s):
     return six.text_type(s)
 
 
-if sys.platform == 'darwin':
+if sys.platform == "darwin":
     # make sure to register the open file event
     OrigQApplication = QApplication
 
     class QApplication(OrigQApplication):
         """Reimplemented QApplication with open file event"""
 
         def event(self, event):
             from psyplot_gui.config.rcsetup import rcParams
 
-            if (rcParams['main.listen_to_port'] and
-                    event.type() == QtCore.QEvent.FileOpen):
+            if (
+                rcParams["main.listen_to_port"]
+                and event.type() == QtCore.QEvent.FileOpen
+            ):
                 from psyplot_gui.main import mainwindow
+
                 if mainwindow is not None:
                     opened = mainwindow.open_files([event.file()])
                     if opened:
                         return True
             return super(QApplication, self).event(event)
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/config/rcsetup.py` & `psyplot-gui-1.5.0/psyplot_gui/config/rcsetup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,50 @@
 """Default management of the psyplot_gui package
 
 This module defines the necessary configuration parts for the psyplot gui"""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import six
 import logging
+
+import six
+from matplotlib.rcsetup import validate_bool, validate_int
 from psyplot.config.rcsetup import (
-    RcParams, psyplot_fname, validate_bool_maybe_none, validate_stringlist)
-from matplotlib.rcsetup import validate_int, validate_bool
+    RcParams,
+    psyplot_fname,
+    validate_bool_maybe_none,
+    validate_stringlist,
+)
 
 
 def try_and_error(*funcs):
     """Apply multiple validation functions
 
     Parameters
     ----------
     ``*funcs``
         Validation functions to test
 
     Returns
     -------
     function"""
+
     def validate(value):
         exc = None
         for func in funcs:
             try:
                 return func(value)
             except (ValueError, TypeError) as e:
                 exc = e
         raise exc
+
     return validate
 
 
 # -----------------------------------------------------------------------------
 # ------------------------- validation functions ------------------------------
 # -----------------------------------------------------------------------------
 
@@ -91,33 +81,33 @@
     None
 
     Raises
     ------
     ValueError"""
     if isinstance(b, six.string_types):
         b = b.lower()
-    if b is None or b == 'none':
+    if b is None or b == "none":
         return None
     else:
         raise ValueError('Could not convert "%s" to None' % b)
 
 
 def validate_all(v):
     """Test if ``v == 'all'``"""
-    if v != 'all':
+    if v != "all":
         raise ValueError("The value must be 'all'")
     return six.text_type(v)
 
 
 class GuiRcParams(RcParams):
     """RcParams for the psyplot-gui package."""
 
     HEADER = RcParams.HEADER.replace(
-        'psyplotrc.yml', 'psyplotguirc.yml').replace(
-            'PSYPLOTRC', 'psyplotrc.yml')
+        "psyplotrc.yml", "psyplotguirc.yml"
+    ).replace("PSYPLOTRC", "psyplotrc.yml")
 
     def load_from_file(self, fname=None):
         """
         Update rcParams from user-defined settings
 
         This function updates the instance with what is found in `fname`
 
@@ -127,52 +117,66 @@
             Path to the yaml configuration file. Possible keys of the
             dictionary are defined by :data:`config.rcsetup.defaultParams`.
             If None, the :func:`config.rcsetup.psyplot_fname` function is used.
 
         See Also
         --------
         dump_to_file, psyplot_fname"""
-        fname = fname or psyplot_fname(env_key='PSYPLOTGUIRC',
-                                       fname='psyplotguirc.yml')
+        fname = fname or psyplot_fname(
+            env_key="PSYPLOTGUIRC", fname="psyplotguirc.yml"
+        )
         if fname:
             super(GuiRcParams, self).load_from_file(fname)
 
     def _load_plugin_entrypoints(self):
         """Load the modules for the psyplot plugins
 
         Yields
         ------
         pkg_resources.EntryPoint
             The entry point for the psyplot plugin module"""
         from pkg_resources import iter_entry_points
-        inc = self['plugins.include']
-        exc = self['plugins.exclude']
+
+        inc = self["plugins.include"]
+        exc = self["plugins.exclude"]
         logger = logging.getLogger(__name__)
         self._plugins = self._plugins or []
-        for ep in iter_entry_points('psyplot_gui'):
-            plugin_name = '%s:%s:%s' % (ep.module_name, ':'.join(ep.attrs),
-                                        ep.name)
+        for ep in iter_entry_points("psyplot_gui"):
+            try:
+                ep.module
+            except AttributeError:  # python<3.10
+                try:
+                    ep.module = ep.pattern.match(ep.value).group("module")
+                except AttributeError:  # python<3.8
+                    ep.module = ep.module_name
+
+            plugin_name = "%s:%s:%s" % (ep.module, ":".join(ep.attrs), ep.name)
             # check if the user wants to explicitly this plugin
             include_user = None
             if inc:
                 include_user = (
-                    ep.module_name in inc or ep.name in inc or
-                    '%s:%s' % (ep.module_name, ':'.join(ep.attrs)) in inc)
-            if include_user is None and exc == 'all':
+                    ep.module in inc
+                    or ep.name in inc
+                    or "%s:%s" % (ep.module, ":".join(ep.attrs)) in inc
+                )
+            if include_user is None and exc == "all":
                 include_user = False
             elif include_user is None:
                 # check for exclude
                 include_user = not (
-                    ep.module_name in exc or ep.name in exc or
-                    '%s:%s' % (ep.module_name, ':'.join(ep.attrs)) in exc)
+                    ep.module in exc
+                    or ep.name in exc
+                    or "%s:%s" % (ep.module, ":".join(ep.attrs)) in exc
+                )
             if not include_user:
-                logger.debug('Skipping plugin %s: Excluded by user',
-                             plugin_name)
+                logger.debug(
+                    "Skipping plugin %s: Excluded by user", plugin_name
+                )
             else:
-                logger.debug('Loading plugin %s', plugin_name)
+                logger.debug("Loading plugin %s", plugin_name)
                 self._plugins.append(str(ep))
                 yield ep
 
     def load_plugins(self, *args, **kwargs):
         """
         Load the plugins for the psyplot_gui MainWindow
 
@@ -181,94 +185,128 @@
         dict
             A mapping from entry point name to the imported widget class
 
         Notes
         -----
         ``*args`` and ``**kwargs`` are ignored
         """
+
         def format_ep(ep):
-            return '%s:%s:%s' % (ep.module_name, ':'.join(ep.attrs), ep.name)
+            return "%s:%s:%s" % (ep.module_name, ":".join(ep.attrs), ep.name)
+
         return {
-            format_ep(ep): ep.load() for ep in self._load_plugin_entrypoints()}
+            format_ep(ep): ep.load() for ep in self._load_plugin_entrypoints()
+        }
 
 
 #: :class:`dict` with default values and validation functions
 defaultParams = {
-
     # gui settings
-    'backend': [
-        'psyplot',
+    "backend": [
+        "psyplot",
         try_and_error(validate_str, validate_none),
-        'Backend to use when using the graphical user interface. The current '
-        'backend is used and no changes are made. Note that it is usually not '
-        'possible to change the backend after importing the psyplot.project '
-        'module. The default backend embeds the figures into the '],
-    'help_explorer.use_webengineview': [
-        True, validate_bool,
+        "Backend to use when using the graphical user interface. The current "
+        "backend is used and no changes are made. Note that it is usually not "
+        "possible to change the backend after importing the psyplot.project "
+        "module. The default backend embeds the figures into the ",
+    ],
+    "help_explorer.use_webengineview": [
+        True,
+        validate_bool,
         "Enable the PyQt5.QtWebEngineWidgets.QWebEngineView which might not "
-        "work under certain circumstances."],
-    'help_explorer.use_intersphinx': [
-        None, validate_bool_maybe_none,
-        'Use the intersphinx extension and link to the online documentations '
-        'of matplotlib, pyplot, psyplot, numpy, etc. when converting rst '
-        'docstrings. The inventories are loaded when the first object is '
-        'documented. If None, intersphinx is only used when '
-        '`help_explorer.online` is True and you are not using windows'],
-    'help_explorer.render_docs_parallel': [
-        True, validate_bool,
-        'Boolean whether the html docs are rendered in a separate process'],
-    'help_explorer.online': [
-        None, validate_bool_maybe_none,
-        'Switch that controls whether the online functions of the help '
-        'explorer shall be enabled. False implies that '
-        'help_explorer.use_intersphinx is set to False'],
-    'console.start_channels': [
-        True, validate_bool,
-        'Start the different channels of the KernelClient'],
-    'console.connect_to_help': [
-        True, validate_bool,
-        'Whether the console shall be connected to the help_explorer or not'],
-    'console.auto_set_mp': [
-        True, validate_bool,
+        "work under certain circumstances.",
+    ],
+    "help_explorer.use_intersphinx": [
+        None,
+        validate_bool_maybe_none,
+        "Use the intersphinx extension and link to the online documentations "
+        "of matplotlib, pyplot, psyplot, numpy, etc. when converting rst "
+        "docstrings. The inventories are loaded when the first object is "
+        "documented. If None, intersphinx is only used when "
+        "`help_explorer.online` is True and you are not using windows",
+    ],
+    "help_explorer.render_docs_parallel": [
+        True,
+        validate_bool,
+        "Boolean whether the html docs are rendered in a separate process",
+    ],
+    "help_explorer.online": [
+        None,
+        validate_bool_maybe_none,
+        "Switch that controls whether the online functions of the help "
+        "explorer shall be enabled. False implies that "
+        "help_explorer.use_intersphinx is set to False",
+    ],
+    "console.start_channels": [
+        True,
+        validate_bool,
+        "Start the different channels of the KernelClient",
+    ],
+    "console.connect_to_help": [
+        True,
+        validate_bool,
+        "Whether the console shall be connected to the help_explorer or not",
+    ],
+    "console.auto_set_mp": [
+        True,
+        validate_bool,
         "If True, then the 'mp' variable in the console is automatically set "
-        "when the current main project changes"],
-    'console.auto_set_sp': [
-        True, validate_bool,
+        "when the current main project changes",
+    ],
+    "console.auto_set_sp": [
+        True,
+        validate_bool,
         "If True, then the 'sp' variable in the console is automatically set "
-        "when the current sub project changes"],
-    'main.open_files_port': [
-        30124, validate_int, "The port number used when new files are opened"],
-    'main.listen_to_port': [
-        True, validate_bool,
+        "when the current sub project changes",
+    ],
+    "main.open_files_port": [
+        30124,
+        validate_int,
+        "The port number used when new files are opened",
+    ],
+    "main.listen_to_port": [
+        True,
+        validate_bool,
         "If True and the psyplot gui is already running, new files are opened "
-        "in that gui"],
-    'main.opengl': [
-        'software', validate_str,
+        "in that gui",
+    ],
+    "main.opengl": [
+        "software",
+        validate_str,
         "The opengl implementation to use. Should be one of 'software', "
-        "'desktop', 'gles' or 'automatic'."],
-    'content.load_tooltips': [
-        True, validate_bool,
+        "'desktop', 'gles' or 'automatic'.",
+    ],
+    "content.load_tooltips": [
+        True,
+        validate_bool,
         "If True, a lazy load is performed on the arrays and data sets and "
         "their string representation is displayed as tool tip. This part of "
         "the data into memory. It is recommended to set this to False for "
-        "remote data."],
-    'fmt.sort_by_key': [
-        True, validate_bool,
+        "remote data.",
+    ],
+    "fmt.sort_by_key": [
+        True,
+        validate_bool,
         "If True, the formatoptions in the Formatoptions widget are sorted by "
-        "their formatoption key rather than by their name."],
-    'plugins.include': [
-        None, try_and_error(validate_none, validate_stringlist),
+        "their formatoption key rather than by their name.",
+    ],
+    "plugins.include": [
+        None,
+        try_and_error(validate_none, validate_stringlist),
         "The plugins to load. Can be either None to load all that are not "
         "explicitly excluded by the 'plugins.exclude' key or a list of "
         "plugins to include. List items can be either module names, plugin "
-        "names or the module name and widget via '<module_name>:<widget>'"],
-    'plugins.exclude': [
-        [], try_and_error(validate_all, validate_stringlist),
+        "names or the module name and widget via '<module_name>:<widget>'",
+    ],
+    "plugins.exclude": [
+        [],
+        try_and_error(validate_all, validate_stringlist),
         "The plugins to exclude from loading. Can be either 'all' to exclude "
-        "all plugins or a list like in 'plugins.include'."],
-    }
+        "all plugins or a list like in 'plugins.include'.",
+    ],
+}
 
 #: :class:`~psyplot.config.rcsetup.RcParams` instance that stores default
 #: formatoptions and configuration settings.
 rcParams = GuiRcParams(defaultParams=defaultParams)
 rcParams.update({key: val[0] for key, val in defaultParams.items()})
 rcParams.load_from_file()
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/console.py` & `psyplot-gui-1.5.0/psyplot_gui/console.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,73 +2,64 @@
 An example of opening up an RichJupyterWidget in a PyQT Application, this can
 execute either stand-alone or by importing this file and calling
 inprocess_qtconsole.show().
 Based on the earlier example in the IPython repository, this has
 been updated to use qtconsole.
 """
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
+import logging
 import re
 import sys
 
-try:
-    from qtconsole.inprocess import QtInProcessRichJupyterWidget
-except ImportError:
-    from qtconsole.rich_jupyter_widget import (
-        RichJupyterWidget as QtInProcessRichJupyterWidget)
-
 import ipykernel
+import psyplot
+import psyplot.project as psy
+from psyplot.docstring import docstrings
+from qtconsole.inprocess import QtInProcessKernelManager
 from tornado import ioloop
 from zmq.eventloop import ioloop as zmq_ioloop
-from qtconsole.inprocess import QtInProcessKernelManager
-from psyplot_gui.compat.qtcompat import (
-    with_qt5, QtCore, Qt, QTextEdit, QTextCursor, QKeySequence, asstring)
-from psyplot_gui.common import StreamToLogger
-import psyplot
+
 import psyplot_gui
 from psyplot_gui import rcParams
-from psyplot_gui.common import DockMixin
-import psyplot.project as psy
-from psyplot.docstring import docstrings
+from psyplot_gui.common import DockMixin, StreamToLogger
+from psyplot_gui.compat.qtcompat import (
+    QKeySequence,
+    Qt,
+    QtCore,
+    QTextCursor,
+    QTextEdit,
+    asstring,
+    with_qt5,
+)
 
+try:
+    from qtconsole.inprocess import QtInProcessRichJupyterWidget
+except ImportError:
+    from qtconsole.rich_jupyter_widget import (
+        RichJupyterWidget as QtInProcessRichJupyterWidget,
+    )
 
-import logging
 
 #: HACK: Boolean that is True if the prompt should be used. This unfortunately
 #: is necessary for qtconsole >= 4.3 when running the tests
 _with_prompt = True
 
 
 modules2import = [
-    ('psyplot.project', 'psy'),
-    ('xarray', 'xr'),
-    ('pandas', 'pd'),
-    ('numpy', 'np')]
+    ("psyplot.project", "psy"),
+    ("xarray", "xr"),
+    ("pandas", "pd"),
+    ("numpy", "np"),
+]
 
 symbols_patt = re.compile(r"[^\'\"a-zA-Z0-9_.]")
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -81,24 +72,28 @@
     do this as early as possible to make it a low priority and overrideable
     ref: https://github.com/tornadoweb/tornado/issues/2608
     FIXME: if/when tornado supports the defaults in asyncio,
            remove and bump tornado requirement for py38
     """
     if sys.platform.startswith("win") and sys.version_info >= (3, 8):
         import asyncio
+
         try:
             from asyncio import (
                 WindowsProactorEventLoopPolicy,
                 WindowsSelectorEventLoopPolicy,
             )
         except ImportError:
             pass
             # not affected
         else:
-            if type(asyncio.get_event_loop_policy()) is WindowsProactorEventLoopPolicy:
+            if (
+                type(asyncio.get_event_loop_policy())
+                is WindowsProactorEventLoopPolicy
+            ):
                 # WindowsProactorEventLoopPolicy is not compatible with tornado 6
                 # fallback to the pre-3.8 default of Selector
                 asyncio.set_event_loop_policy(WindowsSelectorEventLoopPolicy())
 
 
 class IPythonControl(QTextEdit):
     """A modified control to show the help of objects in the help explorer"""
@@ -117,20 +112,19 @@
 class ConsoleWidget(QtInProcessRichJupyterWidget, DockMixin):
     """A console widget to access an inprocess shell"""
 
     custom_control = IPythonControl
 
     dock_position = Qt.RightDockWidgetArea
 
-    title = 'Console'
+    title = "Console"
 
-    rc = rcParams.find_and_replace(
-        'console.', pattern_base='console\.')
+    rc = rcParams.find_and_replace("console.", pattern_base=r"console\.")
 
-    intro_msg = ''
+    intro_msg = ""
 
     run_script = QtCore.pyqtSignal(list)
 
     run_command = QtCore.pyqtSignal(list)
 
     _closed = True
 
@@ -157,34 +151,37 @@
         orig_stdout = sys.stdout
         if sys.stdout is None:
             sys.stdout = StreamToLogger(logger)
         orig_stderr = sys.stderr
         if sys.stderr is None:
             sys.stderr = StreamToLogger(logger)
         kernel_manager.start_kernel(show_banner=False)
-        if ipykernel.__version__ < '5.1.1':
+        if ipykernel.__version__ < "5.1.1":
             # monkey patch to fix
             # https://github.com/ipython/ipykernel/issues/370
             def _abort_queues(kernel):
                 pass
+
             kernel_manager.kernel._abort_queues = _abort_queues
         sys.stdout = orig_stdout
         sys.stderr = orig_stderr
         kernel = kernel_manager.kernel
-        kernel.gui = 'qt4' if not with_qt5 else 'qt'
+        kernel.gui = "qt4" if not with_qt5 else "qt"
 
         kernel_client = kernel_manager.client()
-        if rcParams['console.start_channels']:
+        if rcParams["console.start_channels"]:
             kernel_client.start_channels()
 
-        self.help_explorer = kwargs.pop('help_explorer', None)
+        self.help_explorer = kwargs.pop("help_explorer", None)
 
         super(ConsoleWidget, self).__init__(*args, parent=main, **kwargs)
 
-        self.intro_msg = docstrings.dedent("""
+        self.intro_msg = (
+            docstrings.dedent(
+                """
         psyplot version: %s
 
         gui version: %s
 
         The console provides you the full access to the current project and
         plots.
         To make your life easier, the following modules have been imported
@@ -192,36 +189,43 @@
             - %s
 
         Furthermore, each time you change the selection or the content in the
         plot objects viewer, the `sp` (the selection) and `mp` (all arrays)
         variables in the console are adjusted. To disable this behaviour, set::
 
             >>> import psyplot_gui
-            >>> psyplot_gui.rcParams['console.auto_set_mp'] = False
-            >>> psyplot_gui.rcParams['console.auto_set_sp'] = False
+            >>> psyplot_gui.rcParams["console.auto_set_mp"] = False
+            >>> psyplot_gui.rcParams["console.auto_set_sp"] = False
 
         To inspect and object in the console and display it's documentation in
-        the help explorer, type 'Ctrl + I' or a '?' after the object""") % (
-                psyplot.__version__, psyplot_gui.__version__,
-                '\n    - '.join('%s as %s' % t for t in modules2import))
+        the help explorer, type 'Ctrl + I' or a '?' after the object"""
+            )
+            % (
+                psyplot.__version__,
+                psyplot_gui.__version__,
+                "\n    - ".join("%s as %s" % t for t in modules2import),
+            )
+        )
 
         self.kernel_manager = kernel_manager
         self.kernel_client = kernel_client
 
         self.run_command_in_shell(
-            '\n'.join('import %s as %s' % t for t in modules2import))
+            "\n".join("import %s as %s" % t for t in modules2import)
+        )
         self.exit_requested.connect(self._close_mainwindow)
         self.exit_requested.connect(QtCore.QCoreApplication.instance().quit)
 
         # we overwrite the short cut here because the 'Ctrl+S' shortcut is
         # reserved for mainwindows save action
         try:
             main.register_shortcut(
-                self.export_action, QKeySequence(
-                    'Ctrl+Alt+S', QKeySequence.NativeText))
+                self.export_action,
+                QKeySequence("Ctrl+Alt+S", QKeySequence.NativeText),
+            )
         except AttributeError:
             pass
 
         psy.Project.oncpchange.connect(self.update_mp)
         psy.Project.oncpchange.connect(self.update_sp)
 
         self.run_script.connect(self._run_script_in_shell)
@@ -235,27 +239,35 @@
         #     loop.call_later(0.1, loop.stop)``
         zmq_ioloop.install()
         self.kernel_manager.kernel.io_loop = ioloop.IOLoop.current()
 
     def update_mp(self, project):
         """Update the `mp` variable in the shell is
         ``rcParams['console.auto_set_mp']`` with a main project"""
-        if self.rc['auto_set_mp'] and project is not None and project.is_main:
-            self.run_command_in_shell('mp = psy.gcp(True)')
+        if self.rc["auto_set_mp"] and project is not None and project.is_main:
+            try:
+                self.run_command_in_shell("mp = psy.gcp(True)")
+            except RuntimeError:
+                # probably running a script that via IPythons `run` magick
+                pass
 
     def update_sp(self, project):
         """Update the `sp` variable in the shell is
         ``rcParams['console.auto_set_sp']`` with a sub project"""
-        if self.rc['auto_set_sp'] and (project is None or not project.is_main):
-            self.run_command_in_shell('sp = psy.gcp()')
+        if self.rc["auto_set_sp"] and (project is None or not project.is_main):
+            try:
+                self.run_command_in_shell("sp = psy.gcp()")
+            except RuntimeError:
+                # probably running a script that via IPythons `run` magick
+                pass
 
     def show_current_help(self, to_end=False, force=False):
         """Show the help of the object at the cursor position if
         ``rcParams['console.connect_to_help']`` is set"""
-        if not force and not self.rc['connect_to_help']:
+        if not force and not self.rc["connect_to_help"]:
             return
         obj_text = self.get_current_object(to_end)
         if obj_text is not None and self.help_explorer is not None:
             found, obj = self.get_obj(obj_text)
             if found:
                 self.help_explorer.show_help(obj, obj_text)
                 self._control.setFocus()
@@ -271,16 +283,15 @@
 
         Returns
         -------
         bool
             True, if the object could be found
         object or None
             The requested object or None if it could not be found"""
-        info = self.kernel_manager.kernel.shell._object_find(
-            obj_text)
+        info = self.kernel_manager.kernel.shell._object_find(obj_text)
         if info.found:
             return True, info.obj
         else:
             return False, None
 
     def get_current_object(self, to_end=False):
         """Get the name of the object at cursor position"""
@@ -291,79 +302,82 @@
             except AttributeError:
                 cursor = c.textCursor()
         else:
             cursor = c.textCursor()
         curr = cursor.position()
         start = curr - cursor.positionInBlock()
         txt = c.toPlainText()[start:curr]
-        eol = ''
+        eol = ""
         if to_end:
             cursor.movePosition(QTextCursor.EndOfBlock)
             end = cursor.position()
             if end > curr:
                 eol = c.toPlainText()[curr:end]
                 m = symbols_patt.search(eol)
                 if m:
-                    eol = eol[:m.start()]
+                    eol = eol[: m.start()]
 
         if not txt:
             return txt
         txt = asstring(txt)
-        txt = txt.rsplit('\n', 1)[-1]
+        txt = txt.rsplit("\n", 1)[-1]
         txt_end = ""
         for startchar, endchar in ["[]", "()"]:
             if txt.endswith(endchar):
                 pos = txt.rfind(startchar)
                 if pos:
                     txt_end = txt[pos:]
                     txt = txt[:pos]
         tokens = symbols_patt.split(txt)
         token = None
         try:
             while token is None or symbols_patt.match(token):
                 token = tokens.pop()
-            if token.endswith('.'):
+            if token.endswith("."):
                 token = token[:-1]
-            if token.startswith('.'):
+            if token.startswith("."):
                 # Invalid object name
                 return None
             token += txt_end
             if token:
                 return token + eol
         except IndexError:
             return None
 
     def _run_script_in_shell(self, args):
         self.run_script_in_shell(args[0][0])
 
     def run_script_in_shell(self, script):
         """Run a script in the shell"""
-        self.kernel_manager.kernel.shell.run_line_magic('run', script)
+        self.kernel_manager.kernel.shell.run_line_magic("run", script)
 
     def _run_command_in_shell(self, args):
         # 0: filenames
         # 1: project
         # 2: command
         self.run_command_in_shell(args[2])
 
     def run_command_in_shell(self, code, *args, **kwargs):
         """Run a script in the shell"""
         ret = self.kernel_manager.kernel.shell.run_code(code, *args, **kwargs)
         import IPython
-        if IPython.__version__ < '7.0':  # run_code is an asyncio.coroutine
+
+        if IPython.__version__ < "7.0":  # run_code is an asyncio.coroutine
             return ret
         else:
             import asyncio
+
             gathered = asyncio.gather(ret)
             loop = asyncio.get_event_loop()
             ret = loop.run_until_complete(gathered)
             return ret[0]
 
     def _close_mainwindow(self):
         from psyplot_gui.main import mainwindow
+
         if mainwindow is not None:
             mainwindow.close()
         else:
             self.close()
 
     def close(self):
         if self.kernel_client.channels_running:
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/content_widget.py` & `psyplot-gui-1.5.0/psyplot_gui/content_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,62 +3,54 @@
 
 This module redefines the :class:`psyplot.project.Project` class with
 additional features for an interactive usage with graphical qt user interface.
 There is no need to import this module because the
 :class:`GuiProject` class defined here replaces the project class in the
 :mod:`psyplot.project` module."""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import sys
-import six
 import os.path as osp
 import re
-import sip
+import sys
 import weakref
 from itertools import chain
-from psyplot_gui import rcParams
-from psyplot_gui.compat.qtcompat import (
-    QToolBox, QListWidget, QListWidgetItem, QAbstractItemView,
-    QWidget, QPushButton, QHBoxLayout, QVBoxLayout, QTreeWidget,
-    QTreeWidgetItem, QtCore, QMenu, QAction, Qt, QLabel, QScrollArea)
+from xml.sax.saxutils import escape
+
+import sip
+import six
 from psyplot.config.rcsetup import safe_list
-from psyplot.compat.pycompat import OrderedDict, map, range
-from psyplot.project import scp, gcp, Project
 from psyplot.data import ArrayList, InteractiveList
+from psyplot.project import Project, gcp, scp
 from psyplot.utils import _TempBool
-from psyplot_gui.common import DockMixin
-from xml.sax.saxutils import escape
 
+from psyplot_gui import rcParams
+from psyplot_gui.common import DockMixin
+from psyplot_gui.compat.qtcompat import (
+    QAbstractItemView,
+    QAction,
+    QHBoxLayout,
+    QListWidget,
+    QListWidgetItem,
+    QMenu,
+    QPushButton,
+    Qt,
+    QtCore,
+    QToolBox,
+    QTreeWidget,
+    QTreeWidgetItem,
+    QVBoxLayout,
+    QWidget,
+)
 
-html_escape_table = {
-    '"': "&quot;",
-    "'": "&apos;"
-    }
+html_escape_table = {'"': "&quot;", "'": "&apos;"}
 
 
 def escape_html(s):
     return escape(s, html_escape_table)
 
 
 class ArrayItem(QListWidgetItem):
@@ -86,15 +78,15 @@
 
     def set_text_from_array(self):
         """Set the text and tooltop from the
         :meth:`psyplot.data.InteractiveArray._short_info` and __str__ methods
         """
         if not sip.isdeleted(self):
             self.setText(self.arr()._short_info())
-            if rcParams['content.load_tooltips']:
+            if rcParams["content.load_tooltips"]:
                 if isinstance(self.arr(), InteractiveList):
                     self.setToolTip(str(self.arr()))
                 else:
                     self.setToolTip(str(self.arr().arr))
         else:
             self.disconnect_from_array()
 
@@ -122,23 +114,27 @@
 
     # Determine whether the plotter could be loaded
     can_import_plotter = True
 
     @property
     def arrays(self):
         """List of The InteractiveBase instances in this list"""
-        return ArrayList([
-            getattr(item.arr(), 'arr', item.arr())
-            for item in self.array_items])
+        return ArrayList(
+            [
+                getattr(item.arr(), "arr", item.arr())
+                for item in self.array_items
+            ]
+        )
 
     @property
     def array_items(self):
         """Iterable of :class:`ArrayItem` items in this list"""
-        return filter(lambda i: i is not None,
-                      map(self.item, range(self.count())))
+        return filter(
+            lambda i: i is not None, map(self.item, range(self.count()))
+        )
 
     def __init__(self, plotter_type=None, *args, **kwargs):
         """
         Parameters
         ----------
         plotter_type: str or None
             If str, it mus be an attribute name of the
@@ -207,27 +203,27 @@
                 # resort to match the project
                 for arr in reversed(main_arrays):
                     for i, item in enumerate(self.array_items):
                         if item.arr() is arr.psy:
                             self.insertItem(0, self.takeItem(i))
             cp = gcp()
             for item in self.array_items:
-                item.setSelected(
-                    getattr(item.arr(), 'arr', item.arr()) in cp)
+                item.setSelected(getattr(item.arr(), "arr", item.arr()) in cp)
         self.updated_from_project.emit(self)
 
     def update_cp(self, *args, **kwargs):
         """Update the current project from what is selected in this list"""
         if not self._no_project_update:
             mp = gcp(True)
             sp = gcp()
             selected = [item.arr().arr_name for item in self.selectedItems()]
             arrays = self.arrays
             other_selected = [
-                arr.psy.arr_name for arr in sp if arr not in arrays]
+                arr.psy.arr_name for arr in sp if arr not in arrays
+            ]
             with self._no_project_update:
                 scp(mp(arr_name=selected + other_selected))
 
     def disconnect_items(self):
         """Disconnect the items in this list from the arrays"""
         for item in list(self.array_items):
             item.disconnect_from_array()
@@ -237,41 +233,41 @@
 
 class ProjectContent(QToolBox):
     """Display the content in the current project
 
     This toolbox contains several :class:`PlotterList` that show the content
     of the current main and subproject"""
 
-    #: :class:`OrderedDict` containing the :class:`PlotterList` instances
+    #: :class:`dict` containing the :class:`PlotterList` instances
     #: of the different selection attributes
-    lists = OrderedDict()
+    lists = dict()
 
     @property
     def current_names(self):
         return [self.itemText(i) for i in range(self.count())]
 
     def __init__(self, *args, **kwargs):
         super(ProjectContent, self).__init__(*args, **kwargs)
-        self.lists = OrderedDict()
-        for attr in chain(['All'], sorted(Project._registered_plotters)):
-            item = self.add_plotterlist(attr, force=(attr == 'All'))
+        self.lists = dict()
+        for attr in chain(["All"], sorted(Project._registered_plotters)):
+            item = self.add_plotterlist(attr, force=(attr == "All"))
             self.lists[attr] = item
         self.currentChanged.connect(self.update_current_list)
         Project.oncpchange.connect(self.update_lists)
 
     def enable_list(self, list_widget):
         """Enable a given list widget based upon whether it is empty or not"""
         i = self.indexOf(list_widget)
         if i != -1:
             self.setItemEnabled(i, not list_widget.is_empty)
 
     def add_plotterlist(self, identifier, force=False):
         """Create a :class:`PlotterList` from an identifier from the
         :class:`psyplot.project.Project` class"""
-        attr = identifier if identifier != 'All' else None
+        attr = identifier if identifier != "All" else None
         item = PlotterList(attr)
         if not item.can_import_plotter:
             return item
         if force or not item.is_empty:
             item.setParent(self)
             item.updated_from_project.connect(self.enable_list)
             self.addItem(item, identifier)
@@ -289,28 +285,29 @@
         current_items = self.current_names
         for name, l in self.lists.items():
             if not p.is_main:
                 l.update_from_project(p.main)
             l.update_from_project(p)
             if l.is_empty:
                 l.disconnect_items()
-            if name != 'All' and l.is_empty:
+            if name != "All" and l.is_empty:
                 i = self.indexOf(l)
                 self.removeItem(i)
             elif not l.is_empty and name not in current_items:
                 self.addItem(l, name)
 
 
 class SelectAllButton(QPushButton):
     """A button to select all data objects in the current main project"""
 
     def __init__(self, *args, **kwargs):
         super(SelectAllButton, self).__init__(*args, **kwargs)
         self.setToolTip(
-            'Click to select all data arrays in the entire project')
+            "Click to select all data arrays in the entire project"
+        )
         self.clicked.connect(self.select_all)
         Project.oncpchange.connect(self.enable_from_project)
 
     def select_all(self):
         """Select all arrays"""
         scp(gcp(True)[:])
 
@@ -320,15 +317,15 @@
 
 
 class SelectNoneButton(QPushButton):
     """A button to select no data objects in the current main project"""
 
     def __init__(self, *args, **kwargs):
         super(SelectNoneButton, self).__init__(*args, **kwargs)
-        self.setToolTip('Click to deselect all data arrays')
+        self.setToolTip("Click to deselect all data arrays")
         self.clicked.connect(self.select_none)
         Project.oncpchange.connect(self.enable_from_project)
 
     def select_none(self):
         """Clear current subproject"""
         scp(gcp(True)[:0])
 
@@ -340,16 +337,16 @@
 class ProjectContentWidget(QWidget, DockMixin):
     """A combination of selection buttons and the ProjectContent"""
 
     def __init__(self, *args, **kwargs):
         super(ProjectContentWidget, self).__init__(*args, **kwargs)
         vbox = QVBoxLayout()
         # create buttons for unselecting and selecting all arrays
-        self.unselect_button = SelectNoneButton('Unselect all', parent=self)
-        self.select_all_button = SelectAllButton('Select all', parent=self)
+        self.unselect_button = SelectNoneButton("Unselect all", parent=self)
+        self.select_all_button = SelectAllButton("Select all", parent=self)
         button_hbox = QHBoxLayout()
         button_hbox.addWidget(self.unselect_button)
         button_hbox.addWidget(self.select_all_button)
         mp = gcp(True)
         self.unselect_button.setEnabled(bool(mp))
         self.select_all_button.setEnabled(bool(mp))
         # create widget showing the content of the current project
@@ -363,19 +360,19 @@
     """A QTreeWidgetItem showing informations on one dataset in the main
     project"""
 
     def __init__(self, ds, columns=[], *args, **kwargs):
         super(DatasetTreeItem, self).__init__(*args, **kwargs)
         self.variables = variables = QTreeWidgetItem(0)
         self.columns = columns
-        variables.setText(0, 'variables (%i)' % len(ds))
+        variables.setText(0, "variables (%i)" % len(ds))
         self.coords = coords = QTreeWidgetItem(0)
-        coords.setText(0, 'coords (%i)' % len(ds.coords))
+        coords.setText(0, "coords (%i)" % len(ds.coords))
         self.attrs = attrs = QTreeWidgetItem(0)
-        attrs.setText(0, 'Global Attributes (%i)' % len(ds.attrs))
+        attrs.setText(0, "Global Attributes (%i)" % len(ds.attrs))
         self.addChildren([variables, coords])
         self.addChild(variables)
         self.addChild(attrs)
         self.add_variables(ds)
         self.add_attrs(ds.attrs)
 
     def add_variables(self, ds=None):
@@ -389,166 +386,176 @@
         columns = self.columns
         variables = self.variables
         coords = self.coords
         for vname, variable in six.iteritems(ds.variables):
             item = QTreeWidgetItem(0)
             item.setText(0, str(vname))
             for i, attr in enumerate(columns, 1):
-                if attr == 'dims':
-                    item.setText(i, ', '.join(variable.dims))
+                if attr == "dims":
+                    item.setText(i, ", ".join(variable.dims))
                 else:
-                    item.setText(i, str(variable.attrs.get(attr, getattr(
-                        variable, attr, ''))))
+                    item.setText(
+                        i,
+                        str(
+                            variable.attrs.get(
+                                attr, getattr(variable, attr, "")
+                            )
+                        ),
+                    )
             if vname in ds.coords:
                 coords.addChild(item)
             else:
                 variables.addChild(item)
-            if rcParams['content.load_tooltips']:
+            if rcParams["content.load_tooltips"]:
                 item.setToolTip(
-                    0, '<pre>' + escape_html(str(variable)) + '</pre>')
+                    0, "<pre>" + escape_html(str(variable)) + "</pre>"
+                )
 
             # Add shape
             shape_item = QTreeWidgetItem(0)
-            shape_item.setText(0, 'shape')
+            shape_item.setText(0, "shape")
             shape_item.setText(1, str(variable.shape))
             item.addChild(shape_item)
 
-
             # Add dimensions
             dims_item = QTreeWidgetItem(0)
-            dims_item.setText(0, 'dims')
-            dims_item.setText(1, ', '.join(variable.dims))
+            dims_item.setText(0, "dims")
+            dims_item.setText(1, ", ".join(variable.dims))
             item.addChild(dims_item)
 
             # add open plots
             plots_item = QTreeWidgetItem(0)
-            plots_item.setText(0, 'Plots')
+            plots_item.setText(0, "Plots")
             self.refresh_plots_item(plots_item, vname)
             item.addChild(plots_item)
 
             # add variable attribute
             attrs_item = QTreeWidgetItem(0)
-            attrs_item.setText(0, 'Attributes')
+            attrs_item.setText(0, "Attributes")
             self.add_attrs(variable.attrs, attrs_item)
             item.addChild(attrs_item)
 
             # add variable encoding
             encoding_item = QTreeWidgetItem(0)
-            encoding_item.setText(0, 'Encoded attributes')
+            encoding_item.setText(0, "Encoded attributes")
             self.add_attrs(variable.encoding, encoding_item)
             item.addChild(encoding_item)
 
     def get_plots_item(self, item):
         for child in map(item.child, range(item.childCount())):
-            if child.text(0) == 'Plots':
+            if child.text(0) == "Plots":
                 return child
 
     def refresh_plots_item(self, item, vname, mp=None, sp=None):
         expand = item.isExpanded()
         item.takeChildren()
         try:
             num = self.ds().psy.num
         except AttributeError:
             return
         if mp is None:
             mp = gcp(True)
         if sp is None:
             sp = gcp()
         for i in range(len(mp)):
-            sub = mp[i:i+1]
-            array_info = sub.array_info(ds_description={'arr', 'num'})
+            sub = mp[i : i + 1]
+            array_info = sub.array_info(ds_description={"arr", "num"})
             arrs = sub._get_ds_descriptions(array_info).get(num, {})
-            if arrs and any(vname in arr.psy.base_variables
-                            for arr in arrs['arr']):
+            if arrs and any(
+                vname in arr.psy.base_variables for arr in arrs["arr"]
+            ):
                 child = QTreeWidgetItem(0)
-                prefix = '*' if sub[0] in sp else ''
+                prefix = "*" if sub[0] in sp else ""
                 text = sub[0].psy._short_info()
                 child.setText(0, prefix + text)
                 child.setToolTip(0, text)
                 item.addChild(child)
         if expand and item.childCount():
             item.setExpanded(True)
 
-
     def add_attrs(self, attrs=None, item=None):
         if attrs is None:
             attrs = self.ds().attrs
             self.attrs.takeChildren()
         if item is None:
             item = self.attrs
         for key, val in attrs.items():
             child = QTreeWidgetItem(0)
             child.setText(0, key)
             child.setText(1, str(val))
-            child.setToolTip(1, '{}: {}'.format(key, str(val)))
+            child.setToolTip(1, "{}: {}".format(key, str(val)))
             item.addChild(child)
 
 
 class DatasetTree(QTreeWidget, DockMixin):
-    """A QTreeWidget showing informations on all datasets in the main project
-    """
+    """A QTreeWidget showing informations on all datasets in the main project"""
 
     tooltips = {
-        'Refresh': 'Refresh the selected dataset',
-        'Refresh all': 'Refresh all datasets',
-        'Add to project': ('Add this variable or a plot of it to the current '
-                           'project')}
+        "Refresh": "Refresh the selected dataset",
+        "Refresh all": "Refresh all datasets",
+        "Add to project": (
+            "Add this variable or a plot of it to the current " "project"
+        ),
+    }
 
     def __init__(self, *args, **kwargs):
         super(DatasetTree, self).__init__(*args, **kwargs)
         self.create_dataset_tree()
         self.itemExpanded.connect(self.load_variable_desc)
         self.setContextMenuPolicy(Qt.CustomContextMenu)
         self.customContextMenuRequested.connect(self.open_menu)
         Project.oncpchange.connect(self.add_datasets_from_cp)
         self.hideColumn(1)
 
     @staticmethod
     def is_variable(item):
-        return re.match(r'variables \(\d+\)', item.parent().text(0))
+        return re.match(r"variables \(\d+\)", item.parent().text(0))
 
     @staticmethod
     def is_coord(item):
-        return re.match(r'coords\(\d+\)', item.parent().text(0))
+        return re.match(r"coords\(\d+\)", item.parent().text(0))
 
     def load_variable_desc(self, item):
         parent = item.parent()
-        if parent is self or parent is None or not (self.is_variable(item) or
-                                                    self.is_coord(item)):
+        if (
+            parent is self
+            or parent is None
+            or not (self.is_variable(item) or self.is_coord(item))
+        ):
             return
         if self.isColumnHidden(1):
             self.showColumn(1)
             self.resizeColumnToContents(0)
 
         top = item
         while top.parent() and top.parent() is not self:
             top = top.parent()
         ds = top.ds()
         if ds is None:
             return
         desc = escape_html(str(ds.variables[item.text(0)]))
-        item.setToolTip(0, '<pre>' + desc + '</pre>')
+        item.setToolTip(0, "<pre>" + desc + "</pre>")
 
     def create_dataset_tree(self):
         """Set up the columns and insert the :class:`DatasetTreeItem`
         instances from the current project"""
         self.set_columns()
         self.add_datasets_from_cp(gcp())
 
-    def set_columns(self, columns=['Value']):
+    def set_columns(self, columns=["Value"]):
         """Set up the columns in the DatasetTree.
 
         Parameters
         ----------
         columns: list of str
             A list of netCDF attributes that shall be shown in columns"""
         self.setColumnCount(len(columns) + 1)
         if columns:
             self.setHeaderHidden(False)
-            self.setHeaderLabels(['Dataset'] + list(columns))
+            self.setHeaderLabels(["Dataset"] + list(columns))
         else:
             self.setHeaderHidden(True)
         self.attr_columns = columns
 
     def expanded_items(self):
         "Create a mapping from dataset numbers to variables that are expanded."
         ret = {}
@@ -556,15 +563,16 @@
             if item.isExpanded() and item.ds() is not None:
                 ds = item.ds()
                 ret[ds.psy.num] = d = {}
                 for child in map(item.child, range(item.childCount())):
                     if child.childCount() and child.isExpanded():
                         d[child.text(0)] = variables = []
                         for vchild in map(
-                                child.child, range(child.childCount())):
+                            child.child, range(child.childCount())
+                        ):
                             if vchild.childCount() and vchild.isExpanded():
                                 variables.append(vchild.text(0))
         return ret
 
     def add_datasets_from_cp(self, project=None):
         """Clear the tree and add the datasets based upon the given `project`
 
@@ -582,28 +590,43 @@
         else:
             sp_arrs = project.arrays
             project = project.main
 
         expanded_items = self.expanded_items()
         # remove items from the tree
         self.clear()
-        for i, ds_desc in six.iteritems(project._get_ds_descriptions(
-                project.array_info(ds_description='all'))):
-            top_item = DatasetTreeItem(ds_desc['ds'], self.attr_columns, 0)
-            if ds_desc['fname'] is not None and not all(
-                    s is None for s in ds_desc['fname']):
-                ds_desc['fname'] = ', '.join(map(osp.basename,
-                                                 safe_list(ds_desc['fname'])))
+        for i, ds_desc in six.iteritems(
+            project._get_ds_descriptions(
+                project.array_info(ds_description="all")
+            )
+        ):
+            top_item = DatasetTreeItem(ds_desc["ds"], self.attr_columns, 0)
+            if ds_desc["fname"] is not None and not all(
+                s is None for s in ds_desc["fname"]
+            ):
+                ds_desc["fname"] = ", ".join(
+                    map(osp.basename, safe_list(ds_desc["fname"]))
+                )
             else:
-                ds_desc['fname'] = None
-            top_item.setText(0, '%s%i: %s' % (
-                '*' if any(any(arr is arr2 for arr2 in sp_arrs)
-                           for arr in ds_desc['arr']) else '',
-                i, ds_desc['fname']))
-            for arr in ds_desc['arr']:
+                ds_desc["fname"] = None
+            top_item.setText(
+                0,
+                "%s%i: %s"
+                % (
+                    "*"
+                    if any(
+                        any(arr is arr2 for arr2 in sp_arrs)
+                        for arr in ds_desc["arr"]
+                    )
+                    else "",
+                    i,
+                    ds_desc["fname"],
+                ),
+            )
+            for arr in ds_desc["arr"]:
                 arr.psy.onbasechange.connect(self.add_datasets_from_cp)
             self.addTopLevelItem(top_item)
         self.expand_items(expanded_items)
 
     def expand_items(self, expanded_items):
         """Expand tree items
 
@@ -615,59 +638,63 @@
             ds = top.ds()
             if ds.psy.num in expanded_items:
                 self.expandItem(top)
                 d = expanded_items[ds.psy.num]
                 for child in map(top.child, range(top.childCount())):
                     if child.text(0) in d:
                         self.expandItem(child)
-                        for vchild in map(child.child,
-                                          range(child.childCount())):
+                        for vchild in map(
+                            child.child, range(child.childCount())
+                        ):
                             if vchild.text(0) in d[child.text(0)]:
                                 self.expandItem(vchild)
 
     def open_menu(self, pos):
         menu = QMenu()
         item = self.itemAt(pos)
         parent, item_type, vname = self._get_toplevel_item(item)
         # ---- Refresh the selected item action
-        refresh_action = QAction('Refresh', self)
-        refresh_action.setToolTip(self.tooltips['Refresh'])
+        refresh_action = QAction("Refresh", self)
+        refresh_action.setToolTip(self.tooltips["Refresh"])
         refresh_action.triggered.connect(lambda: self.refresh_items(parent))
 
         # ---- Refresh all items action
-        refresh_all_action = QAction('Refresh all', self)
-        refresh_all_action.setToolTip(self.tooltips['Refresh all'])
+        refresh_all_action = QAction("Refresh all", self)
+        refresh_all_action.setToolTip(self.tooltips["Refresh all"])
         refresh_all_action.triggered.connect(lambda: self.refresh_items())
 
         # ---- add refresh actions
         menu.addActions([refresh_action, refresh_all_action])
 
         # ---- add plot option
-        if item_type == 'variable':
-            add2p_action = QAction(f'Add new plot of {vname}', self)
-            add2p_action.setToolTip(self.tooltips['Add to project'])
-            add2p_action.triggered.connect(lambda: self.make_plot(
-                parent.ds(), item.text(0), True))
+        if item_type == "variable":
+            add2p_action = QAction(f"Add new plot of {vname}", self)
+            add2p_action.setToolTip(self.tooltips["Add to project"])
+            add2p_action.triggered.connect(
+                lambda: self.make_plot(parent.ds(), item.text(0), True)
+            )
             menu.addSeparator()
             menu.addAction(add2p_action)
 
         # ---- show menu
         menu.exec_(self.mapToGlobal(pos))
         return menu
 
     def refresh_items(self, item=None):
         if item is not None:
             item.add_variables()
         else:
-            for item in map(self.topLevelItem,
-                            range(self.topLevelItemCount())):
+            for item in map(
+                self.topLevelItem, range(self.topLevelItemCount())
+            ):
                 item.add_variables()
 
     def make_plot(self, ds, name, exec_=None):
         from psyplot_gui.main import mainwindow
+
         mainwindow.new_plots()
         mainwindow.plot_creator.switch2ds(ds)
         mainwindow.plot_creator.insert_array(safe_list(name))
         if exec_:
             mainwindow.plot_creator.exec_()
 
     def _get_toplevel_item(self, item):
@@ -676,18 +703,18 @@
         else:
             parent = item.parent()
         item_type = None
         vname = None
         while parent is not None:
             if self.is_variable(item):
                 vname = item.text(0)
-                item_type = 'variable'
+                item_type = "variable"
             elif self.is_coord(item):
                 vname = item.text(0)
-                item_type = 'coord'
+                item_type = "coord"
             item = item.parent()
             parent = item.parent()
         return item, item_type, vname
 
 
 class FiguresTreeItem(QTreeWidgetItem):
     """An item displaying the information on a data object in one figure"""
@@ -704,15 +731,15 @@
         ref().psy.onupdate.connect(self.set_text_from_array)
 
     def set_text_from_array(self):
         """Set the text and tooltop from the
         :meth:`psyplot.data.InteractiveArray._short_info` and __str__ methods
         """
         self.setText(0, self.arr().psy._short_info())
-        if rcParams['content.load_tooltips']:
+        if rcParams["content.load_tooltips"]:
             self.setToolTip(0, str(self.arr()))
 
     def disconnect_from_array(self):
         """Disconect this item from the corresponding array"""
         arr = self.arr()
         if arr is not None:
             arr.psy.onupdate.disconnect(self.set_text_from_array)
@@ -723,25 +750,26 @@
     """A tree widget sorting the arrays by their figure
 
     This widget uses the current sub and main project to show the open figures
     """
 
     def __init__(self, *args, **kwargs):
         super(FiguresTree, self).__init__(*args, **kwargs)
-        self.setHeaderLabel('Figure')
+        self.setHeaderLabel("Figure")
         Project.oncpchange.connect(self.add_figures_from_cp)
         self.add_figures_from_cp(gcp(True))
 
     def add_figures_from_cp(self, project):
         """Add the items in this tree based upon the figures in the given
         project"""
         if project is None or not project.is_main:
             return
         for item in map(self.takeTopLevelItem, [0] * self.topLevelItemCount()):
             for child in item.takeChildren():
                 child.disconnect_from_array()
         for fig, arrays in six.iteritems(project.figs):
             item = QTreeWidgetItem(0)
-            item.setText(0, fig.canvas.get_window_title())
+            item.setText(0, fig.canvas.manager.get_window_title())
             item.addChildren(
-                [FiguresTreeItem(weakref.ref(arr), 0) for arr in arrays])
+                [FiguresTreeItem(weakref.ref(arr), 0) for arr in arrays]
+            )
             self.addTopLevelItem(item)
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/dataframeeditor.py` & `psyplot-gui-1.5.0/psyplot_gui/dataframeeditor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 """A widget to display and edit DataFrames"""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
 import os
 import os.path as osp
-import six
 from functools import partial
+
 import numpy as np
+import pandas as pd
+import six
 from psyplot.docstring import docstrings
+
+from psyplot_gui.common import (
+    DockMixin,
+    LoadFromConsoleButton,
+    PyErrorMessage,
+    get_icon,
+)
 from psyplot_gui.compat.qtcompat import (
-    QWidget, QHBoxLayout, QVBoxLayout, QtCore, QLineEdit,
-    QPushButton, Qt, QToolButton, QIcon, QMenu, QLabel, QtGui, QApplication,
-    QCheckBox, QFileDialog, with_qt5, QTableView, QHeaderView,
-    QDockWidget)
-from psyplot_gui.common import (DockMixin, get_icon, LoadFromConsoleButton,
-                                PyErrorMessage)
-import pandas as pd
+    QApplication,
+    QCheckBox,
+    QDockWidget,
+    QFileDialog,
+    QHBoxLayout,
+    QHeaderView,
+    QIcon,
+    QLabel,
+    QLineEdit,
+    QMenu,
+    QPushButton,
+    Qt,
+    QTableView,
+    QtCore,
+    QtGui,
+    QToolButton,
+    QVBoxLayout,
+    QWidget,
+    with_qt5,
+)
 
 if six.PY2:
     try:
         import CStringIO as io
     except ImportError:
         import StringIO as io
 else:
@@ -50,39 +55,40 @@
 LARGE_SIZE = int(5e5)
 LARGE_NROWS = int(1e5)
 LARGE_COLS = 60
 
 REAL_NUMBER_TYPES = (float, int, np.int64, np.int32)
 COMPLEX_NUMBER_TYPES = (complex, np.complex64, np.complex128)
 
-_bool_false = ['false', '0']
+_bool_false = ["false", "0"]
 
 
 def bool_false_check(value):
     """
     Used to convert bool intrance to false since any string in bool('')
     will return True
     """
     if value.lower() in _bool_false:
-        value = ''
+        value = ""
     return value
 
 
 class DataFrameModel(QtCore.QAbstractTableModel):
-    """ DataFrame Table Model"""
+    """DataFrame Table Model"""
 
     ROWS_TO_LOAD = 500
     COLS_TO_LOAD = 40
 
-    _format = '%0.6g'
+    _format = "%0.6g"
 
-    @docstrings.get_sections(base='DataFrameModel')
+    @docstrings.get_sections(base="DataFrameModel")
     @docstrings.dedent
-    def __init__(self, df, parent=None, index_editable=True,
-                 dtypes_changeable=True):
+    def __init__(
+        self, df, parent=None, index_editable=True, dtypes_changeable=True
+    ):
         """
         Parameters
         ----------
         df: pandas.DataFrame
             The data frame that will be shown by this :class:`DataFrameModel`
             instance
         parent: DataFrameEditor
@@ -136,20 +142,20 @@
     def headerData(self, section, orientation, role=Qt.DisplayRole):
         """Set header data"""
         if role != Qt.DisplayRole:
             return None
 
         if orientation == Qt.Horizontal:
             if section == 0:
-                return six.text_type('Index')
-            elif isinstance(self.df_header[section-1], six.string_types):
-                header = self.df_header[section-1]
+                return six.text_type("Index")
+            elif isinstance(self.df_header[section - 1], six.string_types):
+                header = self.df_header[section - 1]
                 return six.text_type(header)
             else:
-                return six.text_type(self.df_header[section-1])
+                return six.text_type(self.df_header[section - 1])
         else:
             return None
 
     def get_value(self, row, column):
         """Returns the value of the DataFrame"""
         # To increase the performance iat is used but that requires error
         # handling, so fallback uses iloc
@@ -165,58 +171,67 @@
             return None
         if role == Qt.DisplayRole or role == Qt.EditRole:
             column = index.column()
             row = index.row()
             if column == 0:
                 return six.text_type(self.df_index[row])
             else:
-                value = self.get_value(row, column-1)
+                value = self.get_value(row, column - 1)
                 if isinstance(value, float):
                     try:
                         return self._format % value
                     except (ValueError, TypeError):
                         # may happen if format = '%d' and value = NaN;
                         # see issue 4139
                         return DataFrameModel._format % value
                 else:
                     return six.text_type(value)
 
-    def sort(self, column, order=Qt.AscendingOrder, return_check=False,
-             report=True):
+    def sort(
+        self, column, order=Qt.AscendingOrder, return_check=False, report=True
+    ):
         """Overriding sort method"""
         try:
             ascending = order == Qt.AscendingOrder
             if column > 0:
                 try:
-                    self.df.sort_values(by=self.df.columns[column-1],
-                                        ascending=ascending, inplace=True,
-                                        kind='mergesort')
+                    self.df.sort_values(
+                        by=self.df.columns[column - 1],
+                        ascending=ascending,
+                        inplace=True,
+                        kind="mergesort",
+                    )
                 except AttributeError:
                     # for pandas version < 0.17
-                    self.df.sort(columns=self.df.columns[column-1],
-                                 ascending=ascending, inplace=True,
-                                 kind='mergesort')
+                    self.df.sort(
+                        columns=self.df.columns[column - 1],
+                        ascending=ascending,
+                        inplace=True,
+                        kind="mergesort",
+                    )
                 self.update_df_index()
             else:
                 self.df.sort_index(inplace=True, ascending=ascending)
                 self.update_df_index()
-        except TypeError as e:
+        except TypeError:
             if report:
                 self._parent.error_msg.showTraceback(
-                    "<b>Failed to sort column!</b>")
+                    "<b>Failed to sort column!</b>"
+                )
             return False if return_check else None
         self.reset()
         return True if return_check else None
 
     def flags(self, index):
         """Set flags"""
         if index.column() == 0 and not self.index_editable:
             return Qt.ItemIsEnabled | Qt.ItemIsSelectable
-        return Qt.ItemFlags(QtCore.QAbstractTableModel.flags(self, index) |
-                            Qt.ItemIsEditable)
+        return Qt.ItemFlags(
+            QtCore.QAbstractTableModel.flags(self, index) | Qt.ItemIsEditable
+        )
 
     def setData(self, index, value, role=Qt.EditRole, change_type=None):
         """Cell content change"""
         column = index.column()
         row = index.row()
 
         if change_type is not None:
@@ -225,50 +240,61 @@
             try:
                 value = current_value = self.data(index, role=Qt.DisplayRole)
                 if change_type is bool:
                     value = bool_false_check(value)
                 value = np.asarray(change_type(value))  # to make sure it works
                 icol = column - 1
                 self.df.iloc[:, icol] = self.df.iloc[:, icol].astype(
-                    change_type)
+                    change_type
+                )
             except ValueError:
-                self.df.iloc[row, icol] = self.df.iloc[row, icol].astype(object)
+                self.df.iloc[row, icol] = self.df.iloc[row, icol].astype(
+                    object
+                )
         else:
-            current_value = self.get_value(row, column-1) if column else \
-                self.df.index[row]
+            current_value = (
+                self.get_value(row, column - 1)
+                if column
+                else self.df.index[row]
+            )
             if isinstance(current_value, bool):
                 value = bool_false_check(value)
-            supported_types = (bool,) + REAL_NUMBER_TYPES + \
-                COMPLEX_NUMBER_TYPES
-            if (isinstance(current_value, supported_types) or
-                    isinstance(current_value, six.string_types)):
+            supported_types = (
+                (bool,) + REAL_NUMBER_TYPES + COMPLEX_NUMBER_TYPES
+            )
+            if isinstance(current_value, supported_types) or isinstance(
+                current_value, six.string_types
+            ):
                 if column:
                     try:
-                        self.df.iloc[row, column-1] = current_value.__class__(
-                            value)
-                    except ValueError as e:
+                        self.df.iloc[
+                            row, column - 1
+                        ] = current_value.__class__(value)
+                    except ValueError:
                         self._parent.error_msg.showTraceback(
-                            "<b>Failed to set value with %r!</b>" % value)
+                            "<b>Failed to set value with %r!</b>" % value
+                        )
                         return False
                 elif self.index_editable:
                     index = self.df.index.values.copy()
                     try:
                         index[row] = value
-                    except ValueError as e:
+                    except ValueError:
                         self._parent.error_msg.showTraceback(
-                            "<b>Failed to set value with %r!</b>" % value)
+                            "<b>Failed to set value with %r!</b>" % value
+                        )
                         return False
                     self.df.index = pd.Index(index, name=self.df.index.name)
                     self.update_df_index()
                 else:
                     return False
             else:
                 self._parent.error_msg.showTraceback(
-                            "<b>The type of the cell is not a supported type"
-                            "</b>")
+                    "<b>The type of the cell is not a supported type" "</b>"
+                )
                 return False
         self._parent.cell_edited.emit(row, column, current_value, value)
         return True
 
     def rowCount(self, index=QtCore.QModelIndex()):
         """DataFrame row number"""
         if self.total_rows <= self.rows_loaded:
@@ -288,38 +314,44 @@
             else:
                 return False
 
     def fetch_more(self, rows=False, columns=False):
         if self.can_fetch_more(rows=rows):
             reminder = self.total_rows - self.rows_loaded
             items_to_fetch = min(reminder, self.ROWS_TO_LOAD)
-            self.beginInsertRows(QtCore.QModelIndex(), self.rows_loaded,
-                                 self.rows_loaded + items_to_fetch - 1)
+            self.beginInsertRows(
+                QtCore.QModelIndex(),
+                self.rows_loaded,
+                self.rows_loaded + items_to_fetch - 1,
+            )
             self.rows_loaded += items_to_fetch
             self.endInsertRows()
         if self.can_fetch_more(columns=columns):
             reminder = self.total_cols - self.cols_loaded
             items_to_fetch = min(reminder, self.COLS_TO_LOAD)
-            self.beginInsertColumns(QtCore.QModelIndex(), self.cols_loaded,
-                                    self.cols_loaded + items_to_fetch - 1)
+            self.beginInsertColumns(
+                QtCore.QModelIndex(),
+                self.cols_loaded,
+                self.cols_loaded + items_to_fetch - 1,
+            )
             self.cols_loaded += items_to_fetch
             self.endInsertColumns()
 
     def columnCount(self, index=QtCore.QModelIndex()):
         """DataFrame column number"""
         # This is done to implement series
         if len(self.df.shape) == 1:
             return 2
         elif self.total_cols <= self.cols_loaded:
             return self.total_cols + 1
         else:
             return self.cols_loaded + 1
 
     def update_df_index(self):
-        """"Update the DataFrame index"""
+        """ "Update the DataFrame index"""
         self.df_index = self.df.index.tolist()
 
     def reset(self):
         self.beginResetModel()
         self.endResetModel()
 
     def insertRow(self, irow):
@@ -347,15 +379,15 @@
         if not irow:
             if not len(df):
                 idx = 0
             else:
                 idx = df.index.values[0]
         else:
             try:
-                idx = df.index.values[irow-1:irow+1].mean()
+                idx = df.index.values[irow - 1 : irow + 1].mean()
             except TypeError:
                 idx = df.index.values[min(irow, len(df) - 1)]
             else:
                 idx = df.index.values[min(irow, len(df) - 1)].__class__(idx)
         # reset the index to sort it correctly
         idx_name = df.index.name
         dtype = df.index.dtype
@@ -369,26 +401,30 @@
             changed = df.index.values.astype(float)
             changed[current_len:] = irow - 0.5
             df.index = changed
             df.sort_index(inplace=True)
         df.set_index(new_idx_name, inplace=True, drop=True)
         df.index.name = idx_name
         self.update_df_index()
-        self.beginInsertRows(QtCore.QModelIndex(), self.rows_loaded,
-                             self.rows_loaded + nrows - 1)
+        self.beginInsertRows(
+            QtCore.QModelIndex(),
+            self.rows_loaded,
+            self.rows_loaded + nrows - 1,
+        )
         self.total_rows += nrows
         self.rows_loaded += nrows
         self.endInsertRows()
         self._parent.rows_inserted.emit(irow, nrows)
 
 
 class FrozenTableView(QTableView):
     """This class implements a table with its first column frozen
     For more information please see:
     http://doc.qt.io/qt-5/qtwidgets-itemviews-frozencolumn-example.html"""
+
     def __init__(self, parent):
         """Constructor."""
         QTableView.__init__(self, parent)
         self.parent = parent
         self.setModel(parent.model())
         self.setFocusPolicy(Qt.NoFocus)
         self.verticalHeader().hide()
@@ -406,27 +442,30 @@
         self.setColumnWidth(0, parent.columnWidth(0))
         self.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
         self.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
         self.show()
         self.setVerticalScrollMode(QTableView.ScrollPerPixel)
 
         self.verticalScrollBar().valueChanged.connect(
-            parent.verticalScrollBar().setValue)
+            parent.verticalScrollBar().setValue
+        )
         parent.verticalScrollBar().valueChanged.connect(
-            self.verticalScrollBar().setValue)
+            self.verticalScrollBar().setValue
+        )
 
     def update_geometry(self):
         """Update the frozen column size when an update occurs in its parent
         table"""
-        self.setGeometry(self.parent.verticalHeader().width() +
-                         self.parent.frameWidth(),
-                         self.parent.frameWidth(),
-                         self.parent.columnWidth(0),
-                         self.parent.viewport().height() +
-                         self.parent.horizontalHeader().height())
+        self.setGeometry(
+            self.parent.verticalHeader().width() + self.parent.frameWidth(),
+            self.parent.frameWidth(),
+            self.parent.columnWidth(0),
+            self.parent.viewport().height()
+            + self.parent.horizontalHeader().height(),
+        )
 
     def contextMenuEvent(self, event):
         """Show the context Menu
 
         Reimplemented to show the use the contextMenuEvent of the parent"""
         self.parent.contextMenuEvent(event)
 
@@ -454,27 +493,32 @@
         self.frozen_table_view = FrozenTableView(self)
         self.frozen_table_view.update_geometry()
 
         self.setHorizontalScrollMode(1)
         self.setVerticalScrollMode(1)
 
         self.horizontalHeader().sectionResized.connect(
-            self.update_section_width)
+            self.update_section_width
+        )
         self.verticalHeader().sectionResized.connect(
-            self.update_section_height)
+            self.update_section_height
+        )
 
         self.sort_old = [None]
         self.header_class = self.horizontalHeader()
         self.header_class.sectionClicked.connect(self.sortByColumn)
         self.frozen_table_view.horizontalHeader().sectionClicked.connect(
-            self.sortByColumn)
+            self.sortByColumn
+        )
         self.horizontalScrollBar().valueChanged.connect(
-                        lambda val: self.load_more_data(val, columns=True))
+            lambda val: self.load_more_data(val, columns=True)
+        )
         self.verticalScrollBar().valueChanged.connect(
-                        lambda val: self.load_more_data(val, rows=True))
+            lambda val: self.load_more_data(val, rows=True)
+        )
 
     def update_section_width(self, logical_index, old_size, new_size):
         """Update the horizontal width of the frozen column when a
         change takes place in the first column of the table"""
         if logical_index == 0:
             self.frozen_table_view.setColumnWidth(0, new_size)
             self.frozen_table_view.update_geometry()
@@ -497,24 +541,24 @@
         """Update the table position.
 
         Updates the position along with the frozen column
         when the cursor (selector) changes its position
         """
         current = QTableView.moveCursor(self, cursor_action, modifiers)
 
-        col_width = (self.columnWidth(0) +
-                     self.columnWidth(1))
+        col_width = self.columnWidth(0) + self.columnWidth(1)
         topleft_x = self.visualRect(current).topLeft().x()
 
         overflow = self.MoveLeft and current.column() > 1
         overflow = overflow and topleft_x < col_width
 
         if cursor_action == overflow:
-            new_value = (self.horizontalScrollBar().value() +
-                         topleft_x - col_width)
+            new_value = (
+                self.horizontalScrollBar().value() + topleft_x - col_width
+            )
             self.horizontalScrollBar().setValue(new_value)
         return current
 
     def scrollTo(self, index, hint):
         """Scroll the table.
 
         It is necessary to ensure that the item at index is visible.
@@ -528,15 +572,15 @@
     def load_more_data(self, value, rows=False, columns=False):
         if rows and value == self.verticalScrollBar().maximum():
             self.model().fetch_more(rows=rows)
         if columns and value == self.horizontalScrollBar().maximum():
             self.model().fetch_more(columns=columns)
 
     def sortByColumn(self, index):
-        """ Implement a Column sort """
+        """Implement a Column sort"""
         frozen_header = self.frozen_table_view.horizontalHeader()
         if not self.isSortingEnabled():
             self.header_class.setSortIndicatorShown(False)
             frozen_header.setSortIndicatorShown(False)
             return
         if self.sort_old == [None]:
             self.header_class.setSortIndicatorShown(True)
@@ -546,28 +590,30 @@
         else:
             sort_order = self.header_class.sortIndicatorOrder()
         if not self.model().sort(index, sort_order, True):
             if len(self.sort_old) != 2:
                 self.header_class.setSortIndicatorShown(False)
                 frozen_header.setSortIndicatorShown(False)
             else:
-                self.header_class.setSortIndicator(self.sort_old[0],
-                                                   self.sort_old[1])
+                self.header_class.setSortIndicator(
+                    self.sort_old[0], self.sort_old[1]
+                )
                 if index == 0:
-                    frozen_header.setSortIndicator(self.sort_old[0],
-                                                   self.sort_old[1])
+                    frozen_header.setSortIndicator(
+                        self.sort_old[0], self.sort_old[1]
+                    )
             return
         self.sort_old = [index, self.header_class.sortIndicatorOrder()]
 
     def change_type(self, func):
         """A function that changes types of cells"""
         model = self.model()
         index_list = self.selectedIndexes()
         for i in index_list:
-            model.setData(i, '', change_type=func)
+            model.setData(i, "", change_type=func)
 
     def insert_row_above_selection(self):
         """Insert rows above the selection
 
         The number of rows inserted depends on the number of selected rows"""
         rows, cols = self._selected_rows_and_cols()
         model = self.model()
@@ -597,15 +643,15 @@
 
     def _selected_rows_and_cols(self):
         index_list = self.selectedIndexes()
         if not index_list:
             return [], []
         return list(zip(*[(i.row(), i.column()) for i in index_list]))
 
-    docstrings.delete_params('DataFrameModel.parameters', 'parent')
+    docstrings.delete_params("DataFrameModel.parameters", "parent")
 
     @docstrings.dedent
     def set_df(self, df, *args, **kwargs):
         """
         Set the :class:`~pandas.DataFrame` for this table
 
         Parameters
@@ -621,44 +667,55 @@
 
     def contextMenuEvent(self, event):
         """Reimplement Qt method"""
         model = self.model()
         for a in self.dtype_actions.values():
             a.setEnabled(model.dtypes_changeable)
         nrows = max(len(set(self._selected_rows_and_cols()[0])), 1)
-        self.insert_row_above_action.setText('Insert %i row%s above' % (
-            nrows, 's' if nrows - 1 else ''))
-        self.insert_row_below_action.setText('Insert %i row%s below' % (
-            nrows, 's' if nrows - 1 else ''))
+        self.insert_row_above_action.setText(
+            "Insert %i row%s above" % (nrows, "s" if nrows - 1 else "")
+        )
+        self.insert_row_below_action.setText(
+            "Insert %i row%s below" % (nrows, "s" if nrows - 1 else "")
+        )
         self.insert_row_above_action.setEnabled(model.index_editable)
         self.insert_row_below_action.setEnabled(model.index_editable)
         self.menu.popup(event.globalPos())
         event.accept()
 
     def setup_menu(self):
         """Setup context menu"""
         menu = QMenu(self)
-        menu.addAction('Copy', self.copy, QtGui.QKeySequence.Copy)
+        menu.addAction("Copy", self.copy, QtGui.QKeySequence.Copy)
         menu.addSeparator()
-        functions = (("To bool", bool), ("To complex", complex),
-                     ("To int", int), ("To float", float),
-                     ("To str", str))
+        functions = (
+            ("To bool", bool),
+            ("To complex", complex),
+            ("To int", int),
+            ("To float", float),
+            ("To str", str),
+        )
         self.dtype_actions = {
             name: menu.addAction(name, partial(self.change_type, func))
-            for name, func in functions}
+            for name, func in functions
+        }
         menu.addSeparator()
         self.insert_row_above_action = menu.addAction(
-            'Insert rows above', self.insert_row_above_selection)
+            "Insert rows above", self.insert_row_above_selection
+        )
         self.insert_row_below_action = menu.addAction(
-            'Insert rows below', self.insert_row_below_selection)
+            "Insert rows below", self.insert_row_below_selection
+        )
         menu.addSeparator()
         self.set_index_action = menu.addAction(
-            'Set as index', partial(self.set_index, False))
+            "Set as index", partial(self.set_index, False)
+        )
         self.append_index_action = menu.addAction(
-            'Append to as index', partial(self.set_index, True))
+            "Append to as index", partial(self.set_index, True)
+        )
         return menu
 
     def set_index(self, append=False):
         """Set the index from the selected columns"""
         model = self.model()
         df = model.df
         args = [model.dtypes_changeable, model.index_editable]
@@ -668,16 +725,17 @@
             df.reset_index(inplace=True)
         else:
             cols -= 1
         cols = cols.tolist()
         if len(cols) == 1:
             df.set_index(df.columns[cols[0]], inplace=True, append=append)
         else:
-            df.set_index(df.columns[cols].tolist(), inplace=True,
-                         append=append)
+            df.set_index(
+                df.columns[cols].tolist(), inplace=True, append=append
+            )
         self.set_df(df, *args)
 
     def copy(self):
         """Copy text to clipboard"""
         rows, cols = self._selected_rows_and_cols()
         if not rows and not cols:
             return
@@ -685,26 +743,29 @@
         col_min, col_max = min(cols), max(cols)
         index = header = False
         if col_min == 0:
             col_min = 1
             index = True
         df = self.model().df
         if col_max == 0:  # To copy indices
-            contents = '\n'.join(map(str, df.index.tolist()[slice(row_min,
-                                                            row_max+1)]))
+            contents = "\n".join(
+                map(str, df.index.tolist()[slice(row_min, row_max + 1)])
+            )
         else:  # To copy DataFrame
             if (col_min == 0 or col_min == 1) and (df.shape[1] == col_max):
                 header = True
-            obj = df.iloc[slice(row_min, row_max+1), slice(col_min-1, col_max)]
+            obj = df.iloc[
+                slice(row_min, row_max + 1), slice(col_min - 1, col_max)
+            ]
             output = io.StringIO()
-            obj.to_csv(output, sep='\t', index=index, header=header)
+            obj.to_csv(output, sep="\t", index=index, header=header)
             if not six.PY2:
                 contents = output.getvalue()
             else:
-                contents = output.getvalue().decode('utf-8')
+                contents = output.getvalue().decode("utf-8")
             output.close()
         clipboard = QApplication.clipboard()
         clipboard.setText(contents)
 
 
 class DataFrameDock(QDockWidget):
     """The QDockWidget for the :class:`DataFrameEditor`"""
@@ -718,15 +779,15 @@
             mainwindow.dataframeeditors.remove(self.widget())
         except Exception:
             pass
         try:
             mainwindow.removeDockWidget(self)
         except Exception:
             pass
-        if getattr(self.widget(), '_view_action', None) is not None:
+        if getattr(self.widget(), "_view_action", None) is not None:
             mainwindow.dataframe_menu.removeAction(self.widget()._view_action)
         return super(DataFrameDock, self).close()
 
 
 class DataFrameEditor(DockMixin, QWidget):
     """An editor for data frames"""
 
@@ -753,54 +814,55 @@
         super(DataFrameEditor, self).__init__(*args, **kwargs)
         self.error_msg = PyErrorMessage(self)
 
         # Label for displaying the DataFrame size
         self.lbl_size = QLabel()
 
         # A Checkbox for enabling and disabling the editability of the index
-        self.cb_index_editable = QCheckBox('Index editable')
+        self.cb_index_editable = QCheckBox("Index editable")
 
         # A checkbox for enabling and disabling the change of data types
-        self.cb_dtypes_changeable = QCheckBox('Datatypes changeable')
+        self.cb_dtypes_changeable = QCheckBox("Datatypes changeable")
 
         # A checkbox for enabling and disabling sorting
-        self.cb_enable_sort = QCheckBox('Enable sorting')
+        self.cb_enable_sort = QCheckBox("Enable sorting")
 
         # A button to open a dataframe from the file
         self.btn_open_df = QToolButton(parent=self)
-        self.btn_open_df.setIcon(QIcon(get_icon('run_arrow.png')))
-        self.btn_open_df.setToolTip('Open a DataFrame from your disk')
+        self.btn_open_df.setIcon(QIcon(get_icon("run_arrow.png")))
+        self.btn_open_df.setToolTip("Open a DataFrame from your disk")
 
         self.btn_from_console = LoadFromConsoleButton(pd.DataFrame)
-        self.btn_from_console.setToolTip('Show a DataFrame from the console')
+        self.btn_from_console.setToolTip("Show a DataFrame from the console")
 
         # The table to display the DataFrame
         self.table = DataFrameView(pd.DataFrame(), self)
 
         # format line edit
         self.format_editor = QLineEdit()
         self.format_editor.setText(self.table.model()._format)
 
         # format update button
-        self.btn_change_format = QPushButton('Update')
+        self.btn_change_format = QPushButton("Update")
         self.btn_change_format.setEnabled(False)
 
         # table clearing button
-        self.btn_clear = QPushButton('Clear')
+        self.btn_clear = QPushButton("Clear")
         self.btn_clear.setToolTip(
-            'Clear the table and disconnect from the DataFrame')
+            "Clear the table and disconnect from the DataFrame"
+        )
 
         # refresh button
         self.btn_refresh = QToolButton()
-        self.btn_refresh.setIcon(QIcon(get_icon('refresh.png')))
-        self.btn_refresh.setToolTip('Refresh the table')
+        self.btn_refresh.setIcon(QIcon(get_icon("refresh.png")))
+        self.btn_refresh.setToolTip("Refresh the table")
 
         # close button
-        self.btn_close = QPushButton('Close')
-        self.btn_close.setToolTip('Close this widget permanentely')
+        self.btn_close = QPushButton("Close")
+        self.btn_close.setToolTip("Close this widget permanentely")
 
         # ---------------------------------------------------------------------
         # ------------------------ layout --------------------------------
         # ---------------------------------------------------------------------
         vbox = QVBoxLayout()
         self.top_hbox = hbox = QHBoxLayout()
         hbox.addWidget(self.cb_index_editable)
@@ -822,48 +884,50 @@
         vbox.addLayout(hbox)
         self.setLayout(vbox)
 
         # ---------------------------------------------------------------------
         # ------------------------ Connections --------------------------------
         # ---------------------------------------------------------------------
         self.cb_dtypes_changeable.stateChanged.connect(
-            self.set_dtypes_changeable)
+            self.set_dtypes_changeable
+        )
         self.cb_index_editable.stateChanged.connect(self.set_index_editable)
         self.btn_from_console.object_loaded.connect(self._open_ds_from_console)
         self.rows_inserted.connect(lambda i, n: self.set_lbl_size_text())
         self.format_editor.textChanged.connect(self.toggle_fmt_button)
         self.btn_change_format.clicked.connect(self.update_format)
         self.btn_clear.clicked.connect(self.clear_table)
         self.btn_close.clicked.connect(self.clear_table)
         self.btn_close.clicked.connect(lambda: self.close())
         self.btn_refresh.clicked.connect(self.table.reset_model)
         self.btn_open_df.clicked.connect(self._open_dataframe)
         self.table.set_index_action.triggered.connect(
-            self.update_index_editable)
+            self.update_index_editable
+        )
         self.table.append_index_action.triggered.connect(
-            self.update_index_editable)
-        self.cb_enable_sort.stateChanged.connect(
-            self.table.setSortingEnabled)
+            self.update_index_editable
+        )
+        self.cb_enable_sort.stateChanged.connect(self.table.setSortingEnabled)
 
     def update_index_editable(self):
         model = self.table.model()
         if len(model.df.index.names) > 1:
             model.index_editable = False
             self.cb_index_editable.setEnabled(False)
         self.cb_index_editable.setChecked(model.index_editable)
 
     def set_lbl_size_text(self, nrows=None, ncols=None):
         """Set the text of the :attr:`lbl_size` label to display the size"""
         model = self.table.model()
         nrows = nrows if nrows is not None else model.rowCount()
         ncols = ncols if ncols is not None else model.columnCount()
         if not nrows and not ncols:
-            self.lbl_size.setText('')
+            self.lbl_size.setText("")
         else:
-            self.lbl_size.setText('Rows: %i, Columns: %i' % (nrows, ncols))
+            self.lbl_size.setText("Rows: %i, Columns: %i" % (nrows, ncols))
 
     def clear_table(self):
         """Clear the table and emit the :attr:`cleared` signal"""
         df = pd.DataFrame()
         self.set_df(df, show=False)
 
     def _open_ds_from_console(self, oname, df):
@@ -876,15 +940,15 @@
 
         Parameters
         ----------
         %(DataFrameModel.parameters.no_parent)s
         show: bool
             If True (default), show and raise_ the editor
         """
-        show = kwargs.pop('show', True)
+        show = kwargs.pop("show", True)
         self.table.set_df(df, *args, **kwargs)
         self.set_lbl_size_text(*df.shape)
         model = self.table.model()
         self.cb_dtypes_changeable.setChecked(model.dtypes_changeable)
 
         if len(model.df.index.names) > 1:
             model.index_editable = False
@@ -908,66 +972,72 @@
     def toggle_fmt_button(self, text):
         try:
             text % 1.1
         except (TypeError, ValueError):
             self.btn_change_format.setEnabled(False)
         else:
             self.btn_change_format.setEnabled(
-                text.strip() != self.table.model()._format)
+                text.strip() != self.table.model()._format
+            )
 
     def update_format(self):
         """Update the format of the table"""
         self.table.model().set_format(self.format_editor.text().strip())
 
     def to_dock(self, main, *args, **kwargs):
         connect = self.dock is None
         super(DataFrameEditor, self).to_dock(main, *args, **kwargs)
         if connect:
             self.dock.toggleViewAction().triggered.connect(self.maybe_tabify)
 
     def maybe_tabify(self):
         main = self.dock.parent()
         if self.is_shown and main.dockWidgetArea(
-                main.help_explorer.dock) == main.dockWidgetArea(self.dock):
+            main.help_explorer.dock
+        ) == main.dockWidgetArea(self.dock):
             main.tabifyDockWidget(main.help_explorer.dock, self.dock)
 
     def _open_dataframe(self):
         self.open_dataframe()
 
     def open_dataframe(self, fname=None, *args, **kwargs):
         """Opens a file dialog and the dataset that has been inserted"""
         if fname is None:
             fname = QFileDialog.getOpenFileName(
-                self, 'Open dataset', os.getcwd(),
-                'Comma separated files (*.csv);;'
-                'Excel files (*.xls *.xlsx);;'
-                'JSON files (*.json);;'
-                'All files (*)'
-                )
+                self,
+                "Open dataset",
+                os.getcwd(),
+                "Comma separated files (*.csv);;"
+                "Excel files (*.xls *.xlsx);;"
+                "JSON files (*.json);;"
+                "All files (*)",
+            )
             if with_qt5:  # the filter is passed as well
                 fname = fname[0]
         if isinstance(fname, pd.DataFrame):
             self.set_df(fname)
         elif not fname:
             return
         else:
             ext = osp.splitext(fname)[1]
             open_funcs = {
-                '.xls': pd.read_excel, '.xlsx': pd.read_excel,
-                '.json': pd.read_json,
-                '.tab': partial(pd.read_csv, delimiter='\t'),
-                '.dat': partial(pd.read_csv, delim_whitespace=True),
-                }
+                ".xls": pd.read_excel,
+                ".xlsx": pd.read_excel,
+                ".json": pd.read_json,
+                ".tab": partial(pd.read_csv, delimiter="\t"),
+                ".dat": partial(pd.read_csv, delim_whitespace=True),
+            }
             open_func = open_funcs.get(ext, pd.read_csv)
             try:
                 df = open_func(fname)
             except Exception:
                 self.error_msg.showTraceback(
-                    '<b>Could not open DataFrame %s with %s</b>' % (
-                        fname, open_func))
+                    "<b>Could not open DataFrame %s with %s</b>"
+                    % (fname, open_func)
+                )
                 return
             self.set_df(df)
 
     def close(self, *args, **kwargs):
         if self.dock is not None:
             self.dock.close(*args, **kwargs)  # removes the dock window
             del self.dock
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/dependencies.py` & `psyplot-gui-1.5.0/psyplot_gui/dependencies.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,62 @@
 """Dependencies widget of the psyplot package
 
 This module defines the :class:`DependenciesWidget` that shows the versions of
 of psyplot, psyplot_gui, psyplot plugins and their requirements"""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-from psyplot_gui.compat.qtcompat import (
-    QDialog, QTreeWidget, QTreeWidgetItem, QVBoxLayout, QLabel, QMenu, QAction,
-    Qt, QApplication, QMessageBox, QPushButton, QHBoxLayout, QAbstractItemView,
-    QDialogButtonBox, QtCore)
 from psyplot.docstring import docstrings
 
+from psyplot_gui.compat.qtcompat import (
+    QAbstractItemView,
+    QAction,
+    QApplication,
+    QDialog,
+    QDialogButtonBox,
+    QHBoxLayout,
+    QLabel,
+    QMenu,
+    QMessageBox,
+    QPushButton,
+    Qt,
+    QtCore,
+    QTreeWidget,
+    QTreeWidgetItem,
+    QVBoxLayout,
+)
+
 
 class DependenciesTree(QTreeWidget):
     """A tree widget to display dependencies
 
     This widget uses a dictionary as created through the
     :func:`psyplot.get_versions` function to display the requirements and
     versions."""
 
-    @docstrings.get_sections(base='DependenciesTree')
+    @docstrings.get_sections(base="DependenciesTree")
     def __init__(self, versions, *args, **kwargs):
         """
         Parameters
         ----------
         versions: dict
             The dictionary that contains the version information
 
         See Also
         --------
         psyplot.get_versions
         """
         super(DependenciesTree, self).__init__(*args, **kwargs)
         self.resizeColumnToContents(0)
         self.setColumnCount(2)
-        self.setHeaderLabels(['Package', 'installed version'])
+        self.setHeaderLabels(["Package", "installed version"])
         self.add_dependencies(versions)
         self.expandAll()
         self.resizeColumnToContents(0)
         self.setContextMenuPolicy(Qt.CustomContextMenu)
         self.customContextMenuRequested.connect(self.open_menu)
 
     @docstrings.dedent
@@ -78,36 +75,36 @@
             `versions`. If None, the newly created items are inserted as
             top level items into the tree
         """
         for pkg, pkg_d in versions.items():
             new_item = QTreeWidgetItem(0)
             new_item.setText(0, pkg)
             if isinstance(pkg_d, dict):
-                new_item.setText(1, pkg_d['version'])
+                new_item.setText(1, pkg_d["version"])
             else:
                 new_item.setText(1, pkg_d)
             if parent is None:
                 self.addTopLevelItem(new_item)
             else:
                 parent.addChild(new_item)
-            if 'requirements' in pkg_d:
-                self.add_dependencies(pkg_d['requirements'], new_item)
+            if "requirements" in pkg_d:
+                self.add_dependencies(pkg_d["requirements"], new_item)
 
     def open_menu(self, position):
         """Open a menu to expand and collapse all items in the tree
 
         Parameters
         ----------
         position: QPosition
             The position where to open the menu"""
         menu = QMenu()
-        expand_all_action = QAction('Expand all', self)
+        expand_all_action = QAction("Expand all", self)
         expand_all_action.triggered.connect(self.expandAll)
         menu.addAction(expand_all_action)
-        collapse_all_action = QAction('Collapse all', self)
+        collapse_all_action = QAction("Collapse all", self)
         collapse_all_action.triggered.connect(self.collapseAll)
         menu.addAction(collapse_all_action)
         menu.exec_(self.viewport().mapToGlobal(position))
 
 
 class DependenciesDialog(QDialog):
     """A dialog for displaying the dependencies"""
@@ -134,66 +131,72 @@
     def __init__(self, versions, *args, **kwargs):
         """
         Parameters
         ----------
         %(DependenciesTree.parameters)s
         """
         super(DependenciesDialog, self).__init__(*args, **kwargs)
-        self.setWindowTitle('Dependencies')
+        self.setWindowTitle("Dependencies")
         self.versions = versions
         self.vbox = layout = QVBoxLayout()
 
-        self.label = QLabel("""
+        self.label = QLabel(
+            """
             psyplot and the plugins depend on several python libraries. The
             tree widget below lists the versions of the plugins and the
             requirements. You can select the items in the tree and copy them to
-            clipboard.""", parent=self)
+            clipboard.""",
+            parent=self,
+        )
 
         layout.addWidget(self.label)
 
         self.tree = DependenciesTree(versions, parent=self)
         self.tree.setSelectionMode(QAbstractItemView.MultiSelection)
         layout.addWidget(self.tree)
 
         # copy button
-        self.bt_copy = QPushButton('Copy selection to clipboard')
+        self.bt_copy = QPushButton("Copy selection to clipboard")
         self.bt_copy.setToolTip(
-            'Copy the selected packages in the above table to the clipboard.')
+            "Copy the selected packages in the above table to the clipboard."
+        )
         self.bt_copy.clicked.connect(lambda: self.copy_selected())
 
         self.bbox = QDialogButtonBox(QDialogButtonBox.Ok)
         self.bbox.accepted.connect(self.accept)
 
         hbox = QHBoxLayout()
         hbox.addWidget(self.bt_copy)
         hbox.addStretch(1)
         hbox.addWidget(self.bbox)
         layout.addLayout(hbox)
 
         #: A label for simple status update
-        self.info_label = QLabel('', self)
+        self.info_label = QLabel("", self)
         layout.addWidget(self.info_label)
         self.timer = QtCore.QTimer(self)
         self.timer.timeout.connect(self.clear_label)
 
         self.setLayout(layout)
 
     def copy_selected(self, label=None):
         """Copy the selected versions and items to the clipboard"""
         d = {}
         items = self.tree.selectedItems()
         if not items:
-            QMessageBox.warning(self, "No packages selected!",
-                                "Please select packages in the tree!")
+            QMessageBox.warning(
+                self,
+                "No packages selected!",
+                "Please select packages in the tree!",
+            )
             return
         for item in items:
             d[item.text(0)] = item.text(1)
         if label is None:
             label = QApplication.clipboard()
-        label.setText("\n".join(
-            '%s: %s' % t for t in d.items()))
-        self.info_label.setText('Packages copied to clipboard.')
+        label.setText("\n".join("%s: %s" % t for t in d.items()))
+        self.info_label.setText("Packages copied to clipboard.")
         self.timer.start(3000)
 
     def clear_label(self):
         """Clear the info label"""
-        self.info_label.setText('')
+        self.info_label.setText("")
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/fmt_widget.py` & `psyplot-gui-1.5.0/psyplot_gui/fmt_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,77 +1,74 @@
 # -*- coding: utf-8 -*-
 """Module defining a widget for updating the formatoption of the current
 project"""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import six
-import yaml
-from functools import partial
+import logging
 from collections import defaultdict
+from functools import partial
 from itertools import chain
-import logging
 from warnings import warn
-from IPython.core.interactiveshell import ExecutionResult
+
+import psyplot.plotter as psyp
 import psyplot.project as psy
+import six
+import yaml
+from IPython.core.interactiveshell import ExecutionResult
+from psyplot.data import isstring, safe_list
 from psyplot.utils import _temp_bool_prop, unique_everseen
+
+from psyplot_gui.common import DockMixin, PyErrorMessage, get_icon
 from psyplot_gui.compat.qtcompat import (
-    QWidget, QHBoxLayout, QComboBox, QLineEdit, QVBoxLayout, QToolButton,
-    QIcon, QPushButton, QCheckBox, QTextEdit, QListView, QCompleter, Qt,
-    QStandardItemModel, QStandardItem, with_qt5)
-from psyplot_gui.plot_creator import CoordComboBox
+    QCheckBox,
+    QComboBox,
+    QCompleter,
+    QHBoxLayout,
+    QIcon,
+    QLineEdit,
+    QListView,
+    QPushButton,
+    QStandardItem,
+    QStandardItemModel,
+    Qt,
+    QTextEdit,
+    QToolButton,
+    QVBoxLayout,
+    QWidget,
+    with_qt5,
+)
 from psyplot_gui.config.rcsetup import rcParams
-from psyplot.compat.pycompat import OrderedDict, map
-from psyplot_gui.common import DockMixin, get_icon, PyErrorMessage
-from psyplot.data import safe_list
-import psyplot.plotter as psyp
-from psyplot.data import isstring
+from psyplot_gui.plot_creator import CoordComboBox
 
 try:
     from IPython.core.interactiveshell import ExecutionInfo
 except ImportError:
     ExecutionInfo = None
 
 
 logger = logging.getLogger(__name__)
 
 
-COORDSGROUP = '__coords'
-ALLGROUP = '__all'
+COORDSGROUP = "__coords"
+ALLGROUP = "__all"
 
 
 class DimensionsWidget(QWidget):
     """A widget for updating the dimensions"""
 
     def __init__(self, parent, dim=None):
         super(DimensionsWidget, self).__init__(parent)
         self.coord_combo = CoordComboBox(self.get_ds, dim)
-        self.cb_use_coord = QCheckBox('show coordinates')
-        self.cb_close_popups = QCheckBox('close dropdowns')
+        self.cb_use_coord = QCheckBox("show coordinates")
+        self.cb_close_popups = QCheckBox("close dropdowns")
         self.cb_close_popups.setChecked(True)
         self.toggle_close_popup()
         self._single_selection = False
 
         self.dim = dim
         hbox = QHBoxLayout()
         hbox.addWidget(self.cb_close_popups)
@@ -100,51 +97,56 @@
         self.coord_combo.close_popups = self.cb_close_popups.isChecked()
 
     def insert_from_combo(self):
         cb = self.coord_combo
         inserts = list(
             ind.row() - 1
             for ind in cb.view().selectionModel().selectedIndexes()
-            if ind.row() > 0)
+            if ind.row() > 0
+        )
         if not inserts:
             return
         elif not self._single_selection:
             try:
-                current = yaml.load(self.parent().get_text(),
-                                    Loader=yaml.Loader)
+                current = yaml.load(
+                    self.parent().get_text(), Loader=yaml.Loader
+                )
             except Exception:
                 pass
             else:
                 if current:
                     current = self.slice2list(current)
                     inserts = sorted(set(chain(inserts, safe_list(current))))
         else:
             inserts = inserts[0]
 
         self.parent().set_obj(inserts)
 
     def get_ds(self):
         import psyplot.project as psy
+
         project = psy.gcp()
         datasets = project.datasets
         dim = self.dim
         dims = {ds.coords[dim].shape[0]: ds for ds in datasets.values()}
         if len(dims) > 1:
-            warn("Datasets have differing dimensions lengths for the "
-                 "%s dimension!" % dim)
+            warn(
+                "Datasets have differing dimensions lengths for the "
+                "%s dimension!" % dim
+            )
         return min(dims.items())[1]
 
     def set_single_selection(self, yes=True):
         self._single_selection = yes
         if yes:
-            self.coord_combo.view().setSelectionMode(
-                QListView.SingleSelection)
+            self.coord_combo.view().setSelectionMode(QListView.SingleSelection)
         else:
             self.coord_combo.view().setSelectionMode(
-                QListView.ExtendedSelection)
+                QListView.ExtendedSelection
+            )
 
 
 class FormatoptionWidget(QWidget, DockMixin):
     """
     Widget to update the formatoptions of the current project
 
     This widget, mainly made out of a combobox for the formatoption group,
@@ -155,15 +157,16 @@
     signal and refills the comboboxes if the current subproject changes.
 
     The text editor either accepts python code that will be executed by the
     given `console`, or yaml code.
     """
 
     no_fmtos_update = _temp_bool_prop(
-        'no_fmtos_update', """update the fmto combo box or not""")
+        "no_fmtos_update", """update the fmto combo box or not"""
+    )
 
     #: The combobox for the formatoption groups
     group_combo = None
 
     #: The combobox for the formatoptions
     fmt_combo = None
 
@@ -201,16 +204,16 @@
 
             where ``**kwargs`` is defined through the selected formatoption
             in the :attr:`fmt_combo` combobox and the value in the
             :attr:`line_edit` editor
         ``*args, **kwargs``
             Any other keyword for the QWidget class
         """
-        help_explorer = kwargs.pop('help_explorer', None)
-        console = kwargs.pop('console', None)
+        help_explorer = kwargs.pop("help_explorer", None)
+        console = kwargs.pop("console", None)
         super(FormatoptionWidget, self).__init__(*args, **kwargs)
         self.help_explorer = help_explorer
         self.console = console
         self.error_msg = PyErrorMessage(self)
 
         # ---------------------------------------------------------------------
         # -------------------------- Child widgets ----------------------------
@@ -221,97 +224,110 @@
         self.text_edit = QTextEdit(parent=self)
         self.run_button = QToolButton(parent=self)
 
         # completer for the fmto widget
         self.fmt_combo.setEditable(True)
         self.fmt_combo.setInsertPolicy(QComboBox.NoInsert)
         self.fmto_completer = completer = QCompleter(
-            ['time', 'lat', 'lon', 'lev'])
-        completer.setCompletionMode(
-            QCompleter.PopupCompletion)
+            ["time", "lat", "lon", "lev"]
+        )
+        completer.setCompletionMode(QCompleter.PopupCompletion)
         completer.activated[str].connect(self.set_fmto)
         if with_qt5:
             completer.setFilterMode(Qt.MatchContains)
         completer.setModel(QStandardItemModel())
         self.fmt_combo.setCompleter(completer)
 
         self.dim_widget = DimensionsWidget(parent=self)
         self.dim_widget.setVisible(False)
 
-        self.multiline_button = QPushButton('Multiline', parent=self)
+        self.multiline_button = QPushButton("Multiline", parent=self)
         self.multiline_button.setCheckable(True)
 
-        self.yaml_cb = QCheckBox('Yaml syntax')
+        self.yaml_cb = QCheckBox("Yaml syntax")
         self.yaml_cb.setChecked(True)
 
-        self.keys_button = QPushButton('Keys', parent=self)
-        self.summaries_button = QPushButton('Summaries', parent=self)
-        self.docs_button = QPushButton('Docs', parent=self)
-
-        self.grouped_cb = QCheckBox('grouped', parent=self)
-        self.all_groups_cb = QCheckBox('all groups', parent=self)
-        self.include_links_cb = QCheckBox('include links', parent=self)
+        self.keys_button = QPushButton("Keys", parent=self)
+        self.summaries_button = QPushButton("Summaries", parent=self)
+        self.docs_button = QPushButton("Docs", parent=self)
+
+        self.grouped_cb = QCheckBox("grouped", parent=self)
+        self.all_groups_cb = QCheckBox("all groups", parent=self)
+        self.include_links_cb = QCheckBox("include links", parent=self)
 
         self.text_edit.setVisible(False)
 
         # ---------------------------------------------------------------------
         # -------------------------- Descriptions -----------------------------
         # ---------------------------------------------------------------------
 
-        self.group_combo.setToolTip('Select the formatoption group')
-        self.fmt_combo.setToolTip('Select the formatoption to update')
+        self.group_combo.setToolTip("Select the formatoption group")
+        self.fmt_combo.setToolTip("Select the formatoption to update")
         self.line_edit.setToolTip(
-            'Insert the value which what you want to update the selected '
-            'formatoption and hit right button. The code is executed in the '
-            'main console.')
+            "Insert the value which what you want to update the selected "
+            "formatoption and hit right button. The code is executed in the "
+            "main console."
+        )
         self.yaml_cb.setToolTip(
             "Use the yaml syntax for the values inserted in the above cell. "
             "Otherwise the content there is evaluated as a python expression "
-            "in the terminal")
+            "in the terminal"
+        )
         self.text_edit.setToolTip(self.line_edit.toolTip())
-        self.run_button.setIcon(QIcon(get_icon('run_arrow.png')))
-        self.run_button.setToolTip('Update the selected formatoption')
+        self.run_button.setIcon(QIcon(get_icon("run_arrow.png")))
+        self.run_button.setToolTip("Update the selected formatoption")
         self.multiline_button.setToolTip(
-            'Allow linebreaks in the text editor line above.')
+            "Allow linebreaks in the text editor line above."
+        )
         self.keys_button.setToolTip(
-            'Show the formatoption keys in this group (or in all '
-            'groups) in the help explorer')
+            "Show the formatoption keys in this group (or in all "
+            "groups) in the help explorer"
+        )
         self.summaries_button.setToolTip(
-            'Show the formatoption summaries in this group (or in all '
-            'groups) in the help explorer')
+            "Show the formatoption summaries in this group (or in all "
+            "groups) in the help explorer"
+        )
         self.docs_button.setToolTip(
-            'Show the formatoption documentations in this group (or in all '
-            'groups) in the help explorer')
+            "Show the formatoption documentations in this group (or in all "
+            "groups) in the help explorer"
+        )
         self.grouped_cb.setToolTip(
-            'Group the formatoptions before displaying them in the help '
-            'explorer')
-        self.all_groups_cb.setToolTip('Use all groups when displaying the '
-                                      'keys, docs or summaries')
+            "Group the formatoptions before displaying them in the help "
+            "explorer"
+        )
+        self.all_groups_cb.setToolTip(
+            "Use all groups when displaying the " "keys, docs or summaries"
+        )
         self.include_links_cb.setToolTip(
-            'Include links to remote documentations when showing the '
-            'keys, docs and summaries in the help explorer (requires '
-            'intersphinx)')
+            "Include links to remote documentations when showing the "
+            "keys, docs and summaries in the help explorer (requires "
+            "intersphinx)"
+        )
 
         # ---------------------------------------------------------------------
         # -------------------------- Connections ------------------------------
         # ---------------------------------------------------------------------
         self.group_combo.currentIndexChanged[int].connect(self.fill_fmt_combo)
         self.fmt_combo.currentIndexChanged[int].connect(self.show_fmt_info)
         self.fmt_combo.currentIndexChanged[int].connect(self.load_fmt_widget)
         self.fmt_combo.currentIndexChanged[int].connect(
-            self.set_current_fmt_value)
+            self.set_current_fmt_value
+        )
         self.run_button.clicked.connect(self.run_code)
         self.line_edit.returnPressed.connect(self.run_button.click)
         self.multiline_button.clicked.connect(self.toggle_line_edit)
         self.keys_button.clicked.connect(
-            partial(self.show_all_fmt_info, 'keys'))
+            partial(self.show_all_fmt_info, "keys")
+        )
         self.summaries_button.clicked.connect(
-            partial(self.show_all_fmt_info, 'summaries'))
+            partial(self.show_all_fmt_info, "summaries")
+        )
         self.docs_button.clicked.connect(
-            partial(self.show_all_fmt_info, 'docs'))
+            partial(self.show_all_fmt_info, "docs")
+        )
 
         # ---------------------------------------------------------------------
         # ------------------------------ Layouts ------------------------------
         # ---------------------------------------------------------------------
         self.combos = QHBoxLayout()
         self.combos.addWidget(self.group_combo)
         self.combos.addWidget(self.fmt_combo)
@@ -321,16 +337,22 @@
         self.execs.addWidget(self.text_edit)
         self.execs.addWidget(self.run_button)
 
         self.info_box = QHBoxLayout()
         self.info_box.addWidget(self.multiline_button)
         self.info_box.addWidget(self.yaml_cb)
         self.info_box.addStretch(0)
-        for w in [self.keys_button, self.summaries_button, self.docs_button,
-                  self.all_groups_cb, self.grouped_cb, self.include_links_cb]:
+        for w in [
+            self.keys_button,
+            self.summaries_button,
+            self.docs_button,
+            self.all_groups_cb,
+            self.grouped_cb,
+            self.include_links_cb,
+        ]:
             self.info_box.addWidget(w)
 
         self.vbox = QVBoxLayout()
         self.vbox.addLayout(self.combos)
         self.vbox.addWidget(self.dim_widget)
         self.vbox.addLayout(self.execs)
         self.vbox.addLayout(self.info_box)
@@ -338,30 +360,33 @@
         self.vbox.setSpacing(0)
 
         self.setLayout(self.vbox)
 
         # fill with content
         self.fill_combos_from_project(psy.gcp())
         psy.Project.oncpchange.connect(self.fill_combos_from_project)
-        rcParams.connect('fmt.sort_by_key', self.refill_from_rc)
+        rcParams.connect("fmt.sort_by_key", self.refill_from_rc)
 
     def refill_from_rc(self, sort_by_key):
         from psyplot.project import gcp
+
         self.fill_combos_from_project(gcp())
 
     def fill_combos_from_project(self, project):
         """Fill :attr:`group_combo` and :attr:`fmt_combo` from a project
 
         Parameters
         ----------
         project: psyplot.project.Project
             The project to use"""
-        if rcParams['fmt.sort_by_key']:
+        if rcParams["fmt.sort_by_key"]:
+
             def sorter(fmto):
                 return fmto.key
+
         else:
             sorter = self.get_name
 
         current_text = self.group_combo.currentText()
         with self.no_fmtos_update:
             self.group_combo.clear()
             if project is None or project.is_main or not len(project):
@@ -369,64 +394,72 @@
                 self.groups = []
                 self.fmtos = []
                 self.line_edit.setEnabled(False)
                 return
             self.line_edit.setEnabled(True)
             # get dimensions
             it_vars = chain.from_iterable(
-                arr.psy.iter_base_variables for arr in project.arrays)
+                arr.psy.iter_base_variables for arr in project.arrays
+            )
             dims = next(it_vars).dims
             sdims = set(dims)
             for var in it_vars:
                 sdims.intersection_update(var.dims)
             coords = [d for d in dims if d in sdims]
             coords_name = [COORDSGROUP] if coords else []
-            coords_verbose = ['Dimensions'] if coords else []
+            coords_verbose = ["Dimensions"] if coords else []
             coords = [coords] if coords else []
 
             if len(project.plotters):
                 # get formatoptions and group them alphabetically
                 grouped_fmts = defaultdict(list)
                 for fmto in project._fmtos:
                     grouped_fmts[fmto.group].append(fmto)
                 for val in six.itervalues(grouped_fmts):
                     val.sort(key=sorter)
-                grouped_fmts = OrderedDict(
-                    sorted(six.iteritems(grouped_fmts),
-                           key=lambda t: psyp.groups.get(t[0], t[0])))
+                grouped_fmts = dict(
+                    sorted(
+                        six.iteritems(grouped_fmts),
+                        key=lambda t: psyp.groups.get(t[0], t[0]),
+                    )
+                )
                 fmt_groups = list(grouped_fmts.keys())
                 # save original names
                 self.groups = coords_name + [ALLGROUP] + fmt_groups
                 # save verbose group names (which are used in the combo box)
                 self.groupnames = (
-                    coords_verbose + ['All formatoptions'] + list(
-                        map(lambda s: psyp.groups.get(s, s), fmt_groups)))
+                    coords_verbose
+                    + ["All formatoptions"]
+                    + list(map(lambda s: psyp.groups.get(s, s), fmt_groups))
+                )
                 # save formatoptions
                 fmtos = list(grouped_fmts.values())
-                self.fmtos = coords + [sorted(
-                    chain(*fmtos), key=sorter)] + fmtos
+                self.fmtos = (
+                    coords + [sorted(chain(*fmtos), key=sorter)] + fmtos
+                )
             else:
                 self.groups = coords_name
                 self.groupnames = coords_verbose
                 self.fmtos = coords
             self.group_combo.addItems(self.groupnames)
             ind = self.group_combo.findText(current_text)
             self.group_combo.setCurrentIndex(ind if ind >= 0 else 0)
         self.fill_fmt_combo(self.group_combo.currentIndex())
 
     def get_name(self, fmto):
         """Get the name of a :class:`psyplot.plotter.Formatoption` instance"""
         if isinstance(fmto, six.string_types):
             return fmto
-        return '%s (%s)' % (fmto.name, fmto.key) if fmto.name else fmto.key
+        return "%s (%s)" % (fmto.name, fmto.key) if fmto.name else fmto.key
 
     @property
     def fmto(self):
         return self.fmtos[self.group_combo.currentIndex()][
-            self.fmt_combo.currentIndex()]
+            self.fmt_combo.currentIndex()
+        ]
 
     @fmto.setter
     def fmto(self, value):
         name = self.get_name(value)
         for i, fmtos in enumerate(self.fmtos):
             if i == 1:  # all formatoptions
                 continue
@@ -440,50 +473,57 @@
         """Switch between the :attr:`line_edit` and :attr:`text_edit`
 
         This method is called when the :attr:`multiline_button` is clicked
         and switches between the single line :attr:``line_edit` and the
         multiline :attr:`text_edit`
         """
         # switch to multiline text edit
-        if (self.multiline_button.isChecked() and
-                not self.text_edit.isVisible()):
+        if (
+            self.multiline_button.isChecked()
+            and not self.text_edit.isVisible()
+        ):
             self.line_edit.setVisible(False)
             self.text_edit.setVisible(True)
             self.text_edit.setPlainText(self.line_edit.text())
-        elif (not self.multiline_button.isChecked() and
-              not self.line_edit.isVisible()):
+        elif (
+            not self.multiline_button.isChecked()
+            and not self.line_edit.isVisible()
+        ):
             self.line_edit.setVisible(True)
             self.text_edit.setVisible(False)
             self.line_edit.setText(self.text_edit.toPlainText())
 
     def fill_fmt_combo(self, i, current_text=None):
-        """Fill the :attr:`fmt_combo` combobox based on the current group name
-        """
+        """Fill the :attr:`fmt_combo` combobox based on the current group name"""
         if not self.no_fmtos_update:
             with self.no_fmtos_update:
                 if current_text is None:
                     current_text = self.fmt_combo.currentText()
                 self.fmt_combo.clear()
                 self.fmt_combo.addItems(
-                    list(map(self.get_name, self.fmtos[i])))
+                    list(map(self.get_name, self.fmtos[i]))
+                )
                 ind = self.fmt_combo.findText(current_text)
                 self.fmt_combo.setCurrentIndex(ind if ind >= 0 else 0)
                 # update completer model
                 self.setup_fmt_completion_model()
             idx = self.fmt_combo.currentIndex()
             self.show_fmt_info(idx)
             self.load_fmt_widget(idx)
             self.set_current_fmt_value(idx)
 
     def set_fmto(self, name):
         self.fmto = name
 
     def setup_fmt_completion_model(self):
-        fmtos = list(unique_everseen(map(
-            self.get_name, chain.from_iterable(self.fmtos))))
+        fmtos = list(
+            unique_everseen(
+                map(self.get_name, chain.from_iterable(self.fmtos))
+            )
+        )
         model = self.fmto_completer.model()
         model.setRowCount(len(fmtos))
         for i, name in enumerate(fmtos):
             model.setItem(i, QStandardItem(name))
 
     def load_fmt_widget(self, i):
         """Load the formatoption specific widget
@@ -496,20 +536,20 @@
         ----------
         i: int
             The index of the current formatoption"""
         self.remove_fmt_widget()
         group_ind = self.group_combo.currentIndex()
         if not self.no_fmtos_update:
             from psyplot.project import gcp
+
             if self.groups[group_ind] == COORDSGROUP:
                 dim = self.fmtos[group_ind][i]
                 self.fmt_widget = self.dim_widget
                 self.dim_widget.set_dim(dim)
-                self.dim_widget.set_single_selection(
-                    dim not in gcp()[0].dims)
+                self.dim_widget.set_single_selection(dim not in gcp()[0].dims)
                 self.dim_widget.setVisible(True)
             else:
                 fmto = self.fmtos[group_ind][i]
                 self.fmt_widget = fmto.get_fmt_widget(self, gcp())
                 if self.fmt_widget is not None:
                     self.vbox.insertWidget(2, self.fmt_widget)
 
@@ -530,53 +570,59 @@
 
     def set_current_fmt_value(self, i):
         """Add the value of the current formatoption to the line text"""
         group_ind = self.group_combo.currentIndex()
         if not self.no_fmtos_update:
             if self.groups[group_ind] == COORDSGROUP:
                 from psyplot.project import gcp
+
                 dim = self.fmtos[group_ind][i]
                 self.set_obj(gcp().arrays[0].psy.idims[dim])
             else:
                 fmto = self.fmtos[group_ind][i]
                 self.set_obj(fmto.value)
 
     def show_fmt_info(self, i):
-        """Show the documentation of the formatoption in the help explorer
-        """
+        """Show the documentation of the formatoption in the help explorer"""
         group_ind = self.group_combo.currentIndex()
-        if (not self.no_fmtos_update and
-                self.groups[group_ind] != COORDSGROUP):
+        if not self.no_fmtos_update and self.groups[group_ind] != COORDSGROUP:
             fmto = self.fmtos[self.group_combo.currentIndex()][i]
             fmto.plotter.show_docs(
-                fmto.key, include_links=self.include_links_cb.isChecked())
+                fmto.key, include_links=self.include_links_cb.isChecked()
+            )
 
     def run_code(self):
         """Run the update of the project inside the :attr:`shell`"""
         if self.line_edit.isVisible():
             text = str(self.line_edit.text())
         else:
             text = str(self.text_edit.toPlainText())
         if not text or not self.fmtos:
             return
         group_ind = self.group_combo.currentIndex()
         if self.groups[group_ind] == COORDSGROUP:
             key = self.fmtos[group_ind][self.fmt_combo.currentIndex()]
-            param = 'dims'
+            param = "dims"
         else:
             key = self.fmtos[group_ind][self.fmt_combo.currentIndex()].key
-            param = 'fmt'
+            param = "fmt"
         if self.yaml_cb.isChecked():
             import psyplot.project as psy
+
             psy.gcp().update(**{key: yaml.load(text, Loader=yaml.Loader)})
         else:
             code = "psy.gcp().update(%s={'%s': %s})" % (param, key, text)
             if ExecutionInfo is not None:
-                info = ExecutionInfo(raw_cell=code, store_history=False,
-                                     silent=True, shell_futures=False)
+                info = ExecutionInfo(
+                    raw_cell=code,
+                    store_history=False,
+                    silent=True,
+                    shell_futures=False,
+                    cell_id=None,
+                )
                 e = ExecutionResult(info)
             else:
                 e = ExecutionResult()
             self.console.run_command_in_shell(code, e)
             try:
                 e.raise_error()
             except Exception:  # reset the console and clear the error message
@@ -622,22 +668,22 @@
                 if current[0] in ['"', "'"]:
                     current = current[1:-1]
                 self.clear_text()
                 if pos == 0:
                     s = '"' + obj + current + '"'
                 else:
                     s = '"' + current + obj + '"'
-                current = ''
+                current = ""
         elif isstring(obj):  # add quotation marks
             s = '"' + obj + '"'
         elif not use_yaml:
             s = repr(obj)
         else:
             s = yaml.dump(obj, default_flow_style=True).strip()
-            if s.endswith('\n...'):
+            if s.endswith("\n..."):
                 s = s[:-4]
         if use_line_edit:
             self.line_edit.insert(s)
         else:
             self.text_edit.insertPlainText(s)
 
     def clear_text(self):
@@ -659,18 +705,26 @@
 
         Parameters
         ----------
         what: {'keys', 'summaries', 'docs'}
             Determines what to show"""
         if not self.fmtos:
             return
-        if (self.all_groups_cb.isChecked() or
-                self.group_combo.currentIndex() < 2):
-            fmtos = list(chain.from_iterable(
-                fmto_group for i, fmto_group in enumerate(self.fmtos)
-                if self.groups[i] not in [ALLGROUP, COORDSGROUP]))
+        if (
+            self.all_groups_cb.isChecked()
+            or self.group_combo.currentIndex() < 2
+        ):
+            fmtos = list(
+                chain.from_iterable(
+                    fmto_group
+                    for i, fmto_group in enumerate(self.fmtos)
+                    if self.groups[i] not in [ALLGROUP, COORDSGROUP]
+                )
+            )
         else:
             fmtos = self.fmtos[self.group_combo.currentIndex()]
         plotter = fmtos[0].plotter
-        getattr(plotter, 'show_' + what)(
-            [fmto.key for fmto in fmtos], grouped=self.grouped_cb.isChecked(),
-            include_links=self.include_links_cb.isChecked())
+        getattr(plotter, "show_" + what)(
+            [fmto.key for fmto in fmtos],
+            grouped=self.grouped_cb.isChecked(),
+            include_links=self.include_links_cb.isChecked(),
+        )
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/help_explorer.py` & `psyplot-gui-1.5.0/psyplot_gui/help_explorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,77 @@
 # -*- coding: utf-8 -*-
 """Help explorer widget supplying a simple web browser and a plain text help
 viewer"""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import sys
+import inspect
+import logging
 import os.path as osp
+import re
+import shutil
+import sys
 from collections import namedtuple
 from itertools import chain
-import re
+from tempfile import mkdtemp
+
 import six
-import types
-import inspect
-import shutil
-from psyplot.docstring import indent, docstrings
-from psyplot.compat.pycompat import OrderedDict
+from IPython.core.oinspect import getdoc, signature
+from psyplot.docstring import docstrings, indent
 from psyplot.utils import _temp_bool_prop
-from psyplot_gui.config.rcsetup import rcParams
+
+from psyplot_gui.common import (
+    DockMixin,
+    PyErrorMessage,
+    StreamToLogger,
+    get_icon,
+    get_module_path,
+    is_running_tests,
+)
 from psyplot_gui.compat.qtcompat import (
-    QWidget, QHBoxLayout, QFrame, QVBoxLayout, QWebEngineView, QToolButton,
-    QIcon, QtCore, QComboBox, Qt,  QSortFilterProxyModel, isstring, asstring,
-    QCompleter, QStandardItemModel, QPlainTextEdit, QAction, QMenu, with_qt5,
-    QtGui)
-from psyplot_gui.common import get_icon, DockMixin, PyErrorMessage
-from IPython.core.oinspect import signature, getdoc
-import logging
-from psyplot_gui.common import get_module_path, StreamToLogger, \
-    is_running_tests
-from tempfile import mkdtemp
+    QAction,
+    QComboBox,
+    QCompleter,
+    QFrame,
+    QHBoxLayout,
+    QIcon,
+    QMenu,
+    QPlainTextEdit,
+    QSortFilterProxyModel,
+    QStandardItemModel,
+    Qt,
+    QtCore,
+    QtGui,
+    QToolButton,
+    QVBoxLayout,
+    QWebEngineView,
+    QWidget,
+    asstring,
+    isstring,
+    with_qt5,
+)
+from psyplot_gui.config.rcsetup import rcParams
+
 try:
     from sphinx.application import Sphinx
     from sphinx.pycode import ModuleAnalyzer
+
     try:
         from psyplot.sphinxext.extended_napoleon import (
+            ExtendedGoogleDocstring as GoogleDocstring,
+        )
+        from psyplot.sphinxext.extended_napoleon import (
             ExtendedNumpyDocstring as NumpyDocstring,
-            ExtendedGoogleDocstring as GoogleDocstring)
+        )
     except ImportError:
-        from sphinx.ext.napoleon import NumpyDocstring, GoogleDocstring
+        from sphinx.ext.napoleon import GoogleDocstring, NumpyDocstring
     with_sphinx = True
 except ImportError:
     with_sphinx = False
 
 if six.PY2:
     from urlparse import urlparse
 else:
@@ -73,25 +83,26 @@
 
     def file2html(fname):
         return pathlib.Path(fname).as_uri()
 
 except ImportError:
 
     def file2html(fname):
-        return 'file://' + fname
+        return "file://" + fname
 
 
 def html2file(url):
     p = urlparse(asstring(url))
     # skip the first '/' on windows platform
-    return osp.abspath(osp.join(p.netloc,
-                                p.path[int(sys.platform == 'win32'):]))
+    return osp.abspath(
+        osp.join(p.netloc, p.path[int(sys.platform == "win32") :])
+    )
 
 
-_viewers = OrderedDict()
+_viewers = dict()
 
 
 logger = logging.getLogger(__name__)
 
 
 class UrlCombo(QComboBox):
     """A editable ComboBox with autocompletion"""
@@ -109,15 +120,16 @@
         self.pFilterModel.setFilterCaseSensitivity(Qt.CaseInsensitive)
 
         self.completer.setPopup(self.completer.popup())
 
         self.setCompleter(self.completer)
 
         self.lineEdit().textEdited[str].connect(
-            self.pFilterModel.setFilterFixedString)
+            self.pFilterModel.setFilterFixedString
+        )
         self.completer.activated.connect(self.add_text_on_top)
         self.setModel(QStandardItemModel())
 
     def setModel(self, model):
         """Reimplemented to also set the model of the filter and completer"""
         super(UrlCombo, self).setModel(model)
         self.pFilterModel.setSourceModel(model)
@@ -154,29 +166,42 @@
 
     Warnings
     --------
     This class is known to crash under PyQt4 when new web page domains are
     loaded. Hence it should be handled with care"""
 
     completed = _temp_bool_prop(
-        'completed', "Boolean whether the html page loading is completed.",
-        default=True)
-
-    url_like_re = re.compile('^\w+://')
-
-    doc_urls = OrderedDict([
-        ('startpage', 'https://startpage.com/'),
-        ('psyplot', 'http://psyplot.github.io/psyplot/'),
-        ('pyplot', 'http://matplotlib.org/api/pyplot_api.html'),
-        ('seaborn', 'http://stanford.edu/~mwaskom/software/seaborn/api.html'),
-        ('cartopy', 'http://scitools.org.uk/cartopy/docs/latest/index.html'),
-        ('xarray', 'http://xarray.pydata.org/en/stable/'),
-        ('pandas', 'http://pandas.pydata.org/pandas-docs/stable/'),
-        ('numpy', 'https://docs.scipy.org/doc/numpy/reference/routines.html'),
-        ])
+        "completed",
+        "Boolean whether the html page loading is completed.",
+        default=True,
+    )
+
+    url_like_re = re.compile(r"^\w+://")
+
+    doc_urls = dict(
+        [
+            ("startpage", "https://startpage.com/"),
+            ("psyplot", "http://psyplot.github.io/psyplot/"),
+            ("pyplot", "http://matplotlib.org/api/pyplot_api.html"),
+            (
+                "seaborn",
+                "http://stanford.edu/~mwaskom/software/seaborn/api.html",
+            ),
+            (
+                "cartopy",
+                "http://scitools.org.uk/cartopy/docs/latest/index.html",
+            ),
+            ("xarray", "http://xarray.pydata.org/en/stable/"),
+            ("pandas", "http://pandas.pydata.org/pandas-docs/stable/"),
+            (
+                "numpy",
+                "https://docs.scipy.org/doc/numpy/reference/routines.html",
+            ),
+        ]
+    )
 
     #: The initial url showed in the webview. If None, nothing will be
     #: displayed
     default_url = None
 
     #: adress line
     tb_url = None
@@ -226,35 +251,35 @@
         self.bt_refresh = QToolButton(self)
         # button to go lock to the current url
         self.bt_lock = QToolButton(self)
         # button to disable browsing in www
         self.bt_url_lock = QToolButton(self)
 
         # ---------------------------- buttons settings -----------------------
-        self.bt_back.setIcon(QIcon(get_icon('previous.png')))
-        self.bt_back.setToolTip('Go back one page')
-        self.bt_ahead.setIcon(QIcon(get_icon('next.png')))
-        self.bt_back.setToolTip('Go forward one page')
+        self.bt_back.setIcon(QIcon(get_icon("previous.png")))
+        self.bt_back.setToolTip("Go back one page")
+        self.bt_ahead.setIcon(QIcon(get_icon("next.png")))
+        self.bt_back.setToolTip("Go forward one page")
 
-        self.bt_refresh.setIcon(QIcon(get_icon('refresh.png')))
-        self.bt_refresh.setToolTip('Refresh the current page')
+        self.bt_refresh.setIcon(QIcon(get_icon("refresh.png")))
+        self.bt_refresh.setToolTip("Refresh the current page")
 
         self.bt_lock.setCheckable(True)
         self.bt_url_lock.setCheckable(True)
 
-        if not with_qt5 and rcParams['help_explorer.online'] is None:
+        if not with_qt5 and rcParams["help_explorer.online"] is None:
             # We now that the browser can crash with Qt4, therefore we disable
             # the browing in the internet
             self.bt_url_lock.click()
-            rcParams['help_explorer.online'] = False
-        elif rcParams['help_explorer.online'] is False:
+            rcParams["help_explorer.online"] = False
+        elif rcParams["help_explorer.online"] is False:
             self.bt_url_lock.click()
-        elif rcParams['help_explorer.online'] is None:
-            rcParams['help_explorer.online'] = True
-        rcParams.connect('help_explorer.online', self.update_url_lock_from_rc)
+        elif rcParams["help_explorer.online"] is None:
+            rcParams["help_explorer.online"] = True
+        rcParams.connect("help_explorer.online", self.update_url_lock_from_rc)
 
         self.bt_url_lock.clicked.connect(self.toogle_url_lock)
         self.bt_lock.clicked.connect(self.toogle_lock)
 
         # tooltip and icons of lock and url_lock are set in toogle_lock and
         # toogle_url_lock
         self.toogle_lock()
@@ -302,88 +327,96 @@
             self.tb_url.addItem(self.default_url)
 
         self.bt_lock_default = bool(self.bt_lock.isChecked())
         self.bt_url_lock_default = bool(self.bt_url_lock.isChecked())
 
     def browse(self, url):
         """Make a web browse on the given url and show the page on the Webview
-        widget. """
+        widget."""
         if self.bt_lock.isChecked():
             return
         if not self.url_like_re.match(url):
-            url = 'https://' + url
-        if self.bt_url_lock.isChecked() and url.startswith('http'):
+            url = "https://" + url
+        if self.bt_url_lock.isChecked() and url.startswith("http"):
             return
         if not self.completed:
-            logger.debug('Stopping current load...')
+            logger.debug("Stopping current load...")
             self.html.stop()
             self.completed = True
-        logger.debug('Loading %s', url)
+        logger.debug("Loading %s", url)
         # we use :meth:`PyQt5.QtWebEngineWidgets.QWebEngineView.setUrl` instead
         # of :meth:`PyQt5.QtWebEngineWidgets.QWebEngineView.load` because that
         # changes the url directly and is more useful for unittests
         self.html.setUrl(QtCore.QUrl(url))
 
     def url_changed(self, url):
         """Triggered when the url is changed to update the adress line"""
         try:
             url = url.toString()
         except AttributeError:
             pass
-        logger.debug('url changed to %s', url)
+        logger.debug("url changed to %s", url)
         try:
             self.tb_url.setCurrentText(url)
         except AttributeError:  # Qt4
             self.tb_url.setEditText(url)
         self.tb_url.add_text_on_top(url, block=True)
 
     def update_url_lock_from_rc(self, online):
-        if (online and self.bt_url_lock.isChecked() or
-                not online and not self.bt_url_lock.isChecked()):
+        if (
+            online
+            and self.bt_url_lock.isChecked()
+            or not online
+            and not self.bt_url_lock.isChecked()
+        ):
             self.bt_url_lock.click()
 
     def toogle_url_lock(self):
         """Disable (or enable) the loading of web pages in www"""
         bt = self.bt_url_lock
         offline = bt.isChecked()
-        bt.setIcon(QIcon(get_icon(
-            'world_red.png' if offline else 'world.png')))
+        bt.setIcon(
+            QIcon(get_icon("world_red.png" if offline else "world.png"))
+        )
         online_message = "Go online"
         if not with_qt5:
-            online_message += ("\nWARNING: This mode is unstable under Qt4 "
-                               "and might result in a complete program crash!")
+            online_message += (
+                "\nWARNING: This mode is unstable under Qt4 "
+                "and might result in a complete program crash!"
+            )
         bt.setToolTip(online_message if offline else "Offline mode")
-        if rcParams['help_explorer.online'] is offline:
-            rcParams['help_explorer.online'] = not offline
+        if rcParams["help_explorer.online"] is offline:
+            rcParams["help_explorer.online"] = not offline
 
     def toogle_lock(self):
         """Disable (or enable) the changing of the current webpage"""
         bt = self.bt_lock
-        bt.setIcon(QIcon(get_icon(
-            'lock.png' if bt.isChecked() else 'lock_open.png')))
+        bt.setIcon(
+            QIcon(get_icon("lock.png" if bt.isChecked() else "lock_open.png"))
+        )
         bt.setToolTip("Unlock" if bt.isChecked() else "Lock to current page")
 
 
 class HelpMixin(object):
     """Base class for providing help on an object"""
 
     #: Object containing the necessary fields to describe an object given to
     #: the help widget. The descriptor is set up by the :meth:`describe_object`
     #: method.
-    object_descriptor = namedtuple('ObjectDescriptor', ['obj', 'name'])
+    object_descriptor = namedtuple("ObjectDescriptor", ["obj", "name"])
 
     #: :class:`bool` determining whether the documentation of an object can be
     #: shown or not
     can_document_object = True
     #: :class:`bool` determining whether this class can show restructured text
     can_show_rst = True
 
-    @docstrings.get_sections(base='HelpMixin.show_help')
+    @docstrings.get_sections(base="HelpMixin.show_help")
     @docstrings.dedent
-    def show_help(self, obj, oname='', files=None):
+    def show_help(self, obj, oname="", files=None):
         """
         Show the rst documentation for the given object
 
         Parameters
         ----------
         obj: object
             The object to get the documentation for
@@ -399,18 +432,18 @@
     def header(self, descriptor, sig):
         """Format the header and include object name and signature `sig`
 
         Returns
         -------
         str
             The header for the documentation"""
-        bars = '=' * len(descriptor.name + sig)
-        return bars + '\n' + descriptor.name + sig + '\n' + bars + '\n'
+        bars = "=" * len(descriptor.name + sig)
+        return bars + "\n" + descriptor.name + sig + "\n" + bars + "\n"
 
-    def describe_object(self, obj, oname=''):
+    def describe_object(self, obj, oname=""):
         """Return an instance of the :attr:`object_descriptor` class
 
         Returns
         -------
         :attr:`object_descriptor`
             The descriptor containing the information on the object"""
         return self.object_descriptor(obj, oname)
@@ -432,59 +465,60 @@
         -----
         This method uses the :func:`IPython.core.oinspect.getdoc` function to
         get the documentation and the :func:`IPython.core.oinspect.signature`
         function to get the signature. Those function (different from the
         inspect module) do not fail when the object is not saved"""
         obj = descriptor.obj
         oname = descriptor.name
-        sig = ''
+        sig = ""
         obj_sig = obj
         if callable(obj):
             if inspect.isclass(obj):
                 oname = oname or obj.__name__
-                obj_sig = getattr(obj, '__init__', obj)
-            elif six.PY2 and type(obj) is types.InstanceType:
-                obj_sig = getattr(obj, '__call__', obj)
+                obj_sig = getattr(obj, "__init__", obj)
+            else:
+                obj_sig = getattr(obj, "__call__", obj)
 
             try:
                 sig = str(signature(obj_sig))
-                sig = re.sub('^\(\s*self,\s*', '(', sig)
-            except:
-                logger.debug('Failed to get signature from %s!' % (obj, ),
-                             exc_info=True)
+                sig = re.sub(r"^\(\s*self,\s*", "(", sig)
+            except Exception:
+                logger.debug(
+                    "Failed to get signature from %s!" % (obj,), exc_info=True
+                )
         oname = oname or type(oname).__name__
         head = self.header(descriptor, sig)
         lines = []
         ds = getdoc(obj)
         if ds:
-            lines.append('')
+            lines.append("")
             lines.append(ds)
-        if inspect.isclass(obj) and hasattr(obj, '__init__'):
+        if inspect.isclass(obj) and hasattr(obj, "__init__"):
             init_ds = getdoc(obj.__init__)
             if init_ds is not None:
-                lines.append('\n' + init_ds)
-        elif hasattr(obj, '__call__'):
+                lines.append("\n" + init_ds)
+        elif hasattr(obj, "__call__"):
             call_ds = getdoc(obj.__call__)
             if call_ds and call_ds != getdoc(object.__call__):
-                lines.append('\n' + call_ds)
+                lines.append("\n" + call_ds)
         doc = self.process_docstring(lines, descriptor)
-        return head + '\n' + doc
+        return head + "\n" + doc
 
     def process_docstring(self, lines, descriptor):
         """Make final modification on the rst lines
 
         Returns
         -------
         str
             The docstring"""
-        return '\n'.join(lines)
+        return "\n".join(lines)
 
-    @docstrings.get_sections(base='HelpMixin.show_rst')
+    @docstrings.get_sections(base="HelpMixin.show_rst")
     @docstrings.dedent
-    def show_rst(self, text, oname='', descriptor=None, files=None):
+    def show_rst(self, text, oname="", descriptor=None, files=None):
         """
         Abstract method which needs to be implemented by th widget to show
         restructured text
 
         Parameters
         ----------
         text: str
@@ -499,39 +533,39 @@
         Returns
         -------
         bool
             True if the text is displayed
         """
         return False
 
-    @docstrings.get_sections(base='HelpMixin.show_intro')
-    def show_intro(self, text=''):
+    @docstrings.get_sections(base="HelpMixin.show_intro")
+    def show_intro(self, text=""):
         """
         Show an intro message
 
         Parameters
         ----------
         s: str
             A string in reStructured Text format to show"""
-        title = 'Welcome to psyplot!'
-        title += '\n' + '-' * len(title) + '\n\n'
-        self.show_rst(title + text, 'intro')
+        title = "Welcome to psyplot!"
+        title += "\n" + "-" * len(title) + "\n\n"
+        self.show_rst(title + text, "intro")
 
 
 class TextHelp(QFrame, HelpMixin):
     """Class to show plain text rst docstrings"""
 
     def __init__(self, *args, **kwargs):
         super(TextHelp, self).__init__(*args, **kwargs)
         self.vbox = QVBoxLayout()
         self.vbox.setContentsMargins(0, 0, 0, 0)
         #: The :class:`PyQt5.QtWidgets.QPlainTextEdit` instance used for
         #: displaying the documentation
         self.editor = QPlainTextEdit(parent=self)
-        self.editor.setFont(QtGui.QFont('Courier New'))
+        self.editor.setFont(QtGui.QFont("Courier New"))
         self.vbox.addWidget(self.editor)
         self.setLayout(self.vbox)
 
     def show_rst(self, text, *args, **kwargs):
         """Show the given text in the editor window
 
         Parameters
@@ -548,157 +582,179 @@
 class UrlHelp(UrlBrowser, HelpMixin):
     """Class to convert rst docstrings to html and show browsers"""
 
     #: Object containing the necessary fields to describe an object given to
     #: the help widget. The descriptor is set up by the :meth:`describe_object`
     #: method and contains an additional objtype attribute
     object_descriptor = namedtuple(
-        'ObjectDescriptor', ['obj', 'name', 'objtype'])
+        "ObjectDescriptor", ["obj", "name", "objtype"]
+    )
 
     can_document_object = with_sphinx
     can_show_rst = with_sphinx
 
     #: menu button with different urls
     bt_url_menus = None
 
     #:
     sphinx_thread = None
 
     def __init__(self, *args, **kwargs):
-        self._temp_dir = 'sphinx_dir' not in kwargs
-        self.sphinx_dir = kwargs.pop('sphinx_dir', mkdtemp(prefix='psyplot_'))
-        self.build_dir = osp.join(self.sphinx_dir, '_build', 'html')
+        self._temp_dir = "sphinx_dir" not in kwargs
+        self.sphinx_dir = kwargs.pop("sphinx_dir", mkdtemp(prefix="psyplot_"))
+        self.build_dir = osp.join(self.sphinx_dir, "_build", "html")
         super(UrlHelp, self).__init__(*args, **kwargs)
 
         self.error_msg = PyErrorMessage(self)
         if with_sphinx:
             self.sphinx_thread = SphinxThread(self.sphinx_dir)
             self.sphinx_thread.html_ready[str].connect(self.browse)
             self.sphinx_thread.html_error[str].connect(
-                self.error_msg.showTraceback)
+                self.error_msg.showTraceback
+            )
             self.sphinx_thread.html_error[str].connect(logger.debug)
-            rcParams.connect('help_explorer.render_docs_parallel',
-                             self.reset_sphinx)
-            rcParams.connect('help_explorer.use_intersphinx',
-                             self.reset_sphinx)
-            rcParams.connect('help_explorer.online',
-                             self.reset_sphinx)
+            rcParams.connect(
+                "help_explorer.render_docs_parallel", self.reset_sphinx
+            )
+            rcParams.connect(
+                "help_explorer.use_intersphinx", self.reset_sphinx
+            )
+            rcParams.connect("help_explorer.online", self.reset_sphinx)
 
         self.bt_connect_console = QToolButton(self)
         self.bt_connect_console.setCheckable(True)
-        if rcParams['console.connect_to_help']:
-            self.bt_connect_console.setIcon(QIcon(get_icon(
-                'ipython_console.png')))
+        if rcParams["console.connect_to_help"]:
+            self.bt_connect_console.setIcon(
+                QIcon(get_icon("ipython_console.png"))
+            )
             self.bt_connect_console.click()
         else:
-            self.bt_connect_console.setIcon(QIcon(get_icon(
-                'ipython_console_t.png')))
+            self.bt_connect_console.setIcon(
+                QIcon(get_icon("ipython_console_t.png"))
+            )
         self.bt_connect_console.clicked.connect(self.toogle_connect_console)
-        rcParams.connect('console.connect_to_help',
-                         self.update_connect_console)
+        rcParams.connect(
+            "console.connect_to_help", self.update_connect_console
+        )
         self.toogle_connect_console()
 
         # menu button with different urls
         self.bt_url_menus = QToolButton(self)
-        self.bt_url_menus.setIcon(QIcon(get_icon('docu_button.png')))
-        self.bt_url_menus.setToolTip('Browse documentations')
+        self.bt_url_menus.setIcon(QIcon(get_icon("docu_button.png")))
+        self.bt_url_menus.setToolTip("Browse documentations")
         self.bt_url_menus.setPopupMode(QToolButton.InstantPopup)
 
         docu_menu = QMenu(self)
         for name, url in six.iteritems(self.doc_urls):
+
             def to_url(b, url=url):
                 self.browse(url)
+
             action = QAction(name, self)
             action.triggered.connect(to_url)
             docu_menu.addAction(action)
         self.bt_url_menus.setMenu(docu_menu)
 
         self.button_box.addWidget(self.bt_connect_console)
         self.button_box.addWidget(self.bt_url_menus)
         # toogle the lock again to set the bt_url_menus enabled state
         self.toogle_url_lock()
 
     def update_connect_console(self, connect):
-        if (connect and not self.bt_connect_console.isChecked() or
-                not connect and self.bt_connect_console.isChecked()):
+        if (
+            connect
+            and not self.bt_connect_console.isChecked()
+            or not connect
+            and self.bt_connect_console.isChecked()
+        ):
             self.bt_connect_console.click()
 
     def toogle_connect_console(self):
         """Disable (or enable) the loading of web pages in www"""
         bt = self.bt_connect_console
         connect = bt.isChecked()
-        bt.setIcon(QIcon(get_icon(
-            'ipython_console.png' if connect else 'ipython_console_t.png')))
-        bt.setToolTip("%sonnect the console to the help explorer" % (
-            "Don't c" if connect else "C"))
-        if rcParams['console.connect_to_help'] is not connect:
-            rcParams['console.connect_to_help'] = connect
+        bt.setIcon(
+            QIcon(
+                get_icon(
+                    "ipython_console.png"
+                    if connect
+                    else "ipython_console_t.png"
+                )
+            )
+        )
+        bt.setToolTip(
+            "%sonnect the console to the help explorer"
+            % ("Don't c" if connect else "C")
+        )
+        if rcParams["console.connect_to_help"] is not connect:
+            rcParams["console.connect_to_help"] = connect
 
     def reset_sphinx(self, value):
         """Method that is called if the configuration changes"""
-        if with_sphinx and hasattr(self.sphinx_thread, 'app'):
+        if with_sphinx and hasattr(self.sphinx_thread, "app"):
             del self.sphinx_thread.app
 
     @docstrings.dedent
-    def show_help(self, obj, oname='', files=None):
+    def show_help(self, obj, oname="", files=None):
         """
         Render the rst docu for the given object with sphinx and show it
 
         Parameters
         ----------
         %(HelpMixin.show_help.parameters)s
         """
         if self.bt_lock.isChecked():
             return
         return super(UrlHelp, self).show_help(obj, oname=oname, files=files)
 
     @docstrings.dedent
-    def show_intro(self, text=''):
+    def show_intro(self, text=""):
         """
         Show the intro text in the explorer
 
         Parameters
         ----------
         %(HelpMixin.show_intro.parameters)s"""
         if self.sphinx_thread is not None:
-            with open(self.sphinx_thread.index_file, 'a') as f:
-                f.write('\n' + text.strip() + '\n\n' +
-                        'Table of Contents\n'
-                        '=================\n\n.. toctree::\n')
+            with open(self.sphinx_thread.index_file, "a") as f:
+                f.write(
+                    "\n" + text.strip() + "\n\n" + "Table of Contents\n"
+                    "=================\n\n.. toctree::\n"
+                )
             self.sphinx_thread.render(None, None)
 
-    def show_rst(self, text, oname='', descriptor=None, files=None):
+    def show_rst(self, text, oname="", descriptor=None, files=None):
         """Render restructured text with sphinx and show it
 
         Parameters
         ----------
         %(HelpMixin.show_rst.parameters)s"""
         if self.bt_lock.isChecked() or self.sphinx_thread is None:
             return False
         if not oname and descriptor:
             oname = descriptor.name
         for f in files or []:
             shutil.copyfile(f, osp.join(self.sphinx_dir, osp.basename(f)))
         self.sphinx_thread.render(text, oname)
         return True
 
-    def describe_object(self, obj, oname=''):
+    def describe_object(self, obj, oname=""):
         """Describe an object using additionaly the object type from the
         :meth:`get_objtype` method
 
         Returns
         -------
         instance of :attr:`object_descriptor`
             The descriptor of the object"""
         return self.object_descriptor(obj, oname, self.get_objtype(obj))
 
     def browse(self, url):
         """Reimplemented to add file paths to the url string"""
         url = asstring(url)
-        html_file = osp.join(self.sphinx_dir, '_build', 'html', url + '.html')
+        html_file = osp.join(self.sphinx_dir, "_build", "html", url + ".html")
         if osp.exists(html_file):
             url = file2html(html_file)
         super(UrlHelp, self).browse(url)
 
     def toogle_url_lock(self):
         """Disable (or enable) the loading of web pages in www"""
         super(UrlHelp, self).toogle_url_lock()
@@ -712,47 +768,51 @@
 
     def url_changed(self, url):
         """Reimplemented to remove file paths from the url string"""
         try:
             url = asstring(url.toString())
         except AttributeError:
             pass
-        if url.startswith('file://'):
+        if url.startswith("file://"):
             fname = html2file(url)
-            if osp.samefile(self.build_dir, osp.commonprefix([
-                    fname, self.build_dir])):
+            if osp.samefile(
+                self.build_dir, osp.commonprefix([fname, self.build_dir])
+            ):
                 url = osp.splitext(osp.basename(fname))[0]
         super(UrlHelp, self).url_changed(url)
 
     def header(self, descriptor, sig):
-        return '%(name)s\n%(bars)s\n\n.. py:%(type)s:: %(name)s%(sig)s\n' % {
-            'name': descriptor.name, 'bars': '-' * len(descriptor.name),
-            'type': descriptor.objtype, 'sig': sig}
+        return "%(name)s\n%(bars)s\n\n.. py:%(type)s:: %(name)s%(sig)s\n" % {
+            "name": descriptor.name,
+            "bars": "-" * len(descriptor.name),
+            "type": descriptor.objtype,
+            "sig": sig,
+        }
 
     def get_objtype(self, obj):
         """Get the object type of the given object and determine wheter the
         object is considered a class, a module, a function, method or data
 
         Parameters
         ----------
         obj: object
 
         Returns
         -------
         str
             One out of {'class', 'module', 'function', 'method', 'data'}"""
         if inspect.isclass(obj):
-            return 'class'
+            return "class"
         if inspect.ismodule(obj):
-            return 'module'
+            return "module"
         if inspect.isfunction(obj) or isinstance(obj, type(all)):
-            return 'function'
+            return "function"
         if inspect.ismethod(obj) or isinstance(obj, type(str.upper)):
-            return 'method'
-        return 'data'
+            return "method"
+        return "data"
 
     def is_importable(self, modname):
         """Determine whether members of the given module can be documented with
         sphinx by using the :func:`sphinx.util.get_module_source` function
 
         Parameters
         ----------
@@ -773,78 +833,101 @@
         """Reimplemented to (potentially) use the features from
         sphinx.ext.autodoc"""
         obj = descriptor.obj
         if inspect.ismodule(obj):
             module = obj
         else:
             module = inspect.getmodule(obj)
-        if module is not None and (re.match('__.*__', module.__name__) or
-                                   not self.is_importable(module.__name__)):
+        if module is not None and (
+            re.match("__.*__", module.__name__)
+            or not self.is_importable(module.__name__)
+        ):
             module = None
         isclass = inspect.isclass(obj)
         # If the module is available, we try to use autodoc
         if module is not None:
-            doc = '.. currentmodule:: ' + module.__name__ + '\n\n'
+            doc = ".. currentmodule:: " + module.__name__ + "\n\n"
             # a module --> use automodule
             if inspect.ismodule(obj):
-                doc += self.header(descriptor, '')
-                doc += '.. automodule:: ' + obj.__name__
+                doc += self.header(descriptor, "")
+                doc += ".. automodule:: " + obj.__name__
             # an importable class --> use autoclass
             elif isclass and getattr(module, obj.__name__, None) is not None:
-                doc += self.header(descriptor, '')
-                doc += '.. autoclass:: ' + obj.__name__
+                doc += self.header(descriptor, "")
+                doc += ".. autoclass:: " + obj.__name__
             # an instance and the class can be imported
             # --> use super get_doc and autoclass for the tyoe
-            elif descriptor.objtype == 'data' and getattr(
-                    module, type(obj).__name__, None) is not None:
-                doc += '\n\n'.join([
-                    super(UrlHelp, self).get_doc(descriptor),
-                    "Class docstring\n===============",
-                    '.. autoclass:: ' + type(obj).__name__])
+            elif (
+                descriptor.objtype == "data"
+                and getattr(module, type(obj).__name__, None) is not None
+            ):
+                doc += "\n\n".join(
+                    [
+                        super(UrlHelp, self).get_doc(descriptor),
+                        "Class docstring\n===============",
+                        ".. autoclass:: " + type(obj).__name__,
+                    ]
+                )
             # an instance --> use super get_doc for instance and the type
-            elif descriptor.objtype == 'data':
-                cls_doc = super(UrlHelp, self).get_doc(self.describe_object(
-                    type(obj), type(obj).__name__))
-                doc += '\n\n'.join([
-                    super(UrlHelp, self).get_doc(descriptor),
-                    "Class docstring\n===============",
-                    cls_doc])
+            elif descriptor.objtype == "data":
+                cls_doc = super(UrlHelp, self).get_doc(
+                    self.describe_object(type(obj), type(obj).__name__)
+                )
+                doc += "\n\n".join(
+                    [
+                        super(UrlHelp, self).get_doc(descriptor),
+                        "Class docstring\n===============",
+                        cls_doc,
+                    ]
+                )
             # a function or method --> use super get_doc
             else:
                 doc += super(UrlHelp, self).get_doc(descriptor)
         # otherwise the object has been defined in this session
         else:
             # an instance --> use super get_doc for instance and the type
-            if descriptor.objtype == 'data':
-                cls_doc = super(UrlHelp, self).get_doc(self.describe_object(
-                    type(obj), type(obj).__name__))
-                doc = '\n\n'.join([
-                    super(UrlHelp, self).get_doc(descriptor),
-                    "Class docstring\n===============",
-                    cls_doc])
+            if descriptor.objtype == "data":
+                cls_doc = super(UrlHelp, self).get_doc(
+                    self.describe_object(type(obj), type(obj).__name__)
+                )
+                doc = "\n\n".join(
+                    [
+                        super(UrlHelp, self).get_doc(descriptor),
+                        "Class docstring\n===============",
+                        cls_doc,
+                    ]
+                )
             # a function or method --> use super get_doc
             else:
                 doc = super(UrlHelp, self).get_doc(descriptor)
-        return doc.rstrip() + '\n'
+        return doc.rstrip() + "\n"
 
     def process_docstring(self, lines, descriptor):
         """Process the lines with the napoleon sphinx extension"""
-        lines = list(chain(*(l.splitlines() for l in lines)))
+        lines = list(chain(*(line.splitlines() for line in lines)))
         lines = NumpyDocstring(
-            lines, what=descriptor.objtype, name=descriptor.name,
-            obj=descriptor.obj).lines()
+            lines,
+            what=descriptor.objtype,
+            name=descriptor.name,
+            obj=descriptor.obj,
+        ).lines()
         lines = GoogleDocstring(
-            lines, what=descriptor.objtype, name=descriptor.name,
-            obj=descriptor.obj).lines()
-        return indent(super(UrlHelp, self).process_docstring(
-            lines, descriptor))
+            lines,
+            what=descriptor.objtype,
+            name=descriptor.name,
+            obj=descriptor.obj,
+        ).lines()
+        return indent(
+            super(UrlHelp, self).process_docstring(lines, descriptor)
+        )
 
     def close(self, *args, **kwargs):
-        if kwargs.pop('force', False) or (
-                not is_running_tests() and self.sphinx_thread is not None):
+        if kwargs.pop("force", False) or (
+            not is_running_tests() and self.sphinx_thread is not None
+        ):
             try:
                 del self.sphinx_thread.app
             except AttributeError:
                 pass
             shutil.rmtree(self.build_dir, ignore_errors=True)
             if self._temp_dir:
                 shutil.rmtree(self.sphinx_dir, ignore_errors=True)
@@ -861,84 +944,91 @@
     """A thread to render sphinx documentation in a separate process"""
 
     #: A signal to be emitted when the rendering finished. The url is the
     #: file location
     html_ready = QtCore.pyqtSignal(str)
     html_error = QtCore.pyqtSignal(str)
 
-    def __init__(self, outdir, html_text_no_doc=''):
+    def __init__(self, outdir, html_text_no_doc=""):
         super(SphinxThread, self).__init__()
         self.doc = None
         self.name = None
         self.html_text_no_doc = html_text_no_doc
         self.outdir = outdir
-        self.index_file = osp.join(self.outdir, 'psyplot.rst')
-        self.confdir = osp.join(get_module_path(__name__), 'sphinx_supp')
-        shutil.copyfile(osp.join(self.confdir, 'psyplot.rst'),
-                        osp.join(self.outdir, 'psyplot.rst'))
-        self.build_dir = osp.join(self.outdir, '_build', 'html')
+        self.index_file = osp.join(self.outdir, "psyplot.rst")
+        self.confdir = osp.join(get_module_path(__name__), "sphinx_supp")
+        shutil.copyfile(
+            osp.join(self.confdir, "psyplot.rst"),
+            osp.join(self.outdir, "psyplot.rst"),
+        )
+        self.build_dir = osp.join(self.outdir, "_build", "html")
 
     def render(self, doc, name):
         """Render the given rst string and save the file as ``name + '.rst'``
 
         Parameters
         ----------
         doc: str
             The rst docstring
         name: str
             the name to use for the file"""
         if self.wait():
             self.doc = doc
             self.name = name
             # start rendering in separate process
-            if rcParams['help_explorer.render_docs_parallel']:
+            if rcParams["help_explorer.render_docs_parallel"]:
                 self.start()
             else:
                 self.run()
 
     def run(self):
         """Create the html file. When called the first time, it may take a
         while because the :class:`sphinx.application.Sphinx` app is build,
         potentially with intersphinx
 
         When finished, the html_ready signal is emitted"""
-        if not hasattr(self, 'app'):
+        if not hasattr(self, "app"):
             from IPython.core.history import HistoryAccessor
+
             # to avoid history access conflicts between different threads,
             # we disable the ipython history
             HistoryAccessor.enabled.default_value = False
-            self.app = Sphinx(self.outdir,
-                              self.confdir,
-                              self.build_dir,
-                              osp.join(self.outdir, '_build', 'doctrees'),
-                              'html',
-                              status=StreamToLogger(logger, logging.DEBUG),
-                              warning=StreamToLogger(logger, logging.DEBUG))
+            self.app = Sphinx(
+                self.outdir,
+                self.confdir,
+                self.build_dir,
+                osp.join(self.outdir, "_build", "doctrees"),
+                "html",
+                status=StreamToLogger(logger, logging.DEBUG),
+                warning=StreamToLogger(logger, logging.DEBUG),
+            )
         if self.name is not None:
-            docfile = osp.abspath(osp.join(self.outdir, self.name + '.rst'))
+            docfile = osp.abspath(osp.join(self.outdir, self.name + ".rst"))
             if docfile == self.index_file:
-                self.name += '1'
+                self.name += "1"
                 docfile = osp.abspath(
-                    osp.join(self.outdir, self.name + '.rst'))
-            html_file = osp.abspath(osp.join(
-                self.outdir, '_build', 'html', self.name + '.html'))
+                    osp.join(self.outdir, self.name + ".rst")
+                )
+            html_file = osp.abspath(
+                osp.join(self.outdir, "_build", "html", self.name + ".html")
+            )
             if not osp.exists(docfile):
-                with open(self.index_file, 'a') as f:
-                    f.write('\n    ' + self.name)
-            with open(docfile, 'w') as f:
+                with open(self.index_file, "a") as f:
+                    f.write("\n    " + self.name)
+            with open(docfile, "w") as f:
                 f.write(self.doc)
         else:
-            html_file = osp.abspath(osp.join(
-                self.outdir, '_build', 'html', 'psyplot.html'))
+            html_file = osp.abspath(
+                osp.join(self.outdir, "_build", "html", "psyplot.html")
+            )
         try:
             self.app.build(None, [])
         except Exception:
-            msg = 'Error while building sphinx document %s' % (
-                self.name)
-            self.html_error.emit('<b>' + msg + '</b>')
+            msg = "Error while building sphinx document %s" % (self.name)
+            self.html_error.emit("<b>" + msg + "</b>")
             logger.debug(msg)
         else:
             self.html_ready.emit(file2html(html_file))
 
 
 class HelpExplorer(QWidget, DockMixin):
     """A widget for showing the documentation. It behaves somewhat similar
@@ -951,32 +1041,35 @@
     The :class:`HelpBrowser` class is known to crash under PyQt4 when new web
     page domains are loaded. Hence you should disable the browsing to different
     remote websites and even disable intersphinx"""
 
     #: The viewer classes used by the help explorer. :class:`HelpExplorer`
     #: instances replace this attribute with the corresponding HelpMixin
     #: instance
-    viewers = OrderedDict([('HTML help', UrlHelp), ('Plain text', TextHelp)])
+    viewers = dict([("HTML help", UrlHelp), ("Plain text", TextHelp)])
 
-    if not rcParams['help_explorer.use_webengineview']:
-        del viewers['HTML help']
+    if not rcParams["help_explorer.use_webengineview"]:
+        del viewers["HTML help"]
 
     def __init__(self, *args, **kwargs):
         super(HelpExplorer, self).__init__(*args, **kwargs)
         self.vbox = vbox = QVBoxLayout()
         self.combo = QComboBox(parent=self)
         vbox.addWidget(self.combo)
         if _viewers:
             self.viewers = _viewers.copy()
             for w in self.viewers.values():
                 w.setParent(self)
         else:
-            self.viewers = OrderedDict(
-                [(key, cls(parent=self)) for key, cls in six.iteritems(
-                    self.viewers)])
+            self.viewers = dict(
+                [
+                    (key, cls(parent=self))
+                    for key, cls in six.iteritems(self.viewers)
+                ]
+            )
             # save the UrlHelp because QWebEngineView creates child processes
             # that are not properly closed by PyQt and as such use too much
             # memory
             if is_running_tests():
                 for key, val in self.viewers.items():
                     _viewers[key] = val
         for key, ini in six.iteritems(self.viewers):
@@ -993,29 +1086,28 @@
 
         Parameters
         ----------
         name: str or object
             A string must be one of the :attr:`viewers` attribute. An object
             can be one of the values in the :attr:`viewers` attribute"""
         if isstring(name) and asstring(name) not in self.viewers:
-            raise ValueError("Don't have a viewer named %s" % (name, ))
+            raise ValueError("Don't have a viewer named %s" % (name,))
         elif not isstring(name):
             viewer = name
         else:
             name = asstring(name)
             viewer = self.viewers[name]
         self.viewer.hide()
         self.viewer = viewer
         self.viewer.show()
-        if (isstring(name) and
-                not self.combo.currentText() == name):
+        if isstring(name) and not self.combo.currentText() == name:
             self.combo.setCurrentIndex(list(self.viewers).index(name))
 
     @docstrings.dedent
-    def show_help(self, obj, oname='', files=None):
+    def show_help(self, obj, oname="", files=None):
         """
         Show the documentaion of the given object
 
         We first try to use the current viewer based upon it's
         :attr:`HelpMixin.can_document_object` attribute. If this does not work,
         we check the other viewers
 
@@ -1024,36 +1116,45 @@
         %(HelpMixin.show_help.parameters)s"""
         oname = asstring(oname)
         ret = None
         if self.viewer.can_document_object:
             try:
                 ret = self.viewer.show_help(obj, oname=oname, files=files)
             except Exception:
-                logger.debug("Could not document %s with %s viewer!",
-                             oname, self.combo.currentText(), exc_info=True)
+                logger.debug(
+                    "Could not document %s with %s viewer!",
+                    oname,
+                    self.combo.currentText(),
+                    exc_info=True,
+                )
         else:
             curr_i = self.combo.currentIndex()
             for i, (viewername, viewer) in enumerate(
-                    six.iteritems(self.viewers)):
+                six.iteritems(self.viewers)
+            ):
                 if i != curr_i and viewer.can_document_object:
                     self.set_viewer(viewername)
                     self.combo.blockSignals(True)
                     self.combo.setCurrentIndex(i)
                     self.combo.blockSignals(False)
                     try:
                         ret = viewer.show_help(obj, oname=oname, files=files)
                     except Exception:
-                        logger.debug("Could not document %s with %s viewer!",
-                                     oname, viewername, exc_info=True)
+                        logger.debug(
+                            "Could not document %s with %s viewer!",
+                            oname,
+                            viewername,
+                            exc_info=True,
+                        )
         if ret:
             self.parent().raise_()
         return ret
 
     @docstrings.dedent
-    def show_rst(self, text, oname='', files=None):
+    def show_rst(self, text, oname="", files=None):
         """
         Show restructured text
 
         We first try to use the current viewer based upon it's
         :attr:`HelpMixin.can_show_rst` attribute. If this does not work,
         we check the other viewers
 
@@ -1070,15 +1171,15 @@
                     ret = viewer.show_rst(text, oname=oname, files=files)
                     break
         if ret:
             self.parent().raise_()
         return ret
 
     @docstrings.dedent
-    def show_intro(self, text=''):
+    def show_intro(self, text=""):
         """
         Show an intro text
 
         We first try to use the current viewer based upon it's
         :attr:`HelpMixin.can_show_rst` attribute. If this does not work,
         we check the other viewers
 
@@ -1091,11 +1192,11 @@
             if not found and viewer.can_show_rst:
                 if i:
                     self.set_viewer(viewer)
                 found = True
 
     def close(self, *args, **kwargs):
         try:
-            self.viewers['HTML help'].close(*args, **kwargs)
+            self.viewers["HTML help"].close(*args, **kwargs)
         except (KeyError, AttributeError):
             pass
         return super(HelpExplorer, self).close(*args, **kwargs)
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/icons/ipython_console.png` & `psyplot-gui-1.5.0/psyplot_gui/icons/ipython_console.png`

 * *Files identical despite different names*

### Comparing `psyplot-gui-1.4.0/psyplot_gui/icons/logo.png` & `psyplot-gui-1.5.0/psyplot_gui/icons/logo.png`

 * *Files identical despite different names*

### Comparing `psyplot-gui-1.4.0/psyplot_gui/icons/plusplus.png` & `psyplot-gui-1.5.0/psyplot_gui/icons/plusplus.png`

 * *Files identical despite different names*

### Comparing `psyplot-gui-1.4.0/psyplot_gui/main.py` & `psyplot-gui-1.5.0/psyplot_gui/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,96 +2,96 @@
 
 This module redefines the :class:`psyplot.project.Project` class with
 additional features for an interactive usage with graphical qt user interface.
 There is no need to import this module because the
 :class:`GuiProject` class defined here replaces the project class in the
 :mod:`psyplot.project` module."""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import sys
-import six
-import socket
 import errno
-import pickle
+import logging
 import os
-from pkg_resources import iter_entry_points
+import pickle
+import socket
+import sys
+from collections import OrderedDict, defaultdict
 from functools import partial
-from collections import defaultdict, OrderedDict
-import matplotlib as mpl
-from psyplot.compat.pycompat import get_default_value
-from psyplot_gui import rcParams
 from threading import Thread
-import logging
 
-# change backend here before the project module is imported
-backend = rcParams['backend']
-if backend is not None:
-    if backend == 'psyplot':
-        backend = 'module://psyplot_gui.backend'
-    mpl.use(backend)
+import matplotlib as mpl
+import psyplot
+import psyplot.data as psyd
+import psyplot.plotter as psyp
+import psyplot.project as psy
+import six
+import xarray as xr
+from psyplot.config.rcsetup import get_configdir
+from psyplot.docstring import docstrings
+from psyplot.utils import get_default_value
 
-from psyplot_gui.console import ConsoleWidget
+import psyplot_gui
+from psyplot_gui import rcParams
+from psyplot_gui.common import PyErrorMessage, StreamToLogger, get_icon
 from psyplot_gui.compat.qtcompat import (
-    QMainWindow, QApplication, Qt, QMenu, QAction, QDesktopWidget, QLabel,
-    QFileDialog, QKeySequence, QtCore, with_qt5, QMessageBox, QIcon,
-    QInputDialog, QActionGroup)
+    QAction,
+    QActionGroup,
+    QApplication,
+    QDesktopWidget,
+    QFileDialog,
+    QIcon,
+    QInputDialog,
+    QKeySequence,
+    QLabel,
+    QMainWindow,
+    QMenu,
+    QMessageBox,
+    Qt,
+    QtCore,
+    with_qt5,
+)
+from psyplot_gui.console import ConsoleWidget
 from psyplot_gui.content_widget import (
-    ProjectContentWidget, DatasetTree, FiguresTree)
-from psyplot_gui.plot_creator import PlotCreator
-from psyplot_gui.help_explorer import HelpExplorer
+    DatasetTree,
+    FiguresTree,
+    ProjectContentWidget,
+)
 from psyplot_gui.dataframeeditor import DataFrameEditor
+from psyplot_gui.dependencies import DependenciesDialog
 from psyplot_gui.fmt_widget import FormatoptionWidget
-from psyplot_gui.common import PyErrorMessage, get_icon, StreamToLogger
+from psyplot_gui.help_explorer import HelpExplorer
+from psyplot_gui.plot_creator import PlotCreator
 from psyplot_gui.preferences import (
-    Prefences, GuiRcParamsWidget, PsyRcParamsWidget)
-from psyplot_gui.dependencies import DependenciesDialog
+    GuiRcParamsWidget,
+    Prefences,
+    PsyRcParamsWidget,
+)
 
-from psyplot.docstring import docstrings
-import psyplot.plotter as psyp
-import psyplot.project as psy
-import psyplot
-from psyplot.config.rcsetup import get_configdir
-import psyplot.data as psyd
-import psyplot_gui
-import xarray as xr
+# change backend here before the project module is imported
+backend = rcParams["backend"]
+if backend is not None:
+    if backend == "psyplot":
+        backend = "module://psyplot_gui.backend"
+    mpl.use(backend)
 
 
 #: The :class:`PyQt5.QtWidgets.QMainWindow` of the graphical user interface
 mainwindow = None
 
 
 def _set_mainwindow(obj):
     global mainwindow
     mainwindow = obj
 
 
 class MainWindow(QMainWindow):
-
     #: A signal that is emmitted when the a signal is received through the
     #: open_files_server
     open_external = QtCore.pyqtSignal(list)
 
     #: The server to open external files
     open_files_server = None
 
@@ -131,278 +131,310 @@
     default_shortcuts = []
 
     #: The current keyboard shortcuts
     current_shortcuts = []
 
     #: The key for the central widget for the main window in the
     #: :attr:`plugins` dictionary
-    central_widget_key = 'console'
+    central_widget_key = "console"
 
     @property
     def logger(self):
         """The logger of this instance"""
-        return logging.getLogger('%s.%s' % (self.__class__.__module__,
-                                            self.__class__.__name__))
+        return logging.getLogger(
+            "%s.%s" % (self.__class__.__module__, self.__class__.__name__)
+        )
 
-    @docstrings.get_sections(base='MainWindow')
+    @docstrings.get_sections(base="MainWindow")
     @docstrings.dedent
     def __init__(self, show=True):
         """
         Parameters
         ----------
         show: bool
             If True, the created mainwindow is show
         """
         if sys.stdout is None:
             sys.stdout = StreamToLogger(self.logger)
         if sys.stderr is None:
             sys.stderr = StreamToLogger(self.logger)
         super(MainWindow, self).__init__()
-        self.setWindowIcon(QIcon(get_icon('logo.png')))
+        self.setWindowIcon(QIcon(get_icon("logo.png")))
 
         #: list of figures from the psyplot backend
         self.figures = []
         self.error_msg = PyErrorMessage(self)
         self.setDockOptions(
-            QMainWindow.AnimatedDocks | QMainWindow.AllowNestedDocks |
-            QMainWindow.AllowTabbedDocks)
+            QMainWindow.AnimatedDocks
+            | QMainWindow.AllowNestedDocks
+            | QMainWindow.AllowTabbedDocks
+        )
         #: Inprocess console
         self.console = ConsoleWidget(self)
         self.project_actions = {}
 
         self.config_pages = []
 
-        self.open_file_options = OrderedDict([
-            ('new psyplot plot from dataset', self.open_external_files),
-            ('new psyplot project', partial(self.open_external_files, [])),
-            ])
+        self.open_file_options = OrderedDict(
+            [
+                ("new psyplot plot from dataset", self.open_external_files),
+                ("new psyplot project", partial(self.open_external_files, [])),
+            ]
+        )
 
         # ---------------------------------------------------------------------
         # ----------------------------- Menus ---------------------------------
         # ---------------------------------------------------------------------
 
         # ######################## File menu ##################################
 
         # --------------------------- New plot --------------------------------
 
-        self.file_menu = QMenu('File', parent=self)
-        self.new_plot_action = QAction('New plot', self)
+        self.file_menu = QMenu("File", parent=self)
+        self.new_plot_action = QAction("New plot", self)
         self.new_plot_action.setStatusTip(
-            'Use an existing dataset (or open a new one) to create one or '
-            'more plots')
+            "Use an existing dataset (or open a new one) to create one or "
+            "more plots"
+        )
         self.register_shortcut(self.new_plot_action, QKeySequence.New)
         self.new_plot_action.triggered.connect(lambda: self.new_plots(True))
         self.file_menu.addAction(self.new_plot_action)
 
         # --------------------------- Open project ----------------------------
 
-        self.open_project_menu = QMenu('Open project', self)
+        self.open_project_menu = QMenu("Open project", self)
         self.file_menu.addMenu(self.open_project_menu)
 
-        self.open_mp_action = QAction('New main project', self)
+        self.open_mp_action = QAction("New main project", self)
         self.register_shortcut(self.open_mp_action, QKeySequence.Open)
-        self.open_mp_action.setStatusTip('Open a new main project')
+        self.open_mp_action.setStatusTip("Open a new main project")
         self.open_mp_action.triggered.connect(self.open_mp)
         self.open_project_menu.addAction(self.open_mp_action)
 
-        self.open_sp_action = QAction('Add to current', self)
+        self.open_sp_action = QAction("Add to current", self)
 
         self.register_shortcut(
-            self.open_sp_action, QKeySequence(
-                'Ctrl+Shift+O', QKeySequence.NativeText))
+            self.open_sp_action,
+            QKeySequence("Ctrl+Shift+O", QKeySequence.NativeText),
+        )
         self.open_sp_action.setStatusTip(
-            'Load a project as a sub project and add it to the current main '
-            'project')
+            "Load a project as a sub project and add it to the current main "
+            "project"
+        )
         self.open_sp_action.triggered.connect(self.open_sp)
         self.open_project_menu.addAction(self.open_sp_action)
 
         # ---------------------- load preset menu -----------------------------
 
-        self.load_preset_menu = QMenu('Load preset', parent=self)
+        self.load_preset_menu = QMenu("Load preset", parent=self)
         self.file_menu.addMenu(self.load_preset_menu)
 
         self.load_sp_preset_action = self.load_preset_menu.addAction(
-            "For selection", self.load_sp_preset)
+            "For selection", self.load_sp_preset
+        )
         self.load_sp_preset_action.setStatusTip(
-            "Load a preset for the selected project")
+            "Load a preset for the selected project"
+        )
 
         self.load_mp_preset_action = self.load_preset_menu.addAction(
-            "For full project", self.load_mp_preset)
+            "For full project", self.load_mp_preset
+        )
         self.load_sp_preset_action.setStatusTip(
-            "Load a preset for the full project")
+            "Load a preset for the full project"
+        )
 
         # ----------------------- Save project --------------------------------
 
-        self.save_project_menu = QMenu('Save', parent=self)
+        self.save_project_menu = QMenu("Save", parent=self)
         self.file_menu.addMenu(self.save_project_menu)
 
-        self.save_mp_action = QAction('Full psyplot project', self)
+        self.save_mp_action = QAction("Full psyplot project", self)
         self.save_mp_action.setStatusTip(
-            'Save the entire project into a pickle file')
+            "Save the entire project into a pickle file"
+        )
         self.register_shortcut(self.save_mp_action, QKeySequence.Save)
         self.save_mp_action.triggered.connect(self.save_mp)
         self.save_project_menu.addAction(self.save_mp_action)
 
-        self.save_sp_action = QAction('Selected psyplot project', self)
+        self.save_sp_action = QAction("Selected psyplot project", self)
         self.save_sp_action.setStatusTip(
-            'Save the selected sub project into a pickle file')
+            "Save the selected sub project into a pickle file"
+        )
         self.save_sp_action.triggered.connect(self.save_sp)
         self.save_project_menu.addAction(self.save_sp_action)
 
         # ------------------------ Save project as ----------------------------
 
-        self.save_project_as_menu = QMenu('Save as', parent=self)
+        self.save_project_as_menu = QMenu("Save as", parent=self)
         self.file_menu.addMenu(self.save_project_as_menu)
 
-        self.save_mp_as_action = QAction('Full psyplot project', self)
+        self.save_mp_as_action = QAction("Full psyplot project", self)
         self.save_mp_as_action.setStatusTip(
-            'Save the entire project into a pickle file')
-        self.register_shortcut(self.save_mp_as_action,
-                                       QKeySequence.SaveAs)
+            "Save the entire project into a pickle file"
+        )
+        self.register_shortcut(self.save_mp_as_action, QKeySequence.SaveAs)
         self.save_mp_as_action.triggered.connect(
-            partial(self.save_mp, new_fname=True))
+            partial(self.save_mp, new_fname=True)
+        )
         self.save_project_as_menu.addAction(self.save_mp_as_action)
 
-        self.save_sp_as_action = QAction('Selected psyplot project', self)
+        self.save_sp_as_action = QAction("Selected psyplot project", self)
         self.save_sp_as_action.setStatusTip(
-            'Save the selected sub project into a pickle file')
+            "Save the selected sub project into a pickle file"
+        )
         self.save_sp_as_action.triggered.connect(
-            partial(self.save_sp, new_fname=True))
+            partial(self.save_sp, new_fname=True)
+        )
         self.save_project_as_menu.addAction(self.save_sp_as_action)
 
         # ------------------------ Save preset --------------------------------
 
-        self.save_preset_menu = QMenu('Save preset', parent=self)
+        self.save_preset_menu = QMenu("Save preset", parent=self)
         self.file_menu.addMenu(self.save_preset_menu)
 
         self.save_sp_preset_action = self.save_preset_menu.addAction(
-            "Selection", self.save_sp_preset)
+            "Selection", self.save_sp_preset
+        )
         self.save_sp_preset_action.setStatusTip(
-            "Save the formatoptions of the selected project as a preset")
+            "Save the formatoptions of the selected project as a preset"
+        )
 
         self.save_mp_preset_action = self.save_preset_menu.addAction(
-            "Full project", self.save_mp_preset)
+            "Full project", self.save_mp_preset
+        )
         self.save_sp_preset_action.setStatusTip(
-            "Save the formatoptions of the full project as a preset")
+            "Save the formatoptions of the full project as a preset"
+        )
 
         # -------------------------- Pack project -----------------------------
 
-        self.pack_project_menu = QMenu('Zip project files', parent=self)
+        self.pack_project_menu = QMenu("Zip project files", parent=self)
         self.file_menu.addMenu(self.pack_project_menu)
 
-        self.pack_mp_action = QAction('Full psyplot project', self)
+        self.pack_mp_action = QAction("Full psyplot project", self)
         self.pack_mp_action.setStatusTip(
-            'Pack all the data of the main project into one folder')
+            "Pack all the data of the main project into one folder"
+        )
         self.pack_mp_action.triggered.connect(partial(self.save_mp, pack=True))
         self.pack_project_menu.addAction(self.pack_mp_action)
 
-        self.pack_sp_action = QAction('Selected psyplot project', self)
+        self.pack_sp_action = QAction("Selected psyplot project", self)
         self.pack_sp_action.setStatusTip(
-            'Pack all the data of the current sub project into one folder')
+            "Pack all the data of the current sub project into one folder"
+        )
         self.pack_sp_action.triggered.connect(partial(self.save_sp, pack=True))
         self.pack_project_menu.addAction(self.pack_sp_action)
 
         # ------------------------ Export figures -----------------------------
 
-        self.export_project_menu = QMenu('Export figures', parent=self)
+        self.export_project_menu = QMenu("Export figures", parent=self)
         self.file_menu.addMenu(self.export_project_menu)
 
-        self.export_mp_action = QAction('Full psyplot project', self)
+        self.export_mp_action = QAction("Full psyplot project", self)
         self.export_mp_action.setStatusTip(
-            'Pack all the data of the main project into one folder')
+            "Pack all the data of the main project into one folder"
+        )
         self.export_mp_action.triggered.connect(self.export_mp)
         self.register_shortcut(
-            self.export_mp_action, QKeySequence(
-                'Ctrl+E', QKeySequence.NativeText))
+            self.export_mp_action,
+            QKeySequence("Ctrl+E", QKeySequence.NativeText),
+        )
         self.export_project_menu.addAction(self.export_mp_action)
 
-        self.export_sp_action = QAction('Selected psyplot project', self)
+        self.export_sp_action = QAction("Selected psyplot project", self)
         self.export_sp_action.setStatusTip(
-            'Pack all the data of the current sub project into one folder')
+            "Pack all the data of the current sub project into one folder"
+        )
         self.register_shortcut(
-            self.export_sp_action, QKeySequence(
-                'Ctrl+Shift+E', QKeySequence.NativeText))
+            self.export_sp_action,
+            QKeySequence("Ctrl+Shift+E", QKeySequence.NativeText),
+        )
         self.export_sp_action.triggered.connect(self.export_sp)
         self.export_project_menu.addAction(self.export_sp_action)
 
         # ------------------------ Close project ------------------------------
 
         self.file_menu.addSeparator()
 
-        self.close_project_menu = QMenu('Close project', parent=self)
+        self.close_project_menu = QMenu("Close project", parent=self)
         self.file_menu.addMenu(self.close_project_menu)
 
-        self.close_mp_action = QAction('Full psyplot project', self)
+        self.close_mp_action = QAction("Full psyplot project", self)
         self.register_shortcut(
-            self.close_mp_action, QKeySequence(
-                'Ctrl+Shift+W', QKeySequence.NativeText))
+            self.close_mp_action,
+            QKeySequence("Ctrl+Shift+W", QKeySequence.NativeText),
+        )
         self.close_mp_action.setStatusTip(
-            'Close the main project and delete all data and plots out of '
-            'memory')
+            "Close the main project and delete all data and plots out of "
+            "memory"
+        )
         self.close_mp_action.triggered.connect(
-            lambda: psy.close(psy.gcp(True).num))
+            lambda: psy.close(psy.gcp(True).num)
+        )
         self.close_project_menu.addAction(self.close_mp_action)
 
-        self.close_sp_action = QAction('Selected psyplot project', self)
+        self.close_sp_action = QAction("Selected psyplot project", self)
         self.close_sp_action.setStatusTip(
-            'Close the selected arrays project and delete all data and plots '
-            'out of memory')
+            "Close the selected arrays project and delete all data and plots "
+            "out of memory"
+        )
         self.register_shortcut(self.close_sp_action, QKeySequence.Close)
         self.close_sp_action.triggered.connect(
-            lambda: psy.gcp().close(True, True))
+            lambda: psy.gcp().close(True, True)
+        )
         self.close_project_menu.addAction(self.close_sp_action)
 
         # ----------------------------- Quit ----------------------------------
 
-        if sys.platform != 'darwin':  # mac os makes this anyway
-            self.quit_action = QAction('Quit', self)
+        if sys.platform != "darwin":  # mac os makes this anyway
+            self.quit_action = QAction("Quit", self)
             self.quit_action.triggered.connect(self.close)
             self.quit_action.triggered.connect(
-                QtCore.QCoreApplication.instance().quit)
-            self.register_shortcut(
-                self.quit_action, QKeySequence.Quit)
+                QtCore.QCoreApplication.instance().quit
+            )
+            self.register_shortcut(self.quit_action, QKeySequence.Quit)
             self.file_menu.addAction(self.quit_action)
 
         self.menuBar().addMenu(self.file_menu)
 
         # ######################## Console menu ###############################
 
-        self.console_menu = QMenu('Console', self)
+        self.console_menu = QMenu("Console", self)
         self.console_menu.addActions(self.console.actions())
         self.menuBar().addMenu(self.console_menu)
 
         # ######################## Windows menu ###############################
 
-        self.windows_menu = QMenu('Windows', self)
+        self.windows_menu = QMenu("Windows", self)
         self.menuBar().addMenu(self.windows_menu)
 
         # ############################ Help menu ##############################
 
-        self.help_menu = QMenu('Help', parent=self)
+        self.help_menu = QMenu("Help", parent=self)
         self.menuBar().addMenu(self.help_menu)
 
         # -------------------------- Preferences ------------------------------
 
-        self.help_action = QAction('Preferences', self)
+        self.help_action = QAction("Preferences", self)
         self.help_action.triggered.connect(lambda: self.edit_preferences(True))
-        self.register_shortcut(self.help_action,
-                                       QKeySequence.Preferences)
+        self.register_shortcut(self.help_action, QKeySequence.Preferences)
         self.help_menu.addAction(self.help_action)
 
         # ---------------------------- About ----------------------------------
 
-        self.about_action = QAction('About', self)
+        self.about_action = QAction("About", self)
         self.about_action.triggered.connect(self.about)
         self.help_menu.addAction(self.about_action)
 
         # ---------------------------- Dependencies ---------------------------
 
-        self.dependencies_action = QAction('Dependencies', self)
+        self.dependencies_action = QAction("Dependencies", self)
         self.dependencies_action.triggered.connect(
-            lambda: self.show_dependencies(True))
+            lambda: self.show_dependencies(True)
+        )
         self.help_menu.addAction(self.dependencies_action)
 
         self.dockwidgets = []
 
         # ---------------------------------------------------------------------
         # -------------------------- Dock windows -----------------------------
         # ---------------------------------------------------------------------
@@ -410,71 +442,77 @@
         #: tree widget displaying the open datasets
         self.project_content = ProjectContentWidget(parent=self)
         self.ds_tree = DatasetTree(parent=self)
         #: tree widget displaying the open figures
         self.figures_tree = FiguresTree(parent=self)
         #: help explorer
         self.help_explorer = help_explorer = HelpExplorer(parent=self)
-        if 'HTML help' in help_explorer.viewers and help_explorer.viewers[
-                'HTML help'].sphinx_thread is not None:
+        if (
+            "HTML help" in help_explorer.viewers
+            and help_explorer.viewers["HTML help"].sphinx_thread is not None
+        ):
             help_explorer.viewers[
-                'HTML help'].sphinx_thread.html_ready.connect(
-                    self.focus_on_console)
+                "HTML help"
+            ].sphinx_thread.html_ready.connect(self.focus_on_console)
         #: the DataFrameEditor widgets
         self.dataframeeditors = []
         #: general formatoptions widget
         self.fmt_widget = FormatoptionWidget(
-            parent=self, help_explorer=help_explorer,
-            console=self.console)
+            parent=self, help_explorer=help_explorer, console=self.console
+        )
 
         # load plugin widgets
-        self.plugins = plugins = OrderedDict([
-            ('console', self.console),
-            ('project_content', self.project_content),
-            ('ds_tree', self.ds_tree),
-            ('figures_tree', self.figures_tree),
-            ('help_explorer', self.help_explorer),
-            ('fmt_widget', self.fmt_widget),
-            ])
+        self.plugins = plugins = OrderedDict(
+            [
+                ("console", self.console),
+                ("project_content", self.project_content),
+                ("ds_tree", self.ds_tree),
+                ("figures_tree", self.figures_tree),
+                ("help_explorer", self.help_explorer),
+                ("fmt_widget", self.fmt_widget),
+            ]
+        )
         self.default_plugins = list(plugins)
         for plugin_name, w_class in six.iteritems(rcParams.load_plugins()):
             plugins[plugin_name] = w_class(parent=self)
 
         self.add_mp_to_menu()
         psy.Project.oncpchange.connect(self.eventually_add_mp_to_menu)
         self.windows_menu.addSeparator()
 
-        self.window_layouts_menu = QMenu('Window layouts', self)
-        self.restore_layout_action = QAction('Restore default layout', self)
+        self.window_layouts_menu = QMenu("Window layouts", self)
+        self.restore_layout_action = QAction("Restore default layout", self)
         self.restore_layout_action.triggered.connect(self.setup_default_layout)
         self.window_layouts_menu.addAction(self.restore_layout_action)
         self.windows_menu.addMenu(self.window_layouts_menu)
 
-        self.panes_menu = QMenu('Panes', self)
+        self.panes_menu = QMenu("Panes", self)
         self.windows_menu.addMenu(self.panes_menu)
 
-        self.dataframe_menu = QMenu('DataFrame editors', self)
+        self.dataframe_menu = QMenu("DataFrame editors", self)
         self.dataframe_menu.addAction(
-            'New Editor', partial(self.new_data_frame_editor, None,
-                                  'DataFrame Editor'))
+            "New Editor",
+            partial(self.new_data_frame_editor, None, "DataFrame Editor"),
+        )
         self.dataframe_menu.addSeparator()
         self.windows_menu.addMenu(self.dataframe_menu)
 
-        self.central_widgets_menu = menu = QMenu('Central widget', self)
+        self.central_widgets_menu = menu = QMenu("Central widget", self)
         self.windows_menu.addMenu(menu)
         self.central_widgets_actions = group = QActionGroup(self)
         group.setExclusive(True)
 
         # ---------------------------------------------------------------------
         # -------------------------- connections ------------------------------
         # ---------------------------------------------------------------------
 
         self.console.help_explorer = help_explorer
-        psyp.default_print_func = partial(help_explorer.show_rst,
-                                          oname='formatoption_docs')
+        psyp.default_print_func = partial(
+            help_explorer.show_rst, oname="formatoption_docs"
+        )
         psy.PlotterInterface._print_func = psyp.default_print_func
         self.setCentralWidget(self.console)
 
         # make sure that the plots are shown between the project content and
         # the help explorer widget
         self.setCorner(Qt.TopLeftCorner, Qt.LeftDockWidgetArea)
         self.setCorner(Qt.TopRightCorner, Qt.RightDockWidgetArea)
@@ -489,26 +527,27 @@
         # ---------------------------------------------------------------------
         if show:
             self.help_explorer.show_intro(self.console.intro_msg)
 
         # ---------------------------------------------------------------------
         # ------------------------- open_files_server -------------------------
         # ---------------------------------------------------------------------
-        self.callbacks = {'new_plot': self.open_external.emit,
-                          'change_cwd': self._change_cwd,
-                          'run_script': self.console.run_script.emit,
-                          'command': self.console.run_command.emit,
-                          }
+        self.callbacks = {
+            "new_plot": self.open_external.emit,
+            "change_cwd": self._change_cwd,
+            "run_script": self.console.run_script.emit,
+            "command": self.console.run_command.emit,
+        }
 
         # Server to open external files on a single instance
-        self.open_files_server = socket.socket(socket.AF_INET,
-                                               socket.SOCK_STREAM,
-                                               socket.IPPROTO_TCP)
+        self.open_files_server = socket.socket(
+            socket.AF_INET, socket.SOCK_STREAM, socket.IPPROTO_TCP
+        )
 
-        if rcParams['main.listen_to_port']:
+        if rcParams["main.listen_to_port"]:
             self._file_thread = Thread(target=self.start_open_files_server)
             self._file_thread.setDaemon(True)
             self._file_thread.start()
 
             self.open_external.connect(self._open_external_files)
 
         self.config_pages.extend([GuiRcParamsWidget, PsyRcParamsWidget])
@@ -545,15 +584,15 @@
 
         self._is_open = True
 
     def focus_on_console(self, *args, **kwargs):
         """Put focus on the ipython console"""
         self.console._control.setFocus()
 
-    def new_data_frame_editor(self, df=None, title='DataFrame Editor'):
+    def new_data_frame_editor(self, df=None, title="DataFrame Editor"):
         """Open a new dataframe editor
 
         Parameters
         ----------
         df: pandas.DataFrame
             The dataframe to display
         title: str
@@ -561,41 +600,43 @@
 
         Returns
         -------
         psyplot_gui.dataframeeditor.DataFrameEditor
             The newly created editor"""
         editor = DataFrameEditor()
         self.dataframeeditors.append(editor)
-        editor.to_dock(self, title,
-                       Qt.RightDockWidgetArea, docktype='df')
+        editor.to_dock(self, title, Qt.RightDockWidgetArea, docktype="df")
         if df is not None:
             editor.set_df(df)
         editor.show_plugin()
         editor.maybe_tabify()
         editor.raise_()
         return editor
 
     def setup_default_layout(self):
         """Set up the default window layout"""
-        self.project_content.to_dock(self, 'Plot objects',
-                                     Qt.LeftDockWidgetArea)
-        self.ds_tree.to_dock(self, 'Datasets', Qt.LeftDockWidgetArea)
-        self.figures_tree.to_dock(self, 'Figures', Qt.LeftDockWidgetArea)
-        self.help_explorer.to_dock(self, 'Help explorer',
-                                   Qt.RightDockWidgetArea)
-        self.fmt_widget.to_dock(self, 'Formatoptions', Qt.BottomDockWidgetArea)
+        self.project_content.to_dock(
+            self, "Plot objects", Qt.LeftDockWidgetArea
+        )
+        self.ds_tree.to_dock(self, "Datasets", Qt.LeftDockWidgetArea)
+        self.figures_tree.to_dock(self, "Figures", Qt.LeftDockWidgetArea)
+        self.help_explorer.to_dock(
+            self, "Help explorer", Qt.RightDockWidgetArea
+        )
+        self.fmt_widget.to_dock(self, "Formatoptions", Qt.BottomDockWidgetArea)
 
         modify_widths = bool(self.default_widths)
         for w in map(self.plugins.__getitem__, self.default_plugins):
             if w.dock is not None:
                 w.show_plugin()
 
                 if modify_widths and with_qt5:
-                    self.resizeDocks([w.dock], [self.default_widths[w]],
-                                     Qt.Horizontal)
+                    self.resizeDocks(
+                        [w.dock], [self.default_widths[w]], Qt.Horizontal
+                    )
 
         # hide plugin widgets that should be hidden at startup
         for name, w in self.plugins.items():
             if name != self.central_widget_key:
                 w.to_dock(self)
                 if w.hidden:
                     w.hide_plugin()
@@ -611,23 +652,23 @@
         """Set the central widget
 
         Parameters
         ----------
         name: str or QWidget
             The key or the plugin widget in the :attr:`plugins` dictionary"""
         from PyQt5.QtCore import QTimer
+
         self.setUpdatesEnabled(False)
         current = self.centralWidget()
         if isinstance(name, six.string_types):
             new = self.plugins[name]
         else:
             new = name
             name = next(key for key, val in self.plugins.items() if val is new)
         if new is not current:
-
             self._dock_widths = dock_widths = OrderedDict()
             self._dock_heights = dock_heights = OrderedDict()
             for key, w in self.plugins.items():
                 if w.dock is not None and w.is_shown:
                     s = w.dock.size()
                     dock_widths[w] = s.width()
                     if w is not new:
@@ -668,70 +709,73 @@
             for w, height in self._dock_heights.items():
                 if w.dock is not None:
                     self.resizeDocks([w.dock], [height], Qt.Vertical)
 
         self.setUpdatesEnabled(True)
 
     def _save_project(self, p, new_fname=False, *args, **kwargs):
-        if new_fname or 'project_file' not in p.attrs:
+        if new_fname or "project_file" not in p.attrs:
             fname = QFileDialog.getSaveFileName(
-                self, 'Project destination', os.getcwd(),
-                'Pickle files (*.pkl);;'
-                'All files (*)'
-                )
+                self,
+                "Project destination",
+                os.getcwd(),
+                "Pickle files (*.pkl);;" "All files (*)",
+            )
             if with_qt5:  # the filter is passed as well
                 fname = fname[0]
             if not fname:
                 return
         else:
-            fname = p.attrs['project_file']
+            fname = p.attrs["project_file"]
         try:
             p.save_project(fname, *args, **kwargs)
         except Exception:
-            self.error_msg.showTraceback('<b>Could not save the project!</b>')
+            self.error_msg.showTraceback("<b>Could not save the project!</b>")
         else:
-            p.attrs['project_file'] = fname
+            p.attrs["project_file"] = fname
             if p.is_main:
                 self.update_project_action(p.num)
 
     def load_mp_preset(self):
         self._load_preset(psy.gcp(True))
 
     def load_sp_preset(self):
         self._load_preset(psy.gcp())
 
     def _load_preset(self, project, *args, **kwargs):
         fname, ok = QFileDialog.getOpenFileName(
-            self, 'Load preset', os.path.join(get_configdir(), "presets"),
-            'YAML files (*.yml *.yaml);;'
-            'All files (*)'
-            )
+            self,
+            "Load preset",
+            os.path.join(get_configdir(), "presets"),
+            "YAML files (*.yml *.yaml);;" "All files (*)",
+        )
         if ok:
             project.load_preset(fname, *args, **kwargs)
 
     def open_mp(self, *args, **kwargs):
         """Open a new main project"""
         self._open_project(main=True)
 
     def open_sp(self, *args, **kwargs):
         """Open a subproject and add it to the current main project"""
         self._open_project(main=False)
 
     def _open_project(self, *args, **kwargs):
         fname = QFileDialog.getOpenFileName(
-            self, 'Project file', os.getcwd(),
-            'Pickle files (*.pkl);;'
-            'All files (*)'
-            )
+            self,
+            "Project file",
+            os.getcwd(),
+            "Pickle files (*.pkl);;" "All files (*)",
+        )
         if with_qt5:  # the filter is passed as well
             fname = fname[0]
         if not fname:
             return
         p = psy.Project.load_project(fname, *args, **kwargs)
-        p.attrs['project_file'] = fname
+        p.attrs["project_file"] = fname
         self.update_project_action(p.num)
 
     def save_mp(self, *args, **kwargs):
         """Save the current main project."""
         self._save_project(psy.gcp(True), **kwargs)
 
     def save_sp(self, *args, **kwargs):
@@ -742,108 +786,114 @@
         self._save_preset(psy.gcp())
 
     def save_mp_preset(self):
         self._save_preset(psy.gcp(True))
 
     def _save_preset(self, project, *args, **kwargs):
         fname, ok = QFileDialog.getSaveFileName(
-            self, 'Save preset', os.path.join(get_configdir(), 'presets'),
-            'YAML file (*.yml *.yaml);;'
-            'All files (*)'
-            )
+            self,
+            "Save preset",
+            os.path.join(get_configdir(), "presets"),
+            "YAML file (*.yml *.yaml);;" "All files (*)",
+        )
         if ok:
             project.save_preset(fname, *args, **kwargs)
 
     def _export_project(self, p, *args, **kwargs):
         fname = QFileDialog.getSaveFileName(
-            self, 'Picture destination', os.getcwd(),
-            'PDF files (*.pdf);;'
-            'Postscript file (*.ps);;'
-            'PNG image (*.png);;'
-            'JPG image (*.jpg *.jpeg);;'
-            'TIFF image (*.tif *.tiff);;'
-            'GIF image (*.gif);;'
-            'All files (*)'
-            )
+            self,
+            "Picture destination",
+            os.getcwd(),
+            "PDF files (*.pdf);;"
+            "Postscript file (*.ps);;"
+            "PNG image (*.png);;"
+            "JPG image (*.jpg *.jpeg);;"
+            "TIFF image (*.tif *.tiff);;"
+            "GIF image (*.gif);;"
+            "All files (*)",
+        )
         if with_qt5:  # the filter is passed as well
             fname = fname[0]
         if not fname:
             return
         try:
             p.export(fname, *args, **kwargs)
         except Exception:
             self.error_msg.showTraceback(
-                '<b>Could not export the figures!</b>')
+                "<b>Could not export the figures!</b>"
+            )
 
     def export_mp(self, *args, **kwargs):
         self._export_project(psy.gcp(True), **kwargs)
 
     def export_sp(self, *args, **kwargs):
         self._export_project(psy.gcp(), **kwargs)
 
     def new_plots(self, exec_=None):
-        if hasattr(self, 'plot_creator'):
+        if hasattr(self, "plot_creator"):
             try:
                 self.plot_creator.close()
             except RuntimeError:
                 pass
         self.plot_creator = PlotCreator(
-            help_explorer=self.help_explorer, parent=self)
-        available_width = QDesktopWidget().availableGeometry().width() / 3.
+            help_explorer=self.help_explorer, parent=self
+        )
+        available_width = QDesktopWidget().availableGeometry().width() // 3
         width = self.plot_creator.sizeHint().width()
         height = self.plot_creator.sizeHint().height()
         # The plot creator window should cover at least one third of the screen
         self.plot_creator.resize(max(available_width, width), height)
         if exec_:
             self.plot_creator.exec_()
 
     def excepthook(self, type, value, traceback):
         """A method to replace the sys.excepthook"""
         self.error_msg.excepthook(type, value, traceback)
 
     def edit_preferences(self, exec_=None):
         """Edit Spyder preferences"""
-        if hasattr(self, 'preferences'):
+        if hasattr(self, "preferences"):
             try:
                 self.preferences.close()
             except RuntimeError:
                 pass
         self.preferences = dlg = Prefences(self)
         for PrefPageClass in self.config_pages:
             widget = PrefPageClass(dlg)
             widget.initialize()
             dlg.add_page(widget)
         available_width = int(
-            0.667*QDesktopWidget().availableGeometry().width()
+            0.667 * QDesktopWidget().availableGeometry().width()
         )
         width = dlg.sizeHint().width()
         height = dlg.sizeHint().height()
         # The preferences window should cover at least one third of the screen
         dlg.resize(max(available_width, width), height)
         if exec_:
             dlg.exec_()
 
     def about(self):
         """About the tool"""
         versions = {
-            key: d['version'] for key, d in psyplot.get_versions(False).items()
-            }
-        versions.update(psyplot_gui.get_versions()['requirements'])
-        versions.update(psyplot._get_versions()['requirements'])
-        versions['github'] = 'https://github.com/psyplot/psyplot'
-        versions['author'] = psyplot.__author__
+            key: d["version"] for key, d in psyplot.get_versions(False).items()
+        }
+        versions.update(psyplot_gui.get_versions()["requirements"])
+        versions.update(psyplot._get_versions()["requirements"])
+        versions["github"] = "https://github.com/psyplot/psyplot"
+        versions["author"] = psyplot.__author__
         QMessageBox.about(
-            self, "About psyplot",
-            u"""<b>psyplot: Interactive data visualization with python</b>
+            self,
+            "About psyplot",
+            """<b>psyplot: Interactive data visualization with python</b>
             <br>Copyright &copy; 2017- Philipp Sommer
             <br>Licensed under the terms of the GNU General Public License v2
             (GPLv2)
             <p>Created by %(author)s</p>
             <p>Most of the icons come from the
-            <a href="https://www.iconfinder.com/"> iconfinder</a>.</p>
+            <a href="https://fontawesome.com/">Fontawesom</a>.</p>
             <p>For bug reports and feature requests, please go
             to our <a href="%(github)s">Github website</a> or contact the
             author via mail.</p>
             <p>This package uses (besides others) the following packages:<br>
             <ul>
                 <li>psyplot %(psyplot)s</li>
                 <li>Python %(python)s </li>
@@ -855,196 +905,262 @@
                 <li>PyQt %(pyqt)s</li>
                 <li>qtconsole %(qtconsole)s</li>
             </ul></p>
             <p>For a full list of requirements see the <em>dependencies</em>
             in the <em>Help</em> menu.</p>
             <p>This software is provided "as is", without warranty or support
             of any kind.</p>"""
-            % versions)
+            % versions,
+        )
 
     def show_dependencies(self, exec_=None):
         """Open a dialog that shows the dependencies"""
-        if hasattr(self, 'dependencies'):
+        if hasattr(self, "dependencies"):
             try:
                 self.dependencies.close()
             except RuntimeError:
                 pass
-        self.dependencies = dlg = DependenciesDialog(psyplot.get_versions(),
-                                                     parent=self)
+        self.dependencies = dlg = DependenciesDialog(
+            psyplot.get_versions(), parent=self
+        )
         dlg.resize(630, 420)
         if exec_:
             dlg.exec_()
 
     def reset_rcParams(self):
         rcParams.update_from_defaultParams()
         psy.rcParams.update_from_defaultParams()
 
     def add_mp_to_menu(self):
         mp = psy.gcp(True)
-        action = QAction(os.path.basename(mp.attrs.get(
-            'project_file', 'Untitled %s*' % mp.num)), self)
-        action.setStatusTip(
-            'Make project %s the current project' % mp.num)
+        action = QAction(
+            os.path.basename(
+                mp.attrs.get("project_file", "Untitled %s*" % mp.num)
+            ),
+            self,
+        )
+        action.setStatusTip("Make project %s the current project" % mp.num)
         action.triggered.connect(lambda: psy.scp(psy.project(mp.num)))
         self.project_actions[mp.num] = action
         self.windows_menu.addAction(action)
 
     def update_project_action(self, num):
         action = self.project_actions.get(num)
         p = psy.project(num)
         if action:
-            action.setText(os.path.basename(p.attrs.get(
-                'project_file', 'Untitled %s*' % num)))
+            action.setText(
+                os.path.basename(
+                    p.attrs.get("project_file", "Untitled %s*" % num)
+                )
+            )
 
     def eventually_add_mp_to_menu(self, p):
         for num in set(self.project_actions).difference(
-                psy.get_project_nums()):
+            psy.get_project_nums()
+        ):
             self.windows_menu.removeAction(self.project_actions.pop(num))
         if p is None or not p.is_main:
             return
         if p.num not in self.project_actions:
             self.add_mp_to_menu()
 
     def start_open_files_server(self):
         """This method listens to the open_files_port and opens the plot
         creator for new files
 
         This method is inspired and to most parts copied from spyder"""
-        self.open_files_server.setsockopt(socket.SOL_SOCKET,
-                                          socket.SO_REUSEADDR, 1)
-        port = rcParams['main.open_files_port']
+        self.open_files_server.setsockopt(
+            socket.SOL_SOCKET, socket.SO_REUSEADDR, 1
+        )
+        port = rcParams["main.open_files_port"]
         try:
-            self.open_files_server.bind(('127.0.0.1', port))
+            self.open_files_server.bind(("127.0.0.1", port))
         except Exception:
             return
         self.open_files_server.listen(20)
         while 1:  # 1 is faster than True
             try:
                 req, dummy = self.open_files_server.accept()
             except socket.error as e:
                 # See Issue 1275 for details on why errno EINTR is
                 # silently ignored here.
                 eintr = errno.EINTR
                 # To avoid a traceback after closing on Windows
                 if e.args[0] == eintr:
                     continue
                 # handle a connection abort on close error
-                enotsock = (errno.WSAENOTSOCK if os.name == 'nt'
-                            else errno.ENOTSOCK)
+                enotsock = (
+                    errno.WSAENOTSOCK if os.name == "nt" else errno.ENOTSOCK
+                )
                 if e.args[0] in [errno.ECONNABORTED, enotsock]:
                     return
                 raise
             args = pickle.loads(req.recv(1024))
             callback = args[0]
             func = self.callbacks[callback]
-            self.logger.debug('Emitting %s callback %s', callback, func)
+            self.logger.debug("Emitting %s callback %s", callback, func)
             func(args[1:])
-            req.sendall(b' ')
+            req.sendall(b" ")
 
     def change_cwd(self, path):
         """Change the current working directory"""
         import os
+
         os.chdir(path)
 
     def _change_cwd(self, args):
         path = args[0][0]
         self.change_cwd(path)
 
     docstrings.keep_params(
-        'make_plot.parameters', 'fnames', 'project', 'engine', 'plot_method',
-        'name', 'dims', 'encoding', 'enable_post', 'seaborn_style',
-        'concat_dim', 'chname', 'preset')
+        "make_plot.parameters",
+        "fnames",
+        "project",
+        "engine",
+        "plot_method",
+        "name",
+        "dims",
+        "encoding",
+        "enable_post",
+        "seaborn_style",
+        "concat_dim",
+        "chname",
+        "preset",
+        "decoder",
+    )
 
     def open_files(self, fnames):
         """Open a file and ask the user how"""
-        fnames_s = ', '.join(map(os.path.basename, fnames))
+        fnames_s = ", ".join(map(os.path.basename, fnames))
         if len(fnames_s) > 30:
-            fnames_s = fnames_s[:27] + '...'
+            fnames_s = fnames_s[:27] + "..."
         item, ok = QInputDialog.getItem(
-            self, 'Open file...', 'Open %s as...' % fnames_s,
-            list(self.open_file_options), current=0, editable=False)
+            self,
+            "Open file...",
+            "Open %s as..." % fnames_s,
+            list(self.open_file_options),
+            current=0,
+            editable=False,
+        )
         if ok:
             return self.open_file_options[item](fnames)
 
-    @docstrings.get_sections(base='MainWindow.open_external_files')
+    @docstrings.get_sections(base="MainWindow.open_external_files")
     @docstrings.dedent
-    def open_external_files(self, fnames=[], project=None, engine=None,
-                            plot_method=None, name=None, dims=None,
-                            encoding=None, enable_post=False,
-                            seaborn_style=None, concat_dim=get_default_value(
-                                xr.open_mfdataset, 'concat_dim'), chname={},
-                            preset=None):
+    def open_external_files(
+        self,
+        fnames=[],
+        project=None,
+        engine=None,
+        plot_method=None,
+        name=None,
+        dims=None,
+        encoding=None,
+        enable_post=False,
+        seaborn_style=None,
+        concat_dim=get_default_value(xr.open_mfdataset, "concat_dim"),
+        chname={},
+        preset=None,
+        decoder=None,
+    ):
         """
         Open external files
 
         Parameters
         ----------
-        %(make_plot.parameters.fnames|project|engine|plot_method|name|dims|encoding|enable_post|seaborn_style|concat_dim|chname|preset)s
+        %(make_plot.parameters.fnames|project|engine|plot_method|name|dims|encoding|enable_post|seaborn_style|concat_dim|chname|preset|decoder)s
         """
         if seaborn_style is not None:
             import seaborn as sns
+
             sns.set_style(seaborn_style)
         if project is not None:
-            fnames = [s.split(',') for s in fnames]
+            fnames = [s.split(",") for s in fnames]
             if not isinstance(project, dict):
                 project = psyd.safe_list(project)[0]
-            single_files = (l[0] for l in fnames if len(l) == 1)
+            single_files = (files[0] for files in fnames if len(files) == 1)
             alternative_paths = defaultdict(lambda: next(single_files, None))
-            alternative_paths.update(list(l for l in fnames if len(l) == 2))
+            alternative_paths.update(
+                list(files for files in fnames if len(files) == 2)
+            )
             p = psy.Project.load_project(
-                project, alternative_paths=alternative_paths,
-                engine=engine, main=not psy.gcp(), encoding=encoding,
-                enable_post=enable_post, chname=chname)
+                project,
+                alternative_paths=alternative_paths,
+                engine=engine,
+                main=not psy.gcp(),
+                encoding=encoding,
+                enable_post=enable_post,
+                chname=chname,
+            )
             if preset:
                 p.load_preset(preset)
             if isinstance(project, six.string_types):
-                p.attrs.setdefault('project_file', project)
+                p.attrs.setdefault("project_file", project)
             return True
         else:
             self.new_plots(False)
-            self.plot_creator.open_dataset(fnames, engine=engine,
-                                           concat_dim=concat_dim)
-            if name == 'all':
+            self.plot_creator.open_dataset(
+                fnames, engine=engine, concat_dim=concat_dim
+            )
+            if name == "all":
                 ds = self.plot_creator.get_ds()
                 name = sorted(set(ds.variables) - set(ds.coords))
             self.plot_creator.insert_array(
-                list(filter(None, psy.safe_list(name))))
+                list(filter(None, psy.safe_list(name)))
+            )
             if dims is not None:
                 ds = self.plot_creator.get_ds()
-                dims = {key: ', '.join(
-                    map(str, val)) for key, val in six.iteritems(
-                        dims)}
+                dims = {
+                    key: ", ".join(map(str, val))
+                    for key, val in six.iteritems(dims)
+                }
                 for i, vname in enumerate(
-                        self.plot_creator.array_table.vnames):
+                    self.plot_creator.array_table.vnames
+                ):
                     self.plot_creator.array_table.selectRow(i)
-                    self.plot_creator.array_table.update_selected(
-                        )
+                    self.plot_creator.array_table.update_selected()
                 self.plot_creator.array_table.selectAll()
                 var = ds[vname[0]]
                 self.plot_creator.array_table.update_selected(
-                    dims=var.psy.decoder.correct_dims(var, dims.copy()))
+                    dims=var.psy.decoder.correct_dims(var, dims.copy())
+                )
             if preset:
                 self.plot_creator.set_preset(preset)
             if plot_method:
                 self.plot_creator.pm_combo.setCurrentIndex(
-                    self.plot_creator.pm_combo.findText(plot_method))
+                    self.plot_creator.pm_combo.findText(plot_method)
+                )
+            if decoder:
+                self.plot_creator.set_decoder(decoder)
             self.plot_creator.exec_()
             return True
 
     def _open_external_files(self, args):
         self.open_external_files(*args)
 
     @classmethod
-    @docstrings.get_sections(base='MainWindow.run')
+    @docstrings.get_sections(base="MainWindow.run")
     @docstrings.dedent
-    def run(cls, fnames=[], project=None, engine=None, plot_method=None,
-            name=None, dims=None, encoding=None, enable_post=False,
-            seaborn_style=None,
-            concat_dim=get_default_value(xr.open_mfdataset, 'concat_dim'),
-            chname={}, preset=None, show=True):
+    def run(
+        cls,
+        fnames=[],
+        project=None,
+        engine=None,
+        plot_method=None,
+        name=None,
+        dims=None,
+        encoding=None,
+        enable_post=False,
+        seaborn_style=None,
+        concat_dim=get_default_value(xr.open_mfdataset, "concat_dim"),
+        chname={},
+        preset=None,
+        decoder=None,
+        show=True,
+    ):
         """
         Create a mainwindow and open the given files or project
 
         This class method creates a new mainwindow instance and sets the
         global :attr:`mainwindow` variable.
 
         Parameters
@@ -1062,30 +1178,45 @@
         --------
         run_app
         """
         mainwindow = cls(show=show)
         _set_mainwindow(mainwindow)
         if fnames or project:
             mainwindow.open_external_files(
-                fnames, project, engine, plot_method, name, dims, encoding,
-                enable_post, seaborn_style, concat_dim, chname, preset)
+                fnames,
+                project,
+                engine,
+                plot_method,
+                name,
+                dims,
+                encoding,
+                enable_post,
+                seaborn_style,
+                concat_dim,
+                chname,
+                preset,
+                decoder,
+            )
         psyplot.with_gui = True
         return mainwindow
 
-    def register_shortcut(self, action, shortcut,
-                          context=Qt.ApplicationShortcut):
+    def register_shortcut(
+        self, action, shortcut, context=Qt.ApplicationShortcut
+    ):
         """Register an action for a shortcut"""
         shortcuts = psy.safe_list(shortcut)
         for j, shortcut in enumerate(shortcuts):
             found = False
             for i, (s, a) in enumerate(self.current_shortcuts):
                 if s == shortcut:
                     new_shortcuts = [
-                        sc for sc in self.current_shortcuts[i][1].shortcuts()
-                        if sc != s]
+                        sc
+                        for sc in self.current_shortcuts[i][1].shortcuts()
+                        if sc != s
+                    ]
                     a.setShortcut(QKeySequence())
                     if new_shortcuts:
                         a.setShortcuts(new_shortcuts)
                     self.current_shortcuts[i][1] = action
                     found = True
                     break
             if not found:
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/plot_creator.py` & `psyplot-gui-1.5.0/psyplot_gui/plot_creator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,78 +1,95 @@
 """This module contains a widget to create new plots with psyplot
 
 The main class is the :class:`PlotCreator` which is used to handle the
 different plotting methods of the :class:`psyplot.project.ProjectPlotter`
 class"""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
 from __future__ import division
-import os
+
 import logging
+import os
 import re
 import types
-import xarray
-from functools import partial
-import numpy as np
 from collections import defaultdict
+from functools import partial
+from itertools import chain, cycle, product, repeat, starmap
 from math import floor
-from itertools import chain, product, cycle, repeat, starmap
+
 import matplotlib as mpl
+import numpy as np
+import psyplot.project as psy
 import six
+import xarray
+from psyplot.config.rcsetup import get_configdir
 from psyplot.utils import _temp_bool_prop
-from psyplot.compat.pycompat import map, range, filter, OrderedDict
+
+from psyplot_gui.common import (
+    ListValidator,
+    LoadFromConsoleButton,
+    PyErrorMessage,
+    get_icon,
+)
 from psyplot_gui.compat.qtcompat import (
-    QWidget, QComboBox, QHBoxLayout, QVBoxLayout, QFileDialog, QToolButton,
-    QIcon, Qt, QListView, QtCore, with_qt5, QAbstractItemView, QPushButton,
-    QLabel, QValidator, QStyledItemDelegate, QLineEdit, QCheckBox, isstring,
-    QTableWidget, QTableWidgetItem, QGridLayout, QIntValidator, QMenu, QAction,
-    QInputDialog, QTabWidget, QDoubleValidator, QGraphicsScene, asstring,
-    QGraphicsRectItem, QGraphicsView, QDialog, QDialogButtonBox, QSplitter)
-from psyplot_gui.common import (get_icon, ListValidator, PyErrorMessage,
-                                LoadFromConsoleButton)
+    QAbstractItemView,
+    QAction,
+    QCheckBox,
+    QComboBox,
+    QDialog,
+    QDialogButtonBox,
+    QDoubleValidator,
+    QFileDialog,
+    QGraphicsRectItem,
+    QGraphicsScene,
+    QGraphicsView,
+    QGridLayout,
+    QHBoxLayout,
+    QIcon,
+    QIntValidator,
+    QLabel,
+    QLineEdit,
+    QListView,
+    QMenu,
+    QPushButton,
+    QSplitter,
+    QStyledItemDelegate,
+    Qt,
+    QTableWidget,
+    QTableWidgetItem,
+    QTabWidget,
+    QtCore,
+    QToolButton,
+    QValidator,
+    QVBoxLayout,
+    QWidget,
+    asstring,
+    isstring,
+    with_qt5,
+)
 from psyplot_gui.preferences import RcParamsTree
-import psyplot.project as psy
-from psyplot.config.rcsetup import get_configdir
-
 
 logger = logging.getLogger(__name__)
 
 
 class CoordComboBox(QComboBox):
     """Combobox showing coordinate information of a dataset
 
     This combobox loads its data from the current dataset and allows the
     popups to be left open. It also has a :attr:`leftclick` signal that is
     emitted when the popup is about to be closed because the user clicked on a
     value"""
 
-    close_popups = _temp_bool_prop('close_popups', default=True)
-    use_coords = _temp_bool_prop('use_coords', default=False)
+    close_popups = _temp_bool_prop("close_popups", default=True)
+    use_coords = _temp_bool_prop("use_coords", default=False)
     leftclick = QtCore.pyqtSignal(QComboBox)
 
     def __init__(self, ds_func, dim, parent=None):
         """
         Parameters
         ----------
         ds_func: function
@@ -120,16 +137,17 @@
         # keep open property is True. Therefore we have to track when the
         # index changes
         view.pressed.connect(self.handleItemPressed)
         view.doubleClicked.connect(self.hide_anyway)
 
     def eventFilter(self, obj, event):
         """Reimplemented to filter right-click events on the view()"""
-        ret = ((event.type() == QtCore.QEvent.MouseButtonPress) and
-               event.button() == Qt.RightButton)
+        ret = (
+            event.type() == QtCore.QEvent.MouseButtonPress
+        ) and event.button() == Qt.RightButton
         return ret
 
     def handleItemPressed(self, index):
         """Function to be called when an item is pressed to make sure that
         we know whether anything changed before closing the popup"""
         item = self.model().itemFromIndex(index)
         if item.checkState() == Qt.Checked:
@@ -143,16 +161,15 @@
         """Function that is called when an item is right_clicked"""
         ind = self.view().indexAt(point).row()
         self.setCurrentIndex(ind)
         self._right_clicked = True
         self._changed = True
 
     def hide_anyway(self, index=None):
-        """Function to hide the popup despite of the :attr:`_changed` attribute
-        """
+        """Function to hide the popup despite of the :attr:`_changed` attribute"""
         self._changed = True
         self.hidePopup()
 
     def hidePopup(self):
         """Reimplemented to only close the popup when the :attr:`close_popup`
         attribute is True or it is clicked outside the window"""
         if not self._right_clicked:
@@ -173,15 +190,15 @@
         super(CoordComboBox, self).mouseDoubleClickEvent(*args, **kwargs)
 
     def load_coord(self):
         """Load the coordinate data from the dataset and fill the combobox with
         it (if it is empty)"""
         if self._is_empty:
             ds = self.get_ds()
-            self.addItem('')
+            self.addItem("")
             if self.use_coords:
                 self.addItems(ds[self.dim].astype(str).values)
             else:
                 self.addItems(list(map(str, range(len(ds[self.dim])))))
             self._is_empty = False
 
 
@@ -195,15 +212,15 @@
         self.current_text = text
         self.current_names = list(table.current_names)
 
     def fixup(self, s):
         s = asstring(s)
         if not s:
             return self.table.next_available_name()
-        return self.table.next_available_name(s + '_{0}')
+        return self.table.next_available_name(s + "_{0}")
 
     def validate(self, s, pos):
         s = asstring(s)
         if not s:
             return QValidator.Intermediate, s, pos
         elif s == self.current_text:
             pass
@@ -216,16 +233,17 @@
     """Delegate using the :class:`ArrayNameValidator` for validation"""
 
     def createEditor(self, widget, option, index):
         if not index.isValid():
             return
         editor = QLineEdit(widget)
         item = self.parent().item(index.row(), index.column())
-        validator = ArrayNameValidator(item.text() if item else '',
-                                       self.parent(), editor)
+        validator = ArrayNameValidator(
+            item.text() if item else "", self.parent(), editor
+        )
         editor.setValidator(validator)
         return editor
 
 
 class VariableItemDelegate(QStyledItemDelegate):
     """Delegate alowing only the variables in the parents dataset.
 
@@ -233,37 +251,47 @@
     """
 
     def createEditor(self, widget, option, index):
         if not index.isValid():
             return
         editor = QLineEdit(widget)
         ds = self.parent().get_ds()
-        validator = ListValidator(ds.variables.keys(), self.parent().sep,
-                                  editor)
+        validator = ListValidator(
+            ds.variables.keys(), self.parent().sep, editor
+        )
         editor.setValidator(validator)
         return editor
 
 
 class VariablesTable(QTableWidget):
     """Table to display the variables of a dataset"""
 
     #: The variables in the dataset
     variables = []
 
     @property
     def selected_variables(self):
         """The currently selected variables"""
         return [
-            self.variables[i] for i in map(
+            self.variables[i]
+            for i in map(
                 list(map(asstring, self.variables)).index,
-                sorted(set(item.text() for item in self.selectedItems()
-                           if item.column() == 0)))]
-
-    def __init__(self, get_func, columns=['long_name', 'dims', 'shape'],
-                 *args, **kwargs):
+                sorted(
+                    set(
+                        item.text()
+                        for item in self.selectedItems()
+                        if item.column() == 0
+                    )
+                ),
+            )
+        ]
+
+    def __init__(
+        self, get_func, columns=["long_name", "dims", "shape"], *args, **kwargs
+    ):
         """
         Parameters
         ----------
         get_func: function
             The function that, when called without arguments, returns the
             xarray.Dataset to use
         columns: list of str
@@ -277,15 +305,15 @@
 
     def set_columns(self, columns=None):
         if columns is None:
             columns = self.column_labels
         else:
             self.column_labels = columns
         self.setColumnCount(len(columns) + 1)
-        self.setHorizontalHeaderLabels(['variable'] + columns)
+        self.setHorizontalHeaderLabels(["variable"] + columns)
 
     def fill_from_ds(self, ds=None):
         """Clear the table and insert items from the given `dataset`"""
         self.clear()
         self.set_columns()
         if ds is None:
             ds = self.get_ds()
@@ -294,21 +322,30 @@
         coords = list(ds.coords)
         self.variables = vnames = [v for v in ds.variables if v not in coords]
         self.setRowCount(len(vnames))
         for i, vname in enumerate(vnames):
             variable = ds.variables[vname]
             self.setItem(i, 0, QTableWidgetItem(asstring(vname)))
             for j, attr in enumerate(self.column_labels, 1):
-                if attr == 'dims':
-                    self.setItem(i, j, QTableWidgetItem(
-                        ', '.join(variable.dims)))
+                if attr == "dims":
+                    self.setItem(
+                        i, j, QTableWidgetItem(", ".join(variable.dims))
+                    )
                 else:
-                    self.setItem(i, j, QTableWidgetItem(
-                        str(variable.attrs.get(attr, getattr(
-                            variable, attr, '')))))
+                    self.setItem(
+                        i,
+                        j,
+                        QTableWidgetItem(
+                            str(
+                                variable.attrs.get(
+                                    attr, getattr(variable, attr, "")
+                                )
+                            )
+                        ),
+                    )
 
 
 class CoordsTable(QTableWidget):
     """A table showing the coordinates of in a dataset via instances of
     :class:`CoordComboBox`"""
 
     def __init__(self, get_func, *args, **kwargs):
@@ -327,31 +364,35 @@
         self.verticalHeader().setVisible(False)
         self.horizontalHeader().setStretchLastSection(True)
         self.verticalHeader().setStretchLastSection(True)
 
     @property
     def combo_boxes(self):
         """A list of :class:`CoordComboBox` in this table"""
-        return list(filter(
-            lambda w: w is not None,
-            (self.cellWidget(0, i) for i in range(self.columnCount()))))
+        return list(
+            filter(
+                lambda w: w is not None,
+                (self.cellWidget(0, i) for i in range(self.columnCount())),
+            )
+        )
 
     def fill_from_ds(self, ds=None):
         """Clear the table and create new comboboxes"""
         for cb in self.combo_boxes:
             cb.blockSignals(True)
         self.clear()
         if ds is None:
             ds = self.get_ds()
         if ds is None:
             return
         coords = list(ds.coords)
         vnames = [v for v in ds.variables if v not in coords]
-        self.dims = dims = list(set(
-            chain(*(ds.variables[vname].dims for vname in vnames))))
+        self.dims = dims = list(
+            set(chain(*(ds.variables[vname].dims for vname in vnames)))
+        )
         try:
             dims.sort()
         except TypeError:
             pass
         self.setColumnCount(len(dims))
         for i, dim in enumerate(dims):
             header_item = QTableWidgetItem(dim)
@@ -359,15 +400,16 @@
             self.setCellWidget(0, i, CoordComboBox(self.get_ds, dim))
 
     def sizeHint(self):
         """Reimplemented to adjust the heigth based upon the header and the
         first row"""
         return QtCore.QSize(
             super(CoordsTable, self).sizeHint().width(),
-            self.horizontalHeader().height() + self.rowHeight(0))
+            self.horizontalHeader().height() + self.rowHeight(0),
+        )
 
 
 class DragDropTable(QTableWidget):
     """Table that allows to exchange rows via drag and drop
 
     This class was mainly taken from
     http://stackoverflow.com/questions/26227885/drag-and-drop-rows-within-qtablewidget
@@ -384,16 +426,17 @@
 
         self.setSelectionMode(QAbstractItemView.ExtendedSelection)
         self.setSelectionBehavior(QAbstractItemView.SelectRows)
         self.setDragDropMode(QAbstractItemView.InternalMove)
 
     def dropEvent(self, event):
         if event.source() == self and (
-                event.dropAction() == Qt.MoveAction or
-                self.dragDropMode() == QAbstractItemView.InternalMove):
+            event.dropAction() == Qt.MoveAction
+            or self.dragDropMode() == QAbstractItemView.InternalMove
+        ):
             self.dropOn(event)
 
         else:
             super(DragDropTable, self).dropEvent(event)
 
     def moveRows(self, row, remove=False):
         """Move all selected rows to the given `row`"""
@@ -430,17 +473,19 @@
 
     def droppingOnItself(self, event, index):
         dropAction = event.dropAction()
 
         if self.dragDropMode() == QAbstractItemView.InternalMove:
             dropAction = Qt.MoveAction
 
-        if (event.source() == self and
-                event.possibleActions() & Qt.MoveAction and
-                dropAction == Qt.MoveAction):
+        if (
+            event.source() == self
+            and event.possibleActions() & Qt.MoveAction
+            and dropAction == Qt.MoveAction
+        ):
             selectedIndexes = self.selectedIndexes()
             child = index
             while child.isValid() and child != self.rootIndex():
                 if child in selectedIndexes:
                     return True
                 child = child.parent()
 
@@ -452,21 +497,23 @@
 
         index = QtCore.QModelIndex()
         row = -1
 
         if self.viewport().rect().contains(event.pos()):
             index = self.indexAt(event.pos())
             if not index.isValid() or not self.visualRect(index).contains(
-                    event.pos()):
+                event.pos()
+            ):
                 index = self.rootIndex()
 
         if self.model().supportedDropActions() & event.dropAction():
             if index != self.rootIndex():
                 dropIndicatorPosition = self.position(
-                    event.pos(), self.visualRect(index), index)
+                    event.pos(), self.visualRect(index), index
+                )
 
                 if dropIndicatorPosition == QAbstractItemView.AboveItem:
                     row = index.row()
                     # index = index.parent()
                 elif dropIndicatorPosition == QAbstractItemView.BelowItem:
                     row = index.row() + 1
                     # index = index.parent()
@@ -484,15 +531,16 @@
             r = QAbstractItemView.AboveItem
         elif rect.bottom() - pos.y() < margin:
             r = QAbstractItemView.BelowItem
         elif rect.contains(pos, True):
             r = QAbstractItemView.OnItem
 
         if r == QAbstractItemView.OnItem and not (
-                self.model().flags(index) & Qt.ItemIsDropEnabled):
+            self.model().flags(index) & Qt.ItemIsDropEnabled
+        ):
             if pos.y() < rect.center().y():
                 r = QAbstractItemView.AboveItem
             else:
                 r = QAbstractItemView.BelowItem
         return r
 
 
@@ -513,100 +561,116 @@
        subplot
     4. The check column. Checks for variable names, array names, axes and
        dimensions via the :meth:`psyplot.project._PlotterInterface.check_data`
        method
     5. Columns containing the dimension informations"""
 
     #: Pattern to interprete subplots
-    subplot_patt = re.compile(r'\((?P<fig>\d+),\s*'  # figure
-                              r'(?P<rows>\d+),\s*'   # rows
-                              r'(?P<cols>\d+),\s*'   # columns
-                              r'(?P<num1>\d+),\s*'   # position
-                              r'(?P<num2>\d+)\s*\)'  # end subplot
-                              )
+    subplot_patt = re.compile(
+        r"\((?P<fig>\d+),\s*"  # figure
+        r"(?P<rows>\d+),\s*"  # rows
+        r"(?P<cols>\d+),\s*"  # columns
+        r"(?P<num1>\d+),\s*"  # position
+        r"(?P<num2>\d+)\s*\)"  # end subplot
+    )
 
     #: pattern to interprete arbitrary axes
-    axes_patt = re.compile(r'\((?P<fig>\d+),\s*'     # figure
-                           r'(?P<x0>0*\.\d+),\s*'    # lower left x
-                           r'(?P<y0>0*\.\d+),\s*'    # lower left y
-                           r'(?P<x1>0*\.\d+),\s*'    # upper right x
-                           r'(?P<y1>0*\.\d+)\s*\)'   # upper right y
-                           )
+    axes_patt = re.compile(
+        r"\((?P<fig>\d+),\s*"  # figure
+        r"(?P<x0>0*\.\d+),\s*"  # lower left x
+        r"(?P<y0>0*\.\d+),\s*"  # lower left y
+        r"(?P<x1>0*\.\d+),\s*"  # upper right x
+        r"(?P<y1>0*\.\d+)\s*\)"  # upper right y
+    )
 
     #: The separator for variable names
-    sep = ';;'
+    sep = ";;"
 
     #: Tool tip for the variable column
-    VARIABLE_TT = ("The variables of the array from the dataset. Multiple"
-                   "variables for one array may be separated by '%s'" % (
-                       sep))
+    VARIABLE_TT = (
+        "The variables of the array from the dataset. Multiple"
+        "variables for one array may be separated by '%s'" % (sep)
+    )
 
     #: Base tool tip for a dimension column
-    DIMS_TT = ("The values for dimension %s."
-               " You can use integers either explicit, e.g."
-               "<ul>"
-               "<li>1, 2, 3, ...,</li>"
-               "</ul>"
-               "or slices like <em>start:end:step</em>, e.g."
-               "<ul>"
-               "<li>'1:6:2'</li>"
-               "</ul>"
-               "where the latter is equivalent to '1, 3, 5'")
+    DIMS_TT = (
+        "The values for dimension %s."
+        " You can use integers either explicit, e.g."
+        "<ul>"
+        "<li>1, 2, 3, ...,</li>"
+        "</ul>"
+        "or slices like <em>start:end:step</em>, e.g."
+        "<ul>"
+        "<li>'1:6:2'</li>"
+        "</ul>"
+        "where the latter is equivalent to '1, 3, 5'"
+    )
 
     def dropEvent(self, event):
         """Reimplemented to call the :meth:`check_arrays` after the call"""
         # apparently the row deletion occurs after the call of this method.
         # therefore our call of `check_arrays` leads to the (wrong) result
         # of a duplicated entry. We therefore filter them out here and make
         # sure that those arrays are not considered when checking for
         # duplicates
         messages = dict(
-            zip(self.current_names, [msg for b, msg in self.check_arrays()]))
+            zip(self.current_names, [msg for b, msg in self.check_arrays()])
+        )
         super(ArrayTable, self).dropEvent(event)
-        ignores = [arr_name for arr_name, msg in messages.items()
-                   if not msg.startswith('Found duplicated entry of')]
+        ignores = [
+            arr_name
+            for arr_name, msg in messages.items()
+            if not msg.startswith("Found duplicated entry of")
+        ]
         self.check_arrays(ignore_duplicates=ignores)
 
     @property
     def prefer_list(self):
         """Return the _prefer_list attribute of the plot_method"""
         return self.plot_method and self.plot_method._prefer_list
 
     @property
     def current_names(self):
         """The names that are currently in use"""
         if self.prefer_list:
             return []
         arr_col = self.arr_col
-        return [asstring(item.text()) for item in filter(None, map(
-            lambda i: self.item(i, arr_col), range(self.rowCount())))]
+        return [
+            asstring(item.text())
+            for item in filter(
+                None,
+                map(lambda i: self.item(i, arr_col), range(self.rowCount())),
+            )
+        ]
 
     @property
     def vnames(self):
         """The list of variable names per array"""
         var_col = self.var_col
-        return [self.item(i, var_col).text().split(';;')
-                for i in range(self.rowCount())]
+        return [
+            self.item(i, var_col).text().split(";;")
+            for i in range(self.rowCount())
+        ]
 
     @property
     def arr_names_dict(self):
         """The final dictionary containing the array names necessary for the
         `arr_names` parameter in the
-        :meth:`psyplot.data.ArrayList.from_dataset` method """
-        ret = OrderedDict()
+        :meth:`psyplot.data.ArrayList.from_dataset` method"""
+        ret = dict()
         arr_col = self.arr_col
         for irow in range(self.rowCount()):
             arr_name = asstring(self.item(irow, arr_col).text())
             if self.plot_method and self.plot_method._prefer_list:
                 d = ret.setdefault(arr_name, defaultdict(list))
-                d['name'].append(self._get_variables(irow))
+                d["name"].append(self._get_variables(irow))
                 for key, val in self._get_dims(irow).items():
                     d[key].append(val)
             else:
-                ret[arr_name] = d = {'name': self._get_variables(irow)}
+                ret[arr_name] = d = {"name": self._get_variables(irow)}
                 d.update(self._get_dims(irow))
 
         return ret
 
     @property
     def axes(self):
         """A list of axes settings corresponding to the arrays in the
@@ -617,24 +681,24 @@
         axes_col = self.axes_col
         # get the projection
         pm = self.plot_method
         kwargs = {}
         if pm is not None:
             projection = self.plot_method.plotter_cls._get_sample_projection()
             if projection is not None:
-                kwargs['projection'] = projection
+                kwargs["projection"] = projection
         for irow in range(self.rowCount()):
             arr_name = self.item(irow, arr_col).text()
             if arr_name in d:
                 continue
             d.add(arr_name)
             axes_type, args = self.axes_info(self.item(irow, axes_col))
-            if axes_type == 'subplot':
+            if axes_type == "subplot":
                 ret.append(SubplotCreator.create_subplot(*args, **kwargs))
-            elif axes_type == 'axes':
+            elif axes_type == "axes":
                 ret.append(AxesCreator.create_axes(*args, **kwargs))
             else:
                 ret.append(None)
         return ret
 
     @property
     def var_col(self):
@@ -663,28 +727,33 @@
         get_func: function
             The function that, when called without arguments, returns the
             xarray.Dataset to use
         columns: list of str
             The coordinates in the dataset"""
         super(ArrayTable, self).__init__(*args, **kwargs)
         self.get_ds = get_func
-        self.VARIABLE_LABEL = 'variable'
-        self.ARRAY_LABEL = 'array name'
-        self.AXES_LABEL = 'axes'
-        self.CHECK_LABEL = 'check'
-        self.desc_cols = [self.VARIABLE_LABEL, self.ARRAY_LABEL,
-                          self.AXES_LABEL, self.CHECK_LABEL]
+        self.VARIABLE_LABEL = "variable"
+        self.ARRAY_LABEL = "array name"
+        self.AXES_LABEL = "axes"
+        self.CHECK_LABEL = "check"
+        self.desc_cols = [
+            self.VARIABLE_LABEL,
+            self.ARRAY_LABEL,
+            self.AXES_LABEL,
+            self.CHECK_LABEL,
+        ]
         self.plot_method = None
         self.setSelectionBehavior(QAbstractItemView.SelectRows)
         self.setContextMenuPolicy(Qt.CustomContextMenu)
         self.customContextMenuRequested.connect(self.showAxesCreator)
         self.set_columns(columns)
         self.setItemDelegateForColumn(self.var_col, VariableItemDelegate(self))
         self.setItemDelegateForColumn(
-            self.arr_col, ArrayNameItemDelegate(self))
+            self.arr_col, ArrayNameItemDelegate(self)
+        )
         self.itemChanged.connect(self.check_item)
         self.itemChanged.connect(self.update_other_items)
 
     def set_columns(self, columns):
         """Set the columns of the table
 
         Parameters
@@ -719,15 +788,16 @@
             self.set_pm(plot_method)
         if ds is None:
             self.set_columns([])
             return
         coords = list(ds.coords)
         vnames = [v for v in ds.variables if v not in coords]
         self.dims = dims = list(
-            set(chain(*(ds.variables[vname].dims for vname in vnames))))
+            set(chain(*(ds.variables[vname].dims for vname in vnames)))
+        )
         try:
             dims.sort()
         except TypeError:
             pass
         self.set_columns(dims)
 
     def next_available_name(self, *args, **kwargs):
@@ -743,15 +813,15 @@
     def insert_array(self, name, check=True, **kwargs):
         """Appends the settings for an array the the list in a new row"""
         dims = set(self.get_ds().variables[name].dims)
         irow = self.rowCount()
         self.setRowCount(irow + 1)
         self.setItem(irow, 0, QTableWidgetItem(asstring(name)))
         self.setItem(irow, 1, QTableWidgetItem(self.next_available_name()))
-        self.setItem(irow, 2, QTableWidgetItem(''))
+        self.setItem(irow, 2, QTableWidgetItem(""))
         for dim in dims.intersection(kwargs):
             icol = len(self.desc_cols) + self.dims.index(dim)
             self.setItem(irow, icol, QTableWidgetItem(kwargs[dim]))
         if check:
             self.check_array(irow)
 
     def remove_arrays(self, selected=True):
@@ -779,68 +849,72 @@
         dims: dict
             a mapping from coordinate names to string values that shall be
             appended to the current text"""
         ds = self.get_ds()
         irows = {item.row() for item in self.selectedItems()}
         var_col = self.desc_cols.index(self.VARIABLE_LABEL)
         for irow in irows:
-            vname = asstring(
-                self.item(irow, var_col).text()).split(self.sep)[0].strip()
+            vname = (
+                asstring(self.item(irow, var_col).text())
+                .split(self.sep)[0]
+                .strip()
+            )
             var_dims = set(ds.variables[vname].dims)
             for dim in var_dims.intersection(dims):
                 icol = len(self.desc_cols) + self.dims.index(dim)
                 item = self.item(irow, icol)
                 curr_text = asstring(item.text())
                 if curr_text:
-                    curr_text += ', '
+                    curr_text += ", "
                 item.setText(curr_text + dims[dim])
         if check:
             for irow in irows:
                 self.check_array(irow)
 
     def add_subplots(self, rows, cols, maxn=None):
         """Add multiple subplots to the selected arrays"""
         import matplotlib.pyplot as plt
+
         irows = sorted({ind.row() for ind in self.selectedIndexes()})
         irows = irows or list(range(self.rowCount()))
         maxn = maxn or rows * cols
-        figs = chain(*(
-            [i] * maxn for i in range(1, 1000) if i not in plt.get_fignums()))
+        figs = chain(
+            *([i] * maxn for i in range(1, 1000) if i not in plt.get_fignums())
+        )
         nums = cycle(range(1, maxn + 1))
         seen = set()
         axes_col = self.desc_cols.index(self.AXES_LABEL)
         arr_col = self.desc_cols.index(self.ARRAY_LABEL)
         for irow in irows:
             arr_item = self.item(irow, arr_col)
             if arr_item is None or arr_item.text() in seen:
                 continue
             seen.add(arr_item.text())
             num = next(nums)
-            text = '(%i, %i, %i, %i, %i)' % (
-                next(figs), rows, cols, num, num)
+            text = "(%i, %i, %i, %i, %i)" % (next(figs), rows, cols, num, num)
             item = QTableWidgetItem(text)
             self.setItem(irow, axes_col, item)
 
     def add_single_subplot(self, rows, cols, row, col):
         """Add one subplot to the selected arrays on multiple figures"""
         import matplotlib.pyplot as plt
+
         irows = sorted({ind.row() for ind in self.selectedIndexes()})
         irows = irows or list(range(self.rowCount()))
         figs = (num for num in range(1, 1000) if num not in plt.get_fignums())
         num = (row - 1) * rows + col
         seen = set()
         axes_col = self.desc_cols.index(self.AXES_LABEL)
         arr_col = self.desc_cols.index(self.ARRAY_LABEL)
         for irow in irows:
             arr_item = self.item(irow, arr_col)
             if arr_item is None or arr_item.text() in seen:
                 continue
             seen.add(arr_item.text())
-            text = '(%i, %i, %i, %i, %i)' % (
-                next(figs), rows, cols, num, num)
+            text = "(%i, %i, %i, %i, %i)" % (next(figs), rows, cols, num, num)
             item = QTableWidgetItem(text)
             self.setItem(irow, axes_col, item)
 
     def showAxesCreator(self, pos):
         """Context menu for right-click on a row"""
         irows = sorted({ind.row() for ind in self.selectedIndexes()})
         if not irows:
@@ -850,91 +924,96 @@
         menu.exec_(self.mapToGlobal(pos))
 
     def axes_creator_action(self, rows):
         """Action to open a :class:`AxesCreatorCollection` for the selected
         rows"""
         axes_col = self.desc_cols.index(self.AXES_LABEL)
         items = [self.item(row, axes_col) for row in rows]
-        action = QAction('Select subplot', self)
+        action = QAction("Select subplot", self)
         types_and_args = list(
-            filter(lambda t: t[0], map(self.axes_info, items)))
+            filter(lambda t: t[0], map(self.axes_info, items))
+        )
         types = [t[0] for t in types_and_args]
         if types and all(t == types[0] for t in types):
-            if types[0] == 'subplot':
-                creator_kws = ['fig', 'rows', 'cols', 'num1', 'num2']
-            elif types[0] == 'axes':
-                creator_kws = ['fig', 'x0', 'y0', 'x1', 'y1']
+            if types[0] == "subplot":
+                creator_kws = ["fig", "rows", "cols", "num1", "num2"]
+            elif types[0] == "axes":
+                creator_kws = ["fig", "x0", "y0", "x1", "y1"]
             else:
                 creator_kws = []
             func_name = types[0]
             args = [t[1] for t in types_and_args]
 
             #: the initialization keywords of the :class:`SubplotCreator` class
             kwargs = {}
 
             if len(items) > 0:
-                kwargs['fig'] = ''
+                kwargs["fig"] = ""
 
             for kw, vals in zip(creator_kws, zip(*args)):
                 if all(val == vals[0] for val in vals):
                     kwargs[kw] = vals[0]
         else:
             func_name = None
             kwargs = {}
 
         action.triggered.connect(
-            self._open_axes_creator(items, func_name, kwargs))
+            self._open_axes_creator(items, func_name, kwargs)
+        )
         return action
 
     def _change_axes(self, items, iterator):
         seen = set()
         arr_col = self.desc_cols.index(self.ARRAY_LABEL)
         for item, text in zip(items, iterator):
             arr_name = self.item(item.row(), arr_col).text()
             if arr_name in seen:
                 continue
             seen.add(arr_name)
             item.setText(text)
 
     def _open_axes_creator(self, items, func_name, kwargs):
-
         def func():
-            if hasattr(self, '_axes_creator'):
+            if hasattr(self, "_axes_creator"):
                 self._axes_creator.close()
             self._axes_creator = obj = AxesCreatorCollection(
-                func_name, kwargs, parent=self)
+                func_name, kwargs, parent=self
+            )
             obj.okpressed.connect(partial(self._change_axes, items))
             obj.exec_()
+
         return func
 
     def axes_info(self, s):
         """Interpretes an axes information"""
         s = asstring(s) if isstring(s) else asstring(s.text())
         m = self.subplot_patt.match(s)
         if m:
-            return 'subplot', list(map(int, m.groups()))
+            return "subplot", list(map(int, m.groups()))
         m = self.axes_patt.match(s)
         if m:
-            return 'axes', [int(m.groupdict()['fig'])] + list(map(
-                float, m.groups()[1:]))
+            return "axes", [int(m.groupdict()["fig"])] + list(
+                map(float, m.groups()[1:])
+            )
         return None, None
 
     def set_pm(self, s):
         """Set the plot method"""
         s = asstring(s)
         self.plot_method = getattr(psy.plot, s, None)
         self.check_arrays()
 
     def check_item(self, item):
         """Check the array corresponding to the given item"""
         if item.column() == self.desc_cols.index(self.CHECK_LABEL):
             return
         for irow in range(self.rowCount()):
             other_item = self.item(
-                irow, self.desc_cols.index(self.ARRAY_LABEL))
+                irow, self.desc_cols.index(self.ARRAY_LABEL)
+            )
             if other_item is not None:
                 self.check_array(irow)
 
     def update_other_items(self, item):
         """Updates the axes information of the other items corresponding
         that have the same array name as the array corresponding to the given
         `item`"""
@@ -952,141 +1031,160 @@
             if row != this_row:
                 arr_item2 = self.item(row, arr_col)
                 if arr_item2 is not None and arr_item2.text() == arr_name:
                     self.item(row, axes_col).setText(item.text())
         self.blockSignals(False)
 
     def get_all_rows(self, row):
-        """Return all the rows that have the same array name as the given `row`
-        """
+        """Return all the rows that have the same array name as the given `row`"""
+
         def check_item(row):
             item = self.item(row, arr_col)
             return item is not None and item.text() == arr_name
 
         if self.plot_method is None or not self.plot_method._prefer_list:
             return [row]
         arr_col = self.desc_cols.index(self.ARRAY_LABEL)
         arr_name = self.item(row, arr_col).text()
         return [r for r in range(self.rowCount()) if check_item(r)]
 
     def check_array(self, row, ignore_duplicates=[]):
         """check whether the array variables are valid, the array name is
         valid, the axes info is valid and the dimensions"""
+
         def set_check(row, valid, msg):
             check_item = QTableWidgetItem()
             check_item.setFlags(check_item.flags() ^ Qt.ItemIsEditable)
             if valid:
-                check_item.setIcon(QIcon(get_icon('valid.png')))
+                check_item.setIcon(QIcon(get_icon("valid.png")))
             elif valid is None:
-                check_item.setIcon(QIcon(get_icon('warning.png')))
+                check_item.setIcon(QIcon(get_icon("warning.png")))
                 check_item.setToolTip(msg)
             else:
-                check_item.setIcon(QIcon(get_icon('invalid.png')))
+                check_item.setIcon(QIcon(get_icon("invalid.png")))
                 check_item.setToolTip(msg)
             self.setItem(row, check_col, check_item)
             self.resizeColumnToContents(check_col)
 
         check_col = self.desc_cols.index(self.CHECK_LABEL)
         valid = True
-        msg = ''
+        msg = ""
 
         # ---------------------------------------------------------------------
         # ----------------- check if a variable is provided -------------------
         # ---------------------------------------------------------------------
 
         var_item = self.item(row, self.desc_cols.index(self.VARIABLE_LABEL))
         if var_item is not None and not asstring(var_item.text()).strip():
             valid = False
-            msg = 'At least one variable name must be provided!'
+            msg = "At least one variable name must be provided!"
 
         # ---------------------------------------------------------------------
         # ----------------- check for duplicates of array names ---------------
         # ---------------------------------------------------------------------
 
         arr_col = self.desc_cols.index(self.ARRAY_LABEL)
         arr_item = self.item(row, arr_col)
         if valid and arr_item is not None:
             arr_name = arr_item.text()
             if arr_name not in ignore_duplicates:
                 if not arr_name:
-                    msg = 'An array name must be provided'
+                    msg = "An array name must be provided"
                     valid = False
-                elif (len([name for name in self.current_names
-                          if name == arr_name]) > 1):
+                elif (
+                    len(
+                        [
+                            name
+                            for name in self.current_names
+                            if name == arr_name
+                        ]
+                    )
+                    > 1
+                ):
                     valid = False
                     msg = "Found duplicated entry of '%s'" % arr_name
 
         # ---------------------------------------------------------------------
         # ------- check the plotmethod if necessary and set the icon ----------
         # ---------------------------------------------------------------------
 
         if valid and self.plot_method is not None:
             rows = self.get_all_rows(row)
             checks, messages = self.plot_method.check_data(
-                    self.get_ds(),
-                    name=list(map(self._get_variables, rows)),
-                    dims=list(map(self._get_dims, rows)))
+                self.get_ds(),
+                name=list(map(self._get_variables, rows)),
+                dims=list(map(self._get_dims, rows)),
+            )
             for row2, valid, msg in zip(rows, checks, messages):
                 set_check(row2, valid, msg)
             valid = checks[rows.index(row)]
             msg = messages[rows.index(row)]
         else:
             set_check(row, valid, msg)
 
         return valid, msg
 
     def check_arrays(self, **kwargs):
         """Convenience function to check all arrays using the
         :meth:`check_array` method"""
-        return list(map(partial(self.check_array, **kwargs),
-                        range(self.rowCount())))
+        return list(
+            map(partial(self.check_array, **kwargs), range(self.rowCount()))
+        )
 
     def _str2slice(self, s):
         s = s.strip()
         if not s:
             return []
-        s = s.split(':')
+        s = s.split(":")
         if len(s) > 1:
             return range(*map(int, s[:3]))
         return [int(s[0])]
 
     def _get_dims(self, row):
         start = len(self.desc_cols)
         ret = {}
-        for dim, item in zip(self.dims,
-                             map(lambda col: self.item(row, col),
-                                 range(start, self.columnCount()))):
+        for dim, item in zip(
+            self.dims,
+            map(
+                lambda col: self.item(row, col),
+                range(start, self.columnCount()),
+            ),
+        ):
             if item:
                 text = asstring(item.text())
                 if text:
                     slices = list(
-                        chain(*map(self._str2slice, text.split(','))))
+                        chain(*map(self._str2slice, text.split(",")))
+                    )
                     if len(slices) == 1:
                         slices = slices[0]
                     ret[dim] = slices
         return ret
 
     def _get_variables(self, row):
         var_col = self.desc_cols.index(self.VARIABLE_LABEL)
-        ret = [s.strip() for s in asstring(
-                   self.item(row, var_col).text()).split(self.sep)]
+        ret = [
+            s.strip()
+            for s in asstring(self.item(row, var_col).text()).split(self.sep)
+        ]
         ds = self.get_ds()
         for i, name in enumerate(ret):
             ret[i] = next(v for v in ds if asstring(v) == name)
         if len(ret) == 1:
             return ret[0]
         return ret
 
 
 class SubplotCreator(QWidget):
     """Select a subplot to which will be created (if not already existing) when
     making the plot"""
 
-    def __init__(self, fig=None, rows=1, cols=1, num1=1, num2=None, *args,
-                 **kwargs):
+    def __init__(
+        self, fig=None, rows=1, cols=1, num1=1, num2=None, *args, **kwargs
+    ):
         """
         Parameters
         ----------
         fig: int or None
             The number of the figure
         rows: int
             The number of rows for the gridspec
@@ -1095,39 +1193,45 @@
         num1: int
             The number of the upper left corner starting from 1
         num2: int or None
             The number of the lower right corner starting from 1. If None,
             `num1` is used"""
         super(SubplotCreator, self).__init__(*args, **kwargs)
 
-        self.fig_label = QLabel('Figure number:', self)
+        self.fig_label = QLabel("Figure number:", self)
         if fig is None:
             import matplotlib.pyplot as plt
+
             fig = next(
-                num for num in range(1, 1000) if num not in plt.get_fignums())
+                num for num in range(1, 1000) if num not in plt.get_fignums()
+            )
         self.fig_edit = QLineEdit(str(fig), self)
         self.fig_edit.setValidator(QIntValidator())
 
-        self.rows_label = QLabel('No. of rows:', self)
+        self.rows_label = QLabel("No. of rows:", self)
         self.rows_edit = QLineEdit(str(rows), self)
         self.rows_edit.setValidator(QIntValidator(1, 9999, parent=self))
 
-        self.cols_label = QLabel('No. of columns:', self)
+        self.cols_label = QLabel("No. of columns:", self)
         self.cols_edit = QLineEdit(str(cols), self)
         self.cols_edit.setValidator(QIntValidator(1, 9999, parent=self))
 
-        self.num1_label = QLabel('Subplot number:', self)
+        self.num1_label = QLabel("Subplot number:", self)
         self.num1_edit = QLineEdit(str(num1), self)
-        self.num1_edit.setValidator(QIntValidator(
-            1,  max(1, (rows or 1)*(cols or 1)), self.num1_edit))
+        self.num1_edit.setValidator(
+            QIntValidator(1, max(1, (rows or 1) * (cols or 1)), self.num1_edit)
+        )
 
-        self.num2_label = QLabel('End of the plot', self)
+        self.num2_label = QLabel("End of the plot", self)
         self.num2_edit = QLineEdit(str(num2 or num1))
-        self.num2_edit.setValidator(QIntValidator(
-            num1,  max(1, (rows or 1)*(cols or 1)), self.num2_edit))
+        self.num2_edit.setValidator(
+            QIntValidator(
+                num1, max(1, (rows or 1) * (cols or 1)), self.num2_edit
+            )
+        )
 
         self.table = table = QTableWidget(self)
         table.setSelectionMode(QAbstractItemView.ContiguousSelection)
         table.resizeRowsToContents()
         table.resizeColumnsToContents()
         table.setEditTriggers(QAbstractItemView.NoEditTriggers)
         self.setup_table()
@@ -1178,28 +1282,37 @@
 
         Returns
         -------
         mpl.axes.Subplot
             The new created subplot"""
         if not isinstance(fig, mpl.figure.Figure):
             import matplotlib.pyplot as plt
-            fig = plt.figure(fig or next(
-                num for num in range(1, 1000) if num not in plt.get_fignums()))
+
+            fig = plt.figure(
+                fig
+                or next(
+                    num
+                    for num in range(1, 1000)
+                    if num not in plt.get_fignums()
+                )
+            )
         if num1 == num2:
             num2 = None
         elif num2 is not None:
             num2 = num2 - 1
         num1 = num1 - 1
         # first check if an axes with this specification already exists and if
         # yes, return it
         for ax in fig.axes:
             ss = ax.get_subplotspec()
             if ss.num1 == num1 and (
-                    ss.num2 == num2 or (ss.num2 is None and num1 == num2) or
-                    (num2 is None and ss.num2 == num1)):
+                ss.num2 == num2
+                or (ss.num2 is None and num1 == num2)
+                or (num2 is None and ss.num2 == num1)
+            ):
                 gs = ss.get_gridspec()
                 if gs.get_geometry() == (rows, cols):
                     return ax
         # if it does not exist, create a new one
         gs = mpl.gridspec.GridSpec(rows, cols)
         ss = mpl.gridspec.SubplotSpec(gs, num1, num2)
         return fig.add_subplot(ss, **kwargs)
@@ -1212,50 +1325,52 @@
         if not rows or not cols:
             return
         self.table.clear()
         self.table.setRowCount(rows)
         self.table.setColumnCount(cols)
         selected = int(self.num1_edit.text() or 0)
         if selected:
-            selected = (int(floor(selected / (cols + 1))),
-                        ((selected % cols) - 1) % cols)
+            selected = (
+                int(floor(selected / (cols + 1))),
+                ((selected % cols) - 1) % cols,
+            )
         else:
             selected = (0, 0)
         for i, (row, col) in enumerate(product(range(rows), range(cols)), 1):
             item = QTableWidgetItem(str(i))
             self.table.setItem(row, col, item)
         self.table.resizeColumnsToContents()
         self.table.resizeRowsToContents()
-        self.num1_edit.validator().setTop(max(1, rows*cols))
+        self.num1_edit.validator().setTop(max(1, rows * cols))
         self.set_num2_validator(self.num1_edit.text())
         self.set_selected_from_num1(self.num1_edit.text())
 
     def set_num2_validator(self, s):
         """Set the validator range for the num2 line edit"""
         num1 = int(s or 1)
         rows = int(self.rows_edit.text() or 0)
         cols = int(self.cols_edit.text() or 0)
         num2 = int(self.num2_edit.text() or num1)
         self.num2_edit.setText(str(max(num1, num2)))
         self.num2_edit.validator().setRange(
-            num1, max(1, (rows or 1)*(cols or 1)))
+            num1, max(1, (rows or 1) * (cols or 1))
+        )
 
     def set_selected_from_num1(self, s):
         """Update the selection of the table after changes of
         :attr:`num1_edit`"""
         self.table.clearSelection()
         if not s:
             return
         num1 = int(s)
         num2 = int(self.num2_edit.text() or num1)
         self.set_selected(num1, num2)
 
     def set_selected_from_num2(self, s):
-        """Update the selection of the table after changes of :attr:`num2_edit`
-        """
+        """Update the selection of the table after changes of :attr:`num2_edit`"""
         self.table.clearSelection()
         if not s:
             return
         num2 = int(s)
         num1 = int(self.num1_edit.text() or 0)
         if not num1:
             return
@@ -1264,18 +1379,20 @@
     def set_selected(self, num1, num2):
         """Update the selection in the table based upon `num1` and `num2`"""
         self.table.clearSelection()
         rows = int(self.rows_edit.text() or 0)
         cols = int(self.cols_edit.text() or 0)
         if not rows or not cols:
             return
-        sel_rows = range(int(floor(num1 / (cols + 1))),
-                         int(floor(num2 / (cols + 1))) + 1)
-        sel_cols = range(((num1 % cols) - 1) % cols,
-                         (((num2 % cols) - 1) % cols) + 1)
+        sel_rows = range(
+            int(floor(num1 / (cols + 1))), int(floor(num2 / (cols + 1))) + 1
+        )
+        sel_cols = range(
+            ((num1 % cols) - 1) % cols, (((num2 % cols) - 1) % cols) + 1
+        )
         for item in starmap(self.table.item, product(sel_rows, sel_cols)):
             if item:
                 self.table.blockSignals(True)
                 item.setSelected(True)
                 self.table.blockSignals(False)
 
     def update_num_edit(self):
@@ -1297,22 +1414,36 @@
     def get_iter(self):
         """Get the iterator over the axes"""
         fig_text = self.fig_edit.text()
         if fig_text:
             figs = repeat(fig_text)
         else:
             import matplotlib.pyplot as plt
-            figs = map(str, (num for num in range(1, 1000)
-                             if num not in plt.get_fignums()))
-        num1 = self.num1_edit.text() or '1'
+
+            figs = map(
+                str,
+                (
+                    num
+                    for num in range(1, 1000)
+                    if num not in plt.get_fignums()
+                ),
+            )
+        num1 = self.num1_edit.text() or "1"
         num2 = self.num2_edit.text() or num1
-        return ('(%s, %s, %s, %s, %s)' % (
-                fig, self.rows_edit.text() or '1',
-                self.cols_edit.text() or '1', num1, num2)
-                for fig in figs)
+        return (
+            "(%s, %s, %s, %s, %s)"
+            % (
+                fig,
+                self.rows_edit.text() or "1",
+                self.cols_edit.text() or "1",
+                num1,
+                num2,
+            )
+            for fig in figs
+        )
 
 
 class AxesViewer(QGraphicsView):
     """Widget to show a rectangle"""
 
     sizeChanged = QtCore.pyqtSignal(QtCore.QSize)
 
@@ -1320,23 +1451,25 @@
         super(AxesViewer, self).__init__(*args, **kwargs)
         self.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
         self.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
 
     def resizeEvent(self, *args, **kwargs):
         super(AxesViewer, self).resizeEvent(*args, **kwargs)
         self.setSceneRect(
-            0, 0, self.frameSize().width(), self.frameSize().height())
+            0, 0, self.frameSize().width(), self.frameSize().height()
+        )
         self.sizeChanged.emit(self.size())
 
 
 class AxesCreator(QWidget):
     """Widget to setup an axes in a arbitrary location"""
 
-    def __init__(self, fig=None, x0=0.125, y0=0.1, x1=0.9, y1=0.9,
-                 *args, **kwargs):
+    def __init__(
+        self, fig=None, x0=0.125, y0=0.1, x1=0.9, y1=0.9, *args, **kwargs
+    ):
         """
         Parameters
         ----------
         fig: int or None
             The figure number. If None, a new figure number will be used
         x0: float
             the x-coordinate of the lower left corner (between 0 and 1)
@@ -1344,53 +1477,52 @@
             the y-coordinate of the lower left corner (between 0 and 1)
         x1: float
             the x-coordinate of the upper right corner (between 0 and 1)
         y1: float
             the y-coordinate of the upper right corner (between 0 and 1)
         """
         super(AxesCreator, self).__init__(*args, **kwargs)
-        self.fig_label = QLabel('Figure number:', self)
+        self.fig_label = QLabel("Figure number:", self)
         if fig is None:
             import matplotlib.pyplot as plt
+
             fig = next(
-                num for num in range(1, 1000) if num not in plt.get_fignums())
+                num for num in range(1, 1000) if num not in plt.get_fignums()
+            )
         self.fig_edit = QLineEdit(str(fig), self)
         self.fig_edit.setValidator(QIntValidator())
 
-        self.x0_label = QLabel('Lower left x: ', self)
+        self.x0_label = QLabel("Lower left x: ", self)
         self.x0_edit = QLineEdit(str(x0), self)
-        self.x0_edit.setValidator(QDoubleValidator(0.0, 1.0, 5,
-                                                   parent=self))
+        self.x0_edit.setValidator(QDoubleValidator(0.0, 1.0, 5, parent=self))
 
-        self.y0_label = QLabel('Lower left y: ', self)
+        self.y0_label = QLabel("Lower left y: ", self)
         self.y0_edit = QLineEdit(str(y0), self)
-        self.y0_edit.setValidator(QDoubleValidator(0.0, 1.0, 5,
-                                                   parent=self))
+        self.y0_edit.setValidator(QDoubleValidator(0.0, 1.0, 5, parent=self))
 
-        self.x1_label = QLabel('Upper right x: ', self)
+        self.x1_label = QLabel("Upper right x: ", self)
         self.x1_edit = QLineEdit(str(x1), self)
-        self.x1_edit.setValidator(QDoubleValidator(0.0, 1.0, 5,
-                                                   parent=self))
+        self.x1_edit.setValidator(QDoubleValidator(0.0, 1.0, 5, parent=self))
 
-        self.y1_label = QLabel('Upper right y: ', self)
+        self.y1_label = QLabel("Upper right y: ", self)
         self.y1_edit = QLineEdit(str(y1), self)
-        self.y1_edit.setValidator(QDoubleValidator(0.5, 1.0, 5,
-                                                   parent=self))
+        self.y1_edit.setValidator(QDoubleValidator(0.5, 1.0, 5, parent=self))
 
         self.graphics_scene = QGraphicsScene(self)
         self.graphics_view = AxesViewer(self.graphics_scene)
 
         size = self.graphics_view.size()
         width = size.width() * float(x1 - x0)
         height = size.height() * float(y1 - y0)
         x0_resized = size.width() * float(x0)
         y0_resized = size.height() * float(y0)
 
         self.box_widget = QGraphicsRectItem(
-            x0_resized, y0_resized, width, height)
+            x0_resized, y0_resized, width, height
+        )
         self.graphics_scene.addItem(self.box_widget)
         self.graphics_view.sizeChanged.connect(self.resize_rectangle)
 
         layout = QGridLayout()
         layout.addWidget(self.fig_label, 0, 0)
         layout.addWidget(self.fig_edit, 0, 1)
         layout.addWidget(self.x0_label, 1, 0)
@@ -1401,23 +1533,28 @@
         layout.addWidget(self.x1_edit, 3, 1)
         layout.addWidget(self.y1_label, 4, 0)
         layout.addWidget(self.y1_edit, 4, 1)
 
         layout.addWidget(self.graphics_view, 1, 2, 4, 4)
 
         for w in [self.x0_edit, self.y0_edit, self.x1_edit, self.y1_edit]:
-            w.textChanged.connect(lambda s: self.resize_rectangle(
-                self.graphics_view.size()))
+            w.textChanged.connect(
+                lambda s: self.resize_rectangle(self.graphics_view.size())
+            )
 
         self.setLayout(layout)
 
     def resize_rectangle(self, size):
         """resize the rectangle after changes of the widget size"""
-        coords = [self.x0_edit.text(), self.y0_edit.text(),
-                  self.x1_edit.text(), self.y1_edit.text()]
+        coords = [
+            self.x0_edit.text(),
+            self.y0_edit.text(),
+            self.x1_edit.text(),
+            self.y1_edit.text(),
+        ]
         if any(not c for c in coords):
             return
         x0, y0, x1, y1 = map(float, coords)
         width = size.width() * float(x1 - x0)
         height = size.height() * float(y1 - y0)
         x0_resized = size.width() * float(x0)
         y1_resized = size.height() * float(1.0 - y1)
@@ -1442,16 +1579,23 @@
             the y-coordinate of the upper right corner (between 0 and 1)
         ``**kwargs``
             Any other keyword argument for the
             :meth:`matplotlib.figure.Figure.add_axes` method
         """
         if not isinstance(fig, mpl.figure.Figure):
             import matplotlib.pyplot as plt
-            fig = plt.figure(fig or next(
-                num for num in range(1, 1000) if num not in plt.get_fignums()))
+
+            fig = plt.figure(
+                fig
+                or next(
+                    num
+                    for num in range(1, 1000)
+                    if num not in plt.get_fignums()
+                )
+            )
         x1 = max([x0, x1])
         y1 = max([y0, y1])
         bbox = mpl.transforms.Bbox.from_extents(x0, y0, x1, y1)
         points = np.round(bbox.get_points(), 5)
         for ax in fig.axes:
             if (np.round(ax.get_position().get_points(), 5) == points).all():
                 return ax
@@ -1460,36 +1604,45 @@
     def get_iter(self):
         """Get the iterator over the axes"""
         fig_text = self.fig_edit.text()
         if fig_text:
             figs = repeat(fig_text)
         else:
             import matplotlib.pyplot as plt
-            figs = map(str, (num for num in range(1, 1000)
-                             if num not in plt.get_fignums()))
-        left = self.x0_edit.text() or '0.125'
-        bottom = self.y0_edit.text() or '0.1'
-        width = self.x1_edit.text() or '0.9'
-        height = self.y1_edit.text() or '0.9'
-        return ('(%s, %s, %s, %s, %s)' % (fig, left, bottom, width, height)
-                for fig in figs)
+
+            figs = map(
+                str,
+                (
+                    num
+                    for num in range(1, 1000)
+                    if num not in plt.get_fignums()
+                ),
+            )
+        left = self.x0_edit.text() or "0.125"
+        bottom = self.y0_edit.text() or "0.1"
+        width = self.x1_edit.text() or "0.9"
+        height = self.y1_edit.text() or "0.9"
+        return (
+            "(%s, %s, %s, %s, %s)" % (fig, left, bottom, width, height)
+            for fig in figs
+        )
 
 
 class AxesSelector(QWidget):
     """Widget to select an already created axes
 
     Click the button, select your axes and click the button again"""
 
     def __init__(self, *args, **kwargs):
         super(AxesSelector, self).__init__(*args, **kwargs)
-        self.bt_choose = QPushButton('Click to select axes', self)
+        self.bt_choose = QPushButton("Click to select axes", self)
         self.bt_choose.setCheckable(True)
-        self.msg_label = QLabel('', self)
+        self.msg_label = QLabel("", self)
 
-        self.result_label = QLabel('', self)
+        self.result_label = QLabel("", self)
 
         self.layout = QVBoxLayout()
         self.layout.addWidget(self.bt_choose)
         self.layout.addWidget(self.msg_label)
         self.layout.addWidget(self.result_label)
 
         self.setLayout(self.layout)
@@ -1498,43 +1651,45 @@
 
     def change_pickers(self, b):
         """Change the pickers of the axes instances
 
         If the push button is clicked, we replace the existing pickers of the
         axes in order to select the plots. Otherwise we restore them"""
         if self.bt_choose.isChecked():
-            self.bt_choose.setText('Click when finished')
-            self.msg_label.setText('Select an existing axes')
-            self.result_label.setText('')
+            self.bt_choose.setText("Click when finished")
+            self.msg_label.setText("Select an existing axes")
+            self.result_label.setText("")
             self.allow_axes_select()
         else:
-            self.bt_choose.setText('Select an axes')
-            self.msg_label.setText('')
+            self.bt_choose.setText("Select an axes")
+            self.msg_label.setText("")
             self.restore_pickers()
 
     def unclick(self):
         """Restore the original pickers"""
         if self.bt_choose.isChecked():
             self.bt_choose.click()
 
     def allow_axes_select(self):
         """Replace make all axes pickable"""
         import matplotlib.pyplot as plt
+
         self.fig_events = d = {}
         self.pickers = pickers = defaultdict(dict)
         for num in plt.get_fignums():
             fig = plt.figure(num)
-            d[num] = fig.canvas.mpl_connect('pick_event', self.get_picked_ax)
+            d[num] = fig.canvas.mpl_connect("pick_event", self.get_picked_ax)
             for ax in fig.axes:
                 pickers[num][ax] = ax.get_picker()
                 ax.set_picker(True)
 
     def restore_pickers(self):
         """Restore the original pickers of the existing axes instances"""
         import matplotlib.pyplot as plt
+
         for num, cid in self.fig_events.items():
             plt.figure(num).canvas.mpl_disconnect(cid)
             for artist, picker in self.pickers[num].items():
                 artist.set_picker(picker)
         self.fig_events.clear()
         self.pickers.clear()
 
@@ -1542,51 +1697,54 @@
         """Function to be called when an axes is picked"""
         try:
             ax = event.artist.axes
         except AttributeError:
             ax = event.artist.get_axes()
         text = self.result_label.text()
         if text:
-            text += ';;'
-        self.result_label.setText(
-            text + self.inspect_axes(ax))
+            text += ";;"
+        self.result_label.setText(text + self.inspect_axes(ax))
 
     def inspect_axes(self, ax):
         """Inspect the given axes and get the right string for making a plot
         with it"""
         from matplotlib.axes import SubplotBase
+
         if isinstance(ax, SubplotBase):
             ss = ax.get_subplotspec()
             gs = ss.get_gridspec()
             rows, cols = gs.get_geometry()
-            return '(%i, %i, %i, %i, %i)' % (
-                ax.get_figure().number, rows, cols, ss.num1 + 1,
-                (ss.num2 or ss.num1) + 1)
+            return "(%i, %i, %i, %i, %i)" % (
+                ax.get_figure().number,
+                rows,
+                cols,
+                ss.num1 + 1,
+                (ss.num2 or ss.num1) + 1,
+            )
         else:
             box = ax.get_position()
             points = np.round(box.get_points().ravel(), 5).tolist()
-            return '(%i, %1.5f, %1.5f, %1.5f, %1.5f)' % tuple(
-                [ax.get_figure().number] + points)
+            return "(%i, %1.5f, %1.5f, %1.5f, %1.5f)" % tuple(
+                [ax.get_figure().number] + points
+            )
 
     def setVisible(self, b):
-        """Reimplemented to restore the pickers if the widget is made invisible
-        """
+        """Reimplemented to restore the pickers if the widget is made invisible"""
         super(AxesSelector, self).setVisible(b)
         if not self.isVisible():
             self.unclick()
 
     def close(self):
-        """Reimplemented to restore the pickers if the widget is closed
-        """
+        """Reimplemented to restore the pickers if the widget is closed"""
         self.unclick()
         return super(AxesSelector, self).close()
 
     def get_iter(self):
         """Get the iterator over the axes"""
-        return (txt for txt in cycle(self.result_label.text().split(';;')))
+        return (txt for txt in cycle(self.result_label.text().split(";;")))
 
 
 class AxesCreatorCollection(QDialog):
     """Wrapper for a QToolBox that holds the different possibilities to select
     an axes
 
     When the user finished, the :attr:`okpressed` symbol is emitted with an
@@ -1595,33 +1753,35 @@
 
     #: signal that is emitted when the 'Ok' pushbutton is pressed and the user
     #: finished the selection
     okpressed = QtCore.pyqtSignal(types.GeneratorType)
 
     #: key, title and class fot the widget that is used to create an
     #: axes
-    widgets = [('subplot', 'Subplot in a grid', SubplotCreator),
-               ('axes', 'Arbitray position', AxesCreator),
-               ('choose', 'Existing subplot', AxesSelector)]
+    widgets = [
+        ("subplot", "Subplot in a grid", SubplotCreator),
+        ("axes", "Arbitray position", AxesCreator),
+        ("choose", "Existing subplot", AxesSelector),
+    ]
 
     def __init__(self, key=None, func_kwargs={}, *args, **kwargs):
         """
         Parameters
         ----------
         key: str or None
             if string, it must be one of the keys in the :attr:`widgets`
             attribute
         func_kwargs: dict
             a dictionary that is passed to the class constructor determined by
             the `key` parameter if `key` is not None
         ``*args,**kwargs``
             Determined by the QWidget class"""
         super(AxesCreatorCollection, self).__init__(*args, **kwargs)
-        self.bt_cancel = QPushButton('Cancel', self)
-        self.bt_ok = QPushButton('Ok', self)
+        self.bt_cancel = QPushButton("Cancel", self)
+        self.bt_ok = QPushButton("Ok", self)
 
         self.tb = QTabWidget(self)
         self.tb.setTabPosition(QTabWidget.West)
         current = 0
         for i, (func_name, title, cls) in enumerate(self.widgets):
             if func_name == key:
                 current = i
@@ -1664,147 +1824,166 @@
 
 
 class PlotCreator(QDialog):
     """
     Widget to extract data from a dataset and eventually create a plot"""
 
     #: Tooltip for not making a plot
-    NO_PM_TT = 'Choose a plot method (or choose none to only extract the data)'
+    NO_PM_TT = "Choose a plot method (or choose none to only extract the data)"
 
     _preset = None
 
+    _decoder = None
+
     def __init__(self, *args, **kwargs):
-        self.help_explorer = kwargs.pop('help_explorer', None)
+        self.help_explorer = kwargs.pop("help_explorer", None)
         super(PlotCreator, self).__init__(*args, **kwargs)
         self.setAttribute(Qt.WA_DeleteOnClose)
-        self.setWindowTitle('Create plots')
+        self.setWindowTitle("Create plots")
         self.error_msg = PyErrorMessage(self)
         mp = psy.gcp(True)
 
         self.splitter = splitter = QSplitter(Qt.Vertical, parent=self)
         self.w = w = QWidget(self)
         self.fmt_tree_widget = QWidget(self)
 
         # ---------------------------------------------------------------------
         # -------------------------- children ---------------------------------
         # ---------------------------------------------------------------------
 
         self.ds_combo = QComboBox(parent=w)
-        self.ds_combo.setToolTip('The data source to use the data from')
+        self.ds_combo.setToolTip("The data source to use the data from")
         self.fill_ds_combo(mp)
         self.bt_open_file = QToolButton(parent=w)
-        self.bt_open_file.setIcon(QIcon(get_icon('run_arrow.png')))
-        self.bt_open_file.setToolTip('Open a new dataset from the hard disk')
+        self.bt_open_file.setIcon(QIcon(get_icon("run_arrow.png")))
+        self.bt_open_file.setToolTip("Open a new dataset from the hard disk")
         self.bt_get_ds = LoadFromConsoleButton(xarray.Dataset, parent=w)
         self.bt_get_ds.setToolTip(
-            'Use a dataset already defined in the console')
+            "Use a dataset already defined in the console"
+        )
 
-        self.pm_label = QLabel('Plot method: ', w)
+        self.pm_label = QLabel("Plot method: ", w)
         self.pm_combo = QComboBox(w)
         self.fill_plot_method_combo()
         self.bt_load_preset = QPushButton("Preset")
         self.bt_load_preset.setEnabled(False)
         self.pm_info = QToolButton(w)
-        self.pm_info.setIcon(QIcon(get_icon('info.png')))
-        self.pm_info.setToolTip('Show information in the help explorer')
+        self.pm_info.setIcon(QIcon(get_icon("info.png")))
+        self.pm_info.setToolTip("Show information in the help explorer")
 
         self.variables_table = VariablesTable(self.get_ds, parent=w)
         self.variables_table.fill_from_ds()
 
         self.coords_table = CoordsTable(self.get_ds, parent=w)
         self.coords_table.fill_from_ds()
 
         self.array_table = ArrayTable(self.get_ds, parent=w)
         self.array_table.setup_from_ds(plot_method=self.pm_combo.currentText())
 
-        self.cbox_load = QCheckBox('load')
+        self.cbox_load = QCheckBox("load")
         self.cbox_load.setToolTip(
-            'Load the selected data arrays into memory when clicking on '
-            '<em>Ok</em>. Note that this might cause problems for large '
-            'arrays!')
+            "Load the selected data arrays into memory when clicking on "
+            "<em>Ok</em>. Note that this might cause problems for large "
+            "arrays!"
+        )
 
-        self.cbox_close_popups = QCheckBox('close dropdowns', w)
+        self.cbox_close_popups = QCheckBox("close dropdowns", w)
         self.cbox_close_popups.setChecked(True)
         self.cbox_close_popups.setToolTip(
-            'Close drop down menues after selecting indices to plot')
-        self.cbox_use_coords = QCheckBox('show coordinates', w)
+            "Close drop down menues after selecting indices to plot"
+        )
+        self.cbox_use_coords = QCheckBox("show coordinates", w)
         self.cbox_use_coords.setChecked(False)
         self.cbox_use_coords.setToolTip(
-            'Show the real coordinates instead of the indices in the drop '
-            'down menues')
+            "Show the real coordinates instead of the indices in the drop "
+            "down menues"
+        )
         self.bt_remove_all = QToolButton(w)
-        self.bt_remove_all.setIcon(QIcon(get_icon('minusminus.png')))
-        self.bt_remove_all.setToolTip('Remove all arrays')
+        self.bt_remove_all.setIcon(QIcon(get_icon("minusminus.png")))
+        self.bt_remove_all.setToolTip("Remove all arrays")
         self.bt_remove = QToolButton(w)
-        self.bt_remove.setIcon(QIcon(get_icon('minus.png')))
-        self.bt_remove.setToolTip('Remove selected arrays')
+        self.bt_remove.setIcon(QIcon(get_icon("minus.png")))
+        self.bt_remove.setToolTip("Remove selected arrays")
         self.bt_add = QToolButton(w)
-        self.bt_add.setIcon(QIcon(get_icon('plus.png')))
-        self.bt_add.setToolTip('Add arrays for the selected variables')
+        self.bt_add.setIcon(QIcon(get_icon("plus.png")))
+        self.bt_add.setToolTip("Add arrays for the selected variables")
         self.bt_add_all = QToolButton(w)
-        self.bt_add_all.setIcon(QIcon(get_icon('plusplus.png')))
+        self.bt_add_all.setIcon(QIcon(get_icon("plusplus.png")))
         self.bt_add_all.setToolTip(
-            'Add arrays for all variables in the dataset')
+            "Add arrays for all variables in the dataset"
+        )
 
-        self.rows_axis_label = QLabel('No. of rows', w)
+        self.rows_axis_label = QLabel("No. of rows", w)
         self.rows_axis_edit = QLineEdit(w)
-        self.rows_axis_edit.setText('1')
-        self.cols_axis_label = QLabel('No. sof columns', w)
+        self.rows_axis_edit.setText("1")
+        self.cols_axis_label = QLabel("No. sof columns", w)
         self.cols_axis_edit = QLineEdit(w)
-        self.cols_axis_edit.setText('1')
-        self.max_axis_label = QLabel('No. of axes per figure', w)
+        self.cols_axis_edit.setText("1")
+        self.max_axis_label = QLabel("No. of axes per figure", w)
         self.max_axis_edit = QLineEdit(w)
-        self.bt_add_axes = QPushButton('Add new subplots', w)
+        self.bt_add_axes = QPushButton("Add new subplots", w)
         self.bt_add_axes.setToolTip(
-            'Adds subplots for the selected arrays based the specified number '
-            'of rows and columns')
+            "Adds subplots for the selected arrays based the specified number "
+            "of rows and columns"
+        )
 
-        self.row_axis_label = QLabel('Row number:', w)
+        self.row_axis_label = QLabel("Row number:", w)
         self.row_axis_edit = QLineEdit(w)
-        self.row_axis_edit.setText('1')
-        self.col_axis_label = QLabel('Column number', w)
+        self.row_axis_edit.setText("1")
+        self.col_axis_label = QLabel("Column number", w)
         self.col_axis_edit = QLineEdit(w)
-        self.col_axis_edit.setText('1')
-        self.bt_add_single_axes = QPushButton('Add one subplot', w)
+        self.col_axis_edit.setText("1")
+        self.bt_add_single_axes = QPushButton("Add one subplot", w)
         self.bt_add_single_axes.setToolTip(
-            'Add one subplot for the specified row and column')
+            "Add one subplot for the specified row and column"
+        )
 
         self.fmt_tree_label = QLabel(
             "Modify the formatoptions of the newly created plots."
             "Values must be entered in yaml syntax",
-            parent=self.fmt_tree_widget)
+            parent=self.fmt_tree_widget,
+        )
 
-        self.fmt_tree = RcParamsTree(None, None, None,
-                                     parent=self.fmt_tree_widget)
+        self.fmt_tree = RcParamsTree(
+            None, None, None, parent=self.fmt_tree_widget
+        )
         self.fmt_tree.value_col = 3
         self.fmt_tree.setColumnCount(4)
-        self.fmt_tree.setHeaderLabels(['Formatoption', '', '', 'Value'])
+        self.fmt_tree.setHeaderLabels(["Formatoption", "", "", "Value"])
 
         # ---------------------------------------------------------------------
         # ---------------------------- connections ----------------------------
         # ---------------------------------------------------------------------
 
         # ----------------- dataset combo connections ------------------------
         self.bt_open_file.clicked.connect(lambda: self.open_dataset())
         self.bt_get_ds.object_loaded.connect(self.add_new_ds)
         self.ds_combo.currentIndexChanged[int].connect(self.set_ds)
 
         self.ds_combo.currentIndexChanged[int].connect(
-            lambda i: self.variables_table.fill_from_ds())
+            lambda i: self.variables_table.fill_from_ds()
+        )
         self.ds_combo.currentIndexChanged[int].connect(
-            lambda i: self.coords_table.fill_from_ds())
+            lambda i: self.coords_table.fill_from_ds()
+        )
         self.ds_combo.currentIndexChanged[int].connect(
-            lambda i: self.array_table.setup_from_ds())
+            lambda i: self.array_table.setup_from_ds()
+        )
         self.ds_combo.currentIndexChanged[int].connect(
-            lambda i: self.connect_combo_boxes())
+            lambda i: self.connect_combo_boxes()
+        )
 
         # ------------------- plot method connections -------------------------
         self.pm_combo.currentIndexChanged[str].connect(
-            lambda s: self.pm_combo.setToolTip(
-                getattr(psy.plot, s)._summary) if s else self.NO_PM_TT)
+            lambda s: (
+                self.pm_combo.setToolTip(getattr(psy.plot, s)._summary)
+                if s
+                else self.NO_PM_TT
+            )
+        )
         self.pm_info.clicked.connect(self.show_pm_info)
         self.pm_combo.currentIndexChanged[str].connect(self.array_table.set_pm)
         self.pm_combo.currentIndexChanged[str].connect(self.fill_fmt_tree)
 
         # ------------------- preset button connections -----------------------
         self.bt_load_preset.clicked.connect(self.load_preset)
 
@@ -1812,47 +1991,57 @@
         self.cbox_close_popups.clicked.connect(self.toggle_close_popups)
         self.cbox_use_coords.clicked.connect(self.reset_comboboxes)
         # connect leftclick of combo boxes to create new arrays or update the
         # selected
         self.connect_combo_boxes()
 
         # ----------------- add and remove button connections -----------------
-        self.bt_add.clicked.connect(lambda b: self.insert_array(
-            variables=self.variables_table.selected_variables))
+        self.bt_add.clicked.connect(
+            lambda b: self.insert_array(
+                variables=self.variables_table.selected_variables
+            )
+        )
         self.bt_add_all.clicked.connect(
             lambda b: self.insert_array(
-                variables=self.variables_table.variables))
+                variables=self.variables_table.variables
+            )
+        )
         self.bt_remove_all.clicked.connect(
-            lambda b: self.array_table.remove_arrays(False))
+            lambda b: self.array_table.remove_arrays(False)
+        )
         self.bt_remove.clicked.connect(
-            lambda b: self.array_table.remove_arrays(True))
+            lambda b: self.array_table.remove_arrays(True)
+        )
 
         # ------------- axes creation connections -----------------------------
         self.rows_axis_edit.returnPressed.connect(self.bt_add_axes.click)
         self.cols_axis_edit.returnPressed.connect(self.bt_add_axes.click)
         self.max_axis_edit.returnPressed.connect(self.bt_add_axes.click)
         self.bt_add_axes.clicked.connect(self.setup_subplots)
         self.row_axis_edit.returnPressed.connect(self.bt_add_single_axes.click)
         self.col_axis_edit.returnPressed.connect(self.bt_add_single_axes.click)
         self.bt_add_single_axes.clicked.connect(self.setup_subplot)
 
         # -------------------- create and cancel connections ------------------
-        self.bbox = bbox = QDialogButtonBox(QDialogButtonBox.Ok |
-                                            QDialogButtonBox.Cancel)
+        self.bbox = bbox = QDialogButtonBox(
+            QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+        )
         bbox.accepted.connect(self.create_plots)
         bbox.rejected.connect(self.reject)
 
         # -------------------- other connections ------------------------------
         # allow only to select either variables or newly created arrays in
         # order to control the behaviour of the combo box left click in
         # self.insert_array_from_combo
         self.array_table.itemSelectionChanged.connect(
-            self.variables_table.clearSelection)
+            self.variables_table.clearSelection
+        )
         self.variables_table.itemSelectionChanged.connect(
-            self.array_table.clearSelection)
+            self.array_table.clearSelection
+        )
 
         # ---------------------------------------------------------------------
         # ---------------------------- layouts --------------------------------
         # ---------------------------------------------------------------------
 
         self.ds_box = QHBoxLayout()
         self.ds_box.addWidget(self.ds_combo)
@@ -1928,33 +2117,38 @@
         for cb in self.coords_table.combo_boxes:
             cb.use_coords = use_coords
             cb.clear()
             cb._is_empty = True
 
     def fill_fmt_tree(self, pm):
         import psyplot.project as psy
+
         self.fmt_tree.clear()
         if not pm:
             self.fmt_tree_widget.setVisible(False)
             self.bt_load_preset.setEnabled(False)
         else:
             pm = getattr(psy.plot, pm)
             plotter = pm.plotter_cls()
             if self._preset:
-                plotter.update(psy.Project.extract_fmts_from_preset(
-                    self._preset, pm))
+                plotter.update(
+                    psy.Project.extract_fmts_from_preset(self._preset, pm)
+                )
             self.fmt_tree.rc = plotter
             self.fmt_tree.validators = {
-                key: getattr(plotter, key).validate for key in plotter}
+                key: getattr(plotter, key).validate for key in plotter
+            }
             self.fmt_tree.descriptions = {
-                key: getattr(plotter, key).name for key in plotter}
+                key: getattr(plotter, key).name for key in plotter
+            }
             self.fmt_tree.initialize()
-            icon = QIcon(get_icon('info.png'))
+            icon = QIcon(get_icon("info.png"))
             docs_funcs = {
-                key: partial(plotter.show_docs, key) for key in plotter}
+                key: partial(plotter.show_docs, key) for key in plotter
+            }
             for item in self.fmt_tree.top_level_items:
                 key = item.text(0)
                 bt = QToolButton()
                 bt.setIcon(icon)
                 bt.clicked.connect(docs_funcs[key])
                 self.fmt_tree.setItemWidget(item, 2, bt)
             self.fmt_tree.resizeColumnToContents(2)
@@ -1980,166 +2174,194 @@
 
     def show_pm_info(self):
         """Shows info on the current plotting method in the help explorer"""
         if self.help_explorer is None:
             return
         pm_name = self.pm_combo.currentText()
         if pm_name:
-            self.help_explorer.show_help(getattr(psy.plot, pm_name),
-                                         'psyplot.project.plot.' + pm_name)
+            self.help_explorer.show_help(
+                getattr(psy.plot, pm_name), "psyplot.project.plot." + pm_name
+            )
         else:
-            self.help_explorer.show_rst("""
+            self.help_explorer.show_rst(
+                """
             No plot
             =======
-            No plot will be created, only the data is extracted""", 'no_plot')
+            No plot will be created, only the data is extracted""",
+                "no_plot",
+            )
 
     def connect_combo_boxes(self):
         for cb in self.coords_table.combo_boxes:
             cb.leftclick.connect(self.insert_array_from_combo)
 
     def fill_plot_method_combo(self):
         """Takes the names of the plotting methods in the current project"""
-        self.pm_combo.addItems([''] + sorted(psy.plot._plot_methods))
+        self.pm_combo.addItems([""] + sorted(psy.plot._plot_methods))
         self.pm_combo.setToolTip(self.NO_PM_TT)
 
     def set_pm(self, plot_method):
         self.pm_combo.setCurrentIndex(
-            self.pm_combo.findText(plot_method or ''))
+            self.pm_combo.findText(plot_method or "")
+        )
 
     def create_plots(self):
         """Method to be called when the `Create plot` button is pressed
 
         This method reads the data from the :attr:`array_table` attribute and
         makes the plot (or extracts the data) based upon the
         :attr:`plot_method` attribute"""
         import matplotlib.pyplot as plt
+
         names = self.array_table.arr_names_dict
         pm = self.pm_combo.currentText()
         if pm:
             pm = getattr(psy.plot, pm)
             for d, (default_dim, default_slice) in product(
-                    six.itervalues(names), six.iteritems(pm._default_dims)):
+                six.itervalues(names), six.iteritems(pm._default_dims)
+            ):
                 d.setdefault(default_dim, default_slice)
-            kwargs = {'ax': self.array_table.axes,
-                      'fmt': {t[1]: t[2] for t in self.fmt_tree._get_rc()}}
+            kwargs = {
+                "ax": self.array_table.axes,
+                "fmt": {t[1]: t[2] for t in self.fmt_tree._get_rc()},
+            }
         else:
             pm = self.open_data
             kwargs = {}
         fig_nums = plt.get_fignums()[:]
         try:
-            pm(self.ds, arr_names=names, load=self.cbox_load.isChecked(),
-               **kwargs)
+            pm(
+                self.ds,
+                arr_names=names,
+                load=self.cbox_load.isChecked(),
+                decoder=self._decoder,
+                **kwargs,
+            )
         except Exception:
             for num in set(plt.get_fignums()).difference(fig_nums):
                 plt.close(num)
-            self.error_msg.showTraceback('<b>Failed to create the plots!</b>')
-            logger.debug('Error while creating the plots with %s!',
-                         names, exc_info=True)
+            self.error_msg.showTraceback("<b>Failed to create the plots!</b>")
+            logger.debug(
+                "Error while creating the plots with %s!", names, exc_info=True
+            )
         else:
             self.close()
 
     def load_preset(self):
         """Load a preset file"""
         fname, ok = QFileDialog.getOpenFileName(
-            self, 'Load preset', os.path.join(get_configdir(), 'presets'),
-            'YAML files (*.yml *.yaml);;'
-            'All files (*)')
+            self,
+            "Load preset",
+            os.path.join(get_configdir(), "presets"),
+            "YAML files (*.yml *.yaml);;" "All files (*)",
+        )
         if ok:
             self.set_preset(fname)
 
     def open_dataset(self, fnames=None, *args, **kwargs):
         """Opens a file dialog and the dataset that has been inserted"""
 
         def open_ds():
             if len(fnames) == 1:
-                kwargs.pop('concat_dim', None)
+                kwargs.pop("concat_dim", None)
                 return psy.open_dataset(fnames[0], *args, **kwargs)
             else:
                 return psy.open_mfdataset(fnames, *args, **kwargs)
 
         if fnames is None:
             fnames = QFileDialog.getOpenFileNames(
-                self, 'Open dataset', os.getcwd(),
-                'NetCDF files (*.nc *.nc4);;'
-                'Shape files (*.shp);;'
-                'All files (*)'
-                )
+                self,
+                "Open dataset",
+                os.getcwd(),
+                "NetCDF files (*.nc *.nc4);;"
+                "Shape files (*.shp);;"
+                "All files (*)",
+            )
             if with_qt5:  # the filter is passed as well
                 fnames = fnames[0]
         if isinstance(fnames, xarray.Dataset):
             ds = fnames
-            self.add_new_ds('ds', ds)
+            self.add_new_ds("ds", ds)
         elif not fnames:
             return
         else:
             try:
                 ds = open_ds()
             except Exception:
-                kwargs['decode_times'] = False
+                kwargs["decode_times"] = False
                 try:
                     ds = open_ds()
                 except Exception:
                     self.error_msg.showTraceback(
-                        '<b>Could not open dataset %s</b>' % (fnames, ))
+                        "<b>Could not open dataset %s</b>" % (fnames,)
+                    )
                     return
-            fnames_str = ', '.join(fnames)
+            fnames_str = ", ".join(fnames)
             self.add_new_ds(fnames_str, ds, fnames_str)
 
     def set_preset(self, preset):
         import psyplot.project as psy
+
         self._preset = psy.Project._load_preset(preset)
         if self.fmt_tree_widget.isVisible():
             self.fill_fmt_tree(self.pm_combo.currentText())
 
+    def set_decoder(self, decoder):
+        """Set the decoder for the new plots."""
+        self._decoder = decoder
+
     def add_new_ds(self, oname, ds, fname=None):
-        d = {'ds': ds}
+        d = {"ds": ds}
         if fname:
-            d['fname'] = fname
+            d["fname"] = fname
         self.ds_descs.insert(0, d)
-        self.ds_combo.insertItem(0, 'New: ' + oname)
+        self.ds_combo.insertItem(0, "New: " + oname)
         self.ds_combo.setCurrentIndex(0)
 
     def set_ds(self, i):
         """Set the current dataset"""
-        self.ds = self.ds_descs[i]['ds']
+        self.ds = self.ds_descs[i]["ds"]
 
     def fill_ds_combo(self, project):
-        """fill the dataset combobox with datasets of the current main project
-        """
+        """fill the dataset combobox with datasets of the current main project"""
         self.ds_combo.clear()
         self.ds_combo.setInsertPolicy(QComboBox.InsertAtBottom)
         ds_descs = project._get_ds_descriptions(
-            project.array_info(ds_description='all'))
+            project.array_info(ds_description="all")
+        )
         self.ds_combo.addItems(
-            ['%i: %s' % (i, ds_desc['fname']) for i, ds_desc in six.iteritems(
-                ds_descs)])
+            [
+                "%i: %s" % (i, ds_desc["fname"])
+                for i, ds_desc in six.iteritems(ds_descs)
+            ]
+        )
         self.ds_descs = list(ds_descs.values())
         if len(self.ds_descs):
             self.set_ds(0)
 
     def insert_array_from_combo(self, cb, variables=None):
-        """Insert new arrays into the dataset when the combobox is left-clicked
-        """
+        """Insert new arrays into the dataset when the combobox is left-clicked"""
         if variables is None:
             variables = self.variables_table.selected_variables
         dims = {}
         for other_cb in self.coords_table.combo_boxes:
             ind = other_cb.currentIndex()
-            dims[other_cb.dim] = str((ind - 1) if ind not in [-1, 0] else '')
+            dims[other_cb.dim] = str((ind - 1) if ind not in [-1, 0] else "")
         dim = cb.dim
         inserts = list(
             str(ind.row() - 1)
             for ind in cb.view().selectionModel().selectedIndexes()
-            if ind.row() > 0)
+            if ind.row() > 0
+        )
         dims.pop(dim)
         for name, val in product(variables, inserts):
             dims[dim] = val
             self.array_table.insert_array(name, check=False, **dims)
         if len(inserts) > 1:
-            inserts = '%s:%s' % (min(inserts), max(inserts))
+            inserts = "%s:%s" % (min(inserts), max(inserts))
         elif inserts:
             inserts = inserts[0]
         else:
             return
         self.array_table.update_selected(check=False, dims={dim: inserts})
         self.array_table.check_arrays()
 
@@ -2148,15 +2370,15 @@
         the :attr:`variable_table` if `variables` is None)
         """
         if variables is None:
             variables = self.variables_table.selected_variables
         dims = {}
         for other_cb in self.coords_table.combo_boxes:
             ind = other_cb.currentIndex()
-            dims[other_cb.dim] = str((ind - 1) if ind not in [-1, 0] else '')
+            dims[other_cb.dim] = str((ind - 1) if ind not in [-1, 0] else "")
         for name in variables:
             self.array_table.insert_array(name, check=False, **dims)
         self.array_table.check_arrays()
 
     def get_ds(self, i=None):
         """Get the dataset
 
@@ -2171,20 +2393,20 @@
         -------
         xarray.Dataset
             The requested dataset"""
         if i is None:
             i = self.ds_combo.currentIndex()
         if not len(self.ds_descs):
             return
-        return self.ds_descs[i]['ds']
+        return self.ds_descs[i]["ds"]
 
     def close(self, *args, **kwargs):
         """Reimplemented to make sure that the data sets are deleted"""
         super(PlotCreator, self).close(*args, **kwargs)
-        if hasattr(self, 'ds_descs'):
+        if hasattr(self, "ds_descs"):
             del self.ds_descs
 
     def open_data(self, *args, **kwargs):
         """Convenience method to create a sub project without a plotter
 
         This method is used when the :attr:`pm_combo` is empty"""
         p = psy.Project.from_dataset(*args, main=psy.gcp(True), **kwargs)
@@ -2195,15 +2417,15 @@
 
         Parameters
         ----------
         ds: xarray.Dataset
             The dataset to use. It is assumed that this dataset is already
             in the dataset combobox"""
         for i, desc in enumerate(self.ds_descs):
-            if desc['ds'] is ds:
+            if desc["ds"] is ds:
                 self.ds_combo.setCurrentIndex(i)
                 return
 
     def keyPressEvent(self, e):
         """Reimplemented to close the window when escape is hitted"""
         if e.key() == QtCore.Qt.Key_Escape:
             self.close()
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/preferences.py` & `psyplot-gui-1.5.0/psyplot_gui/preferences.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 """Preferences widget for psyplot_gui
 
 This module defines the :class:`Preferences` widget that creates an interface
 to the rcParams of psyplot and psyplot_gui"""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import yaml
 from warnings import warn
-from psyplot_gui.compat.qtcompat import (
-    QTreeWidget, QTreeWidgetItem, Qt, QMenu, QAction, QTextEdit, QIcon,
-    QWidget, QVBoxLayout, QHBoxLayout, QtCore, QDialog, QScrollArea,
-    QDialogButtonBox, QStackedWidget, QListWidget, QListView, QSplitter,
-    QListWidgetItem, QPushButton, QFileDialog, with_qt5,
-    QAbstractItemView, QToolButton, QLabel, QtGui, asstring)
-from psyplot_gui.common import get_icon
+
+import yaml
+from psyplot.config.rcsetup import RcParams, psyplot_fname
+from psyplot.config.rcsetup import rcParams as psy_rcParams
+
 from psyplot_gui import rcParams as rcParams
-from psyplot.config.rcsetup import (
-    psyplot_fname, RcParams, rcParams as psy_rcParams)
+from psyplot_gui.common import get_icon
+from psyplot_gui.compat.qtcompat import (
+    QAbstractItemView,
+    QAction,
+    QDialog,
+    QDialogButtonBox,
+    QFileDialog,
+    QHBoxLayout,
+    QIcon,
+    QLabel,
+    QListView,
+    QListWidget,
+    QListWidgetItem,
+    QMenu,
+    QPushButton,
+    QScrollArea,
+    QSplitter,
+    QStackedWidget,
+    Qt,
+    QtCore,
+    QTextEdit,
+    QtGui,
+    QToolButton,
+    QTreeWidget,
+    QTreeWidgetItem,
+    QVBoxLayout,
+    QWidget,
+    asstring,
+    with_qt5,
+)
 
 
 class ConfigPage(object):
     """An abstract base class for configuration pages"""
 
     #: A signal that shall be emitted if the validation state changes
     validChanged = QtCore.pyqtSignal(bool)
@@ -123,15 +131,15 @@
         super(RcParamsTree, self).__init__(*args, **kwargs)
         self.rc = rcParams
         self.validators = validators
         self.descriptions = descriptions
         self.setContextMenuPolicy(Qt.CustomContextMenu)
         self.customContextMenuRequested.connect(self.open_menu)
         self.setColumnCount(self.value_col + 1)
-        self.setHeaderLabels(['RcParams key', '', 'Value'])
+        self.setHeaderLabels(["RcParams key", "", "Value"])
 
     @property
     def is_valid(self):
         """True if all the proposed values in this tree are valid"""
         return all(self.valid)
 
     @property
@@ -146,30 +154,32 @@
         self.valid = [True] * len(rcParams)
         validators = self.validators
         vcol = self.value_col
         for i, (key, val) in enumerate(sorted(rcParams.items())):
             item = QTreeWidgetItem(0)
             item.setText(0, key)
             item.setToolTip(0, key)
-            item.setIcon(1, QIcon(get_icon('valid.png')))
+            item.setIcon(1, QIcon(get_icon("valid.png")))
             desc = descriptions.get(key)
             if desc:
                 item.setText(vcol, desc)
                 item.setToolTip(vcol, desc)
             child = QTreeWidgetItem(0)
             item.addChild(child)
             self.addTopLevelItem(item)
             editor = QTextEdit(self)
             # set maximal height of the editor to 3 rows
             editor.setMaximumHeight(
-                4 * QtGui.QFontMetrics(editor.font()).height())
+                4 * QtGui.QFontMetrics(editor.font()).height()
+            )
             editor.setPlainText(yaml.dump(val))
             self.setItemWidget(child, vcol, editor)
             editor.textChanged.connect(
-                self.set_icon_func(i, item, validators[key]))
+                self.set_icon_func(i, item, validators[key])
+            )
         self.resizeColumnToContents(0)
         self.resizeColumnToContents(1)
 
     def set_icon_func(self, i, item, validator):
         """Create a function to change the icon of one topLevelItem
 
         This method creates a function that can be called when the value of an
@@ -187,34 +197,36 @@
         validator: func
             The validation function
 
         Returns
         -------
         function
             The function that can be called to set the correct icon"""
+
         def func():
             editor = self.itemWidget(item.child(0), self.value_col)
             s = asstring(editor.toPlainText())
             try:
                 val = yaml.load(s, Loader=yaml.Loader)
             except Exception as e:
-                item.setIcon(1, QIcon(get_icon('warning.png')))
+                item.setIcon(1, QIcon(get_icon("warning.png")))
                 item.setToolTip(1, "Could not parse yaml code: %s" % e)
                 self.set_valid(i, False)
                 return
             try:
                 validator(val)
             except Exception as e:
-                item.setIcon(1, QIcon(get_icon('invalid.png')))
+                item.setIcon(1, QIcon(get_icon("invalid.png")))
                 item.setToolTip(1, "Wrong value: %s" % e)
                 self.set_valid(i, False)
             else:
-                item.setIcon(1, QIcon(get_icon('valid.png')))
+                item.setIcon(1, QIcon(get_icon("valid.png")))
                 self.set_valid(i, True)
             self.propose_changes.emit(self.parent() or self)
+
         return func
 
     def set_valid(self, i, b):
         """Set the validation status
 
         If the validation status changed compared to the old one, the
         :attr:`validChanged` signal is emitted
@@ -236,18 +248,18 @@
         """Open a menu to expand and collapse all items in the tree
 
         Parameters
         ----------
         position: QPosition
             The position where to open the menu"""
         menu = QMenu()
-        expand_all_action = QAction('Expand all', self)
+        expand_all_action = QAction("Expand all", self)
         expand_all_action.triggered.connect(self.expandAll)
         menu.addAction(expand_all_action)
-        collapse_all_action = QAction('Collapse all', self)
+        collapse_all_action = QAction("Collapse all", self)
         collapse_all_action.triggered.connect(self.collapseAll)
         menu.addAction(collapse_all_action)
         menu.exec_(self.viewport().mapToGlobal(position))
 
     def changed_rc(self, use_items=False):
         """Iterate over the changed rcParams
 
@@ -258,16 +270,18 @@
 
         Yields
         ------
         QTreeWidgetItem or str
             The item identifier
         object
             The proposed value"""
+
         def equals(item, key, val, orig):
             return val != orig
+
         for t in self._get_rc(equals):
             yield t[0 if use_items else 1], t[2]
 
     def selected_rc(self, use_items=False):
         """Iterate over the selected rcParams
 
         Parameters
@@ -277,16 +291,18 @@
 
         Yields
         ------
         QTreeWidgetItem or str
             The item identifier
         object
             The proposed value"""
+
         def is_selected(item, key, val, orig):
             return item.isSelected()
+
         for t in self._get_rc(is_selected):
             yield t[0 if use_items else 1], t[2]
 
     def _get_rc(self, filter_func=None):
         """Iterate over the rcParams
 
         This function applies the given `filter_func` to check whether the
@@ -313,44 +329,44 @@
         str
             The rcParams key
         object
             The proposed value
         object
             The current value
         """
+
         def no_check(item, key, val, orig):
             return True
+
         rc = self.rc
         filter_func = filter_func or no_check
         for item in self.top_level_items:
             key = asstring(item.text(0))
             editor = self.itemWidget(item.child(0), self.value_col)
             val = yaml.load(asstring(editor.toPlainText()), Loader=yaml.Loader)
             try:
                 val = rc.validate[key](val)
-            except:
+            except Exception:
                 pass
             try:
                 include = filter_func(item, key, val, rc[key])
-            except:
-                warn('Could not check state for %s key' % key,
-                     RuntimeWarning)
+            except Exception:
+                warn("Could not check state for %s key" % key, RuntimeWarning)
             else:
                 if include:
                     yield (item, key, val, rc[key])
 
     def apply_changes(self):
         """Update the :attr:`rc` with the proposed changes"""
         new = dict(self.changed_rc())
         if new != self.rc:
             self.rc.update(new)
 
     def select_changes(self):
-        """Select all the items that changed comparing to the current rcParams
-        """
+        """Select all the items that changed comparing to the current rcParams"""
         for item, val in self.changed_rc(True):
             item.setSelected(True)
 
 
 class RcParamsWidget(ConfigPage, QWidget):
     """A configuration page for RcParams instances
 
@@ -388,37 +404,42 @@
     def is_valid(self):
         """True if all the settings are valid"""
         return self.tree.is_valid
 
     @property
     def icon(self):
         """The icon of this instance in the :class:`Preferences` dialog"""
-        return QIcon(get_icon('rcParams.png'))
+        return QIcon(get_icon("rcParams.png"))
 
     def __init__(self, *args, **kwargs):
         super(RcParamsWidget, self).__init__(*args, **kwargs)
         self.vbox = vbox = QVBoxLayout()
 
         self.description = QLabel(
-            '<p>Modify the rcParams for your need. Changes will not be applied'
-            ' until you click the Apply or Ok button.</p>'
-            '<p>Values must be entered in yaml syntax</p>', parent=self)
+            "<p>Modify the rcParams for your need. Changes will not be applied"
+            " until you click the Apply or Ok button.</p>"
+            "<p>Values must be entered in yaml syntax</p>",
+            parent=self,
+        )
         vbox.addWidget(self.description)
         self.tree = tree = RcParamsTree(
-            self.rc, getattr(self.rc, 'validate', None),
-            getattr(self.rc, 'descriptions', None), parent=self)
+            self.rc,
+            getattr(self.rc, "validate", None),
+            getattr(self.rc, "descriptions", None),
+            parent=self,
+        )
         tree.setSelectionMode(QAbstractItemView.MultiSelection)
         vbox.addWidget(self.tree)
 
-        self.bt_select_all = QPushButton('Select All', self)
-        self.bt_select_changed = QPushButton('Select changes', self)
-        self.bt_select_none = QPushButton('Clear Selection', self)
+        self.bt_select_all = QPushButton("Select All", self)
+        self.bt_select_changed = QPushButton("Select changes", self)
+        self.bt_select_none = QPushButton("Clear Selection", self)
         self.bt_export = QToolButton(self)
-        self.bt_export.setText('Export Selection...')
-        self.bt_export.setToolTip('Export the selected rcParams to a file')
+        self.bt_export.setText("Export Selection...")
+        self.bt_export.setToolTip("Export the selected rcParams to a file")
         self.bt_export.setPopupMode(QToolButton.InstantPopup)
         self.export_menu = export_menu = QMenu(self)
         export_menu.addAction(self.save_settings_action())
         export_menu.addAction(self.save_settings_action(True))
         self.bt_export.setMenu(export_menu)
         hbox = QHBoxLayout()
         hbox.addWidget(self.bt_select_all)
@@ -439,48 +460,51 @@
 
         Parameters
         ----------
         update: bool
             If True, it is expected that the file already exists and it will be
             updated. Otherwise, existing files will be overwritten
         """
+
         def func():
             if update:
                 meth = QFileDialog.getOpenFileName
             else:
                 meth = QFileDialog.getSaveFileName
             if target is None:
                 fname = meth(
-                    self, 'Select a file to %s' % (
-                        'update' if update else 'create'),
+                    self,
+                    "Select a file to %s" % ("update" if update else "create"),
                     self.default_path,
-                    'YAML files (*.yml);;'
-                    'All files (*)'
-                    )
+                    "YAML files (*.yml);;" "All files (*)",
+                )
                 if with_qt5:  # the filter is passed as well
                     fname = fname[0]
             else:
                 fname = target
             if not fname:
                 return
             if update:
                 rc = self.rc.__class__(defaultParams=self.rc.defaultParams)
                 rc.load_from_file(fname)
                 old_keys = list(rc)
                 selected = dict(self.tree.selected_rc())
                 new_keys = list(selected)
                 rc.update(selected)
-                rc.dump(fname, include_keys=old_keys + new_keys,
-                        exclude_keys=[])
+                rc.dump(
+                    fname, include_keys=old_keys + new_keys, exclude_keys=[]
+                )
             else:
-                rc = self.rc.__class__(self.tree.selected_rc(),
-                                       defaultParams=self.rc.defaultParams)
+                rc = self.rc.__class__(
+                    self.tree.selected_rc(),
+                    defaultParams=self.rc.defaultParams,
+                )
                 rc.dump(fname, exclude_keys=[])
 
-        action = QAction('Update...' if update else 'Overwrite...', self)
+        action = QAction("Update..." if update else "Overwrite...", self)
         action.triggered.connect(func)
         return action
 
     def initialize(self, rcParams=None, validators=None, descriptions=None):
         """Initialize the config page
 
         Parameters
@@ -512,26 +536,27 @@
 
 
 class GuiRcParamsWidget(RcParamsWidget):
     """The config page for the :class:`psyplot_gui.config.rcsetup.rcParams`"""
 
     rc = rcParams
 
-    title = 'GUI defaults'
+    title = "GUI defaults"
 
-    default_path = psyplot_fname('PSYPLOTGUIRC', 'psyplotguirc.yml',
-                                 if_exists=False)
+    default_path = psyplot_fname(
+        "PSYPLOTGUIRC", "psyplotguirc.yml", if_exists=False
+    )
 
 
 class PsyRcParamsWidget(RcParamsWidget):
     """The config page for the :class:`psyplot.config.rcsetup.rcParams`"""
 
     rc = psy_rcParams
 
-    title = 'psyplot defaults'
+    title = "psyplot defaults"
 
     default_path = psyplot_fname(if_exists=False)
 
 
 class Prefences(QDialog):
     """Preferences dialog"""
 
@@ -541,35 +566,38 @@
 
     @property
     def pages(self):
         return map(self.get_page, range(self.pages_widget.count()))
 
     def __init__(self, main=None):
         super(Prefences, self).__init__(parent=main)
-        self.setWindowTitle('Preferences')
+        self.setWindowTitle("Preferences")
 
         # Widgets
         self.pages_widget = QStackedWidget()
         self.contents_widget = QListWidget()
-        self.bt_reset = QPushButton('Reset to defaults')
-        self.bt_load_plugins = QPushButton('Load plugin pages')
+        self.bt_reset = QPushButton("Reset to defaults")
+        self.bt_load_plugins = QPushButton("Load plugin pages")
         self.bt_load_plugins.setToolTip(
-            'Load the rcParams for the plugins in separate pages')
+            "Load the rcParams for the plugins in separate pages"
+        )
 
         self.bbox = bbox = QDialogButtonBox(
-            QDialogButtonBox.Ok | QDialogButtonBox.Apply |
-            QDialogButtonBox.Cancel)
+            QDialogButtonBox.Ok
+            | QDialogButtonBox.Apply
+            | QDialogButtonBox.Cancel
+        )
 
         # Widgets setup
         # Destroying the C++ object right after closing the dialog box,
         # otherwise it may be garbage-collected in another QThread
         # (e.g. the editor's analysis thread in Spyder), thus leading to
         # a segmentation fault on UNIX or an application crash on Windows
         self.setAttribute(Qt.WA_DeleteOnClose)
-        self.setWindowTitle('Preferences')
+        self.setWindowTitle("Preferences")
         self.contents_widget.setMovement(QListView.Static)
         self.contents_widget.setSpacing(1)
         self.contents_widget.setCurrentRow(0)
 
         # Layout
         hsplitter = QSplitter()
         hsplitter.addWidget(self.contents_widget)
@@ -590,15 +618,16 @@
 
         # Signals and slots
         if main is not None:
             self.bt_reset.clicked.connect(main.reset_rcParams)
         self.bt_load_plugins.clicked.connect(self.load_plugin_pages)
         self.pages_widget.currentChanged.connect(self.current_page_changed)
         self.contents_widget.currentRowChanged.connect(
-            self.pages_widget.setCurrentIndex)
+            self.pages_widget.setCurrentIndex
+        )
         bbox.accepted.connect(self.accept)
         bbox.rejected.connect(self.reject)
         self.bt_apply.clicked.connect(self.apply_clicked)
         self.bt_apply.setEnabled(False)
 
     def set_current_index(self, index):
         """Set current page index"""
@@ -637,15 +666,16 @@
 
         Parameters
         ----------
         widget: ConfigPage
             The page to add"""
         widget.validChanged.connect(self.bt_apply.setEnabled)
         widget.validChanged.connect(
-            self.bbox.button(QDialogButtonBox.Ok).setEnabled)
+            self.bbox.button(QDialogButtonBox.Ok).setEnabled
+        )
         scrollarea = QScrollArea(self)
         scrollarea.setWidgetResizable(True)
         scrollarea.setWidget(widget)
         self.pages_widget.addWidget(scrollarea)
         item = QListWidgetItem(self.contents_widget)
         try:
             item.setIcon(widget.icon)
@@ -657,27 +687,30 @@
         widget.propose_changes.connect(self.check_changes)
 
     def check_changes(self, configpage):
         """Enable the apply button if there are changes to the settings"""
         if configpage != self.get_page():
             return
         self.bt_apply.setEnabled(
-            not configpage.auto_updates and configpage.is_valid and
-            configpage.changed)
+            not configpage.auto_updates
+            and configpage.is_valid
+            and configpage.changed
+        )
 
     def load_plugin_pages(self):
         """Load the rcParams for the plugins in separate pages"""
         validators = psy_rcParams.validate
         descriptions = psy_rcParams.descriptions
         for ep in psy_rcParams._load_plugin_entrypoints():
             plugin = ep.load()
-            rc = getattr(plugin, 'rcParams', None)
+            rc = getattr(plugin, "rcParams", None)
             if rc is None:
                 rc = RcParams()
             w = RcParamsWidget(parent=self)
-            w.title = 'rcParams of ' + ep.module_name
+            w.title = "rcParams of " + ep.module
             w.default_path = PsyRcParamsWidget.default_path
-            w.initialize(rcParams=rc, validators=validators,
-                         descriptions=descriptions)
+            w.initialize(
+                rcParams=rc, validators=validators, descriptions=descriptions
+            )
             # use the full rcParams after initialization
             w.rc = psy_rcParams
             self.add_page(w)
```

### Comparing `psyplot-gui-1.4.0/psyplot_gui/sphinx_supp/conf.py` & `psyplot-gui-1.5.0/psyplot_gui/sphinx_supp/conf.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,173 +8,153 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psyplot-gui and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import sys
-import sphinx
-import sphinx_rtd_theme
 import re
-import six
+import sys
 from itertools import product
+
 import psyplot_gui
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autosummary',
-    'sphinx.ext.todo',
-    'sphinx.ext.viewcode',
-    'psyplot.sphinxext.extended_napoleon',
+    "sphinx.ext.autosummary",
+    "sphinx.ext.todo",
+    "sphinx.ext.viewcode",
+    "psyplot.sphinxext.extended_napoleon",
 ]
 
-if psyplot_gui.rcParams['help_explorer.use_intersphinx'] is None:
+if psyplot_gui.rcParams["help_explorer.use_intersphinx"] is None:
     if sys.platform.startswith("win"):
         use_intersphinx = False
     else:
-        use_intersphinx = psyplot_gui.rcParams['help_explorer.online']
+        use_intersphinx = psyplot_gui.rcParams["help_explorer.online"]
 else:
-    use_intersphinx = psyplot_gui.rcParams['help_explorer.use_intersphinx']
+    use_intersphinx = psyplot_gui.rcParams["help_explorer.use_intersphinx"]
 
 if use_intersphinx:
-    extensions.append('sphinx.ext.intersphinx')
+    extensions.append("sphinx.ext.intersphinx")
 del use_intersphinx
 
-autodoc_default_options = {
-    'show_inheritance': True
-}
+autodoc_default_options = {"show_inheritance": True}
 
 try:
-    import autodocsumm
+    import autodocsumm  # noqa: F401
 except ImportError:
     pass
 else:
-    extensions.append('autodocsumm')
-    autodoc_default_options['autosummary'] = True
-    not_document_data = ['psyplot.config.rcsetup.defaultParams',
-                         'psyplot.config.rcsetup.rcParams']
+    extensions.append("autodocsumm")
+    autodoc_default_options["autosummary"] = True
+    not_document_data = [
+        "psyplot.config.rcsetup.defaultParams",
+        "psyplot.config.rcsetup.rcParams",
+    ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 napoleon_use_admonition_for_examples = True
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'psyplot'
+master_doc = "psyplot"
 
-autoclass_content = 'both'
+autoclass_content = "both"
 
 # General information about the project.
-project = 'psyplot Help'
+project = "psyplot Help"
 copyright = psyplot_gui.__copyright__
 author = psyplot_gui.__author__
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = re.match(r'\d+\.\d+\.\d+', psyplot_gui.__version__).group()
+version = re.match(r"\d+\.\d+\.\d+", psyplot_gui.__version__).group()
 # The full version, including alpha/beta/rc tags.
 release = psyplot_gui.__version__
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build']
+exclude_patterns = ["_build"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'sphinx_rtd_theme'
-html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
+html_theme = "sphinx_rtd_theme"
 html_theme_options = {
-    'prev_next_buttons_location': None
-    }
+    "prev_next_buttons_location": None,
+    "collapse_navigation": False,
+}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'psyplotdoc'
+htmlhelp_basename = "psyplotdoc"
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    'pandas': ('https://pandas.pydata.org/pandas-docs/stable/', None),
-    'numpy': ('https://numpy.org/doc/stable/', None),
-    'matplotlib': ('https://matplotlib.org/', None),
-    'sphinx': ('https://www.sphinx-doc.org/en/master/', None),
-    'xarray': ('https://xarray.pydata.org/en/stable/', None),
-    'cartopy': ('https://scitools.org.uk/cartopy/docs/latest/', None),
-    'psyplot': ('https://psyplot.github.io/psyplot/', None),
-    'psyplot_gui': ('https://psyplot.github.io/psyplot-gui/', None),
-    'psy_maps': ('https://psyplot.github.io/psy-maps/', None),
-    'psy_simple': ('https://psyplot.github.io/psy-simple/', None),
-    'psy_view': ('https://psyplot.github.io/psy-view/', None),
-    'psy_reg': ('https://psyplot.github.io/psy-reg/', None),
-    'python': ('https://docs.python.org/3/', None),
+    "pandas": ("https://pandas.pydata.org/pandas-docs/stable/", None),
+    "numpy": ("https://numpy.org/doc/stable/", None),
+    "matplotlib": ("https://matplotlib.org/", None),
+    "sphinx": ("https://www.sphinx-doc.org/en/master/", None),
+    "xarray": ("https://xarray.pydata.org/en/stable/", None),
+    "cartopy": ("https://scitools.org.uk/cartopy/docs/latest/", None),
+    "psyplot": ("https://psyplot.github.io/psyplot/", None),
+    "psyplot_gui": ("https://psyplot.github.io/psyplot-gui/", None),
+    "psy_maps": ("https://psyplot.github.io/psy-maps/", None),
+    "psy_simple": ("https://psyplot.github.io/psy-simple/", None),
+    "psy_view": ("https://psyplot.github.io/psy-view/", None),
+    "psy_reg": ("https://psyplot.github.io/psy-reg/", None),
+    "python": ("https://docs.python.org/3/", None),
 }
 
 replacements = {
-    '`psyplot.rcParams`': '`~psyplot.config.rcsetup.rcParams`',
-    '`psyplot.InteractiveList`': '`~psyplot.data.InteractiveList`',
-    '`psyplot.InteractiveArray`': '`~psyplot.data.InteractiveArray`',
-    '`psyplot.open_dataset`': '`~psyplot.data.open_dataset`',
-    '`psyplot.open_mfdataset`': '`~psyplot.data.open_mfdataset`',
-    }
+    "`psyplot.rcParams`": "`~psyplot.config.rcsetup.rcParams`",
+    "`psyplot.InteractiveList`": "`~psyplot.data.InteractiveList`",
+    "`psyplot.InteractiveArray`": "`~psyplot.data.InteractiveArray`",
+    "`psyplot.open_dataset`": "`~psyplot.data.open_dataset`",
+    "`psyplot.open_mfdataset`": "`~psyplot.data.open_mfdataset`",
+}
 
 
 def link_aliases(app, what, name, obj, options, lines):
-    for (key, val), (i, line) in product(six.iteritems(replacements),
-                                         enumerate(lines)):
+    for (key, val), (i, line) in product(
+        replacements.items(), enumerate(lines)
+    ):
         lines[i] = line.replace(key, val)
 
 
 def setup(app):
-    app.connect('autodoc-process-docstring', link_aliases)
-    return {'version': sphinx.__display_version__, 'parallel_read_safe': True}
+    app.connect("autodoc-process-docstring", link_aliases)
```

