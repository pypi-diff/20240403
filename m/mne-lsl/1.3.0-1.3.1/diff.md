# Comparing `tmp/mne_lsl-1.3.0.tar.gz` & `tmp/mne_lsl-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mne_lsl-1.3.0.tar", last modified: Mon Mar 18 13:27:27 2024, max compression
+gzip compressed data, was "mne_lsl-1.3.1.tar", last modified: Wed Apr  3 12:53:24 2024, max compression
```

## Comparing `mne_lsl-1.3.0.tar` & `mne_lsl-1.3.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:27:27.665963 mne_lsl-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-03-18 13:27:27.665963 mne_lsl-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:27:27.649963 mne_lsl-1.3.0/mne_lsl/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/_typing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:27:27.649963 mne_lsl-1.3.0/mne_lsl/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/commands/mne_lsl_player.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/commands/mne_lsl_stream_viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/commands/sys_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:27:27.649963 mne_lsl-1.3.0/mne_lsl/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/datasets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/datasets/_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/datasets/_fetch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/datasets/sample-registry.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/datasets/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/datasets/sample.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/datasets/testing-registry.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/datasets/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/datasets/testing.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:27:27.653963 mne_lsl-1.3.0/mne_lsl/lsl/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/lsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/lsl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/lsl/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/lsl/_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/lsl/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/lsl/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/lsl/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    23651 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/lsl/load_liblsl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/lsl/load_liblsl.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    35798 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/lsl/stream_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    14643 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/lsl/stream_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18838 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/lsl/stream_inlet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/lsl/stream_inlet.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/lsl/stream_outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/lsl/stream_outlet.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:27:27.653963 mne_lsl-1.3.0/mne_lsl/player/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/player/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/player/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/player/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12689 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/player/_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15895 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/player/player_lsl.py
--rw-r--r--   0 runner    (1001) docker     (127)    10982 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/player/player_lsl.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:27:27.657963 mne_lsl-1.3.0/mne_lsl/stream/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/stream/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    44645 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    31935 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/stream/_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream/_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/stream/_filters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream/stream_lsl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/stream/stream_lsl.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:27:27.657963 mne_lsl-1.3.0/mne_lsl/stream_viewer/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream_viewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:27:27.657963 mne_lsl-1.3.0/mne_lsl/stream_viewer/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream_viewer/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream_viewer/backends/_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream_viewer/backends/pyqtgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:27:27.657963 mne_lsl-1.3.0/mne_lsl/stream_viewer/control_gui/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream_viewer/control_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream_viewer/control_gui/_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream_viewer/control_gui/_ui_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream_viewer/control_gui/control_eeg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:27:27.657963 mne_lsl-1.3.0/mne_lsl/stream_viewer/control_gui/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream_viewer/control_gui/settings/settings_scope_eeg.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:27:27.657963 mne_lsl-1.3.0/mne_lsl/stream_viewer/scope/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream_viewer/scope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream_viewer/scope/_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream_viewer/scope/scope_eeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/stream_viewer/stream_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:27:27.661963 mne_lsl-1.3.0/mne_lsl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/utils/_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/utils/_checks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/utils/_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/utils/_docs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/utils/_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/utils/_fixes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/utils/_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/utils/_imports.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/utils/_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/utils/_path.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/utils/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/utils/_tests.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/utils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-03-18 13:26:12.000000 mne_lsl-1.3.0/mne_lsl/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/utils/logs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11770 2024-03-18 13:26:13.000000 mne_lsl-1.3.0/mne_lsl/utils/meas_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-03-18 13:27:24.000000 mne_lsl-1.3.0/mne_lsl/utils/meas_info.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 13:27:27.661963 mne_lsl-1.3.0/mne_lsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-03-18 13:27:27.000000 mne_lsl-1.3.0/mne_lsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-03-18 13:27:27.000000 mne_lsl-1.3.0/mne_lsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 13:27:27.000000 mne_lsl-1.3.0/mne_lsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-18 13:27:27.000000 mne_lsl-1.3.0/mne_lsl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-18 13:27:27.000000 mne_lsl-1.3.0/mne_lsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-18 13:27:27.000000 mne_lsl-1.3.0/mne_lsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-03-18 13:26:13.000000 mne_lsl-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 13:27:27.665963 mne_lsl-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:53:24.531739 mne_lsl-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-04-03 12:53:24.531739 mne_lsl-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:53:24.515739 mne_lsl-1.3.1/mne_lsl/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/_typing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:53:24.515739 mne_lsl-1.3.1/mne_lsl/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/commands/mne_lsl_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/commands/mne_lsl_stream_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/commands/sys_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:53:24.515739 mne_lsl-1.3.1/mne_lsl/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/datasets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/datasets/_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/datasets/_fetch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/datasets/sample-registry.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/datasets/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/datasets/sample.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/datasets/testing-registry.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/datasets/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/datasets/testing.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:53:24.519739 mne_lsl-1.3.1/mne_lsl/lsl/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/lsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/lsl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/lsl/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/lsl/_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/lsl/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/lsl/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/lsl/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/lsl/load_liblsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/lsl/load_liblsl.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    35495 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/lsl/stream_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14639 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/lsl/stream_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18851 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/lsl/stream_inlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/lsl/stream_inlet.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/lsl/stream_outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/lsl/stream_outlet.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:53:24.519739 mne_lsl-1.3.1/mne_lsl/player/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/player/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/player/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14303 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/player/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12727 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/player/_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15761 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/player/player_lsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/player/player_lsl.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:53:24.523739 mne_lsl-1.3.1/mne_lsl/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/stream/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    44485 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31973 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/stream/_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream/_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/stream/_filters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream/stream_lsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/stream/stream_lsl.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:53:24.523739 mne_lsl-1.3.1/mne_lsl/stream_viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream_viewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:53:24.523739 mne_lsl-1.3.1/mne_lsl/stream_viewer/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream_viewer/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream_viewer/backends/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream_viewer/backends/pyqtgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:53:24.523739 mne_lsl-1.3.1/mne_lsl/stream_viewer/control_gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream_viewer/control_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream_viewer/control_gui/_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream_viewer/control_gui/_ui_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream_viewer/control_gui/control_eeg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:53:24.523739 mne_lsl-1.3.1/mne_lsl/stream_viewer/control_gui/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream_viewer/control_gui/settings/settings_scope_eeg.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:53:24.523739 mne_lsl-1.3.1/mne_lsl/stream_viewer/scope/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream_viewer/scope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream_viewer/scope/_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream_viewer/scope/scope_eeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/stream_viewer/stream_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:53:24.527739 mne_lsl-1.3.1/mne_lsl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6910 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/utils/_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/utils/_checks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8487 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/utils/_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/utils/_docs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/utils/_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/utils/_fixes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/utils/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/utils/_imports.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/utils/_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/utils/_path.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/utils/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/utils/_tests.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/utils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/utils/logs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/mne_lsl/utils/meas_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-03 12:53:22.000000 mne_lsl-1.3.1/mne_lsl/utils/meas_info.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:53:24.527739 mne_lsl-1.3.1/mne_lsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-04-03 12:53:24.000000 mne_lsl-1.3.1/mne_lsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-03 12:53:24.000000 mne_lsl-1.3.1/mne_lsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:53:24.000000 mne_lsl-1.3.1/mne_lsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-03 12:53:24.000000 mne_lsl-1.3.1/mne_lsl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-03 12:53:24.000000 mne_lsl-1.3.1/mne_lsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 12:53:24.000000 mne_lsl-1.3.1/mne_lsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-04-03 12:51:57.000000 mne_lsl-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:53:24.531739 mne_lsl-1.3.1/setup.cfg
```

### Comparing `mne_lsl-1.3.0/LICENSE` & `mne_lsl-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/PKG-INFO` & `mne_lsl-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mne_lsl
-Version: 1.3.0
+Version: 1.3.1
 Summary: Real-time framework integrated with MNE-Python for online neuroscience research through LSL-compatible devices.
 Author-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 Maintainer-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 License: Copyright © 2023-2024, authors of MNE-LSL
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `mne_lsl-1.3.0/README.md` & `mne_lsl-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/commands/mne_lsl_player.py` & `mne_lsl-1.3.1/mne_lsl/commands/mne_lsl_player.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/commands/mne_lsl_stream_viewer.py` & `mne_lsl-1.3.1/mne_lsl/commands/mne_lsl_stream_viewer.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/datasets/_fetch.py` & `mne_lsl-1.3.1/mne_lsl/datasets/_fetch.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/datasets/_fetch.pyi` & `mne_lsl-1.3.1/mne_lsl/datasets/_fetch.pyi`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/datasets/sample.py` & `mne_lsl-1.3.1/mne_lsl/datasets/sample.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/datasets/sample.pyi` & `mne_lsl-1.3.1/mne_lsl/datasets/sample.pyi`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/datasets/testing.py` & `mne_lsl-1.3.1/mne_lsl/datasets/testing.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/datasets/testing.pyi` & `mne_lsl-1.3.1/mne_lsl/datasets/testing.pyi`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/lsl/_utils.py` & `mne_lsl-1.3.1/mne_lsl/lsl/_utils.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/lsl/_utils.pyi` & `mne_lsl-1.3.1/mne_lsl/lsl/_utils.pyi`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/lsl/constants.py` & `mne_lsl-1.3.1/mne_lsl/lsl/constants.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/lsl/functions.py` & `mne_lsl-1.3.1/mne_lsl/lsl/functions.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/lsl/functions.pyi` & `mne_lsl-1.3.1/mne_lsl/lsl/functions.pyi`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/lsl/load_liblsl.py` & `mne_lsl-1.3.1/mne_lsl/lsl/load_liblsl.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,22 @@
 import zipfile
 from ctypes import CDLL, c_char_p, c_double, c_long, c_void_p, sizeof
 from ctypes.util import find_library
 from importlib.resources import files
 from pathlib import Path
 from shutil import move, rmtree
 from typing import TYPE_CHECKING
-from warnings import warn
 
 import pooch
 import requests
 
 from .._version import __version__
 from ..utils._checks import ensure_path
 from ..utils._path import walk
-from ..utils.logs import logger
+from ..utils.logs import logger, warn
 
 if TYPE_CHECKING:
     from typing import Optional, Union
 
     from pooch import Pooch
 
 
@@ -148,16 +147,14 @@
         logger.debug("Loading previously downloaded liblsl '%s'.", libpath)
         libpath, version = _attempt_load_liblsl(libpath, issue_warning=False)
         if version is None:
             libpath = ensure_path(libpath, must_exist=False)
             warn(
                 f"The previously downloaded LIBLSL '{libpath.name}' in "
                 f"'{libpath.parent}' could not be loaded. It will be removed.",
-                RuntimeWarning,
-                stacklevel=2,
             )
             libpath.unlink(missing_ok=False)
             continue
         # we do not accept outdated versions from the mne-lsl folder and we will remove
         # outdated versions.
         # disable the generic version warning in favor of a detailed warning mentioning
         # the file deletion.
@@ -165,16 +162,14 @@
             return libpath
         libpath = ensure_path(libpath, must_exist=False)
         warn(
             f"The previously downloaded LIBLSL '{libpath.name}' in '{libpath.parent}' "
             f"is outdated. The version is {version // 100}.{version % 100} while the "
             "minimum version required by MNE-LSL is "
             f"{_VERSION_MIN // 100}.{_VERSION_MIN % 100}. It will be removed.",
-            RuntimeWarning,
-            stacklevel=2,
         )
         libpath.unlink(missing_ok=False)
     return None
 
 
 def _fetch_liblsl(
     *,
@@ -349,19 +344,15 @@
             lines = file.readlines()
         lines = [
             line.split("Depends:")[1].strip()
             for line in lines
             if line.startswith("Depends:")
         ]
         if len(lines) != 1:  # pragma: no cover
-            warn(
-                "Dependencies from debian liblsl package could not be parsed.",
-                RuntimeWarning,
-                stacklevel=2,
-            )
+            warn("Dependencies from debian liblsl package could not be parsed.")
         else:
             logger.info(
                 "Attempting to retrieve liblsl from the release page. It requires %s.",
                 lines[0],
             )
         # find and move the library
         for file in walk(uncompressed / "data"):
@@ -415,25 +406,19 @@
     """Check if the library path is valid."""
     assert isinstance(libpath, str)  # sanity-check
     libpath = ensure_path(libpath, must_exist=False)
     if libpath.suffix != _PLATFORM_SUFFIXES[_PLATFORM]:
         warn(
             f"The LIBLSL '{libpath}' ends with '{libpath.suffix}' which is "
             f"different from the expected extension '{_PLATFORM_SUFFIXES[_PLATFORM]}' "
-            f"for {_PLATFORM} based OS.",
-            RuntimeWarning,
-            stacklevel=2,
+            f"for {_PLATFORM} based OS."
         )
         return False
     if not libpath.exists():
-        warn(
-            f"The LIBLSL '{libpath}' does not exist.",
-            RuntimeWarning,
-            stacklevel=2,
-        )
+        warn(f"The LIBLSL '{libpath}' does not exist.")
         return False
     return True
 
 
 def _attempt_load_liblsl(
     libpath: Union[str, Path], *, issue_warning: bool = True
 ) -> tuple[str, Optional[int]]:
@@ -459,19 +444,15 @@
     try:
         lib = CDLL(libpath)
         version = lib.lsl_library_version()
         del lib
     except OSError:
         version = None
         if issue_warning:
-            warn(
-                f"The LIBLSL '{libpath}' can not be loaded.",
-                RuntimeWarning,
-                stacklevel=2,
-            )
+            warn(f"The LIBLSL '{libpath}' can not be loaded.")
     return libpath, version
 
 
 def _is_valid_version(
     libpath: str, version: int, *, issue_warning: bool = True
 ) -> bool:
     """Check if the version of the library is supported by MNE-LSL.
@@ -495,17 +476,15 @@
     assert isinstance(libpath, str)  # sanity-check
     assert isinstance(version, int)  # sanity-check
     if version < _VERSION_MIN:
         if issue_warning:
             warn(
                 f"The LIBLSL '{libpath}' is outdated. The version is "
                 f"{version // 100}.{version % 100} while the minimum version required "
-                f"by MNE-LSL is {_VERSION_MIN // 100}.{_VERSION_MIN % 100}.",
-                RuntimeWarning,
-                stacklevel=2,
+                f"by MNE-LSL is {_VERSION_MIN // 100}.{_VERSION_MIN % 100}."
             )
         return False
     return True
 
 
 def _set_types(lib: CDLL) -> CDLL:
     """Set the argument and return types for the different liblsl functions.
```

### Comparing `mne_lsl-1.3.0/mne_lsl/lsl/load_liblsl.pyi` & `mne_lsl-1.3.1/mne_lsl/lsl/load_liblsl.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from _typeshed import Incomplete
 from pooch import Pooch
 
 from .._version import __version__ as __version__
 from ..utils._checks import ensure_path as ensure_path
 from ..utils._path import walk as walk
 from ..utils.logs import logger as logger
+from ..utils.logs import warn as warn
 
 _LIB_FOLDER: Path
 _VERSION_MIN: int
 _VERSION_PROTOCOL: int
 _PLATFORM: str
 _PLATFORM_SUFFIXES: dict[str, str]
 _ERROR_MSG: str
```

### Comparing `mne_lsl-1.3.0/mne_lsl/lsl/stream_info.py` & `mne_lsl-1.3.1/mne_lsl/lsl/stream_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import TYPE_CHECKING
 
 import numpy as np
 from mne import Info, Projection
 from mne.utils import check_version
 
 from ..utils._checks import check_type, check_value, ensure_int
-from ..utils.logs import logger
+from ..utils.logs import warn
 from ..utils.meas_info import create_info
 from ._utils import XMLElement
 from .constants import fmt2idx, fmt2numpy, idx2fmt, numpy2fmt, string2fmt
 from .load_liblsl import lib
 
 if check_version("mne", "1.6"):
     from mne._fiff._digitization import DigPoint
@@ -368,17 +368,17 @@
             if range_cals is not None:
                 for k, range_cal in enumerate(range_cals):
                     if range_cal is not None:
                         try:
                             info["chs"][k]["range"] = 1.0
                             info["chs"][k]["cal"] = float(range_cal)
                         except ValueError:
-                            logger.warning(
-                                "Could not cast 'range_cal' factor %s to float.",
-                                range_cal,
+                            warn(
+                                f"Could not cast 'range_cal' factor {range_cal} to "
+                                "float.",
                             )
             for k, loc in enumerate(locs):
                 info["chs"][k]["loc"] = loc
 
         # filters
         filters = self.desc.child("filters")
         if not filters.empty() and self.sfreq != 0:
@@ -386,19 +386,17 @@
             lowpass = filters.child("lowpass").first_child().value()
             with info._unlock():
                 for name, value in zip(("highpass", "lowpass"), (highpass, lowpass)):
                     if len(value) != 0:
                         try:
                             info[name] = float(value)
                         except ValueError:
-                            logger.warning(
-                                "Could not cast '%s' %s to float.", name, value
-                            )
+                            warn(f"Could not cast '{name}' {value} to float.")
         elif not filters.empty() and self.sfreq == 0:
-            logger.warning(
+            warn(
                 "Node 'filters' found in the description of an irregularly sampled "
                 "stream. This is inconsistent and will be skipped."
             )
 
         projs = self._get_channel_projectors()
         dig = self._get_digitization()
         with info._unlock(update_redundant=True, check_after=True):
@@ -477,63 +475,59 @@
             else:
                 ch_infos.append(None)
             ch = ch.next_sibling()
 
         if all(ch_info is None for ch_info in ch_infos):
             return None
         if len(ch_infos) != self.n_channels:
-            logger.warning(
-                "The stream description contains %i elements for %i channels.",
-                len(ch_infos),
-                self.n_channels,
+            warn(
+                f"The stream description contains {len(ch_infos)} elements for "
+                f"{self.n_channels} channels."
             )
         return ch_infos
 
     def _get_channel_projectors(self) -> list[Projection]:
         """Get the SSP vectors in the XML tree."""
         projs = list()
         projectors = self.desc.child("projectors")
         projector = projectors.child("projector")
         while not projector.empty():
             desc = projector.child("desc").first_child().value()
             if len(desc) == 0:
-                logger.warning(
-                    "An SSP projector without description was found. Skipping."
-                )
+                warn("An SSP projector without description was found. Skipping.")
                 projector = projector.next_sibling()
                 continue
             kind = projector.child("kind").first_child().value()
             try:
                 kind = int(kind)
             except ValueError:
-                logger.warning("Could not cast the SSP kind %s to integer.", kind)
+                warn(f"Could not cast the SSP kind {kind} to integer.")
                 projector = projector.next_sibling()
                 continue
 
             ch_names = list()
             ch_datas = list()
             data = projector.child("data")
             ch = data.child("channel")
             while not ch.empty():
                 ch_name = ch.child("label").first_child().value()
                 if len(ch_name) == 0:
-                    logger.warning(
+                    warn(
                         "SSP projector has an empty-channel label. The channel will "
                         "be skipped."
                     )
                     ch.next_sibling()
                     continue
                 ch_data = ch.child("data").first_child().value()
                 try:
                     ch_data = float(ch_data)
                 except ValueError:
-                    logger.warning(
-                        "Could not cast the SSP value %s for channel %s to float.",
-                        ch_data,
-                        ch_name,
+                    warn(
+                        f"Could not cast the SSP value {ch_data} for channel {ch_name} "
+                        "to float.",
                     )
                     ch.next_sibling()
                     continue
                 ch_names.append(ch_name)
                 ch_datas.append(ch_data)
                 ch = ch.next_sibling()
 
@@ -569,26 +563,26 @@
                     "dig_ident",
                     _dig_cardinal_named,
                 )
             else:
                 try:
                     ident = int(ident)
                 except ValueError:
-                    logger.warning("Could not cast 'ident' %s to integer.", ident)
+                    warn(f"Could not cast 'ident' {ident} to integer.")
                     point = point.next_sibling()
                     continue
             loc = point.child("loc")
             r = [loc.child(pos).first_child().value() for pos in ("X", "Y", "Z")]
             if ident is None or any(len(elt) == 0 for elt in r):
                 point = point.next_sibling()
                 continue
             try:
                 r = np.array([float(elt) for elt in r], dtype=np.float32)
             except ValueError:
-                logger.warning("Could not cast dig point location %s to float.", r)
+                warn(f"Could not cast dig point location {r} to float.")
                 point = point.next_sibling()
                 continue
             dig_points.append(
                 DigPoint(kind=kind, ident=ident, r=r, coord_frame=FIFF.FIFFV_COORD_HEAD)
             )
             point = point.next_sibling()
         return dig_points
@@ -825,21 +819,19 @@
         if value is None:
             return None
         try:
             idx = int(value)
             value = mapping[idx]
             return value
         except ValueError:
-            logger.warning("Could not cast '%s' %s to integer.", name, value)
+            warn(f"Could not cast '{name}' {value} to integer.")
         except KeyError:
-            logger.warning(
-                "Could not convert '%s' %i to a known FIFF code: %s.",
-                name,
-                int(value),
-                tuple(mapping.keys()),
+            warn(
+                f"Could not convert '{name}' {int(value)} to a known FIFF "
+                "code: {tuple(mapping.keys())}.",
             )
         return None
 
 
 class StreamInfo(_BaseStreamInfo):
     """Base Stream information object, storing the declaration of a stream.
```

### Comparing `mne_lsl-1.3.0/mne_lsl/lsl/stream_info.pyi` & `mne_lsl-1.3.1/mne_lsl/lsl/stream_info.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from numpy.typing import DTypeLike as DTypeLike
 from numpy.typing import NDArray as NDArray
 
 from .._typing import ScalarIntType as ScalarIntType
 from ..utils._checks import check_type as check_type
 from ..utils._checks import check_value as check_value
 from ..utils._checks import ensure_int as ensure_int
-from ..utils.logs import logger as logger
+from ..utils.logs import warn as warn
 from ..utils.meas_info import create_info as create_info
 from ._utils import XMLElement as XMLElement
 from .constants import fmt2idx as fmt2idx
 from .constants import fmt2numpy as fmt2numpy
 from .constants import idx2fmt as idx2fmt
 from .constants import numpy2fmt as numpy2fmt
 from .constants import string2fmt as string2fmt
```

### Comparing `mne_lsl-1.3.0/mne_lsl/lsl/stream_inlet.py` & `mne_lsl-1.3.1/mne_lsl/lsl/stream_inlet.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from threading import Lock
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from ..utils._checks import check_type, check_value, ensure_int
 from ..utils._docs import copy_doc
-from ..utils.logs import logger
+from ..utils.logs import warn
 from ._utils import check_timeout, free_char_p_array_memory, handle_error
 from .constants import fmt2numpy, fmt2pull_chunk, fmt2pull_sample, post_processing_flags
 from .load_liblsl import lib
 from .stream_info import _BaseStreamInfo
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
@@ -147,22 +147,22 @@
         The inlet will automatically disconnect.
         """
         if self.__obj is None:
             return
         try:
             self.close_stream()
         except Exception as exc:
-            logger.warning("Error closing stream: %s", str(exc))
+            warn(f"Error closing stream: {str(exc)}")
         self._stream_is_open = False
         with self._lock:
             obj, self._obj = self._obj, None
             try:
                 lib.lsl_destroy_inlet(obj)
             except Exception as exc:
-                logger.warning("Error destroying inlet: %s", str(exc))
+                warn(f"Error destroying inlet: {str(exc)}")
 
     def open_stream(self, timeout: Optional[float] = None) -> None:
         """Subscribe to a data stream.
 
         All samples pushed in at the other end from this moment onwards will be queued
         and eventually be delivered in response to
         :meth:`~mne_lsl.lsl.StreamInlet.pull_sample` or
@@ -204,15 +204,15 @@
         .. warning::
 
             At the moment, ``liblsl`` is released in version 1.16. Closing and
             re-opening a stream does not work and new samples pushed to the outlet do
             not arrive at the inlet. c.f. this
             `github issue <https://github.com/sccn/liblsl/issues/180>`_.
         """
-        if not self._stream_is_open:
+        if hasattr(self, "_stream_is_open") and not self._stream_is_open:
             return
         with self._lock:
             lib.lsl_close_stream(self._obj)
         self._stream_is_open = False
 
     def time_correction(self, timeout: Optional[float] = None) -> float:
         """Retrieve an estimated time correction offset for the given stream.
```

### Comparing `mne_lsl-1.3.0/mne_lsl/lsl/stream_inlet.pyi` & `mne_lsl-1.3.1/mne_lsl/lsl/stream_inlet.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from numpy.typing import NDArray as NDArray
 
 from .._typing import ScalarType as ScalarType
 from ..utils._checks import check_type as check_type
 from ..utils._checks import check_value as check_value
 from ..utils._checks import ensure_int as ensure_int
 from ..utils._docs import copy_doc as copy_doc
-from ..utils.logs import logger as logger
+from ..utils.logs import warn as warn
 from ._utils import check_timeout as check_timeout
 from ._utils import free_char_p_array_memory as free_char_p_array_memory
 from ._utils import handle_error as handle_error
 from .constants import fmt2numpy as fmt2numpy
 from .constants import fmt2pull_chunk as fmt2pull_chunk
 from .constants import fmt2pull_sample as fmt2pull_sample
 from .constants import post_processing_flags as post_processing_flags
```

### Comparing `mne_lsl-1.3.0/mne_lsl/lsl/stream_outlet.py` & `mne_lsl-1.3.1/mne_lsl/lsl/stream_outlet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations  # c.f. PEP 563, PEP 649
 
 from ctypes import c_char_p, c_double, c_int, c_long, c_void_p
 from threading import Lock
 from typing import TYPE_CHECKING
-from warnings import warn
 
 import numpy as np
 
 from ..utils._checks import check_type, ensure_int
 from ..utils._docs import copy_doc
-from ..utils.logs import logger
+from ..utils.logs import warn
 from ._utils import check_timeout, handle_error
 from .constants import fmt2numpy, fmt2push_chunk, fmt2push_chunk_n, fmt2push_sample
 from .load_liblsl import lib
 from .stream_info import _BaseStreamInfo
 
 if TYPE_CHECKING:
     from typing import Optional, Union
@@ -101,15 +100,15 @@
         except AttributeError:  # in the process of deletion, __obj was already None
             return
         with self._lock:
             obj, self._obj = self._obj, None
             try:
                 lib.lsl_destroy_outlet(obj)
             except Exception as exc:
-                logger.warning("Error destroying outlet: %s", str(exc))
+                warn("Error destroying outlet: %s", str(exc))
 
     def push_sample(
         self,
         x: Union[list[str], NDArray[+ScalarType]],
         timestamp: float = 0.0,
         pushThrough: bool = True,
     ) -> None:
@@ -213,19 +212,15 @@
             x = x if x.dtype == npdtype else x.astype(npdtype)
             x = x if x.flags["C_CONTIGUOUS"] else np.ascontiguousarray(x)
             n_elements = x.size
             n_samples = x.shape[0]
             data_buffer = (self._dtype * n_elements).from_buffer(x)
 
         if n_samples == 1:
-            warn(
-                "A single sample is pushed. Consider using push_sample().",
-                RuntimeWarning,
-                stacklevel=2,
-            )
+            warn("A single sample is pushed. Consider using push_sample().")
 
         # convert timestamps to the corresponding ctype
         if timestamp is None:
             timestamp = 0
         if isinstance(timestamp, np.ndarray):
             if timestamp.ndim != 1 or timestamp.size != n_samples:
                 raise ValueError(
@@ -252,17 +247,15 @@
             timestamp_c = (c_double * timestamp.size)(*timestamp.astype(np.float64))
             liblsl_push_chunk_func = self._do_push_chunk_n
         elif isinstance(timestamp, (float, int)):
             if self.sfreq == 0.0 and n_samples != 1 and timestamp != 0:
                 warn(
                     "The stream is irregularly sampled and timestamp is a float and "
                     "will be applied to all samples. Consider using an array of "
-                    "timestamps to provide the individual timestamps for each sample.",
-                    RuntimeWarning,
-                    stacklevel=2,
+                    "timestamps to provide the individual timestamps for each sample."
                 )
             timestamp_c = c_double(timestamp)
             liblsl_push_chunk_func = self._do_push_chunk
         else:
             raise TypeError(
                 "The argument 'timestamps' must be a float, an array or None to use "
                 "the current time."
```

### Comparing `mne_lsl-1.3.0/mne_lsl/lsl/stream_outlet.pyi` & `mne_lsl-1.3.1/mne_lsl/lsl/stream_outlet.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from numpy.typing import NDArray as NDArray
 
 from .._typing import ScalarFloatType as ScalarFloatType
 from .._typing import ScalarType as ScalarType
 from ..utils._checks import check_type as check_type
 from ..utils._checks import ensure_int as ensure_int
 from ..utils._docs import copy_doc as copy_doc
-from ..utils.logs import logger as logger
+from ..utils.logs import warn as warn
 from ._utils import check_timeout as check_timeout
 from ._utils import handle_error as handle_error
 from .constants import fmt2numpy as fmt2numpy
 from .constants import fmt2push_chunk as fmt2push_chunk
 from .constants import fmt2push_chunk_n as fmt2push_chunk_n
 from .constants import fmt2push_sample as fmt2push_sample
 from .load_liblsl import lib as lib
```

### Comparing `mne_lsl-1.3.0/mne_lsl/player/_base.py` & `mne_lsl-1.3.1/mne_lsl/player/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations  # c.f. PEP 563, PEP 649
 
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import TYPE_CHECKING
-from warnings import warn
 
 import numpy as np
 from mne import rename_channels
 from mne.io import BaseRaw, read_raw
 from mne.utils import check_version
 
 if check_version("mne", "1.6"):
@@ -19,15 +18,15 @@
 else:
     from mne.io.meas_info import ContainsMixin
     from mne.io.pick import _picks_to_idx
     from mne.channels.channels import SetChannelsMixin
 
 from ..utils._checks import check_type, ensure_int, ensure_path
 from ..utils._docs import fill_doc
-from ..utils.logs import logger, verbose
+from ..utils.logs import logger, verbose, warn
 from ..utils.meas_info import _set_channel_units
 
 if TYPE_CHECKING:
     from datetime import datetime
     from typing import Any, Callable, Optional, Union
 
     from mne import Info
@@ -109,17 +108,15 @@
         Notes
         -----
         %(anonymize_info_notes)s
         """
         self._check_not_started("anonymize()")
         warn(
             "Player.anonymize() is partially implemented and does not impact the "
-            "stream information yet. It will call Player.set_meas_date() internally.",
-            RuntimeWarning,
-            stacklevel=2,
+            "stream information yet. It will call Player.set_meas_date() internally."
         )
         super().anonymize(
             daysback=daysback,
             keep_his=keep_his,
             verbose=logger.level if verbose is None else verbose,
         )
         return self
@@ -309,17 +306,15 @@
         See Also
         --------
         anonymize
         """
         self._check_not_started(name=f"{type(self).__name__}.set_meas_date()")
         warn(
             "Player.set_meas_date() is partially implemented and does not impact the "
-            "stream information yet.",
-            RuntimeWarning,
-            stacklevel=2,
+            "stream information yet."
         )
         super().set_meas_date(meas_date)
         return self
 
     @abstractmethod
     def stop(self) -> BasePlayer:
         """Stop streaming data on the mock real-time stream."""
```

### Comparing `mne_lsl-1.3.0/mne_lsl/player/_base.pyi` & `mne_lsl-1.3.1/mne_lsl/player/_base.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from ..utils._checks import check_type as check_type
 from ..utils._checks import ensure_int as ensure_int
 from ..utils._checks import ensure_path as ensure_path
 from ..utils._docs import fill_doc as fill_doc
 from ..utils.logs import logger as logger
 from ..utils.logs import verbose as verbose
+from ..utils.logs import warn as warn
 from ..utils.meas_info import _set_channel_units as _set_channel_units
 
 class BasePlayer(ABC, ContainsMixin, SetChannelsMixin):
     """Class for creating a mock real-time stream.
 
     Parameters
     ----------
```

### Comparing `mne_lsl-1.3.0/mne_lsl/player/player_lsl.py` & `mne_lsl-1.3.1/mne_lsl/player/player_lsl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations  # c.f. PEP 563, PEP 649
 
 from threading import Timer
 from typing import TYPE_CHECKING
-from warnings import catch_warnings, filterwarnings, warn
+from warnings import catch_warnings, filterwarnings
 
 import numpy as np
 from mne import Annotations
 from mne.annotations import _handle_meas_date
 
 from ..lsl import StreamInfo, StreamOutlet, local_clock
 from ..utils._checks import check_type
 from ..utils._docs import copy_doc, fill_doc
-from ..utils.logs import logger
+from ..utils.logs import logger, warn
 from ._base import BasePlayer
 
 if TYPE_CHECKING:
     from pathlib import Path
     from typing import Callable, Optional, Union
 
 
@@ -102,17 +102,15 @@
         # look for annotations
         if annotations is None:
             self._annotations = True if len(self._raw.annotations) != 0 else False
         else:
             if annotations and len(self._raw.annotations) == 0:
                 warn(
                     f"{self._name}: The raw file has no annotations. The annotations "
-                    "will be ignored.",
-                    RuntimeWarning,
-                    stacklevel=2,
+                    "will be ignored."
                 )
                 self._annotations = False
             else:
                 self._annotations = annotations
         # create stream info based on raw
         ch_types = self._raw.get_channel_types(unique=True)
         self._sinfo = StreamInfo(
@@ -169,17 +167,15 @@
         -------
         player : instance of :class:`~mne_lsl.player.PlayerLSL`
             The player instance modified in-place.
         """
         if self._streaming_thread is not None:
             warn(
                 f"{self._name}: The player is already started. "
-                "Use Player.stop() to stop streaming.",
-                RuntimeWarning,
-                stacklevel=2,
+                "Use Player.stop() to stop streaming."
             )
             return self
         self._outlet = StreamOutlet(self._sinfo, self._chunk_size)
         self._outlet_annotations = (
             StreamOutlet(self._sinfo_annotations, 1) if self._annotations else None
         )
         self._streaming_delay = self.chunk_size / self.info["sfreq"]
```

### Comparing `mne_lsl-1.3.0/mne_lsl/player/player_lsl.pyi` & `mne_lsl-1.3.1/mne_lsl/player/player_lsl.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ..lsl import StreamInfo as StreamInfo
 from ..lsl import StreamOutlet as StreamOutlet
 from ..lsl import local_clock as local_clock
 from ..utils._checks import check_type as check_type
 from ..utils._docs import copy_doc as copy_doc
 from ..utils._docs import fill_doc as fill_doc
 from ..utils.logs import logger as logger
+from ..utils.logs import warn as warn
 from ._base import BasePlayer as BasePlayer
 
 class PlayerLSL(BasePlayer):
     """Class for creating a mock LSL stream.
 
     Parameters
     ----------
```

### Comparing `mne_lsl-1.3.0/mne_lsl/stream/_base.py` & `mne_lsl-1.3.1/mne_lsl/stream/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations  # c.f. PEP 563, PEP 649
 
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from math import ceil
 from threading import Timer
 from typing import TYPE_CHECKING
-from warnings import warn
 
 import numpy as np
 from mne import pick_info, pick_types
 from mne.channels import rename_channels
 from mne.utils import check_version
 
 if check_version("mne", "1.6"):
@@ -24,15 +23,15 @@
     from mne.io.constants import FIFF, _ch_unit_mul_named
     from mne.io.meas_info import ContainsMixin
     from mne.io.pick import _picks_to_idx
     from mne.channels.channels import SetChannelsMixin
 
 from ..utils._checks import check_type, check_value, ensure_int
 from ..utils._docs import copy_doc, fill_doc
-from ..utils.logs import logger, verbose
+from ..utils.logs import logger, verbose, warn
 from ..utils.meas_info import _HUMAN_UNITS, _set_channel_units
 from ._filters import StreamFilter, create_filter, ensure_sos_iir_params
 
 if TYPE_CHECKING:
     from datetime import datetime
     from typing import Any, Callable, Optional, Union
 
@@ -173,17 +172,15 @@
             ref_dig_loc = [
                 dl
                 for dl in self._info["dig"]
                 if (dl["kind"] == FIFF.FIFFV_POINT_EEG and dl["ident"] == 0)
             ]
             if len(ref_channels) > 1 or len(ref_dig_loc) != len(ref_channels):
                 ref_dig_array = np.full(12, np.nan)
-                logger.warning(
-                    "The locations of multiple reference channels are ignored."
-                )
+                warn("The locations of multiple reference channels are ignored.")
             else:  # n_ref_channels == 1 and a single ref digitization exists
                 ref_dig_array = np.concatenate(
                     (ref_dig_loc[0]["r"], ref_dig_loc[0]["r"], np.zeros(6))
                 )
                 # replace the (possibly new) ref location for each channel
                 with self._info._unlock():
                     for idx in pick_types(self._info, meg=False, eeg=True, exclude=[]):
@@ -265,15 +262,15 @@
 
         Returns
         -------
         stream : instance of ``Stream``
             The stream instance modified in-place.
         """
         if self.connected:
-            logger.warning("The stream is already connected. Skipping.")
+            warn("The stream is already connected. Skipping.")
             return self
         check_type(acquisition_delay, ("numeric",), "acquisition_delay")
         if acquisition_delay < 0:
             raise ValueError(
                 "The acquisition delay must be a positive number "
                 "defining the delay at which new samples are acquired in seconds. For "
                 "instance, 0.2 corresponds to a pull every 200 ms. The provided "
@@ -349,18 +346,15 @@
                 "The index 'idx' must be a positive integer or a list of positive "
                 "integers not exceeding the number of filters minus 1: "
                 f"{len(self._filters) - 1}."
             )
         idx_unique = np.unique(idx)
         if idx_unique.size != idx.size:
             warn(
-                "The index 'idx' contains duplicates. Only unique indices will be "
-                "used.",
-                RuntimeWarning,
-                stacklevel=2,
+                "The index 'idx' contains duplicates. Only unique indices will be used."
             )
         idx = np.sort(idx_unique)
         logger.info(
             "Removing filters at index(es): %s\n%s",
             ", ".join([str(k) for k in idx]),
             "\n".join([repr(self._filters[k]) for k in idx]),
         )
```

### Comparing `mne_lsl-1.3.0/mne_lsl/stream/_base.pyi` & `mne_lsl-1.3.1/mne_lsl/stream/_base.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from ..utils._checks import check_type as check_type
 from ..utils._checks import check_value as check_value
 from ..utils._checks import ensure_int as ensure_int
 from ..utils._docs import copy_doc as copy_doc
 from ..utils._docs import fill_doc as fill_doc
 from ..utils.logs import logger as logger
 from ..utils.logs import verbose as verbose
+from ..utils.logs import warn as warn
 from ..utils.meas_info import _HUMAN_UNITS as _HUMAN_UNITS
 from ..utils.meas_info import _set_channel_units as _set_channel_units
 from ._filters import StreamFilter as StreamFilter
 from ._filters import create_filter as create_filter
 from ._filters import ensure_sos_iir_params as ensure_sos_iir_params
 
 class BaseStream(ABC, ContainsMixin, SetChannelsMixin):
```

### Comparing `mne_lsl-1.3.0/mne_lsl/stream/_filters.py` & `mne_lsl-1.3.1/mne_lsl/stream/_filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 from __future__ import annotations  # c.f. PEP 563, PEP 649
 
 from typing import TYPE_CHECKING
-from warnings import warn
 
 import numpy as np
 from mne.filter import create_filter as create_filter_mne
 from scipy.signal import sosfilt_zi
 
 from ..utils._checks import check_type
-from ..utils.logs import logger
+from ..utils.logs import logger, warn
 
 if TYPE_CHECKING:
     from typing import Any, Optional
 
 
 class StreamFilter(dict):
     """Class defining a filter."""
 
     _ORDER_STR: dict[int, str] = {1: "1st", 2: "2nd"}
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if "iir_params" not in self:
-            warn(
-                "The 'iir_params' key is missing, which is unexpected.",
-                RuntimeWarning,
-                stacklevel=2,
-            )
+            warn("The 'iir_params' key is missing, which is unexpected.")
             self["iir_params"] = dict()
         for key in ("ftype", "order"):
             if key not in self:
                 continue
             if key not in self["iir_params"]:
                 self["iir_params"][key] = self[key]
             else:
@@ -75,17 +70,15 @@
                 ):
                     return False
                 continue
             type_ = type(self[key])
             if not isinstance(other[key], type_):  # sanity-check
                 warn(
                     f"The type of the key '{key}' is different between the 2 filters, "
-                    "which should not be possible. Please contact the developers.",
-                    RuntimeWarning,
-                    stacklevel=2,
+                    "which should not be possible. Please contact the developers."
                 )
                 return False
             if (
                 type_ is np.ndarray
                 and not np.array_equal(self[key], other[key], equal_nan=True)
             ) or (type_ is not np.ndarray and self[key] != other[key]):
                 return False
@@ -103,15 +96,15 @@
     iir_params: dict[str, Any],
 ) -> dict[str, Any]:
     """Create an IIR causal filter.
 
     Parameters
     ----------
     sfreq : float
-        The sampling ferquency in Hz.
+        The sampling frequency in Hz.
     %(l_freq)s
     %(h_freq)s
     %(iir_params)s
 
     Returns
     -------
     filt : dict
@@ -148,16 +141,14 @@
     check_type(iir_params, (dict,), "iir_params")
     if ("output" in iir_params and iir_params["output"] != "sos") or all(
         key in iir_params for key in ("a", "b")
     ):
         warn(
             "Only 'sos' output is supported for real-time filtering. The filter "
             "output will be automatically changed. Please set "
-            "iir_params=dict(output='sos', ...) in your call to the filtering method.",
-            RuntimeWarning,
-            stacklevel=2,
+            "iir_params=dict(output='sos', ...) in your call to the filtering method."
         )
         for key in ("a", "b"):
             if key in iir_params:
                 del iir_params[key]
     iir_params["output"] = "sos"
     return iir_params
```

### Comparing `mne_lsl-1.3.0/mne_lsl/stream/_filters.pyi` & `mne_lsl-1.3.1/mne_lsl/stream/_filters.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 from ..utils._checks import check_type as check_type
 from ..utils.logs import logger as logger
+from ..utils.logs import warn as warn
 
 class StreamFilter(dict):
     """Class defining a filter."""
 
     _ORDER_STR: dict[int, str]
 
     def __init__(self, *args, **kwargs) -> None: ...
@@ -20,15 +21,15 @@
     sfreq: float, l_freq: float | None, h_freq: float | None, iir_params: dict[str, Any]
 ) -> dict[str, Any]:
     """Create an IIR causal filter.
 
     Parameters
     ----------
     sfreq : float
-        The sampling ferquency in Hz.
+        The sampling frequency in Hz.
     %(l_freq)s
     %(h_freq)s
     %(iir_params)s
 
     Returns
     -------
     filt : dict
```

### Comparing `mne_lsl-1.3.0/mne_lsl/stream/stream_lsl.py` & `mne_lsl-1.3.1/mne_lsl/stream/stream_lsl.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/stream/stream_lsl.pyi` & `mne_lsl-1.3.1/mne_lsl/stream/stream_lsl.pyi`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/stream_viewer/backends/_backend.py` & `mne_lsl-1.3.1/mne_lsl/stream_viewer/backends/_backend.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/stream_viewer/backends/pyqtgraph.py` & `mne_lsl-1.3.1/mne_lsl/stream_viewer/backends/pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/stream_viewer/control_gui/_control.py` & `mne_lsl-1.3.1/mne_lsl/stream_viewer/control_gui/_control.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/stream_viewer/control_gui/_ui_control.py` & `mne_lsl-1.3.1/mne_lsl/stream_viewer/control_gui/_ui_control.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/stream_viewer/control_gui/control_eeg.py` & `mne_lsl-1.3.1/mne_lsl/stream_viewer/control_gui/control_eeg.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/stream_viewer/scope/_scope.py` & `mne_lsl-1.3.1/mne_lsl/stream_viewer/scope/_scope.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/stream_viewer/scope/scope_eeg.py` & `mne_lsl-1.3.1/mne_lsl/stream_viewer/scope/scope_eeg.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/stream_viewer/stream_viewer.py` & `mne_lsl-1.3.1/mne_lsl/stream_viewer/stream_viewer.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/utils/_checks.py` & `mne_lsl-1.3.1/mne_lsl/utils/_checks.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/utils/_checks.pyi` & `mne_lsl-1.3.1/mne_lsl/utils/_checks.pyi`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/utils/_docs.py` & `mne_lsl-1.3.1/mne_lsl/utils/_docs.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/utils/_docs.pyi` & `mne_lsl-1.3.1/mne_lsl/utils/_docs.pyi`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/utils/_fixes.py` & `mne_lsl-1.3.1/mne_lsl/utils/_fixes.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/utils/_imports.py` & `mne_lsl-1.3.1/mne_lsl/utils/_imports.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/utils/_imports.pyi` & `mne_lsl-1.3.1/mne_lsl/utils/_imports.pyi`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/utils/_path.py` & `mne_lsl-1.3.1/mne_lsl/utils/_path.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/utils/_tests.py` & `mne_lsl-1.3.1/mne_lsl/utils/_tests.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/utils/_tests.pyi` & `mne_lsl-1.3.1/mne_lsl/utils/_tests.pyi`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/utils/config.py` & `mne_lsl-1.3.1/mne_lsl/utils/config.py`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/utils/config.pyi` & `mne_lsl-1.3.1/mne_lsl/utils/config.pyi`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl/utils/meas_info.py` & `mne_lsl-1.3.1/mne_lsl/utils/meas_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from mne._fiff.constants import FIFF, _ch_unit_mul_named
     from mne._fiff.pick import get_channel_type_constants
 else:
     from mne.io.constants import FIFF, _ch_unit_mul_named
     from mne.io.pick import get_channel_type_constants
 
 from ._checks import check_type, check_value, ensure_int
-from .logs import logger
+from .logs import logger, warn
 
 if TYPE_CHECKING:
     from typing import Any, Optional, Union
 
     from mne import Info
 
     from ..lsl.stream_info import _BaseStreamInfo
@@ -63,15 +63,15 @@
         Type of the stream. This type will be used as a default for all channels with
         an unknown type. If the ``stype`` provided is not among the MNE-known channel
         types, defaults to ``'misc'``.
     desc : StreamInfo | dict | None
         If provided, dictionary or :class:`~mne_lsl.lsl.StreamInfo` containing the
         channel information. A `~mne_lsl.lsl.StreamInfo` contains the number of
         channels,csampling frequency and stream type, which will be checked against the
-        providedcarguments ``n_channels``, ``sfreq`` and ``stype``.
+        provided arguments ``n_channels``, ``sfreq`` and ``stype``.
 
     Returns
     -------
     info : Info
         MNE :class:`~mne.Info` object corresponding.
 
     Notes
@@ -94,14 +94,18 @@
 
     # try to identify the main channel type
     stype = stype.lower().strip()
     stype = "stim" if stype in _STIM_TYPES else stype
     stype = stype if stype in _CH_TYPES_DICT else "misc"
 
     # attempt to create the info depending on the provided description
+    if desc is None:
+        logger.info("No description provided. Creating a default Info object.")
+        return _create_default_info(n_channels, sfreq, stype)
+
     try:
         if isinstance(desc, dict):
             ch_names, ch_types, ch_units, manufacturer = _read_desc_dict(
                 n_channels, stype, desc
             )
         elif isinstance(desc, _BaseStreamInfo):
             ch_names, ch_types, ch_units, manufacturer = _read_desc_sinfo(
@@ -122,26 +126,50 @@
             info["device_info"]["model"] = manufacturer
         elif (
             isinstance(manufacturer, list)
             and len(manufacturer) == 1
             and isinstance(manufacturer[0], str)
         ):
             info["device_info"]["model"] = manufacturer[0]
+        info._check_consistency()
     except Exception:
-        logger.warning(
+        warn(
             "Something went wrong while reading the channel description. Defaulting to "
             "channel IDs and MNE-compatible stream type."
         )
-        info = mne_create_info(n_channels, 1.0, stype)
-        info["device_info"] = dict()
-        with info._unlock():
-            info["sfreq"] = sfreq
-        info["device_info"] = dict()
+        info = _create_default_info(n_channels, sfreq, stype)
+    return info
+
+
+def _create_default_info(
+    n_channels: int,
+    sfreq: float,
+    stype: str,
+) -> Info:
+    """Create a default Info object.
+
+    Parameters
+    ----------
+    n_channels : int
+        Number of channels.
+    sfreq : float
+        Sampling frequency in Hz. ``0`` corresponds to an irregular sampling rate.
+    stype : str
+        Type of the stream.
 
-    info._check_consistency()
+    Returns
+    -------
+    info : Info
+        MNE :class:`~mne.Info` object corresponding.
+    """
+    info = mne_create_info(n_channels, 1.0, stype)
+    info["device_info"] = dict()
+    with info._unlock():
+        info["sfreq"] = sfreq
+    info["device_info"] = dict()
     return info
 
 
 # --------------------- Functions to read from a description sinfo ---------------------
 def _read_desc_sinfo(
     n_channels: int, stype: str, desc: _BaseStreamInfo
 ) -> tuple[list[str], list[str], list[int], Optional[str]]:
```

### Comparing `mne_lsl-1.3.0/mne_lsl/utils/meas_info.pyi` & `mne_lsl-1.3.1/mne_lsl/utils/meas_info.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from mne import Info
 
 from ..lsl.stream_info import _BaseStreamInfo as _BaseStreamInfo
 from ._checks import check_type as check_type
 from ._checks import check_value as check_value
 from ._checks import ensure_int as ensure_int
 from .logs import logger as logger
+from .logs import warn as warn
 
 _CH_TYPES_DICT: Incomplete
 _STIM_TYPES: tuple[str, ...]
 _HUMAN_UNITS: dict[int, dict[str, int]]
 
 def create_info(
     n_channels: int,
@@ -31,27 +32,45 @@
         Type of the stream. This type will be used as a default for all channels with
         an unknown type. If the ``stype`` provided is not among the MNE-known channel
         types, defaults to ``'misc'``.
     desc : StreamInfo | dict | None
         If provided, dictionary or :class:`~mne_lsl.lsl.StreamInfo` containing the
         channel information. A `~mne_lsl.lsl.StreamInfo` contains the number of
         channels,csampling frequency and stream type, which will be checked against the
-        providedcarguments ``n_channels``, ``sfreq`` and ``stype``.
+        provided arguments ``n_channels``, ``sfreq`` and ``stype``.
 
     Returns
     -------
     info : Info
         MNE :class:`~mne.Info` object corresponding.
 
     Notes
     -----
     If the argument ``desc`` is not aligned with ``n_channels``, it is ignored and an
     :class:`mne.Info` with the number of channels definbed in ``n_channels`` is created.
     """
 
+def _create_default_info(n_channels: int, sfreq: float, stype: str) -> Info:
+    """Create a default Info object.
+
+    Parameters
+    ----------
+    n_channels : int
+        Number of channels.
+    sfreq : float
+        Sampling frequency in Hz. ``0`` corresponds to an irregular sampling rate.
+    stype : str
+        Type of the stream.
+
+    Returns
+    -------
+    info : Info
+        MNE :class:`~mne.Info` object corresponding.
+    """
+
 def _read_desc_sinfo(
     n_channels: int, stype: str, desc: _BaseStreamInfo
 ) -> tuple[list[str], list[str], list[int], str | None]:
     """Read channel information from a StreamInfo.
 
     If the StreamInfo is retrieved by resolve_streams, the description will be empty.
     An inlet should be created and the inlet StreamInfo should be used to retrieve the
```

### Comparing `mne_lsl-1.3.0/mne_lsl.egg-info/PKG-INFO` & `mne_lsl-1.3.1/mne_lsl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mne_lsl
-Version: 1.3.0
+Version: 1.3.1
 Summary: Real-time framework integrated with MNE-Python for online neuroscience research through LSL-compatible devices.
 Author-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 Maintainer-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 License: Copyright © 2023-2024, authors of MNE-LSL
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `mne_lsl-1.3.0/mne_lsl.egg-info/SOURCES.txt` & `mne_lsl-1.3.1/mne_lsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/mne_lsl.egg-info/requires.txt` & `mne_lsl-1.3.1/mne_lsl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mne_lsl-1.3.0/pyproject.toml` & `mne_lsl-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 license = {file = 'LICENSE'}
 maintainers = [
   {email = 'mathieu.scheltienne@fcbg.ch', name = 'Mathieu Scheltienne'},
 ]
 name = 'mne_lsl'
 readme = 'README.md'
 requires-python = '>=3.9'
-version = '1.3.0'
+version = '1.3.1'
 
 [project.optional-dependencies]
 all = [
   'mne_lsl[build]',
   'mne_lsl[doc]',
   'mne_lsl[stubs]',
   'mne_lsl[style]',
```

