# Comparing `tmp/misleep-0.1.0b0.tar.gz` & `tmp/misleep-0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misleep-0.1.0b0.tar", last modified: Tue Apr  2 10:37:37 2024, max compression
+gzip compressed data, was "misleep-0.1.1b0.tar", last modified: Wed Apr  3 09:04:05 2024, max compression
```

## Comparing `misleep-0.1.0b0.tar` & `misleep-0.1.1b0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:37.924588 misleep-0.1.0b0/
--rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.1.0b0/LICENSE
--rw-rw-rw-   0        0        0     1110 2024-04-02 10:37:37.923588 misleep-0.1.0b0/PKG-INFO
--rw-rw-rw-   0        0        0      121 2024-03-05 06:34:51.000000 misleep-0.1.0b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:37.902587 misleep-0.1.0b0/misleep/
--rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.1.0b0/misleep/__init__.py
--rw-rw-rw-   0        0        0      167 2024-04-02 10:19:29.000000 misleep-0.1.0b0/misleep/__main__.py
--rw-rw-rw-   0        0        0      515 2024-04-02 09:20:21.000000 misleep-0.1.0b0/misleep/config.ini
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:37.908587 misleep-0.1.0b0/misleep/gui/
--rw-rw-rw-   0        0        0      340 2024-04-02 09:30:59.000000 misleep-0.1.0b0/misleep/gui/__init__.py
--rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.1.0b0/misleep/gui/about.py
--rw-rw-rw-   0        0        0     4633 2024-04-02 07:00:24.000000 misleep-0.1.0b0/misleep/gui/label_dialog.py
--rw-rw-rw-   0        0        0    50157 2024-04-02 10:37:33.000000 misleep-0.1.0b0/misleep/gui/main_window.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:37.911587 misleep-0.1.0b0/misleep/gui/resources/
--rw-rw-rw-   0        0        0       47 2024-04-02 09:32:49.000000 misleep-0.1.0b0/misleep/gui/resources/__init__.py
--rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.1.0b0/misleep/gui/resources/entire_logo.png
--rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.1.0b0/misleep/gui/resources/logo.png
--rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.1.0b0/misleep/gui/resources/misleep.py
--rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.1.0b0/misleep/gui/resources/misleep.qrc
--rw-rw-rw-   0        0        0      473 2024-04-02 10:20:22.000000 misleep-0.1.0b0/misleep/gui/show.py
--rw-rw-rw-   0        0        0     4092 2024-04-01 13:45:14.000000 misleep-0.1.0b0/misleep/gui/spec_window.py
--rw-rw-rw-   0        0        0     2681 2024-04-02 08:45:40.000000 misleep-0.1.0b0/misleep/gui/thread.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:37.914587 misleep-0.1.0b0/misleep/gui/uis/
--rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.1.0b0/misleep/gui/uis/__init__.py
--rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.1.0b0/misleep/gui/uis/about_ui.py
--rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.1.0b0/misleep/gui/uis/label_dialog_ui.py
--rw-rw-rw-   0        0        0    24099 2024-04-01 05:02:43.000000 misleep-0.1.0b0/misleep/gui/uis/main_window_ui.py
--rw-rw-rw-   0        0        0     4468 2024-03-31 07:18:43.000000 misleep-0.1.0b0/misleep/gui/uis/spec_window_ui.py
--rw-rw-rw-   0        0        0      757 2024-04-02 06:53:09.000000 misleep-0.1.0b0/misleep/gui/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:37.915587 misleep-0.1.0b0/misleep/io/
--rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.1.0b0/misleep/io/__init__.py
--rw-rw-rw-   0        0        0     1551 2024-03-13 06:17:48.000000 misleep-0.1.0b0/misleep/io/annotation_io.py
--rw-rw-rw-   0        0        0    15021 2024-04-02 09:18:06.000000 misleep-0.1.0b0/misleep/io/base.py
--rw-rw-rw-   0        0        0     3366 2024-04-02 09:20:10.000000 misleep-0.1.0b0/misleep/io/signal_io.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:37.916587 misleep-0.1.0b0/misleep/preprocessing/
--rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.1.0b0/misleep/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.1.0b0/misleep/preprocessing/channel.py
--rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.1.0b0/misleep/preprocessing/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:37.919587 misleep-0.1.0b0/misleep/utils/
--rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.1.0b0/misleep/utils/__init__.py
--rw-rw-rw-   0        0        0     1692 2024-04-02 07:16:03.000000 misleep-0.1.0b0/misleep/utils/annotation.py
--rw-rw-rw-   0        0        0     2050 2024-03-13 06:17:48.000000 misleep-0.1.0b0/misleep/utils/only4gui.py
--rw-rw-rw-   0        0        0        0 2024-04-01 05:02:43.000000 misleep-0.1.0b0/misleep/utils/others.py
--rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.1.0b0/misleep/utils/signals.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:37.920587 misleep-0.1.0b0/misleep/viz/
--rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.1.0b0/misleep/viz/__init__.py
--rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.1.0b0/misleep/viz/hypnogram.py
--rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.1.0b0/misleep/viz/signals.py
--rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.1.0b0/misleep/viz/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:37.904587 misleep-0.1.0b0/misleep.egg-info/
--rw-rw-rw-   0        0        0     1110 2024-04-02 10:37:37.000000 misleep-0.1.0b0/misleep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1317 2024-04-02 10:37:37.000000 misleep-0.1.0b0/misleep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 10:37:37.000000 misleep-0.1.0b0/misleep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-04-02 10:37:37.000000 misleep-0.1.0b0/misleep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-02 10:37:37.000000 misleep-0.1.0b0/misleep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 10:37:37.924588 misleep-0.1.0b0/setup.cfg
--rw-rw-rw-   0        0        0     2043 2024-04-02 10:34:01.000000 misleep-0.1.0b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:37.923588 misleep-0.1.0b0/test/
--rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.1.0b0/test/test_annotation_io.py
--rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.1.0b0/test/test_midata.py
--rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.1.0b0/test/test_show.py
--rw-rw-rw-   0        0        0     1376 2024-03-06 08:30:45.000000 misleep-0.1.0b0/test/test_signal_io.py
--rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.1.0b0/test/test_signals_viz.py
--rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.1.0b0/test/test_spectral_viz.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.724379 misleep-0.1.1b0/
+-rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.1.1b0/LICENSE
+-rw-rw-rw-   0        0        0     1132 2024-04-03 09:04:05.723214 misleep-0.1.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0      121 2024-03-05 06:34:51.000000 misleep-0.1.1b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.697214 misleep-0.1.1b0/misleep/
+-rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.1.1b0/misleep/__init__.py
+-rw-rw-rw-   0        0        0      167 2024-04-02 10:19:29.000000 misleep-0.1.1b0/misleep/__main__.py
+-rw-rw-rw-   0        0        0      510 2024-04-03 08:56:33.000000 misleep-0.1.1b0/misleep/config.ini
+drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.702214 misleep-0.1.1b0/misleep/gui/
+-rw-rw-rw-   0        0        0      340 2024-04-02 09:30:59.000000 misleep-0.1.1b0/misleep/gui/__init__.py
+-rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.1.1b0/misleep/gui/about.py
+-rw-rw-rw-   0        0        0     4633 2024-04-02 07:00:24.000000 misleep-0.1.1b0/misleep/gui/label_dialog.py
+-rw-rw-rw-   0        0        0    52166 2024-04-03 08:56:06.000000 misleep-0.1.1b0/misleep/gui/main_window.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.705213 misleep-0.1.1b0/misleep/gui/resources/
+-rw-rw-rw-   0        0        0       47 2024-04-02 09:32:49.000000 misleep-0.1.1b0/misleep/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/gui/resources/entire_logo.png
+-rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/gui/resources/logo.png
+-rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.1.1b0/misleep/gui/resources/misleep.py
+-rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/gui/resources/misleep.qrc
+-rw-rw-rw-   0        0        0      473 2024-04-02 10:20:22.000000 misleep-0.1.1b0/misleep/gui/show.py
+-rw-rw-rw-   0        0        0     4092 2024-04-01 13:45:14.000000 misleep-0.1.1b0/misleep/gui/spec_window.py
+-rw-rw-rw-   0        0        0     3177 2024-04-03 08:49:26.000000 misleep-0.1.1b0/misleep/gui/thread.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.709214 misleep-0.1.1b0/misleep/gui/uis/
+-rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/gui/uis/__init__.py
+-rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/gui/uis/about_ui.py
+-rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.1.1b0/misleep/gui/uis/label_dialog_ui.py
+-rw-rw-rw-   0        0        0    23842 2024-04-03 02:14:41.000000 misleep-0.1.1b0/misleep/gui/uis/main_window_ui.py
+-rw-rw-rw-   0        0        0     4468 2024-03-31 07:18:43.000000 misleep-0.1.1b0/misleep/gui/uis/spec_window_ui.py
+-rw-rw-rw-   0        0        0      757 2024-04-02 06:53:09.000000 misleep-0.1.1b0/misleep/gui/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.711214 misleep-0.1.1b0/misleep/io/
+-rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.1.1b0/misleep/io/__init__.py
+-rw-rw-rw-   0        0        0     1551 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/io/annotation_io.py
+-rw-rw-rw-   0        0        0    14995 2024-04-03 08:28:39.000000 misleep-0.1.1b0/misleep/io/base.py
+-rw-rw-rw-   0        0        0     5908 2024-04-03 09:01:34.000000 misleep-0.1.1b0/misleep/io/signal_io.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.713214 misleep-0.1.1b0/misleep/preprocessing/
+-rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.1.1b0/misleep/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.1.1b0/misleep/preprocessing/channel.py
+-rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.1.1b0/misleep/preprocessing/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.718213 misleep-0.1.1b0/misleep/utils/
+-rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.1.1b0/misleep/utils/__init__.py
+-rw-rw-rw-   0        0        0     1692 2024-04-02 07:16:03.000000 misleep-0.1.1b0/misleep/utils/annotation.py
+-rw-rw-rw-   0        0        0     2050 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/utils/only4gui.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 05:02:43.000000 misleep-0.1.1b0/misleep/utils/others.py
+-rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/utils/signals.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.719214 misleep-0.1.1b0/misleep/viz/
+-rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.1.1b0/misleep/viz/__init__.py
+-rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.1.1b0/misleep/viz/hypnogram.py
+-rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.1.1b0/misleep/viz/signals.py
+-rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.1.1b0/misleep/viz/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.699214 misleep-0.1.1b0/misleep.egg-info/
+-rw-rw-rw-   0        0        0     1132 2024-04-03 09:04:05.000000 misleep-0.1.1b0/misleep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1340 2024-04-03 09:04:05.000000 misleep-0.1.1b0/misleep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 09:04:05.000000 misleep-0.1.1b0/misleep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-04-03 09:04:05.000000 misleep-0.1.1b0/misleep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-03 09:04:05.000000 misleep-0.1.1b0/misleep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 09:04:05.724379 misleep-0.1.1b0/setup.cfg
+-rw-rw-rw-   0        0        0     2057 2024-04-03 09:04:01.000000 misleep-0.1.1b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:04:05.722214 misleep-0.1.1b0/test/
+-rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.1.1b0/test/test_annotation_io.py
+-rw-rw-rw-   0        0        0      143 2024-04-03 07:20:46.000000 misleep-0.1.1b0/test/test_loadmat73.py
+-rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.1.1b0/test/test_midata.py
+-rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.1.1b0/test/test_show.py
+-rw-rw-rw-   0        0        0     1376 2024-03-06 08:30:45.000000 misleep-0.1.1b0/test/test_signal_io.py
+-rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.1.1b0/test/test_signals_viz.py
+-rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.1.1b0/test/test_spectral_viz.py
```

### Comparing `misleep-0.1.0b0/LICENSE` & `misleep-0.1.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/PKG-INFO` & `misleep-0.1.1b0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.1.0b0
+Version: 0.1.1b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
@@ -21,14 +21,15 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: pyedflib
 Requires-Dist: hdf5storage
 Requires-Dist: pyqt5
+Requires-Dist: mat73
 
 # MiSleep
 MiSleep is for EEG/EMG signal processing and visualization
 
 ## Get start
 ```shell
 pip install misleep
```

### Comparing `misleep-0.1.0b0/misleep/gui/about.py` & `misleep-0.1.1b0/misleep/gui/about.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/gui/label_dialog.py` & `misleep-0.1.1b0/misleep/gui/label_dialog.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/gui/main_window.py` & `misleep-0.1.1b0/misleep/gui/main_window.py`

 * *Files 4% similar despite different names*

```diff
@@ -196,17 +196,52 @@
         self.nremSc.activated.connect(self.nrem_label)
         self.remSc = QShortcut(QKeySequence('2'), self)
         self.remSc.activated.connect(self.rem_label)
         self.wakeSc = QShortcut(QKeySequence('3'), self)
         self.wakeSc.activated.connect(self.wake_label)
         self.initSc = QShortcut(QKeySequence('4'), self)
         self.initSc.activated.connect(self.init_label)
+        self.labelSc = QShortcut(QKeySequence('a'), self)
+        self.labelSc.activated.connect(self.append_start_end)
 
         # save labels
         self.SaveLabelBt.clicked.connect(self.save_anno)
+        self.saveSc = QShortcut(QKeySequence('CTRL+s'), self)
+        self.saveSc.activated.connect(self.save_anno)
+
+        self.change_Bts_status(True)
+
+    def change_Bts_status(self, status=True):
+        """Change some buttons' status"""
+        self.MetaDock.setDisabled(status)
+        self.AcTimeEdit.setDisabled(status)
+        self.DeleteChBt.setDisabled(status)
+        self.HideChBt.setDisabled(status)
+        self.ScalerDownBt.setDisabled(status)
+        self.ShiftDownBt.setDisabled(status)
+        self.ShowChBt.setDisabled(status)
+        self.ScalerUpBt.setDisabled(status)
+        self.ShiftUpBt.setDisabled(status)
+        self.FilterConfirmBt.setDisabled(status)
+        self.DefaultCh4SpecBt.setDisabled(status)
+        self.FilterTypeCombo.setDisabled(status)
+        self.PlotSpecBt.setDisabled(status)
+        self.WakeBt.setDisabled(status)
+        self.REMBt.setDisabled(status)
+        self.InitBt.setDisabled(status)
+        self.LabelBt.setDisabled(status)
+        self.StartEndRadio.setDisabled(status)
+        self.SleepStateRadio.setDisabled(status)
+        self.SaveLabelBt.setDisabled(status)
+        self.MarkerRadio.setDisabled(status)
+        self.NREMBt.setDisabled(status)
+        self.DateTimeEdit.setDisabled(status)
+        self.ShowRangeCombo.setDisabled(status)
+        self.SaveBar.setDisabled(status)
+        self.AboutBar.setDisabled(status)
 
     def load_data(self):
         """Triggered by actionLoad_Data, get MiData"""
         data_path, _ = QFileDialog.getOpenFileName(
             self,
             "Select data file",
             f"{self.config['gui']['openpath']}",
@@ -222,27 +257,29 @@
                 QMessageBox.about(
                     self,
                     "Error",
                     r"Data file invalid, check "
                     r"<a href='https://github.com/BryanWang0702/MiSleep'>MiSleep</a> for detail.",
                 )
                 self.data_path = ""
+                self.change_Bts_status(True)
                 return
 
         if self.data_path.endswith((".edf", ".EDF")):
             try:
                 self.midata = load_edf(data_path=self.data_path)
             except Exception:
                 QMessageBox.about(
                     self,
                     "Error",
                     r"Data file invalid, check "
                     r"<a href='https://github.com/BryanWang0702/MiSleep'>MiSleep</a> for detail.",
                 )
                 self.data_path = ""
+                self.change_Bts_status(True)
                 return
 
         # Save config
         self.save_config({'openpath': self.data_path})
 
         # Set meta info
         self.DataPathEdit.setText(self.data_path)
@@ -278,24 +315,26 @@
                     else:
                         QMessageBox.about(
                             self,
                             "Error",
                             "To create a new annotation file, load a data file first.",
                         )
                         self.anno_path = ""
+                        self.change_Bts_status(True)
                         return
 
                 if e.args[0] == "Invalid":
                     QMessageBox.about(
                         self,
                         "Error",
                         r"Annotation file invalid, check "
                         r"<a href='https://github.com/BryanWang0702/MiSleep'>MiSleep</a> for detail.",
                     )
-                    self.data_path = ""
+                    self.anno_path = ""
+                    self.change_Bts_status(True)
                     return
                 
         # Save config
         self.save_config({'openpath': self.anno_path})
 
         # Set meta info
         self.AnnoPathEdit.setText(self.anno_path)
@@ -313,25 +352,31 @@
             return
 
         self.show_idx = list(range(self.midata.n_channels))
         self.y_lims = [max(each[:1000]) for each in self.midata.signals]
         self.y_lims = [1e-3 if each == 0.0 else each for each in self.y_lims]
         self.y_shift = [0 for _ in range(self.midata.n_channels)]
 
+        if abs(self.midata.duration - self.mianno.anno_length) >= 600:
+            QMessageBox.about(
+                self, "Error", r"Data and annotation do not match!"
+            )
+            return
         self.total_seconds = self.midata.duration if self.midata.duration < self.mianno.anno_length else self.mianno.anno_length
         self.reset_sec_limit()
 
         self.hypo_ax = self.hypo_figure.subplots(nrows=1, ncols=1)
 
         # Set canvas for plot area
         self.SignalArea.setWidget(self.signal_canvas)
         self.HypnoArea.setWidget(self.hypo_canvas)
 
         self.redraw_all(second=0)
         self.clear_refresh(clf=False)
+        self.change_Bts_status(False)
 
     def reset_sec_limit(self):
         """When show duration changes, change the limitation of 
         ScrollerBar, DateTimeEdit, SecondSpin
         """
         self.ScrollerBar.setRange(0, self.total_seconds-self.show_duration)
         self.SecondSpin.setRange(0, self.total_seconds-self.show_duration)
@@ -622,16 +667,16 @@
                         self.signal_ax[idx + 1].axvline(
                         int((each[0] - self.current_sec) * self.midata.sf[show_]),
                         color="Red",
                         alpha=1,
                     ))
                 self.signal_marker_axvline.append(
                     self.signal_ax[1].text(
-                    x=int((each[0] - self.current_sec) * self.midata.sf[show_]),
-                    y=self.y_lims[self.show_idx[0]] + self.y_shift[self.show_idx[1]],
+                    x=int((each[0] - self.current_sec) * self.midata.sf[self.show_idx[0]]),
+                    y=self.y_lims[self.show_idx[0]] + self.y_shift[self.show_idx[0]],
                     s=each[1],
                     verticalalignment="top",
                     color="Red",
                 ))
         
         if flush:
             self.signal_figure.canvas.draw()
@@ -645,31 +690,31 @@
                 for idx, show_ in enumerate(self.show_idx):
                     self.signal_ax[idx + 1].axvline(
                         int((each[0] - self.current_sec) * self.midata.sf[show_]),
                         color="blue",
                         alpha=1,
                     )
                 self.signal_ax[1].text(
-                    x=int((each[0] - self.current_sec) * self.midata.sf[show_]),
-                    y=self.y_lims[self.show_idx[0]] + self.y_shift[self.show_idx[1]],
+                    x=int((each[0] - self.current_sec) * self.midata.sf[self.show_idx[0]]),
+                    y=self.y_lims[self.show_idx[0]] + self.y_shift[self.show_idx[0]],
                     s=each[2]+'-S',
                     verticalalignment="top",
                     color="blue",
                 )
 
             if self.current_sec <= each[1] <= self.current_sec + self.show_duration:
                 for idx, show_ in enumerate(self.show_idx):
                     self.signal_ax[idx + 1].axvline(
                         int((each[1] - self.current_sec) * self.midata.sf[show_]),
                         color="blue",
                         alpha=1,
                     )
                 self.signal_ax[1].text(
-                    x=int((each[1] - self.current_sec) * self.midata.sf[show_]),
-                    y=self.y_lims[self.show_idx[0]] + self.y_shift[self.show_idx[1]],
+                    x=int((each[1] - self.current_sec) * self.midata.sf[self.show_idx[0]]),
+                    y=self.y_lims[self.show_idx[0]] + self.y_shift[self.show_idx[0]],
                     s=each[2]+'-E',
                     verticalalignment="top",
                     horizontalalignment='right',
                     color="blue",
                 )
 
         if flush:
@@ -1215,15 +1260,15 @@
             self.load_anno()
         if signal.text() == "Show":
             self.check_show()
 
     def save_bar_dispatcher(self, signal):
         """Triggered by SaveBar action, save data, save annotation"""
         if signal.text() == "Save Data":
-            self.save_data()
+            pass
         if signal.text() == "Save Annotation":
             self.save_anno()
 
     def save_anno(self):
         """Save annotation into file"""
         save_thread = SaveThread(file=[self.mianno, self.midata], 
                                  file_path=self.anno_path)
```

### Comparing `misleep-0.1.0b0/misleep/gui/resources/entire_logo.png` & `misleep-0.1.1b0/misleep/gui/resources/entire_logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/gui/resources/logo.png` & `misleep-0.1.1b0/misleep/gui/resources/logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/gui/resources/misleep.py` & `misleep-0.1.1b0/misleep/gui/resources/misleep.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/gui/spec_window.py` & `misleep-0.1.1b0/misleep/gui/spec_window.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/gui/thread.py` & `misleep-0.1.1b0/misleep/gui/thread.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from PyQt5.QtCore import QObject, QThread
 from misleep.gui.utils import second2time
 from misleep.utils.annotation import lst2group
+from misleep.io.signal_io import load_mat
 import datetime
 
 class SaveThread(QThread):
 
     def __init__(self, parent=None, file=None, file_path=None):
         """Save file to file path
 
@@ -65,7 +66,26 @@
             "==========Sleep stage==========", '\n'.join(sleep_state)
         ]
 
         with open(self.file_path, 'w') as f:
             f.write('\n'.join(annos))
         return True
 
+class LoadThread(QThread):
+
+    def __init__(self, parent=None, file_path=None):
+        """Load data
+
+        Parameters
+        ----------
+        parent : optional
+        file_path : str, optional
+            File path to load 
+        """
+        super().__init__(parent)
+        self.file_path = file_path
+
+    def load_mat_data(self):
+        """Load data from a.mat file"""
+        return load_mat(data_path=self.file_path)
+
+
```

### Comparing `misleep-0.1.0b0/misleep/gui/uis/about_ui.py` & `misleep-0.1.1b0/misleep/gui/uis/about_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/gui/uis/label_dialog_ui.py` & `misleep-0.1.1b0/misleep/gui/uis/label_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/gui/uis/main_window_ui.py` & `misleep-0.1.1b0/misleep/gui/uis/main_window_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         self.ScrollerBar.setTracking(False)
         self.ScrollerBar.setOrientation(QtCore.Qt.Horizontal)
         self.ScrollerBar.setObjectName("ScrollerBar")
         self.gridLayout_3.addWidget(self.ScrollerBar, 1, 0, 1, 1)
         MiSleep.setCentralWidget(self.centralwidget)
         self.MetaDock = QtWidgets.QDockWidget(MiSleep)
         self.MetaDock.setMinimumSize(QtCore.QSize(264, 112))
-        self.MetaDock.setMaximumSize(QtCore.QSize(540, 400))
         self.MetaDock.setFeatures(QtWidgets.QDockWidget.DockWidgetFloatable|QtWidgets.QDockWidget.DockWidgetMovable)
         self.MetaDock.setObjectName("MetaDock")
         self.dockWidgetContents_3 = QtWidgets.QWidget()
         self.dockWidgetContents_3.setObjectName("dockWidgetContents_3")
         self.formLayout = QtWidgets.QFormLayout(self.dockWidgetContents_3)
         self.formLayout.setObjectName("formLayout")
         self.label_4 = QtWidgets.QLabel(self.dockWidgetContents_3)
@@ -94,15 +93,14 @@
         self.ChannelDock = QtWidgets.QDockWidget(MiSleep)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Ignored, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.ChannelDock.sizePolicy().hasHeightForWidth())
         self.ChannelDock.setSizePolicy(sizePolicy)
         self.ChannelDock.setMinimumSize(QtCore.QSize(315, 450))
-        self.ChannelDock.setMaximumSize(QtCore.QSize(540, 600))
         self.ChannelDock.setLayoutDirection(QtCore.Qt.LeftToRight)
         self.ChannelDock.setFeatures(QtWidgets.QDockWidget.DockWidgetFloatable|QtWidgets.QDockWidget.DockWidgetMovable)
         self.ChannelDock.setObjectName("ChannelDock")
         self.dockWidgetContents_4 = QtWidgets.QWidget()
         self.dockWidgetContents_4.setObjectName("dockWidgetContents_4")
         self.gridLayout = QtWidgets.QGridLayout(self.dockWidgetContents_4)
         self.gridLayout.setObjectName("gridLayout")
@@ -198,15 +196,14 @@
         self.PlotSpecBt = QtWidgets.QPushButton(self.dockWidgetContents_4)
         self.PlotSpecBt.setObjectName("PlotSpecBt")
         self.gridLayout.addWidget(self.PlotSpecBt, 11, 0, 1, 3)
         self.ChannelDock.setWidget(self.dockWidgetContents_4)
         MiSleep.addDockWidget(QtCore.Qt.DockWidgetArea(2), self.ChannelDock)
         self.AnnotationDock = QtWidgets.QDockWidget(MiSleep)
         self.AnnotationDock.setMinimumSize(QtCore.QSize(302, 200))
-        self.AnnotationDock.setMaximumSize(QtCore.QSize(540, 200))
         self.AnnotationDock.setFeatures(QtWidgets.QDockWidget.DockWidgetFloatable|QtWidgets.QDockWidget.DockWidgetMovable)
         self.AnnotationDock.setObjectName("AnnotationDock")
         self.dockWidgetContents_5 = QtWidgets.QWidget()
         self.dockWidgetContents_5.setObjectName("dockWidgetContents_5")
         self.gridLayout_2 = QtWidgets.QGridLayout(self.dockWidgetContents_5)
         self.gridLayout_2.setObjectName("gridLayout_2")
         self.WakeBt = QtWidgets.QPushButton(self.dockWidgetContents_5)
@@ -246,15 +243,14 @@
         self.line_4.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_4.setObjectName("line_4")
         self.gridLayout_2.addWidget(self.line_4, 1, 1, 1, 1)
         self.AnnotationDock.setWidget(self.dockWidgetContents_5)
         MiSleep.addDockWidget(QtCore.Qt.DockWidgetArea(2), self.AnnotationDock)
         self.TimeDock = QtWidgets.QDockWidget(MiSleep)
         self.TimeDock.setMinimumSize(QtCore.QSize(167, 148))
-        self.TimeDock.setMaximumSize(QtCore.QSize(540, 200))
         self.TimeDock.setAcceptDrops(False)
         self.TimeDock.setAutoFillBackground(True)
         self.TimeDock.setFeatures(QtWidgets.QDockWidget.DockWidgetFloatable|QtWidgets.QDockWidget.DockWidgetMovable)
         self.TimeDock.setAllowedAreas(QtCore.Qt.AllDockWidgetAreas)
         self.TimeDock.setObjectName("TimeDock")
         self.dockWidgetContents_7 = QtWidgets.QWidget()
         self.dockWidgetContents_7.setObjectName("dockWidgetContents_7")
```

### Comparing `misleep-0.1.0b0/misleep/gui/uis/spec_window_ui.py` & `misleep-0.1.1b0/misleep/gui/uis/spec_window_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/gui/utils.py` & `misleep-0.1.1b0/misleep/gui/utils.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/io/annotation_io.py` & `misleep-0.1.1b0/misleep/io/annotation_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/io/base.py` & `misleep-0.1.1b0/misleep/io/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,19 +77,19 @@
             if each in temp_channel:
                 temp_channel.append(f"{each}_1")
             else:
                 temp_channel.append(each)
         channels = temp_channel
 
         # Verify the duration of each signal channel, and modify to a same integer duration in second
-        temp_duration = set([math.floor(len(signals[idx]) / each) for idx, each in enumerate(sf)])
-        if len(temp_duration) != 1:
-            raise ValueError(f"The duration of all signal channels are different.")
+        temp_duration = [math.floor(len(signals[idx]) / each) for idx, each in enumerate(sf)]
+        # Use the minimum duration for data duration
+        self._duration = min(temp_duration)
 
-        self._duration = list(temp_duration)[0]
+        # self._duration = list(temp_duration)[0]
         self._signals = [signals[idx][:int(self._duration * each)] for idx, each in enumerate(sf)]
         self._channels = channels
         self._n_channels = len(self._channels)
         self._sf = sf
         self._time = time
 
     def differential(self, chan1=None, chan2=None):
```

### Comparing `misleep-0.1.0b0/misleep/preprocessing/spectral.py` & `misleep-0.1.1b0/misleep/preprocessing/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/utils/annotation.py` & `misleep-0.1.1b0/misleep/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/utils/only4gui.py` & `misleep-0.1.1b0/misleep/utils/only4gui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/utils/signals.py` & `misleep-0.1.1b0/misleep/utils/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/viz/hypnogram.py` & `misleep-0.1.1b0/misleep/viz/hypnogram.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/viz/signals.py` & `misleep-0.1.1b0/misleep/viz/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep/viz/spectral.py` & `misleep-0.1.1b0/misleep/viz/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/misleep.egg-info/PKG-INFO` & `misleep-0.1.1b0/misleep.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.1.0b0
+Version: 0.1.1b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
@@ -21,14 +21,15 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: pyedflib
 Requires-Dist: hdf5storage
 Requires-Dist: pyqt5
+Requires-Dist: mat73
 
 # MiSleep
 MiSleep is for EEG/EMG signal processing and visualization
 
 ## Get start
 ```shell
 pip install misleep
```

### Comparing `misleep-0.1.0b0/misleep.egg-info/SOURCES.txt` & `misleep-0.1.1b0/misleep.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -40,12 +40,13 @@
 misleep/utils/others.py
 misleep/utils/signals.py
 misleep/viz/__init__.py
 misleep/viz/hypnogram.py
 misleep/viz/signals.py
 misleep/viz/spectral.py
 test/test_annotation_io.py
+test/test_loadmat73.py
 test/test_midata.py
 test/test_show.py
 test/test_signal_io.py
 test/test_signals_viz.py
 test/test_spectral_viz.py
```

### Comparing `misleep-0.1.0b0/setup.py` & `misleep-0.1.1b0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 
 DISTNAME = "misleep"
 MAINTAINER = "Xueqiang Wang"
 MAINTAINER_EMAIL = "swang@gmail.com"
 URL = "https://github.com/BryanWang0702/MiSleep/"
 LICENSE = "BSD (3-clause)"
 DOWNLOAD_URL = "https://github.com/BryanWang0702/MiSleep/"
-VERSION = "0.1.0 Beta"
+VERSION = "0.1.1 Beta"
 
 INSTALL_REQUIRES = [
     "numpy>=1.18.1",
     "matplotlib",
     "scipy",
     "pyedflib",
     "hdf5storage",
-    "pyqt5"
+    "pyqt5",
+    "mat73"
 ]
 
 PACKAGES = [
     "misleep",
 ]
 
 CLASSIFIERS = [
```

### Comparing `misleep-0.1.0b0/test/test_midata.py` & `misleep-0.1.1b0/test/test_midata.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/test/test_signal_io.py` & `misleep-0.1.1b0/test/test_signal_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/test/test_signals_viz.py` & `misleep-0.1.1b0/test/test_signals_viz.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.0b0/test/test_spectral_viz.py` & `misleep-0.1.1b0/test/test_spectral_viz.py`

 * *Files identical despite different names*

