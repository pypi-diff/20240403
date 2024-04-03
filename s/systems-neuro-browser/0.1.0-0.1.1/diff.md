# Comparing `tmp/systems-neuro-browser-0.1.0.tar.gz` & `tmp/systems-neuro-browser-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systems-neuro-browser-0.1.0.tar", last modified: Wed Mar 13 13:30:20 2024, max compression
+gzip compressed data, was "systems-neuro-browser-0.1.1.tar", last modified: Wed Apr  3 14:42:31 2024, max compression
```

## Comparing `systems-neuro-browser-0.1.0.tar` & `systems-neuro-browser-0.1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-03-13 13:30:20.748871 systems-neuro-browser-0.1.0/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1080 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/LICENSE
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4797 2024-03-13 13:30:20.748678 systems-neuro-browser-0.1.0/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     3545 2024-02-05 20:40:46.000000 systems-neuro-browser-0.1.0/README.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1108 2024-03-13 13:30:20.749865 systems-neuro-browser-0.1.0/setup.cfg
--rw-r--r--   0 calebweinreb   (501) staff       (20)      254 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/setup.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-03-13 13:30:20.750248 systems-neuro-browser-0.1.0/snub/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      109 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)       68 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/__main__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2024-03-13 13:30:20.750344 systems-neuro-browser-0.1.0/snub/_version.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-03-13 13:30:20.725210 systems-neuro-browser-0.1.0/snub/gui/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      101 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.0/snub/gui/__init__.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-03-13 13:30:20.729564 systems-neuro-browser-0.1.0/snub/gui/help/
--rw-r--r--   0 calebweinreb   (501) staff       (20)       32 2024-02-23 04:28:36.000000 systems-neuro-browser-0.1.0/snub/gui/help/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1666 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.0/snub/gui/help/heatmaps.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)     2776 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.0/snub/gui/help/help_menu.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1427 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.0/snub/gui/help/layout.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      496 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.0/snub/gui/help/loading_data.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1869 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.0/snub/gui/help/scatter_plots.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1789 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.0/snub/gui/help/selections.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1446 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.0/snub/gui/help/timeline.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1153 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.0/snub/gui/help/trace_plots.md
--rw-r--r--   0 calebweinreb   (501) staff       (20)      597 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.0/snub/gui/help/video.md
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-03-13 13:30:20.732937 systems-neuro-browser-0.1.0/snub/gui/icons/
--rw-r--r--   0 calebweinreb   (501) staff       (20)    15772 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/icons/app_icon.png
--rw-r--r--   0 calebweinreb   (501) staff       (20)     2149 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/icons/checkbox_checked.png
--rw-r--r--   0 calebweinreb   (501) staff       (20)      451 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/icons/checkbox_unchecked.png
--rw-r--r--   0 calebweinreb   (501) staff       (20)      557 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/icons/minus.png
--rw-r--r--   0 calebweinreb   (501) staff       (20)      571 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/icons/pause.png
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1363 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/icons/play.png
--rw-r--r--   0 calebweinreb   (501) staff       (20)      608 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/icons/plus.png
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4473 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/icons/x.png
--rw-r--r--   0 calebweinreb   (501) staff       (20)    16921 2024-02-23 04:28:36.000000 systems-neuro-browser-0.1.0/snub/gui/main.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-03-13 13:30:20.735584 systems-neuro-browser-0.1.0/snub/gui/panels/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      146 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/panels/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)      745 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/panels/base.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     6390 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/panels/pose3D.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     6607 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/panels/roi.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    14835 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.0/snub/gui/panels/scatter.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     3853 2024-02-12 18:34:37.000000 systems-neuro-browser-0.1.0/snub/gui/panels/video.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-03-13 13:30:20.737280 systems-neuro-browser-0.1.0/snub/gui/stacks/
--rw-r--r--   0 calebweinreb   (501) staff       (20)       84 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/stacks/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)      748 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/stacks/base.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     2257 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/stacks/panel.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     6889 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/stacks/track.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-03-13 13:30:20.739509 systems-neuro-browser-0.1.0/snub/gui/tracks/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      322 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/tracks/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    11496 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/tracks/base.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    17601 2024-02-05 20:29:03.000000 systems-neuro-browser-0.1.0/snub/gui/tracks/heatmap.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     6354 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/tracks/spike.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    12199 2024-02-22 07:11:54.000000 systems-neuro-browser-0.1.0/snub/gui/tracks/trace.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-03-13 13:30:20.740814 systems-neuro-browser-0.1.0/snub/gui/utils/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      166 2024-02-05 20:29:03.000000 systems-neuro-browser-0.1.0/snub/gui/utils/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     5560 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/gui/utils/interval.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     7444 2024-02-05 20:29:03.000000 systems-neuro-browser-0.1.0/snub/gui/utils/widgets.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-03-13 13:30:20.743381 systems-neuro-browser-0.1.0/snub/io/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      107 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/io/__init__.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     6166 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/io/manifold.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    16237 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/io/nwb.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1061 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/io/plot.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    63062 2024-02-22 06:37:06.000000 systems-neuro-browser-0.1.0/snub/io/project.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     6222 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/snub/io/video.py
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-03-13 13:30:20.745800 systems-neuro-browser-0.1.0/systems_neuro_browser.egg-info/
--rw-r--r--   0 calebweinreb   (501) staff       (20)     4797 2024-03-13 13:30:20.000000 systems-neuro-browser-0.1.0/systems_neuro_browser.egg-info/PKG-INFO
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1526 2024-03-13 13:30:20.000000 systems-neuro-browser-0.1.0/systems_neuro_browser.egg-info/SOURCES.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2024-03-13 13:30:20.000000 systems-neuro-browser-0.1.0/systems_neuro_browser.egg-info/dependency_links.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)       43 2024-03-13 13:30:20.000000 systems-neuro-browser-0.1.0/systems_neuro_browser.egg-info/entry_points.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)      324 2024-03-13 13:30:20.000000 systems-neuro-browser-0.1.0/systems_neuro_browser.egg-info/requires.txt
--rw-r--r--   0 calebweinreb   (501) staff       (20)        5 2024-03-13 13:30:20.000000 systems-neuro-browser-0.1.0/systems_neuro_browser.egg-info/top_level.txt
-drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-03-13 13:30:20.747025 systems-neuro-browser-0.1.0/tests/
--rw-r--r--   0 calebweinreb   (501) staff       (20)      744 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/tests/test_gui.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     2648 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/tests/test_io.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)     1189 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.0/tests/test_nwb.py
--rw-r--r--   0 calebweinreb   (501) staff       (20)    83912 2024-02-23 05:35:30.000000 systems-neuro-browser-0.1.0/versioneer.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-03 14:42:31.983244 systems-neuro-browser-0.1.1/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1080 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/LICENSE
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4163 2024-04-03 14:42:31.983505 systems-neuro-browser-0.1.1/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     3763 2024-04-03 14:42:07.000000 systems-neuro-browser-0.1.1/README.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1166 2024-04-03 14:42:31.984981 systems-neuro-browser-0.1.1/setup.cfg
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      254 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/setup.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-03 14:42:31.985416 systems-neuro-browser-0.1.1/snub/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      109 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       68 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/__main__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      497 2024-04-03 14:42:31.985521 systems-neuro-browser-0.1.1/snub/_version.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-03 14:42:31.952474 systems-neuro-browser-0.1.1/snub/gui/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      101 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.1/snub/gui/__init__.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-03 14:42:31.959013 systems-neuro-browser-0.1.1/snub/gui/help/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       32 2024-02-23 04:28:36.000000 systems-neuro-browser-0.1.1/snub/gui/help/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1666 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.1/snub/gui/help/heatmaps.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     2776 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.1/snub/gui/help/help_menu.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1427 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.1/snub/gui/help/layout.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      496 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.1/snub/gui/help/loading_data.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1869 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.1/snub/gui/help/scatter_plots.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1789 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.1/snub/gui/help/selections.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1446 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.1/snub/gui/help/timeline.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1153 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.1/snub/gui/help/trace_plots.md
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      597 2024-02-22 05:19:28.000000 systems-neuro-browser-0.1.1/snub/gui/help/video.md
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-03 14:42:31.963694 systems-neuro-browser-0.1.1/snub/gui/icons/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    15772 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/icons/app_icon.png
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     2149 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/icons/checkbox_checked.png
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      451 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/icons/checkbox_unchecked.png
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      557 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/icons/minus.png
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      571 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/icons/pause.png
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1363 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/icons/play.png
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      608 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/icons/plus.png
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4473 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/icons/x.png
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17508 2024-04-03 14:42:07.000000 systems-neuro-browser-0.1.1/snub/gui/main.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-03 14:42:31.967232 systems-neuro-browser-0.1.1/snub/gui/panels/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      146 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/panels/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      745 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/panels/base.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     5923 2024-04-03 14:42:07.000000 systems-neuro-browser-0.1.1/snub/gui/panels/pose3D.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     6335 2024-04-03 14:42:07.000000 systems-neuro-browser-0.1.1/snub/gui/panels/roi.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    14792 2024-04-03 14:42:07.000000 systems-neuro-browser-0.1.1/snub/gui/panels/scatter.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     3723 2024-04-03 14:42:07.000000 systems-neuro-browser-0.1.1/snub/gui/panels/video.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-03 14:42:31.969643 systems-neuro-browser-0.1.1/snub/gui/stacks/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       84 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/stacks/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      748 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/stacks/base.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     2257 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/stacks/panel.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     6889 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/stacks/track.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-03 14:42:31.972808 systems-neuro-browser-0.1.1/snub/gui/tracks/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      322 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/tracks/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    11496 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/tracks/base.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    17312 2024-04-03 14:42:07.000000 systems-neuro-browser-0.1.1/snub/gui/tracks/heatmap.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     6311 2024-04-03 14:42:07.000000 systems-neuro-browser-0.1.1/snub/gui/tracks/spike.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    12126 2024-04-03 14:42:07.000000 systems-neuro-browser-0.1.1/snub/gui/tracks/trace.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-03 14:42:31.974441 systems-neuro-browser-0.1.1/snub/gui/utils/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      166 2024-02-05 20:29:03.000000 systems-neuro-browser-0.1.1/snub/gui/utils/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     5560 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/gui/utils/interval.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     7444 2024-02-05 20:29:03.000000 systems-neuro-browser-0.1.1/snub/gui/utils/widgets.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-03 14:42:31.978345 systems-neuro-browser-0.1.1/snub/io/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      107 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/io/__init__.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     6166 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/io/manifold.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    16237 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/io/nwb.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1061 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/io/plot.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    63112 2024-04-03 14:42:07.000000 systems-neuro-browser-0.1.1/snub/io/project.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     6222 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/snub/io/video.py
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-03 14:42:31.981090 systems-neuro-browser-0.1.1/systems_neuro_browser.egg-info/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     4163 2024-04-03 14:42:31.000000 systems-neuro-browser-0.1.1/systems_neuro_browser.egg-info/PKG-INFO
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1526 2024-04-03 14:42:31.000000 systems-neuro-browser-0.1.1/systems_neuro_browser.egg-info/SOURCES.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        1 2024-04-03 14:42:31.000000 systems-neuro-browser-0.1.1/systems_neuro_browser.egg-info/dependency_links.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)       43 2024-04-03 14:42:31.000000 systems-neuro-browser-0.1.1/systems_neuro_browser.egg-info/entry_points.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      393 2024-04-03 14:42:31.000000 systems-neuro-browser-0.1.1/systems_neuro_browser.egg-info/requires.txt
+-rw-r--r--   0 calebweinreb   (501) staff       (20)        5 2024-04-03 14:42:31.000000 systems-neuro-browser-0.1.1/systems_neuro_browser.egg-info/top_level.txt
+drwxr-xr-x   0 calebweinreb   (501) staff       (20)        0 2024-04-03 14:42:31.982711 systems-neuro-browser-0.1.1/tests/
+-rw-r--r--   0 calebweinreb   (501) staff       (20)      744 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/tests/test_gui.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     2648 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/tests/test_io.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)     1189 2024-02-04 23:09:58.000000 systems-neuro-browser-0.1.1/tests/test_nwb.py
+-rw-r--r--   0 calebweinreb   (501) staff       (20)    83912 2024-02-23 05:35:30.000000 systems-neuro-browser-0.1.1/versioneer.py
```

### Comparing `systems-neuro-browser-0.1.0/LICENSE` & `systems-neuro-browser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/README.md` & `systems-neuro-browser-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Systems Neuro Browser (SNUB)
 
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.06187/status.svg)](https://doi.org/10.21105/joss.06187)
+
 ## [Read the documentation!](https://snub.readthedocs.io/en/latest/)
 
 SNUB is a visual interface for systems neuroscience. Using a set of linked data-views, users can explore relationships between raw video, 3D animal pose, behavior annotations, neural activity, or any other relevant time-series data.
 
 ![](https://github.com/calebweinreb/SNUB/blob/main/docs/media/use_case1.gif)
 
 
@@ -11,14 +13,17 @@
 
 Create and activate a new conda environment with python≥3.8 and install via pip
 ```
 conda create -n snub python=3.8
 conda activate snub
 pip install systems-neuro-browser
 ```
+
+**Note: Python version 3.8 is required for Linux. For Windows and MacOS, any version ≥3.8 should work.**
+
 To speed up selections, `pip install ncls`. To install optional developer dependencies, `pip install systems-neuro-browser[dev]`. The docs include more detailed [installation instructions](https://snub.readthedocs.io/en/latest/install.html).
 
 ## Getting Started
 
 * Download the [example project](https://zenodo.org/records/10578025/files/miniscope_project.zip?download=1). 
 * Launch SNUB from the command line with the command `snub`.
 * Go to `File > Open Project`, navigate to the project directory, and hit `Choose` with the directory selected.
```

### Comparing `systems-neuro-browser-0.1.0/setup.cfg` & `systems-neuro-browser-0.1.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 classifiers = 
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
-python_requires = >=3.8, <3.9
+python_requires = >=3.8
 install_requires = 
 	PyQt5
 	numpy
 	scikit-learn
 	tqdm
 	cmapy
 	interlap
@@ -25,15 +25,16 @@
 	imageio
 	imageio-ffmpeg
 	umap-learn
 	rastermap==0.1.3
 	ipykernel
 	pyqtgraph
 	networkx
-	opencv-python==4.1.2.30
+	opencv-python; python_version > '3.8'
+	opencv-python==4.1.2.30; python_version == '3.8'
 	vidio>=0.0.3
 	pynwb
 	ndx-pose
 	ndx-photometry
 	ndx-depth-moseq
 	pandas
 	dandi
```

### Comparing `systems-neuro-browser-0.1.0/snub/gui/help/heatmaps.md` & `systems-neuro-browser-0.1.1/snub/gui/help/heatmaps.md`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/help/help_menu.py` & `systems-neuro-browser-0.1.1/snub/gui/help/help_menu.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/help/layout.md` & `systems-neuro-browser-0.1.1/snub/gui/help/layout.md`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/help/scatter_plots.md` & `systems-neuro-browser-0.1.1/snub/gui/help/scatter_plots.md`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/help/selections.md` & `systems-neuro-browser-0.1.1/snub/gui/help/selections.md`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/help/timeline.md` & `systems-neuro-browser-0.1.1/snub/gui/help/timeline.md`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/help/trace_plots.md` & `systems-neuro-browser-0.1.1/snub/gui/help/trace_plots.md`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/help/video.md` & `systems-neuro-browser-0.1.1/snub/gui/help/video.md`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/icons/app_icon.png` & `systems-neuro-browser-0.1.1/snub/gui/icons/app_icon.png`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/icons/checkbox_checked.png` & `systems-neuro-browser-0.1.1/snub/gui/icons/checkbox_checked.png`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/icons/minus.png` & `systems-neuro-browser-0.1.1/snub/gui/icons/minus.png`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/icons/pause.png` & `systems-neuro-browser-0.1.1/snub/gui/icons/pause.png`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/icons/play.png` & `systems-neuro-browser-0.1.1/snub/gui/icons/play.png`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/icons/plus.png` & `systems-neuro-browser-0.1.1/snub/gui/icons/plus.png`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/icons/x.png` & `systems-neuro-browser-0.1.1/snub/gui/icons/x.png`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/main.py` & `systems-neuro-browser-0.1.1/snub/gui/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 import sys, os, json
 from functools import partial
 from snub.gui.utils import IntervalIndex, CheckBox
 from snub.gui.stacks import PanelStack, TrackStack
 from snub.gui.tracks import TracePlot
 from snub.gui.help import HelpMenu
 
+WIDGET_NAMES = [
+    "heatmap",
+    "video",
+    "traceplot",
+    "spikeplot",
+    "roiplot",
+    "scatter",
+    "pose3D",
+]
+
 
 def set_style(app):
     # https://www.wenzhaodesign.com/devblog/python-pyside2-simple-dark-theme
     # button from here https://github.com/persepolisdm/persepolis/blob/master/persepolis/gui/palettes.py
     app.setStyle(QStyleFactory.create("Fusion"))
 
     darktheme = QPalette()
@@ -156,26 +166,28 @@
     def update_track_playhead(self, checkstate):
         self.track_playhead = checkstate
         if self.track_playhead:
             self.trackStack.center_at_time(self.current_time)
 
     def validate_and_autofill_config(self, config):
         error_messages = []
-        config["project_directory"] = self.project_directory
 
+        # check for required global keys
         for k in ["bounds"]:
             if not k in config:
                 error_messages.append('config is missing the key "{}"'.format(k))
 
+        # initialize current time if not provided
         if not "init_current_time" in config:
             if "bounds" in config:
                 config["init_current_time"] = config["bounds"][0]
             else:
                 config["init_current_time"] = 0
 
+        # autofill missing keys
         default_config = {
             "layout_mode": "columns",
             "min_step": 1 / 30,
             "zoom_gain": 0.003,
             "min_range": 0.01,
             "initial_playspeed": 1,
             "animation_fps": 30,
@@ -187,19 +199,19 @@
             "roiplot": [],
             "scatter": [],
             "heatmap": [],
             "pose3D": [],
             "video": [],
             "markers": {},
         }
-
         for key, value in default_config.items():
             if not key in config:
                 config[key] = value
 
+        # check for required keys in each widget
         for widget_name, requred_keys in {
             "heatmap": ["name", "data_path", "intervals_path", "add_traceplot"],
             "video": ["name", "video_path", "timestamps_path"],
             "traceplot": ["name", "data_path"],
             "spikeplot": ["name", "heatmap_path", "spikes_path", "intervals_path"],
             "roiplot": ["name", "video_paths", "rois_path", "timestamps_path"],
             "scatter": ["name", "data_path"],
@@ -207,14 +219,22 @@
             for props in config[widget_name]:
                 for k in requred_keys:
                     if not k in props:
                         error_messages.append(
                             '{} is missing the key "{}"'.format(widget_name, k)
                         )
 
+        # resolve paths
+        for widget_name in WIDGET_NAMES:
+            for widget_config in config[widget_name]:
+                for k, v in widget_config.items():
+                    if k.endswith("_path"):
+                        if not os.path.isabs(v):
+                            widget_config[k] = os.path.join(self.project_directory, v)
+
         return config, error_messages
 
     def config_error(self, config_path, error_messages):
         title = QLabel("The following config file is incomplete")
         path = QLabel("   " + config_path)
         errors = QLabel(
             "<html><ul><li>" + "</li><li>".join(error_messages) + "</li></ul></html>"
```

### Comparing `systems-neuro-browser-0.1.0/snub/gui/panels/base.py` & `systems-neuro-browser-0.1.1/snub/gui/panels/base.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/panels/pose3D.py` & `systems-neuro-browser-0.1.1/snub/gui/panels/pose3D.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,46 +28,34 @@
         floor_height=0,
         floor_spacing=10,
         floor_color=(1, 1, 1, 0.5),
         **kwargs
     ):
         super().__init__(config, **kwargs)
 
-        self.data = np.load(os.path.join(config["project_directory"], data_path))
-        self.intervals = np.load(
-            os.path.join(config["project_directory"], intervals_path)
-        )
+        self.data = np.load(data_path)
+        self.intervals = np.load(intervals_path)
+
         if labels_path is None:
             self.labels = [str(i) for i in range(self.data.shape[0])]
         else:
-            self.labels = (
-                open(os.path.join(config["project_directory"], labels_path), "r")
-                .read()
-                .split("\n")
-            )
+            self.labels = open(labels_path, "r").read().split("\n")
         if links_path is None:
             self.link_indexes = np.zeros((0, 2), dtype=int)
         else:
-            self.link_indexes = np.load(
-                os.path.join(config["project_directory"], links_path)
-            ).astype(int)
+            self.link_indexes = np.load(links_path).astype(int)
         if joint_colors_path is None:
             self.joint_colors = np.ones((self.data.shape[0], 3))
         else:
-            self.joint_colors = np.load(
-                os.path.join(config["project_directory"], joint_colors_path)
-            )
+            self.joint_colors = np.load(joint_colors_path)
+
         if link_colors_path is None:
             self.link_colors = np.ones((len(self.links) * 2, 3))
         else:
-            self.link_colors = np.repeat(
-                np.load(os.path.join(config["project_directory"], link_colors_path)),
-                2,
-                axis=0,
-            )
+            self.link_colors = np.repeat(np.load(link_colors_path), 2, axis=0)
 
         self.joint_size = joint_size
         self.link_width = link_width
         self.scaling = scaling
 
         self.canvas = SceneCanvas(keys="interactive", show=True)
         self.view = self.canvas.central_widget.add_view(camera="arcball")
```

### Comparing `systems-neuro-browser-0.1.0/snub/gui/panels/roi.py` & `systems-neuro-browser-0.1.1/snub/gui/panels/roi.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,27 +52,21 @@
         self.linewidth = linewidth
         self.colormap = colormap
         self.vmin, self.vmax = vmin, vmax
         self.dims = dimensions
         self.current_frame_index = None
         self.is_visible = True
 
-        self.rois = load_npz(os.path.join(config["project_directory"], rois_path))
-        self.timestamps = np.load(
-            os.path.join(config["project_directory"], timestamps_path)
-        )
+        self.rois = load_npz(rois_path)
+        self.timestamps = np.load(timestamps_path)
 
         if labels_path is None:
             self.labels = [str(i) for i in range(self.rois.shape[0])]
         else:
-            self.labels = (
-                open(os.path.join(config["project_directory"], labels_path), "r")
-                .read()
-                .split("\n")
-            )
+            self.labels = open(labels_path, "r").read().split("\n")
 
         self.adjust_colormap_dialog = AdjustColormapDialog(self, self.vmin, self.vmax)
         self.adjust_colormap_dialog.new_range.connect(self.update_colormap_range)
 
         self.canvas = SceneCanvas(self, keys="interactive", show=True)
         self.canvas.events.mouse_release.connect(self.mouse_release)
         self.viewbox = self.canvas.central_widget.add_grid().add_view(
@@ -93,16 +87,15 @@
                 color=np.array(color) / 255,
                 width=self.linewidth,
                 connect="strip",
                 parent=None,
             )
 
         self.vids = {
-            name: VideoReader(os.path.join(config["project_directory"], video_path))
-            for name, video_path in video_paths.items()
+            name: VideoReader(video_path) for name, video_path in video_paths.items()
         }
 
         self.dropDown = QComboBox()
         self.dropDown.addItems(list(video_paths.keys())[::-1])
         self.dropDown.activated.connect(self.update_image)
 
         self.image = Image(
```

### Comparing `systems-neuro-browser-0.1.0/snub/gui/panels/scatter.py` & `systems-neuro-browser-0.1.1/snub/gui/panels/scatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self.selection_intersection_threshold = selection_intersection_threshold
         self.variable_labels = ["Interval start", "Interval end"] + variable_labels
         self.vmin, self.vmax = 0, 1
         self.current_variable_label = "(No color)"
         self.sort_nodes_by_variable = True
         self.show_marker_trail = False
 
-        self.data = np.load(os.path.join(config["project_directory"], data_path))
+        self.data = np.load(data_path)
         self.data[:, 2:4] = self.data[:, 2:4] + np.array([-self.eps, self.eps])
         self.is_selected = np.zeros(self.data.shape[0]) > 0
         self.plot_order = np.arange(self.data.shape[0])
         self.interval_index = IntervalIndex(
             min_step=self.min_step, intervals=self.data[:, 2:4]
         )
```

### Comparing `systems-neuro-browser-0.1.0/snub/gui/panels/video.py` & `systems-neuro-browser-0.1.1/snub/gui/panels/video.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,20 +27,16 @@
     qpixmap = QPixmap(QImage(image, W, H, image.strides[0], format))
     return qpixmap
 
 
 class VideoPanel(Panel, HeaderMixin):
     def __init__(self, config, video_path=None, timestamps_path=None, **kwargs):
         super().__init__(config, **kwargs)
-        self.video_frame = VideoFrame(
-            os.path.join(config["project_directory"], video_path)
-        )
-        self.timestamps = np.load(
-            os.path.join(config["project_directory"], timestamps_path)
-        )
+        self.video_frame = VideoFrame(video_path)
+        self.timestamps = np.load(timestamps_path)
         self.current_frame_index = None
         self.is_visible = True
         self.update_current_time(config["init_current_time"])
         self.initUI(**kwargs)
 
     def initUI(self, **kwargs):
         super().initUI(**kwargs)
```

### Comparing `systems-neuro-browser-0.1.0/snub/gui/stacks/base.py` & `systems-neuro-browser-0.1.1/snub/gui/stacks/base.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/stacks/panel.py` & `systems-neuro-browser-0.1.1/snub/gui/stacks/panel.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/stacks/track.py` & `systems-neuro-browser-0.1.1/snub/gui/stacks/track.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/tracks/base.py` & `systems-neuro-browser-0.1.1/snub/gui/tracks/base.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/tracks/heatmap.py` & `systems-neuro-browser-0.1.1/snub/gui/tracks/heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,38 +254,31 @@
         super().__init__(config, **kwargs)
         self.selected_intervals = selected_intervals
         self.vmin, self.vmax = vmin, vmax
         self.colormap = colormap
         self.add_traceplot = add_traceplot
         self.min_step = config["min_step"]
 
-        self.data = np.load(os.path.join(config["project_directory"], data_path))
-        self.intervals = np.load(
-            os.path.join(config["project_directory"], intervals_path)
-        )
+        self.data = np.load(data_path)
+        self.intervals = np.load(intervals_path)
 
         if labels_path is None:
             self.labels = [str(i) for i in range(self.data.shape[0])]
         else:
-            self.labels = (
-                open(os.path.join(config["project_directory"], labels_path), "r")
-                .read()
-                .split("\n")
-            )
+            self.labels = open(labels_path, "r").read().split("\n")
 
         if row_colors is None:
             row_colors = [_random_color() for i in range(self.data.shape[0])]
         self.row_colors = row_colors
 
         if row_order_path is None:
             self.row_order = np.arange(self.data.shape[0])
         else:
-            self.row_order = np.load(
-                os.path.join(config["project_directory"], row_order_path)
-            )
+            self.row_order = np.load(row_order_path)
+
         self.initial_row_order = self.row_order.copy()
 
         if vertical_range is None:
             self.vertical_range = [0, self.data.shape[0]]
         else:
             self.vertical_range = vertical_range
```

### Comparing `systems-neuro-browser-0.1.0/snub/gui/tracks/spike.py` & `systems-neuro-browser-0.1.1/snub/gui/tracks/spike.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         heatmap_path=None,
         heatmap_range=60,
         colormap="viridis",
         **kwargs
     ):
         super().__init__(config, selected_intervals, data_path=heatmap_path, **kwargs)
         self.heatmap_range = heatmap_range
-        spike_data = np.load(os.path.join(config["project_directory"], spikes_path))
+        spike_data = np.load(spikes_path)
         self.spike_times, self.spike_labels = spike_data[:, 0], spike_data[:, 1].astype(
             int
         )
         self.max_label = self.spike_labels.max()
         self.markersize = markersize
         self.colormap = colormap
         self.cmap = (
```

### Comparing `systems-neuro-browser-0.1.0/snub/gui/tracks/trace.py` & `systems-neuro-browser-0.1.1/snub/gui/tracks/trace.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,15 @@
 
         self.adjust_linewidth_dialog = AdjustLinewidthDialog(self, linewidth)
         self.adjust_linewidth_dialog.new_linewidth.connect(self.update_linewidth)
 
         if data is not None:
             self.data = data
         else:
-            self.data = pickle.load(
-                open(os.path.join(config["project_directory"], data_path), "rb")
-            )
+            self.data = pickle.load(open(data_path), "rb")
 
         if initial_visible_traces is not None:
             self.visible_traces = set(initial_visible_traces)
         elif len(self.data) > 0:
             self.visible_traces = set([np.random.choice(list(self.data.keys()))])
         else:
             self.visible_traces = set([])
```

### Comparing `systems-neuro-browser-0.1.0/snub/gui/utils/interval.py` & `systems-neuro-browser-0.1.1/snub/gui/utils/interval.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/gui/utils/widgets.py` & `systems-neuro-browser-0.1.1/snub/gui/utils/widgets.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/io/manifold.py` & `systems-neuro-browser-0.1.1/snub/io/manifold.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/io/nwb.py` & `systems-neuro-browser-0.1.1/snub/io/nwb.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/io/plot.py` & `systems-neuro-browser-0.1.1/snub/io/plot.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/snub/io/project.py` & `systems-neuro-browser-0.1.1/snub/io/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,19 +499,21 @@
     timestamps_path_rel = name + ".timestamps.npy"
     timestamps_path_abs = os.path.join(project_directory, timestamps_path_rel)
     np.save(timestamps_path_abs, timestamps)
     print("Saved timestamps to " + timestamps_path_abs)
 
     # optionally copy video
     if copy:
-        videopath = name + os.path.splitext(videopath)[1]
-        videopath_abs = os.path.join(project_directory, videopath)
+        videopath_abs = os.path.join(
+            project_directory, name + os.path.splitext(videopath)[1]
+        )
         if not os.path.exists(videopath_abs):
             shutil.copy(videopath, videopath_abs)
             print("Copying video to " + videopath_abs)
+        videopath = name + os.path.splitext(videopath)[1]
     else:
         videopath = os.path.realpath(videopath)
 
     # add props to config
     props = {
         "name": name,
         "video_path": videopath,
```

### Comparing `systems-neuro-browser-0.1.0/snub/io/video.py` & `systems-neuro-browser-0.1.1/snub/io/video.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/systems_neuro_browser.egg-info/SOURCES.txt` & `systems-neuro-browser-0.1.1/systems_neuro_browser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/tests/test_gui.py` & `systems-neuro-browser-0.1.1/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/tests/test_io.py` & `systems-neuro-browser-0.1.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/tests/test_nwb.py` & `systems-neuro-browser-0.1.1/tests/test_nwb.py`

 * *Files identical despite different names*

### Comparing `systems-neuro-browser-0.1.0/versioneer.py` & `systems-neuro-browser-0.1.1/versioneer.py`

 * *Files identical despite different names*

