# Comparing `tmp/mg-pso-gui-0.1.8.tar.gz` & `tmp/mg-pso-gui-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mg-pso-gui-0.1.8.tar", last modified: Wed Mar  6 06:34:13 2024, max compression
+gzip compressed data, was "mg-pso-gui-0.1.9.tar", last modified: Wed Mar  6 06:42:33 2024, max compression
```

## Comparing `mg-pso-gui-0.1.8.tar` & `mg-pso-gui-0.1.9.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.154402 mg-pso-gui-0.1.8/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     9457 2024-03-06 06:34:13.153815 mg-pso-gui-0.1.8/PKG-INFO
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.118332 mg-pso-gui-0.1.8/mg_pso_gui.egg-info/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     9457 2024-03-06 06:34:13.000000 mg-pso-gui-0.1.8/mg_pso_gui.egg-info/PKG-INFO
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1759 2024-03-06 06:34:13.000000 mg-pso-gui-0.1.8/mg_pso_gui.egg-info/SOURCES.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)        1 2024-03-06 06:34:13.000000 mg-pso-gui-0.1.8/mg_pso_gui.egg-info/dependency_links.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)      117 2024-03-06 06:34:13.000000 mg-pso-gui-0.1.8/mg_pso_gui.egg-info/entry_points.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)       76 2024-03-06 06:34:13.000000 mg-pso-gui-0.1.8/mg_pso_gui.egg-info/requires.txt
--rw-r--r--   0 robertcordingly   (501) staff       (20)        9 2024-03-06 06:34:13.000000 mg-pso-gui-0.1.8/mg_pso_gui.egg-info/top_level.txt
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.120161 mg-pso-gui-0.1.8/mgpsogui/
--rw-r--r--   0 robertcordingly   (501) staff       (20)       42 2023-10-10 00:40:24.000000 mg-pso-gui-0.1.8/mgpsogui/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.122432 mg-pso-gui-0.1.8/mgpsogui/gui/
--rwxr--r--   0 robertcordingly   (501) staff       (20)    25874 2024-03-06 06:33:23.000000 mg-pso-gui-0.1.8/mgpsogui/gui/HomePage.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    11712 2024-01-24 22:27:36.000000 mg-pso-gui-0.1.8/mgpsogui/gui/OptionManager.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.123704 mg-pso-gui-0.1.8/mgpsogui/gui/PlatformTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)    10486 2024-02-14 07:13:08.000000 mg-pso-gui-0.1.8/mgpsogui/gui/PlatformTab/PlatformTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:36:09.000000 mg-pso-gui-0.1.8/mgpsogui/gui/PlatformTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.125106 mg-pso-gui-0.1.8/mgpsogui/gui/RunTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2850 2024-02-14 07:26:36.000000 mg-pso-gui-0.1.8/mgpsogui/gui/RunTab/RunTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 06:41:01.000000 mg-pso-gui-0.1.8/mgpsogui/gui/RunTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.132488 mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2866 2024-02-14 07:40:24.000000 mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/BoundsEditorWindow.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12268 2024-02-14 08:06:06.000000 mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/BoundsList.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2784 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/CalibrationParametersView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4092 2024-02-13 06:33:07.000000 mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/FunctionsList.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     7352 2023-10-18 05:17:22.000000 mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/ListParametersView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1881 2024-02-14 08:15:40.000000 mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/SetupTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2739 2024-02-13 05:33:08.000000 mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/StaticParameterView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     5531 2024-02-13 06:31:26.000000 mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/StepView.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:20:36.000000 mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.133947 mg-pso-gui-0.1.8/mgpsogui/gui/VisualizeTab/
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3271 2024-02-28 21:07:31.000000 mg-pso-gui-0.1.8/mgpsogui/gui/VisualizeTab/VisualizeTab.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-14 03:49:32.000000 mg-pso-gui-0.1.8/mgpsogui/gui/VisualizeTab/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:33:58.000000 mg-pso-gui-0.1.8/mgpsogui/gui/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.144293 mg-pso-gui-0.1.8/mgpsogui/gui/images/
--rw-r--r--   0 robertcordingly   (501) staff       (20)   433752 2024-02-27 04:32:36.000000 mg-pso-gui-0.1.8/mgpsogui/gui/images/IGOW 4 Logo.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2989 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.8/mgpsogui/gui/images/collapse.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2654 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.8/mgpsogui/gui/images/down.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2922 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.8/mgpsogui/gui/images/expand.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2790 2024-02-14 06:41:01.000000 mg-pso-gui-0.1.8/mgpsogui/gui/images/play.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4657 2024-02-14 06:39:03.000000 mg-pso-gui-0.1.8/mgpsogui/gui/images/refresh.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)    31242 2024-02-14 08:26:13.000000 mg-pso-gui-0.1.8/mgpsogui/gui/images/refresh_hd.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2153 2024-02-14 06:41:07.000000 mg-pso-gui-0.1.8/mgpsogui/gui/images/stop.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2958 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.8/mgpsogui/gui/images/trash.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2457 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.8/mgpsogui/gui/images/up.png
--rw-r--r--   0 robertcordingly   (501) staff       (20)      148 2023-10-04 08:06:40.000000 mg-pso-gui-0.1.8/mgpsogui/mgpsogui.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     4713 2023-11-08 23:03:41.000000 mg-pso-gui-0.1.8/mgpsogui/start.yaml
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.146589 mg-pso-gui-0.1.8/mgpsogui/util/
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.147729 mg-pso-gui-0.1.8/mgpsogui/util/CTkToolTip/
--rw-rw-r--   0 robertcordingly   (501) staff       (20)      225 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.8/mgpsogui/util/CTkToolTip/__init__.py
--rw-rw-r--   0 robertcordingly   (501) staff       (20)     6329 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.8/mgpsogui/util/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     7851 2024-02-28 07:09:24.000000 mg-pso-gui-0.1.8/mgpsogui/util/GraphGenerator.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     6328 2024-03-06 06:26:18.000000 mg-pso-gui-0.1.8/mgpsogui/util/PSORunner.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:32:18.000000 mg-pso-gui-0.1.8/mgpsogui/util/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.148356 mg-pso-gui-0.1.8/mgpsogui/util/recosu/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      236 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.8/mgpsogui/util/recosu/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.150271 mg-pso-gui-0.1.8/mgpsogui/util/recosu/pso/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      247 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.8/mgpsogui/util/recosu/pso/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     2611 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.8/mgpsogui/util/recosu/pso/csip_access.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)    12467 2024-03-06 06:30:10.000000 mg-pso-gui-0.1.8/mgpsogui/util/recosu/pso/pso.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.151932 mg-pso-gui-0.1.8/mgpsogui/util/recosu/utils/
--rw-r--r--   0 robertcordingly   (501) staff       (20)      196 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.8/mgpsogui/util/recosu/utils/__init__.py
-drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:34:13.153003 mg-pso-gui-0.1.8/mgpsogui/util/recosu/utils/plot/
--rw-r--r--   0 robertcordingly   (501) staff       (20)       71 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.8/mgpsogui/util/recosu/utils/plot/__init__.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3779 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.8/mgpsogui/util/recosu/utils/plot/cost_steps.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3023 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.8/mgpsogui/util/recosu/utils/trace_writer.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)     3951 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.8/mgpsogui/util/recosu/utils/utils.py
--rw-r--r--   0 robertcordingly   (501) staff       (20)       38 2024-03-06 06:34:13.154539 mg-pso-gui-0.1.8/setup.cfg
--rw-r--r--   0 robertcordingly   (501) staff       (20)     1525 2024-03-06 06:34:10.000000 mg-pso-gui-0.1.8/setup.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.877754 mg-pso-gui-0.1.9/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     9457 2024-03-06 06:42:33.877183 mg-pso-gui-0.1.9/PKG-INFO
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.846222 mg-pso-gui-0.1.9/mg_pso_gui.egg-info/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     9457 2024-03-06 06:42:33.000000 mg-pso-gui-0.1.9/mg_pso_gui.egg-info/PKG-INFO
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1759 2024-03-06 06:42:33.000000 mg-pso-gui-0.1.9/mg_pso_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        1 2024-03-06 06:42:33.000000 mg-pso-gui-0.1.9/mg_pso_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      117 2024-03-06 06:42:33.000000 mg-pso-gui-0.1.9/mg_pso_gui.egg-info/entry_points.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       76 2024-03-06 06:42:33.000000 mg-pso-gui-0.1.9/mg_pso_gui.egg-info/requires.txt
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        9 2024-03-06 06:42:33.000000 mg-pso-gui-0.1.9/mg_pso_gui.egg-info/top_level.txt
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.847771 mg-pso-gui-0.1.9/mgpsogui/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       42 2023-10-10 00:40:24.000000 mg-pso-gui-0.1.9/mgpsogui/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.850629 mg-pso-gui-0.1.9/mgpsogui/gui/
+-rwxr--r--   0 robertcordingly   (501) staff       (20)    25874 2024-03-06 06:33:23.000000 mg-pso-gui-0.1.9/mgpsogui/gui/HomePage.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    11712 2024-01-24 22:27:36.000000 mg-pso-gui-0.1.9/mgpsogui/gui/OptionManager.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.851516 mg-pso-gui-0.1.9/mgpsogui/gui/PlatformTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    10486 2024-02-14 07:13:08.000000 mg-pso-gui-0.1.9/mgpsogui/gui/PlatformTab/PlatformTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:36:09.000000 mg-pso-gui-0.1.9/mgpsogui/gui/PlatformTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.852229 mg-pso-gui-0.1.9/mgpsogui/gui/RunTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2850 2024-02-14 07:26:36.000000 mg-pso-gui-0.1.9/mgpsogui/gui/RunTab/RunTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 06:41:01.000000 mg-pso-gui-0.1.9/mgpsogui/gui/RunTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.857952 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2866 2024-02-14 07:40:24.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/BoundsEditorWindow.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    12268 2024-02-14 08:06:06.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/BoundsList.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2784 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/CalibrationParametersView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4092 2024-02-13 06:33:07.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/FunctionsList.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     7352 2023-10-18 05:17:22.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/ListParametersView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1881 2024-02-14 08:15:40.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/SetupTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2739 2024-02-13 05:33:08.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/StaticParameterView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     5531 2024-02-13 06:31:26.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/StepView.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-13 05:20:36.000000 mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.859222 mg-pso-gui-0.1.9/mgpsogui/gui/VisualizeTab/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3271 2024-02-28 21:07:31.000000 mg-pso-gui-0.1.9/mgpsogui/gui/VisualizeTab/VisualizeTab.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2024-02-14 03:49:32.000000 mg-pso-gui-0.1.9/mgpsogui/gui/VisualizeTab/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:33:58.000000 mg-pso-gui-0.1.9/mgpsogui/gui/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.869677 mg-pso-gui-0.1.9/mgpsogui/gui/images/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)   433752 2024-02-27 04:32:36.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/IGOW 4 Logo.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2989 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/collapse.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2654 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/down.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2922 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/expand.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2790 2024-02-14 06:41:01.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/play.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4657 2024-02-14 06:39:03.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/refresh.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    31242 2024-02-14 08:26:13.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/refresh_hd.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2153 2024-02-14 06:41:07.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/stop.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2958 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/trash.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2457 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/gui/images/up.png
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      148 2023-10-04 08:06:40.000000 mg-pso-gui-0.1.9/mgpsogui/mgpsogui.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     4713 2023-11-08 23:03:41.000000 mg-pso-gui-0.1.9/mgpsogui/start.yaml
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.871312 mg-pso-gui-0.1.9/mgpsogui/util/
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.872044 mg-pso-gui-0.1.9/mgpsogui/util/CTkToolTip/
+-rw-rw-r--   0 robertcordingly   (501) staff       (20)      225 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/util/CTkToolTip/__init__.py
+-rw-rw-r--   0 robertcordingly   (501) staff       (20)     6329 2023-09-20 19:36:20.000000 mg-pso-gui-0.1.9/mgpsogui/util/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     7851 2024-02-28 07:09:24.000000 mg-pso-gui-0.1.9/mgpsogui/util/GraphGenerator.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     6328 2024-03-06 06:26:18.000000 mg-pso-gui-0.1.9/mgpsogui/util/PSORunner.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)        0 2023-10-03 21:32:18.000000 mg-pso-gui-0.1.9/mgpsogui/util/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.872587 mg-pso-gui-0.1.9/mgpsogui/util/recosu/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      236 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.874160 mg-pso-gui-0.1.9/mgpsogui/util/recosu/pso/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      247 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/pso/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     2611 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/pso/csip_access.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)    13058 2024-03-06 06:42:27.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/pso/pso.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.875592 mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)      196 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/__init__.py
+drwxr-xr-x   0 robertcordingly   (501) staff       (20)        0 2024-03-06 06:42:33.876493 mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/plot/
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       71 2024-03-06 06:18:26.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/plot/__init__.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3779 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/plot/cost_steps.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3023 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/trace_writer.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     3951 2024-03-06 06:18:27.000000 mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/utils.py
+-rw-r--r--   0 robertcordingly   (501) staff       (20)       38 2024-03-06 06:42:33.877868 mg-pso-gui-0.1.9/setup.cfg
+-rw-r--r--   0 robertcordingly   (501) staff       (20)     1525 2024-03-06 06:42:29.000000 mg-pso-gui-0.1.9/setup.py
```

### Comparing `mg-pso-gui-0.1.8/PKG-INFO` & `mg-pso-gui-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mg-pso-gui
-Version: 0.1.8
+Version: 0.1.9
 Summary: GUI for MG-PSO
 Author: Robert Cordingly
 Author-email: <rcording@uw.ed>
 Keywords: python,muti-group,pso,particle,swarm,optimization,gui
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mg-pso-gui-0.1.8/mg_pso_gui.egg-info/PKG-INFO` & `mg-pso-gui-0.1.9/mg_pso_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mg-pso-gui
-Version: 0.1.8
+Version: 0.1.9
 Summary: GUI for MG-PSO
 Author: Robert Cordingly
 Author-email: <rcording@uw.ed>
 Keywords: python,muti-group,pso,particle,swarm,optimization,gui
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mg-pso-gui-0.1.8/mg_pso_gui.egg-info/SOURCES.txt` & `mg-pso-gui-0.1.9/mg_pso_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/HomePage.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/HomePage.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/OptionManager.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/OptionManager.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/PlatformTab/PlatformTab.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/PlatformTab/PlatformTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/RunTab/RunTab.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/RunTab/RunTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/BoundsEditorWindow.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/BoundsEditorWindow.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/BoundsList.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/BoundsList.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/CalibrationParametersView.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/CalibrationParametersView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/FunctionsList.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/FunctionsList.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/ListParametersView.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/ListParametersView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/SetupTab.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/SetupTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/StaticParameterView.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/StaticParameterView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/SetupTab/StepView.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/SetupTab/StepView.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/VisualizeTab/VisualizeTab.py` & `mg-pso-gui-0.1.9/mgpsogui/gui/VisualizeTab/VisualizeTab.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/images/IGOW 4 Logo.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/IGOW 4 Logo.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/images/collapse.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/collapse.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/images/down.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/down.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/images/expand.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/expand.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/images/play.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/play.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/images/refresh.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/refresh.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/images/refresh_hd.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/refresh_hd.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/images/stop.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/stop.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/images/trash.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/trash.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/gui/images/up.png` & `mg-pso-gui-0.1.9/mgpsogui/gui/images/up.png`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/start.yaml` & `mg-pso-gui-0.1.9/mgpsogui/start.yaml`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/util/CTkToolTip/ctk_tooltip.py` & `mg-pso-gui-0.1.9/mgpsogui/util/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/util/GraphGenerator.py` & `mg-pso-gui-0.1.9/mgpsogui/util/GraphGenerator.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/util/PSORunner.py` & `mg-pso-gui-0.1.9/mgpsogui/util/PSORunner.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/util/recosu/pso/csip_access.py` & `mg-pso-gui-0.1.9/mgpsogui/util/recosu/pso/csip_access.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/util/recosu/pso/pso.py` & `mg-pso-gui-0.1.9/mgpsogui/util/recosu/pso/pso.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,19 +74,30 @@
     # assign the mean value to all failed runs.
     mean = np.nanmean(cost)
     cost[nan_idx[0]] = mean
 
     print(flush=True)
     return cost
 
-
+# Simulator
 def global_best(steps: Dict, rounds: Tuple, args: Dict, n_particles: int, iters: int, options: Dict,
                 oh_strategy: Dict = None, n_threads: int = 4, rtol: float = 0.001, ftol: float = -np.inf,
                 ftol_iter: int = 1, full_trace: List = None, rtol_iter: int = 1,
                 conf: Dict = None, metainfo: Dict = None, cost_target: float = -np.inf, result_queue: Queue = None) -> Tuple:
+    import time
+    while True:
+        print("WOW", flush=True)
+        if result_queue is not None:
+            result_queue.put('WOW')
+        time.sleep(1)
+
+def global_best_real(steps: Dict, rounds: Tuple, args: Dict, n_particles: int, iters: int, options: Dict,
+                oh_strategy: Dict = None, n_threads: int = 4, rtol: float = 0.001, ftol: float = -np.inf,
+                ftol_iter: int = 1, full_trace: List = None, rtol_iter: int = 1,
+                conf: Dict = None, metainfo: Dict = None, cost_target: float = -np.inf, result_queue: Queue = None) -> Tuple:
     """Performs a stepwise particle swarm optimization PSO using a global best approach.
 
         Parameters
         ----------
         steps : Dict
             step definitions
         rounds : tuple
```

### Comparing `mg-pso-gui-0.1.8/mgpsogui/util/recosu/utils/plot/cost_steps.py` & `mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/plot/cost_steps.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/util/recosu/utils/trace_writer.py` & `mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/trace_writer.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/mgpsogui/util/recosu/utils/utils.py` & `mg-pso-gui-0.1.9/mgpsogui/util/recosu/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mg-pso-gui-0.1.8/setup.py` & `mg-pso-gui-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 DESCRIPTION = 'GUI for MG-PSO'
 LONG_DESCRIPTION = open('../README.md').read()
 
 # Setting up
 setup(
     name="mg-pso-gui",
     version=VERSION,
```

