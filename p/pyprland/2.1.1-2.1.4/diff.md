# Comparing `tmp/pyprland-2.1.1.tar.gz` & `tmp/pyprland-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprland-2.1.1.tar", max compression
+gzip compressed data, was "pyprland-2.1.4.tar", max compression
```

## Comparing `pyprland-2.1.1.tar` & `pyprland-2.1.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.1.1/LICENSE
--rw-r--r--   0        0        0     5344 2024-03-31 20:26:52.948509 pyprland-2.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.1.1/pyprland/__init__.py
--rw-r--r--   0        0        0        0 2024-03-02 14:42:00.069047 pyprland-2.1.1/pyprland/__init__.py,cover
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.1.1/pyprland/adapters/__init__.py
--rw-r--r--   0        0        0        0 2024-03-02 14:42:00.069047 pyprland-2.1.1/pyprland/adapters/__init__.py,cover
--rw-r--r--   0        0        0      165 2024-03-03 01:49:11.929817 pyprland-2.1.1/pyprland/adapters/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7499 2024-03-03 11:48:19.793333 pyprland-2.1.1/pyprland/adapters/__pycache__/menus.cpython-311.pyc
--rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.1.1/pyprland/adapters/menus.py
--rw-r--r--   0        0        0     4703 2024-03-02 14:42:00.072380 pyprland-2.1.1/pyprland/adapters/menus.py,cover
--rwxr-xr-x   0        0        0    15371 2024-03-31 20:31:24.911790 pyprland-2.1.1/pyprland/command.py
--rw-r--r--   0        0        0    15442 2024-03-02 14:42:00.079047 pyprland-2.1.1/pyprland/command.py,cover
--rwxr-xr-x   0        0        0    15518 2024-03-30 19:02:09.575863 pyprland-2.1.1/pyprland/command.py.orig
--rw-r--r--   0        0        0     4133 2024-03-03 01:47:24.921035 pyprland-2.1.1/pyprland/common.py
--rw-r--r--   0        0        0     4409 2024-03-02 14:42:00.079047 pyprland-2.1.1/pyprland/common.py,cover
--rw-r--r--   0        0        0     5948 2024-03-31 20:05:57.091220 pyprland-2.1.1/pyprland/ipc.py
--rw-r--r--   0        0        0     6104 2024-03-02 14:42:00.082381 pyprland-2.1.1/pyprland/ipc.py,cover
--rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.1.1/pyprland/plugins/__init__.py
--rw-r--r--   0        0        0       49 2024-03-02 14:42:00.082381 pyprland-2.1.1/pyprland/plugins/__init__.py,cover
--rw-r--r--   0        0        0      227 2024-03-03 01:49:11.929817 pyprland-2.1.1/pyprland/plugins/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2902 2024-03-03 11:48:21.296667 pyprland-2.1.1/pyprland/plugins/__pycache__/expose.cpython-311.pyc
--rw-r--r--   0        0        0     3207 2024-03-30 18:24:39.387692 pyprland-2.1.1/pyprland/plugins/__pycache__/fetch_client_menu.cpython-311.pyc
--rw-r--r--   0        0        0     3905 2024-03-03 01:50:19.494487 pyprland-2.1.1/pyprland/plugins/__pycache__/interface.cpython-311.pyc
--rw-r--r--   0        0        0    14058 2024-03-03 11:48:21.256667 pyprland-2.1.1/pyprland/plugins/__pycache__/layout_center.cpython-311.pyc
--rw-r--r--   0        0        0     3740 2024-03-03 11:48:21.256667 pyprland-2.1.1/pyprland/plugins/__pycache__/lost_windows.cpython-311.pyc
--rw-r--r--   0        0        0     1467 2024-03-03 11:48:21.296667 pyprland-2.1.1/pyprland/plugins/__pycache__/magnify.cpython-311.pyc
--rw-r--r--   0        0        0    13040 2024-03-31 17:52:50.637188 pyprland-2.1.1/pyprland/plugins/__pycache__/monitors.cpython-311.pyc
--rw-r--r--   0        0        0     2817 2024-03-03 11:48:19.756667 pyprland-2.1.1/pyprland/plugins/__pycache__/pyprland.cpython-311.pyc
--rw-r--r--   0        0        0    54525 2024-03-31 20:16:48.503352 pyprland-2.1.1/pyprland/plugins/__pycache__/scratchpads.cpython-311.pyc
--rw-r--r--   0        0        0     2600 2024-03-03 11:48:21.263333 pyprland-2.1.1/pyprland/plugins/__pycache__/shift_monitors.cpython-311.pyc
--rw-r--r--   0        0        0     7268 2024-03-03 11:48:19.790000 pyprland-2.1.1/pyprland/plugins/__pycache__/shortcuts_menu.cpython-311.pyc
--rw-r--r--   0        0        0     5631 2024-03-03 11:48:19.803333 pyprland-2.1.1/pyprland/plugins/__pycache__/system_notifier.cpython-311.pyc
--rw-r--r--   0        0        0     1582 2024-03-03 11:48:21.296667 pyprland-2.1.1/pyprland/plugins/__pycache__/toggle_dpms.cpython-311.pyc
--rw-r--r--   0        0        0     1916 2024-03-03 11:48:19.803333 pyprland-2.1.1/pyprland/plugins/__pycache__/toggle_special.cpython-311.pyc
--rw-r--r--   0        0        0     5090 2024-03-03 11:48:21.296667 pyprland-2.1.1/pyprland/plugins/__pycache__/workspaces_follow_focus.cpython-311.pyc
--rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.1.1/pyprland/plugins/experimental.py
--rw-r--r--   0        0        0     1647 2024-03-03 01:47:24.914368 pyprland-2.1.1/pyprland/plugins/expose.py
--rw-r--r--   0        0        0     1733 2024-03-02 14:42:00.082381 pyprland-2.1.1/pyprland/plugins/expose.py,cover
--rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.1.1/pyprland/plugins/fetch_client_menu.py
--rw-r--r--   0        0        0      978 2024-03-02 14:42:00.082381 pyprland-2.1.1/pyprland/plugins/fetch_client_menu.py,cover
--rw-r--r--   0        0        0     2601 2024-03-03 01:47:24.901034 pyprland-2.1.1/pyprland/plugins/interface.py
--rw-r--r--   0        0        0     2771 2024-03-02 14:42:00.085714 pyprland-2.1.1/pyprland/plugins/interface.py,cover
--rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.1.1/pyprland/plugins/layout_center.py
--rw-r--r--   0        0        0     8414 2024-03-02 14:42:00.085714 pyprland-2.1.1/pyprland/plugins/layout_center.py,cover
--rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.1.1/pyprland/plugins/lost_windows.py
--rw-r--r--   0        0        0     1765 2024-03-02 14:42:00.089047 pyprland-2.1.1/pyprland/plugins/lost_windows.py,cover
--rw-r--r--   0        0        0      761 2024-03-03 01:47:24.904368 pyprland-2.1.1/pyprland/plugins/magnify.py
--rw-r--r--   0        0        0      801 2024-03-02 14:42:00.089047 pyprland-2.1.1/pyprland/plugins/magnify.py,cover
--rw-r--r--   0        0        0     8684 2024-03-31 17:52:13.879696 pyprland-2.1.1/pyprland/plugins/monitors.py
--rw-r--r--   0        0        0    12264 2024-03-02 14:42:00.092381 pyprland-2.1.1/pyprland/plugins/monitors.py,cover
--rw-r--r--   0        0        0     8720 2024-03-30 19:02:09.575863 pyprland-2.1.1/pyprland/plugins/monitors.py.orig
--rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.1.1/pyprland/plugins/monitors_v0.py
--rw-r--r--   0        0        0     1218 2024-03-03 01:47:24.907701 pyprland-2.1.1/pyprland/plugins/pyprland.py
--rw-r--r--   0        0        0     1286 2024-03-02 14:42:00.092381 pyprland-2.1.1/pyprland/plugins/pyprland.py,cover
--rw-r--r--   0        0        0    35230 2024-03-31 20:15:12.257746 pyprland-2.1.1/pyprland/plugins/scratchpads.py
--rw-r--r--   0        0        0    36868 2024-03-02 14:42:00.102381 pyprland-2.1.1/pyprland/plugins/scratchpads.py,cover
--rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.1.1/pyprland/plugins/shift_monitors.py
--rw-r--r--   0        0        0     1126 2024-03-02 14:42:00.105714 pyprland-2.1.1/pyprland/plugins/shift_monitors.py,cover
--rw-r--r--   0        0        0     4122 2024-03-03 01:47:24.917701 pyprland-2.1.1/pyprland/plugins/shortcuts_menu.py
--rw-r--r--   0        0        0     4340 2024-03-02 14:42:00.105714 pyprland-2.1.1/pyprland/plugins/shortcuts_menu.py,cover
--rw-r--r--   0        0        0     3124 2024-03-03 01:47:24.911034 pyprland-2.1.1/pyprland/plugins/system_notifier.py
--rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.1.1/pyprland/plugins/toggle_dpms.py
--rw-r--r--   0        0        0      549 2024-03-02 14:42:00.105714 pyprland-2.1.1/pyprland/plugins/toggle_dpms.py,cover
--rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.1.1/pyprland/plugins/toggle_special.py
--rw-r--r--   0        0        0     1117 2024-03-02 14:42:00.105714 pyprland-2.1.1/pyprland/plugins/toggle_special.py,cover
--rw-r--r--   0        0        0     2589 2024-03-03 01:47:24.911034 pyprland-2.1.1/pyprland/plugins/workspaces_follow_focus.py
--rw-r--r--   0        0        0     2731 2024-03-02 14:42:00.109048 pyprland-2.1.1/pyprland/plugins/workspaces_follow_focus.py,cover
--rw-r--r--   0        0        0      725 2024-03-31 20:31:24.568449 pyprland-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     5883 1970-01-01 00:00:00.000000 pyprland-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.1.4/LICENSE
+-rw-r--r--   0        0        0     5338 2024-03-31 23:50:07.712880 pyprland-2.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.1.4/pyprland/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-02 14:42:00.069047 pyprland-2.1.4/pyprland/__init__.py,cover
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.1.4/pyprland/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-02 14:42:00.069047 pyprland-2.1.4/pyprland/adapters/__init__.py,cover
+-rw-r--r--   0        0        0      165 2024-03-03 01:49:11.929817 pyprland-2.1.4/pyprland/adapters/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7499 2024-03-03 11:48:19.793333 pyprland-2.1.4/pyprland/adapters/__pycache__/menus.cpython-311.pyc
+-rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.1.4/pyprland/adapters/menus.py
+-rw-r--r--   0        0        0     4703 2024-03-02 14:42:00.072380 pyprland-2.1.4/pyprland/adapters/menus.py,cover
+-rwxr-xr-x   0        0        0    15373 2024-04-03 21:51:25.315300 pyprland-2.1.4/pyprland/command.py
+-rw-r--r--   0        0        0    15442 2024-03-02 14:42:00.079047 pyprland-2.1.4/pyprland/command.py,cover
+-rwxr-xr-x   0        0        0    15518 2024-03-30 19:02:09.575863 pyprland-2.1.4/pyprland/command.py.orig
+-rw-r--r--   0        0        0     4133 2024-03-03 01:47:24.921035 pyprland-2.1.4/pyprland/common.py
+-rw-r--r--   0        0        0     4409 2024-03-02 14:42:00.079047 pyprland-2.1.4/pyprland/common.py,cover
+-rw-r--r--   0        0        0     5948 2024-03-31 20:05:57.091220 pyprland-2.1.4/pyprland/ipc.py
+-rw-r--r--   0        0        0     6104 2024-03-02 14:42:00.082381 pyprland-2.1.4/pyprland/ipc.py,cover
+-rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.1.4/pyprland/plugins/__init__.py
+-rw-r--r--   0        0        0       49 2024-03-02 14:42:00.082381 pyprland-2.1.4/pyprland/plugins/__init__.py,cover
+-rw-r--r--   0        0        0      227 2024-03-03 01:49:11.929817 pyprland-2.1.4/pyprland/plugins/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2902 2024-03-03 11:48:21.296667 pyprland-2.1.4/pyprland/plugins/__pycache__/expose.cpython-311.pyc
+-rw-r--r--   0        0        0     3207 2024-03-30 18:24:39.387692 pyprland-2.1.4/pyprland/plugins/__pycache__/fetch_client_menu.cpython-311.pyc
+-rw-r--r--   0        0        0     3905 2024-03-03 01:50:19.494487 pyprland-2.1.4/pyprland/plugins/__pycache__/interface.cpython-311.pyc
+-rw-r--r--   0        0        0    14058 2024-03-03 11:48:21.256667 pyprland-2.1.4/pyprland/plugins/__pycache__/layout_center.cpython-311.pyc
+-rw-r--r--   0        0        0     3740 2024-03-03 11:48:21.256667 pyprland-2.1.4/pyprland/plugins/__pycache__/lost_windows.cpython-311.pyc
+-rw-r--r--   0        0        0     1814 2024-04-03 21:48:46.484412 pyprland-2.1.4/pyprland/plugins/__pycache__/magnify.cpython-311.pyc
+-rw-r--r--   0        0        0    13040 2024-03-31 17:52:50.637188 pyprland-2.1.4/pyprland/plugins/__pycache__/monitors.cpython-311.pyc
+-rw-r--r--   0        0        0     2817 2024-03-03 11:48:19.756667 pyprland-2.1.4/pyprland/plugins/__pycache__/pyprland.cpython-311.pyc
+-rw-r--r--   0        0        0    54691 2024-04-03 21:46:08.496667 pyprland-2.1.4/pyprland/plugins/__pycache__/scratchpads.cpython-311.pyc
+-rw-r--r--   0        0        0     2600 2024-03-03 11:48:21.263333 pyprland-2.1.4/pyprland/plugins/__pycache__/shift_monitors.cpython-311.pyc
+-rw-r--r--   0        0        0     7268 2024-03-03 11:48:19.790000 pyprland-2.1.4/pyprland/plugins/__pycache__/shortcuts_menu.cpython-311.pyc
+-rw-r--r--   0        0        0     5631 2024-03-03 11:48:19.803333 pyprland-2.1.4/pyprland/plugins/__pycache__/system_notifier.cpython-311.pyc
+-rw-r--r--   0        0        0     1582 2024-03-03 11:48:21.296667 pyprland-2.1.4/pyprland/plugins/__pycache__/toggle_dpms.cpython-311.pyc
+-rw-r--r--   0        0        0     1916 2024-03-03 11:48:19.803333 pyprland-2.1.4/pyprland/plugins/__pycache__/toggle_special.cpython-311.pyc
+-rw-r--r--   0        0        0     5090 2024-03-03 11:48:21.296667 pyprland-2.1.4/pyprland/plugins/__pycache__/workspaces_follow_focus.cpython-311.pyc
+-rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.1.4/pyprland/plugins/experimental.py
+-rw-r--r--   0        0        0     1647 2024-03-03 01:47:24.914368 pyprland-2.1.4/pyprland/plugins/expose.py
+-rw-r--r--   0        0        0     1733 2024-03-02 14:42:00.082381 pyprland-2.1.4/pyprland/plugins/expose.py,cover
+-rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.1.4/pyprland/plugins/fetch_client_menu.py
+-rw-r--r--   0        0        0      978 2024-03-02 14:42:00.082381 pyprland-2.1.4/pyprland/plugins/fetch_client_menu.py,cover
+-rw-r--r--   0        0        0     2601 2024-03-03 01:47:24.901034 pyprland-2.1.4/pyprland/plugins/interface.py
+-rw-r--r--   0        0        0     2771 2024-03-02 14:42:00.085714 pyprland-2.1.4/pyprland/plugins/interface.py,cover
+-rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.1.4/pyprland/plugins/layout_center.py
+-rw-r--r--   0        0        0     8414 2024-03-02 14:42:00.085714 pyprland-2.1.4/pyprland/plugins/layout_center.py,cover
+-rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.1.4/pyprland/plugins/lost_windows.py
+-rw-r--r--   0        0        0     1765 2024-03-02 14:42:00.089047 pyprland-2.1.4/pyprland/plugins/lost_windows.py,cover
+-rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.1.4/pyprland/plugins/magnify.py
+-rw-r--r--   0        0        0      801 2024-03-02 14:42:00.089047 pyprland-2.1.4/pyprland/plugins/magnify.py,cover
+-rw-r--r--   0        0        0     8684 2024-03-31 17:52:13.879696 pyprland-2.1.4/pyprland/plugins/monitors.py
+-rw-r--r--   0        0        0    12264 2024-03-02 14:42:00.092381 pyprland-2.1.4/pyprland/plugins/monitors.py,cover
+-rw-r--r--   0        0        0     8720 2024-03-30 19:02:09.575863 pyprland-2.1.4/pyprland/plugins/monitors.py.orig
+-rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.1.4/pyprland/plugins/monitors_v0.py
+-rw-r--r--   0        0        0     1218 2024-03-03 01:47:24.907701 pyprland-2.1.4/pyprland/plugins/pyprland.py
+-rw-r--r--   0        0        0     1286 2024-03-02 14:42:00.092381 pyprland-2.1.4/pyprland/plugins/pyprland.py,cover
+-rw-r--r--   0        0        0    35404 2024-04-03 18:49:20.111659 pyprland-2.1.4/pyprland/plugins/scratchpads.py
+-rw-r--r--   0        0        0    36868 2024-03-02 14:42:00.102381 pyprland-2.1.4/pyprland/plugins/scratchpads.py,cover
+-rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.1.4/pyprland/plugins/shift_monitors.py
+-rw-r--r--   0        0        0     1126 2024-03-02 14:42:00.105714 pyprland-2.1.4/pyprland/plugins/shift_monitors.py,cover
+-rw-r--r--   0        0        0     4122 2024-03-03 01:47:24.917701 pyprland-2.1.4/pyprland/plugins/shortcuts_menu.py
+-rw-r--r--   0        0        0     4340 2024-03-02 14:42:00.105714 pyprland-2.1.4/pyprland/plugins/shortcuts_menu.py,cover
+-rw-r--r--   0        0        0     3124 2024-03-03 01:47:24.911034 pyprland-2.1.4/pyprland/plugins/system_notifier.py
+-rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.1.4/pyprland/plugins/toggle_dpms.py
+-rw-r--r--   0        0        0      549 2024-03-02 14:42:00.105714 pyprland-2.1.4/pyprland/plugins/toggle_dpms.py,cover
+-rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.1.4/pyprland/plugins/toggle_special.py
+-rw-r--r--   0        0        0     1117 2024-03-02 14:42:00.105714 pyprland-2.1.4/pyprland/plugins/toggle_special.py,cover
+-rw-r--r--   0        0        0     2589 2024-03-03 01:47:24.911034 pyprland-2.1.4/pyprland/plugins/workspaces_follow_focus.py
+-rw-r--r--   0        0        0     2731 2024-03-02 14:42:00.109048 pyprland-2.1.4/pyprland/plugins/workspaces_follow_focus.py,cover
+-rw-r--r--   0        0        0      725 2024-04-03 21:51:25.295300 pyprland-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5877 1970-01-01 00:00:00.000000 pyprland-2.1.4/PKG-INFO
```

### Comparing `pyprland-2.1.1/LICENSE` & `pyprland-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/README.md` & `pyprland-2.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 ## Latest major changes
 
 Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
 
 ### 2.1
 
-- Requires Hyprland 0.37 or better
+- Requires Hyprland >= 0.37
 - [monitors](https://github.com/hyprland-community/pyprland/wiki//monitors)
   - Drops the `wlr-randr` dependency
   - simplified the syntax, no need for `()` around a screen name (will try matching the exact name first, then partial description)
 
 ### 2.0
 
 - New dependency: [aiofiles](https://pypi.org/project/aiofiles/)
@@ -96,7 +96,8 @@
 <a href="https://star-history.com/#fdev31/pyprland&Date">
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline&theme=dark" />
     <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline" />
     <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline" />
   </picture>
 </a>
+
```

### Comparing `pyprland-2.1.1/pyprland/adapters/__pycache__/menus.cpython-311.pyc` & `pyprland-2.1.4/pyprland/adapters/__pycache__/menus.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/adapters/menus.py` & `pyprland-2.1.4/pyprland/adapters/menus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/adapters/menus.py,cover` & `pyprland-2.1.4/pyprland/adapters/menus.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/command.py` & `pyprland-2.1.4/pyprland/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,15 +329,15 @@
 
 
 async def run_client():
     "Runs the client (CLI)"
     manager = Pyprland()
 
     if sys.argv[1] == "version":
-        print("2.1.1")  # Automatically updated version
+        print('2.1.4-1')  # Automatically updated version
         return
 
     if sys.argv[1] in ("--help", "-h", "help"):
         await manager.load_config(init=False)
 
         def format_doc(txt):
             return txt.split("\n")[0]
```

### Comparing `pyprland-2.1.1/pyprland/command.py,cover` & `pyprland-2.1.4/pyprland/command.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/command.py.orig` & `pyprland-2.1.4/pyprland/command.py.orig`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/common.py` & `pyprland-2.1.4/pyprland/common.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/common.py,cover` & `pyprland-2.1.4/pyprland/common.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/ipc.py` & `pyprland-2.1.4/pyprland/ipc.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/ipc.py,cover` & `pyprland-2.1.4/pyprland/ipc.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/__pycache__/expose.cpython-311.pyc` & `pyprland-2.1.4/pyprland/plugins/__pycache__/expose.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/__pycache__/fetch_client_menu.cpython-311.pyc` & `pyprland-2.1.4/pyprland/plugins/__pycache__/fetch_client_menu.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/__pycache__/interface.cpython-311.pyc` & `pyprland-2.1.4/pyprland/plugins/__pycache__/interface.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/__pycache__/layout_center.cpython-311.pyc` & `pyprland-2.1.4/pyprland/plugins/__pycache__/layout_center.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/__pycache__/lost_windows.cpython-311.pyc` & `pyprland-2.1.4/pyprland/plugins/__pycache__/lost_windows.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/__pycache__/monitors.cpython-311.pyc` & `pyprland-2.1.4/pyprland/plugins/__pycache__/monitors.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/__pycache__/pyprland.cpython-311.pyc` & `pyprland-2.1.4/pyprland/plugins/__pycache__/pyprland.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/__pycache__/scratchpads.cpython-311.pyc` & `pyprland-2.1.4/pyprland/plugins/__pycache__/scratchpads.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x50c40966 (Sun Mar 31 20:15:12 2024 UTC)
-files sz: 35230
+moddate:  0xb0a40d66 (Wed Apr  3 18:49:20 2024 UTC)
+files sz: 35404
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x970064005a00640164026c015a01640164026c025a02640164026c035a
@@ -2957,119 +2957,119 @@
                      192 LOAD_CONST               6 ('return')
                      194 LOAD_NAME               20 (bool)
                      196 BUILD_TUPLE              2
                      198 LOAD_CONST              12 (<code object __wait_for_client, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 482>)
                      200 MAKE_FUNCTION            5 (defaults, annotations)
                      202 STORE_NAME              21 (_Extension__wait_for_client)
          
-         512         204 LOAD_CONST               6 ('return')
+         513         204 LOAD_CONST               6 ('return')
                      206 LOAD_NAME               20 (bool)
                      208 BUILD_TUPLE              2
-                     210 LOAD_CONST              13 (<code object _start_scratch_classbased, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 512>)
+                     210 LOAD_CONST              13 (<code object _start_scratch_classbased, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 513>)
                      212 MAKE_FUNCTION            4 (annotations)
                      214 STORE_NAME              22 (_start_scratch_classbased)
          
-         526         216 LOAD_CONST              14 (<code object _start_scratch, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 526>)
+         527         216 LOAD_CONST              14 (<code object _start_scratch, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 527>)
                      218 MAKE_FUNCTION            0
                      220 STORE_NAME              23 (_start_scratch)
          
-         553         222 LOAD_CONST              15 (<code object ensure_alive, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 553>)
+         554         222 LOAD_CONST              15 (<code object ensure_alive, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 554>)
                      224 MAKE_FUNCTION            0
                      226 STORE_NAME              24 (ensure_alive)
          
-         571         228 LOAD_CONST              16 ('name')
+         572         228 LOAD_CONST              16 ('name')
                      230 LOAD_NAME                5 (str)
                      232 LOAD_CONST               6 ('return')
                      234 LOAD_CONST               7 (None)
                      236 BUILD_TUPLE              4
-                     238 LOAD_CONST              17 (<code object start_scratch_command, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 571>)
+                     238 LOAD_CONST              17 (<code object start_scratch_command, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 572>)
                      240 MAKE_FUNCTION            4 (annotations)
                      242 STORE_NAME              25 (start_scratch_command)
          
-         588         244 LOAD_CONST              39 ((None,))
+         589         244 LOAD_CONST              39 ((None,))
                      246 LOAD_CONST              18 ('orig_scratch')
                      248 LOAD_NAME               26 (Scratch)
                      250 LOAD_CONST               7 (None)
                      252 BINARY_OP                7 (|)
                      256 LOAD_CONST               6 ('return')
                      258 LOAD_CONST               7 (None)
                      260 BUILD_TUPLE              4
-                     262 LOAD_CONST              19 (<code object updateScratchInfo, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 588>)
+                     262 LOAD_CONST              19 (<code object updateScratchInfo, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 589>)
                      264 MAKE_FUNCTION            5 (defaults, annotations)
                      266 STORE_NAME              27 (updateScratchInfo)
          
-         609         268 LOAD_CONST              37 (('return', None))
-                     270 LOAD_CONST              20 (<code object event_monitorremoved, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 609>)
+         610         268 LOAD_CONST              37 (('return', None))
+                     270 LOAD_CONST              20 (<code object event_monitorremoved, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 610>)
                      272 MAKE_FUNCTION            4 (annotations)
                      274 STORE_NAME              28 (event_monitorremoved)
          
-         615         276 LOAD_CONST              21 (<code object event_configreloaded, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 615>)
+         616         276 LOAD_CONST              21 (<code object event_configreloaded, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 616>)
                      278 MAKE_FUNCTION            0
                      280 STORE_NAME              29 (event_configreloaded)
          
-         621         282 LOAD_CONST              37 (('return', None))
-                     284 LOAD_CONST              22 (<code object event_activewindowv2, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 621>)
+         622         282 LOAD_CONST              37 (('return', None))
+                     284 LOAD_CONST              22 (<code object event_activewindowv2, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 622>)
                      286 MAKE_FUNCTION            4 (annotations)
                      288 STORE_NAME              30 (event_activewindowv2)
          
-         673         290 LOAD_CONST              23 (<code object _alternative_lookup, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 673>)
+         674         290 LOAD_CONST              23 (<code object _alternative_lookup, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 674>)
                      292 MAKE_FUNCTION            0
                      294 STORE_NAME              31 (_alternative_lookup)
          
-         693         296 LOAD_CONST              37 (('return', None))
-                     298 LOAD_CONST              24 (<code object event_openwindow, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 693>)
+         694         296 LOAD_CONST              37 (('return', None))
+                     298 LOAD_CONST              24 (<code object event_openwindow, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 694>)
                      300 MAKE_FUNCTION            4 (annotations)
                      302 STORE_NAME              32 (event_openwindow)
          
-         711         304 LOAD_CONST              25 ('uid_or_uids')
+         712         304 LOAD_CONST              25 ('uid_or_uids')
                      306 LOAD_NAME                5 (str)
                      308 LOAD_CONST               6 ('return')
                      310 LOAD_CONST               7 (None)
                      312 BUILD_TUPLE              4
-                     314 LOAD_CONST              26 (<code object run_toggle, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 711>)
+                     314 LOAD_CONST              26 (<code object run_toggle, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 712>)
                      316 MAKE_FUNCTION            4 (annotations)
                      318 STORE_NAME              33 (run_toggle)
          
-         747         320 LOAD_CONST              39 ((None,))
-                     322 LOAD_CONST              27 (<code object get_offsets, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 747>)
+         748         320 LOAD_CONST              39 ((None,))
+                     322 LOAD_CONST              27 (<code object get_offsets, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 748>)
                      324 MAKE_FUNCTION            1 (defaults)
                      326 STORE_NAME              34 (get_offsets)
          
-         754         328 LOAD_CONST              28 (<code object _anim_hide, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 754>)
+         755         328 LOAD_CONST              28 (<code object _hide_transition, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 755>)
                      330 MAKE_FUNCTION            0
-                     332 STORE_NAME              35 (_anim_hide)
+                     332 STORE_NAME              35 (_hide_transition)
          
-         762         334 LOAD_CONST              29 (<code object _slide_animation, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 762>)
+         768         334 LOAD_CONST              29 (<code object _slide_animation, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 768>)
                      336 MAKE_FUNCTION            0
                      338 STORE_NAME              36 (_slide_animation)
          
-         776         340 LOAD_CONST              37 (('return', None))
-                     342 LOAD_CONST              30 (<code object run_show, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 776>)
+         782         340 LOAD_CONST              37 (('return', None))
+                     342 LOAD_CONST              30 (<code object run_show, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 782>)
                      344 MAKE_FUNCTION            4 (annotations)
                      346 STORE_NAME              37 (run_show)
          
-         820         348 LOAD_CONST              31 (<code object _show_transition, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 820>)
+         826         348 LOAD_CONST              31 (<code object _show_transition, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 826>)
                      350 MAKE_FUNCTION            0
                      352 STORE_NAME              38 (_show_transition)
          
-         871         354 LOAD_CONST              32 (<code object _fix_size, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 871>)
+         878         354 LOAD_CONST              32 (<code object _fix_size, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 878>)
                      356 MAKE_FUNCTION            0
                      358 STORE_NAME              39 (_fix_size)
          
-         886         360 LOAD_CONST              33 (<code object _fix_position, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 886>)
+         893         360 LOAD_CONST              33 (<code object _fix_position, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 893>)
                      362 MAKE_FUNCTION            0
                      364 STORE_NAME              40 (_fix_position)
          
-         899         366 LOAD_CONST              40 ((False, False))
+         906         366 LOAD_CONST              40 ((False, False))
                      368 LOAD_CONST              35 ('uid')
                      370 LOAD_NAME                5 (str)
                      372 LOAD_CONST               6 ('return')
                      374 LOAD_CONST               7 (None)
                      376 BUILD_TUPLE              4
-                     378 LOAD_CONST              36 (<code object run_hide, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 899>)
+                     378 LOAD_CONST              36 (<code object run_hide, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 906>)
                      380 MAKE_FUNCTION            5 (defaults, annotations)
                      382 STORE_NAME              41 (run_hide)
                      384 LOAD_CLOSURE             0 (__class__)
                      386 COPY                     1
                      388 STORE_NAME              42 (__classcell__)
                      390 RETURN_VALUE
          consts
@@ -3953,245 +3953,255 @@
                lnotab
                   0x060236010401040136015a0136010601180132ff1e030c0142ff16050a
                   ff04045a0118011aff10045a0104011c011c0308010801080108fc040502
                   fb0c063802180116ff10043cde
             True
             code
                argcount  : 3
-               nlocals   : 6
+               nlocals   : 7
                stacksize : 7
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   000000000000000000000064017c016a020000000000000000a6020000ab
-                  020000000000000000010074070000000000000000000064026403a60200
-                  00ab020000000000000000440090015d4d7d037409000000000000000000
-                  006a0500000000000000007c0364047a08000064057a0b0000a6010000ab
-                  010000000000000000830064067b0356009703860401007c01a006000000
+                  02000000000000000001006402670164037a0500006404670164057a0500
+                  007a0000006406670164077a0500007a0000007d037c03440090015d477d
+                  047407000000000000000000006a0400000000000000007c04a6010000ab
+                  010000000000000000830064087b0356009703860401007c01a005000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
-                  00830064067b035600970386047d047c0473037c02900173047c00a00700
-                  000000000000000000000000000000000000007c016a0800000000000000
-                  00a00900000000000000000000000000000000000000006407a6010000ab
-                  010000000000000000a6010000ab01000000000000000072357c00a00a00
-                  000000000000000000000000000000000000007c016a0800000000000000
-                  00a00900000000000000000000000000000000000000006408a6010000ab
-                  010000000000000000ac09a6010000ab010000000000000000830064067b
-                  035600970386047d056e217c00a00a000000000000000000000000000000
-                  00000000007c016a0b0000000000000000ac0aa6010000ab010000000000
-                  000000830064067b035600970386047d057c05727f7c01a00c0000000000
-                  0000000000000000000000000000007c05a6010000ab0100000000000000
-                  00830064067b0356009703860401007c006a000000000000000000a00100
-                  00000000000000000000000000000000000000640b7c016a020000000000
-                  0000007c016a0b00000000000000007c016a0d0000000000000000a60400
-                  00ab04000000000000000001007c006a0e0000000000000000a00f000000
+                  00830064087b035600970386047d057c0573037c02900173047c00a00600
+                  000000000000000000000000000000000000007c016a0700000000000000
+                  00a00800000000000000000000000000000000000000006409a6010000ab
+                  010000000000000000a6010000ab01000000000000000072357c00a00900
+                  000000000000000000000000000000000000007c016a0700000000000000
+                  00a0080000000000000000000000000000000000000000640aa6010000ab
+                  010000000000000000ac0ba6010000ab010000000000000000830064087b
+                  035600970386047d066e217c00a009000000000000000000000000000000
+                  00000000007c016a0a0000000000000000ac0ca6010000ab010000000000
+                  000000830064087b035600970386047d067c06727f7c01a00b0000000000
+                  0000000000000000000000000000007c06a6010000ab0100000000000000
+                  00830064087b0356009703860401007c006a000000000000000000a00100
+                  00000000000000000000000000000000000000640d7c016a020000000000
+                  0000007c016a0a00000000000000007c016a0c0000000000000000a60400
+                  00ab04000000000000000001007c006a0d0000000000000000a00e000000
                   00000000000000000000000000000000007c01a6010000ab010000000000
-                  00000001007c006a0e0000000000000000a0100000000000000000000000
-                  0000000000000000007c01640ca6020000ab020000000000000000010001
-                  00640d53007c0272057c0473030100640e530090018c4f640e5300
+                  00000001007c006a0d0000000000000000a00f0000000000000000000000
+                  0000000000000000007c01640ea6020000ab020000000000000000010001
+                  00640f53007c0272057c05730301006410530090018c4964105300
                482           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
                486           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (log)
                             18 LOAD_METHOD              1 (info)
                             40 LOAD_CONST               1 ('==> Wait for %s spawning')
                             42 LOAD_FAST                1 (item)
                             44 LOAD_ATTR                2 (uid)
                             54 PRECALL                  2
                             58 CALL                     2
                             68 POP_TOP
                
-               487          70 LOAD_GLOBAL              7 (NULL + range)
-                            82 LOAD_CONST               2 (1)
-                            84 LOAD_CONST               3 (8)
-                            86 PRECALL                  2
-                            90 CALL                     2
-                           100 GET_ITER
-                       >>  102 EXTENDED_ARG             1
-                           104 FOR_ITER               333 (to 772)
-                           106 STORE_FAST               3 (loop_count)
-               
-               488         108 LOAD_GLOBAL              9 (NULL + asyncio)
-                           120 LOAD_ATTR                5 (sleep)
-                           130 LOAD_FAST                3 (loop_count)
-                           132 LOAD_CONST               4 (2)
-                           134 BINARY_OP                8 (**)
-                           138 LOAD_CONST               5 (10.0)
-                           140 BINARY_OP               11 (/)
+               487          70 LOAD_CONST               2 (0.1)
+                            72 BUILD_LIST               1
+                            74 LOAD_CONST               3 (10)
+                            76 BINARY_OP                5 (*)
+                            80 LOAD_CONST               4 (0.2)
+                            82 BUILD_LIST               1
+                            84 LOAD_CONST               5 (20)
+                            86 BINARY_OP                5 (*)
+                            90 BINARY_OP                0 (+)
+                            94 LOAD_CONST               6 (0.5)
+                            96 BUILD_LIST               1
+                            98 LOAD_CONST               7 (15)
+                           100 BINARY_OP                5 (*)
+                           104 BINARY_OP                0 (+)
+                           108 STORE_FAST               3 (interval_range)
+               
+               488         110 LOAD_FAST                3 (interval_range)
+                           112 GET_ITER
+                       >>  114 EXTENDED_ARG             1
+                           116 FOR_ITER               327 (to 772)
+                           118 STORE_FAST               4 (interval)
+               
+               489         120 LOAD_GLOBAL              7 (NULL + asyncio)
+                           132 LOAD_ATTR                4 (sleep)
+                           142 LOAD_FAST                4 (interval)
                            144 PRECALL                  1
                            148 CALL                     1
                            158 GET_AWAITABLE            0
-                           160 LOAD_CONST               6 (None)
+                           160 LOAD_CONST               8 (None)
                        >>  162 SEND                     3 (to 170)
                            164 YIELD_VALUE
                            166 RESUME                   3
                            168 JUMP_BACKWARD_NO_INTERRUPT     4 (to 162)
                        >>  170 POP_TOP
                
-               489         172 LOAD_FAST                1 (item)
-                           174 LOAD_METHOD              6 (isAlive)
+               490         172 LOAD_FAST                1 (item)
+                           174 LOAD_METHOD              5 (isAlive)
                            196 PRECALL                  0
                            200 CALL                     0
                            210 GET_AWAITABLE            0
-                           212 LOAD_CONST               6 (None)
+                           212 LOAD_CONST               8 (None)
                        >>  214 SEND                     3 (to 222)
                            216 YIELD_VALUE
                            218 RESUME                   3
                            220 JUMP_BACKWARD_NO_INTERRUPT     4 (to 214)
-                       >>  222 STORE_FAST               4 (is_alive)
+                       >>  222 STORE_FAST               5 (is_alive)
                
-               492         224 LOAD_FAST                4 (is_alive)
+               493         224 LOAD_FAST                5 (is_alive)
                            226 POP_JUMP_FORWARD_IF_TRUE     3 (to 234)
                            228 LOAD_FAST                2 (use_proc)
                            230 EXTENDED_ARG             1
                            232 POP_JUMP_FORWARD_IF_TRUE   260 (to 754)
                
-               493     >>  234 LOAD_FAST                0 (self)
-                           236 LOAD_METHOD              7 (cast_bool)
+               494     >>  234 LOAD_FAST                0 (self)
+                           236 LOAD_METHOD              6 (cast_bool)
                            258 LOAD_FAST                1 (item)
-                           260 LOAD_ATTR                8 (conf)
-                           270 LOAD_METHOD              9 (get)
-                           292 LOAD_CONST               7 ('class_match')
+                           260 LOAD_ATTR                7 (conf)
+                           270 LOAD_METHOD              8 (get)
+                           292 LOAD_CONST               9 ('class_match')
                            294 PRECALL                  1
                            298 CALL                     1
                            308 PRECALL                  1
                            312 CALL                     1
                            322 POP_JUMP_FORWARD_IF_FALSE    53 (to 430)
                
-               494         324 LOAD_FAST                0 (self)
-                           326 LOAD_METHOD             10 (get_client_props)
+               495         324 LOAD_FAST                0 (self)
+                           326 LOAD_METHOD              9 (get_client_props)
                            348 LOAD_FAST                1 (item)
-                           350 LOAD_ATTR                8 (conf)
-                           360 LOAD_METHOD              9 (get)
-                           382 LOAD_CONST               8 ('class')
+                           350 LOAD_ATTR                7 (conf)
+                           360 LOAD_METHOD              8 (get)
+                           382 LOAD_CONST              10 ('class')
                            384 PRECALL                  1
                            388 CALL                     1
-                           398 KW_NAMES                 9
+                           398 KW_NAMES                11
                            400 PRECALL                  1
                            404 CALL                     1
                            414 GET_AWAITABLE            0
-                           416 LOAD_CONST               6 (None)
+                           416 LOAD_CONST               8 (None)
                        >>  418 SEND                     3 (to 426)
                            420 YIELD_VALUE
                            422 RESUME                   3
                            424 JUMP_BACKWARD_NO_INTERRUPT     4 (to 418)
-                       >>  426 STORE_FAST               5 (info)
+                       >>  426 STORE_FAST               6 (info)
                            428 JUMP_FORWARD            33 (to 496)
                
-               496     >>  430 LOAD_FAST                0 (self)
-                           432 LOAD_METHOD             10 (get_client_props)
+               497     >>  430 LOAD_FAST                0 (self)
+                           432 LOAD_METHOD              9 (get_client_props)
                            454 LOAD_FAST                1 (item)
-                           456 LOAD_ATTR               11 (pid)
-                           466 KW_NAMES                10
+                           456 LOAD_ATTR               10 (pid)
+                           466 KW_NAMES                12
                            468 PRECALL                  1
                            472 CALL                     1
                            482 GET_AWAITABLE            0
-                           484 LOAD_CONST               6 (None)
+                           484 LOAD_CONST               8 (None)
                        >>  486 SEND                     3 (to 494)
                            488 YIELD_VALUE
                            490 RESUME                   3
                            492 JUMP_BACKWARD_NO_INTERRUPT     4 (to 486)
-                       >>  494 STORE_FAST               5 (info)
+                       >>  494 STORE_FAST               6 (info)
                
-               497     >>  496 LOAD_FAST                5 (info)
+               498     >>  496 LOAD_FAST                6 (info)
                            498 POP_JUMP_FORWARD_IF_FALSE   127 (to 754)
                
-               498         500 LOAD_FAST                1 (item)
-                           502 LOAD_METHOD             12 (updateClientInfo)
-                           524 LOAD_FAST                5 (info)
+               499         500 LOAD_FAST                1 (item)
+                           502 LOAD_METHOD             11 (updateClientInfo)
+                           524 LOAD_FAST                6 (info)
                            526 PRECALL                  1
                            530 CALL                     1
                            540 GET_AWAITABLE            0
-                           542 LOAD_CONST               6 (None)
+                           542 LOAD_CONST               8 (None)
                        >>  544 SEND                     3 (to 552)
                            546 YIELD_VALUE
                            548 RESUME                   3
                            550 JUMP_BACKWARD_NO_INTERRUPT     4 (to 544)
                        >>  552 POP_TOP
                
-               499         554 LOAD_FAST                0 (self)
+               500         554 LOAD_FAST                0 (self)
                            556 LOAD_ATTR                0 (log)
                            566 LOAD_METHOD              1 (info)
                
-               500         588 LOAD_CONST              11 ('=> %s client (proc:%s, addr:%s) detected on time')
+               501         588 LOAD_CONST              13 ('=> %s client (proc:%s, addr:%s) detected on time')
                
-               501         590 LOAD_FAST                1 (item)
+               502         590 LOAD_FAST                1 (item)
                            592 LOAD_ATTR                2 (uid)
                
-               502         602 LOAD_FAST                1 (item)
-                           604 LOAD_ATTR               11 (pid)
+               503         602 LOAD_FAST                1 (item)
+                           604 LOAD_ATTR               10 (pid)
                
-               503         614 LOAD_FAST                1 (item)
-                           616 LOAD_ATTR               13 (full_address)
+               504         614 LOAD_FAST                1 (item)
+                           616 LOAD_ATTR               12 (full_address)
                
-               499         626 PRECALL                  4
+               500         626 PRECALL                  4
                            630 CALL                     4
                            640 POP_TOP
                
-               505         642 LOAD_FAST                0 (self)
-                           644 LOAD_ATTR               14 (scratches)
-                           654 LOAD_METHOD             15 (register)
+               506         642 LOAD_FAST                0 (self)
+                           644 LOAD_ATTR               13 (scratches)
+                           654 LOAD_METHOD             14 (register)
                            676 LOAD_FAST                1 (item)
                            678 PRECALL                  1
                            682 CALL                     1
                            692 POP_TOP
                
-               506         694 LOAD_FAST                0 (self)
-                           696 LOAD_ATTR               14 (scratches)
-                           706 LOAD_METHOD             16 (clearState)
+               507         694 LOAD_FAST                0 (self)
+                           696 LOAD_ATTR               13 (scratches)
+                           706 LOAD_METHOD             15 (clearState)
                            728 LOAD_FAST                1 (item)
-                           730 LOAD_CONST              12 ('respawned')
+                           730 LOAD_CONST              14 ('respawned')
                            732 PRECALL                  2
                            736 CALL                     2
                            746 POP_TOP
                
-               507         748 POP_TOP
-                           750 LOAD_CONST              13 (True)
+               508         748 POP_TOP
+                           750 LOAD_CONST              15 (True)
                            752 RETURN_VALUE
                
-               508     >>  754 LOAD_FAST                2 (use_proc)
+               509     >>  754 LOAD_FAST                2 (use_proc)
                            756 POP_JUMP_FORWARD_IF_FALSE     5 (to 768)
-                           758 LOAD_FAST                4 (is_alive)
+                           758 LOAD_FAST                5 (is_alive)
                            760 POP_JUMP_FORWARD_IF_TRUE     3 (to 768)
                
-               509         762 POP_TOP
-                           764 LOAD_CONST              14 (False)
+               510         762 POP_TOP
+                           764 LOAD_CONST              16 (False)
                            766 RETURN_VALUE
                        >>  768 EXTENDED_ARG             1
-                           770 JUMP_BACKWARD          335 (to 102)
+                           770 JUMP_BACKWARD          329 (to 114)
                
-               510     >>  772 LOAD_CONST              14 (False)
+               511     >>  772 LOAD_CONST              16 (False)
                            774 RETURN_VALUE
                consts
                   "Waits for a client to be up and running\n        if `class_match` is enabled, will use the class, else the process's PID will be used.\n        "
                   '==> Wait for %s spawning'
-                  1
-                  8
-                  2
-                  10.0
+                  0.1
+                  10
+                  0.2
+                  20
+                  0.5
+                  15
                   None
                   'class_match'
                   'class'
                   ('cls',)
                   ('pid',)
                   '=> %s client (proc:%s, addr:%s) detected on time'
                   'respawned'
                   True
                   False
-               names      ('log', 'info', 'uid', 'range', 'asyncio', 'sleep', 'isAlive', 'cast_bool', 'conf', 'get', 'get_client_props', 'pid', 'updateClientInfo', 'full_address', 'scratches', 'register', 'clearState')
-               varnames   ('self', 'item', 'use_proc', 'loop_count', 'is_alive', 'info')
+               names      ('log', 'info', 'uid', 'asyncio', 'sleep', 'isAlive', 'cast_bool', 'conf', 'get', 'get_client_props', 'pid', 'updateClientInfo', 'full_address', 'scratches', 'register', 'clearState')
+               varnames   ('self', 'item', 'use_proc', 'interval_range', 'interval', 'is_alive', 'info')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       '__wait_for_client'
                firstlineno 482
                lnotab
-                  0x060440012601400134030a015a016a02420104013601220102010c010c
-                  010cfc100634013601060108010a01
+                  0x0604400128010a01340134030a015a016a02420104013601220102010c
+                  010c010cfc100634013601060108010a01
             code
                argcount  : 2
                nlocals   : 5
                stacksize : 5
                flags     : 131
                code
                   0x4b00010097007c016a0000000000000000007d02740300000000000000
@@ -4201,107 +4211,107 @@
                   00000000000000a00400000000000000000000000000000000000000007c
                   01a6010000ab01000000000000000001007c00a005000000000000000000
                   00000000000000000000007c02a6010000ab010000000000000000830064
                   037b0356009703860401007c00a006000000000000000000000000000000
                   00000000007c016402ac04a6020000ab020000000000000000830064037b
                   035600970386047d0464057c015f0700000000000000007c045300640553
                   00
-               512           0 RETURN_GENERATOR
+               513           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               514           6 LOAD_FAST                1 (item)
+               515           6 LOAD_FAST                1 (item)
                              8 LOAD_ATTR                0 (uid)
                             18 STORE_FAST               2 (uid)
                
-               515          20 LOAD_GLOBAL              3 (NULL + getattr)
+               516          20 LOAD_GLOBAL              3 (NULL + getattr)
                             32 LOAD_FAST                1 (item)
                             34 LOAD_CONST               1 ('bogus_pid')
                             36 LOAD_CONST               2 (False)
                             38 PRECALL                  3
                             42 CALL                     3
                             52 STORE_FAST               3 (started)
                
-               516          54 LOAD_FAST                1 (item)
+               517          54 LOAD_FAST                1 (item)
                             56 LOAD_METHOD              2 (isAlive)
                             78 PRECALL                  0
                             82 CALL                     0
                             92 GET_AWAITABLE            0
                             94 LOAD_CONST               3 (None)
                        >>   96 SEND                     3 (to 104)
                             98 YIELD_VALUE
                            100 RESUME                   3
                            102 JUMP_BACKWARD_NO_INTERRUPT     4 (to 96)
                        >>  104 POP_JUMP_FORWARD_IF_TRUE     2 (to 110)
                
-               517         106 LOAD_CONST               2 (False)
+               518         106 LOAD_CONST               2 (False)
                            108 STORE_FAST               3 (started)
                
-               518     >>  110 LOAD_FAST                3 (started)
+               519     >>  110 LOAD_FAST                3 (started)
                            112 POP_JUMP_FORWARD_IF_TRUE    91 (to 296)
                
-               519         114 LOAD_FAST                0 (self)
+               520         114 LOAD_FAST                0 (self)
                            116 LOAD_ATTR                3 (scratches)
                            126 LOAD_METHOD              4 (reset)
                            148 LOAD_FAST                1 (item)
                            150 PRECALL                  1
                            154 CALL                     1
                            164 POP_TOP
                
-               520         166 LOAD_FAST                0 (self)
+               521         166 LOAD_FAST                0 (self)
                            168 LOAD_METHOD              5 (start_scratch_command)
                            190 LOAD_FAST                2 (uid)
                            192 PRECALL                  1
                            196 CALL                     1
                            206 GET_AWAITABLE            0
                            208 LOAD_CONST               3 (None)
                        >>  210 SEND                     3 (to 218)
                            212 YIELD_VALUE
                            214 RESUME                   3
                            216 JUMP_BACKWARD_NO_INTERRUPT     4 (to 210)
                        >>  218 POP_TOP
                
-               521         220 LOAD_FAST                0 (self)
+               522         220 LOAD_FAST                0 (self)
                            222 LOAD_METHOD              6 (_Extension__wait_for_client)
                            244 LOAD_FAST                1 (item)
                            246 LOAD_CONST               2 (False)
                            248 KW_NAMES                 4
                            250 PRECALL                  2
                            254 CALL                     2
                            264 GET_AWAITABLE            0
                            266 LOAD_CONST               3 (None)
                        >>  268 SEND                     3 (to 276)
                            270 YIELD_VALUE
                            272 RESUME                   3
                            274 JUMP_BACKWARD_NO_INTERRUPT     4 (to 268)
                        >>  276 STORE_FAST               4 (r)
                
-               522         278 LOAD_CONST               5 (True)
+               523         278 LOAD_CONST               5 (True)
                            280 LOAD_FAST                1 (item)
                            282 STORE_ATTR               7 (bogus_pid)
                
-               523         292 LOAD_FAST                4 (r)
+               524         292 LOAD_FAST                4 (r)
                            294 RETURN_VALUE
                
-               524     >>  296 LOAD_CONST               5 (True)
+               525     >>  296 LOAD_CONST               5 (True)
                            298 RETURN_VALUE
                consts
                   'Ensure alive, PWA version'
                   'bogus_pid'
                   False
                   None
                   ('use_proc',)
                   True
                names      ('uid', 'getattr', 'isAlive', 'scratches', 'reset', 'start_scratch_command', '_Extension__wait_for_client', 'bogus_pid')
                varnames   ('self', 'item', 'uid', 'started', 'r')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       '_start_scratch_classbased'
-               firstlineno 512
+               firstlineno 513
                lnotab 0x06020e012201340104010401340136013a010e010401
             code
                argcount  : 2
                nlocals   : 5
                stacksize : 5
                flags     : 131
                code
@@ -4326,188 +4336,188 @@
                   0356009703860401007c006a0100000000000000007c0219000000000000
                   0000006a0e00000000000000007d047c04720664057c049b009d027d036e
                   0264067d037c006a070000000000000000a00a0000000000000000000000
                   00000000000000000064077c016a0f000000000000000064081900000000
                   00000000007c03a6030000ab030000000000000000010074210000000000
                   00000000007c03a6010000ab010000000000000000830064017b03560097
                   038604010064095300640a5300
-               526           0 RETURN_GENERATOR
+               527           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               528           6 LOAD_FAST                1 (item)
+               529           6 LOAD_FAST                1 (item)
                              8 LOAD_ATTR                0 (uid)
                             18 STORE_FAST               2 (uid)
                
-               529          20 LOAD_FAST                2 (uid)
+               530          20 LOAD_FAST                2 (uid)
                             22 LOAD_FAST                0 (self)
                             24 LOAD_ATTR                1 (procs)
                             34 CONTAINS_OP              0
                             36 POP_JUMP_FORWARD_IF_FALSE    49 (to 136)
                
-               530          38 NOP
+               531          38 NOP
                
-               531          40 LOAD_FAST                0 (self)
+               532          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                1 (procs)
                             52 LOAD_FAST                2 (uid)
                             54 BINARY_SUBSCR
                             64 LOAD_METHOD              2 (kill)
                             86 PRECALL                  0
                             90 CALL                     0
                            100 POP_TOP
                            102 JUMP_FORWARD            16 (to 136)
                        >>  104 PUSH_EXC_INFO
                
-               532         106 LOAD_GLOBAL              6 (ProcessLookupError)
+               533         106 LOAD_GLOBAL              6 (ProcessLookupError)
                            118 CHECK_EXC_MATCH
                            120 POP_JUMP_FORWARD_IF_FALSE     3 (to 128)
                            122 POP_TOP
                
-               533         124 POP_EXCEPT
+               534         124 POP_EXCEPT
                            126 JUMP_FORWARD             4 (to 136)
                
-               532     >>  128 RERAISE                  0
+               533     >>  128 RERAISE                  0
                        >>  130 COPY                     3
                            132 POP_EXCEPT
                            134 RERAISE                  1
                
-               534     >>  136 LOAD_FAST                0 (self)
+               535     >>  136 LOAD_FAST                0 (self)
                            138 LOAD_ATTR                4 (scratches)
                            148 LOAD_METHOD              5 (reset)
                            170 LOAD_FAST                1 (item)
                            172 PRECALL                  1
                            176 CALL                     1
                            186 POP_TOP
                
-               535         188 LOAD_FAST                0 (self)
+               536         188 LOAD_FAST                0 (self)
                            190 LOAD_METHOD              6 (start_scratch_command)
                            212 LOAD_FAST                2 (uid)
                            214 PRECALL                  1
                            218 CALL                     1
                            228 GET_AWAITABLE            0
                            230 LOAD_CONST               1 (None)
                        >>  232 SEND                     3 (to 240)
                            234 YIELD_VALUE
                            236 RESUME                   3
                            238 JUMP_BACKWARD_NO_INTERRUPT     4 (to 232)
                        >>  240 POP_TOP
                
-               536         242 LOAD_FAST                0 (self)
+               537         242 LOAD_FAST                0 (self)
                            244 LOAD_ATTR                7 (log)
                            254 LOAD_METHOD              8 (info)
                            276 LOAD_CONST               2 ('starting %s')
                            278 LOAD_FAST                2 (uid)
                            280 PRECALL                  2
                            284 CALL                     2
                            294 POP_TOP
                
-               537         296 LOAD_FAST                0 (self)
+               538         296 LOAD_FAST                0 (self)
                            298 LOAD_METHOD              9 (_Extension__wait_for_client)
                            320 LOAD_FAST                1 (item)
                            322 PRECALL                  1
                            326 CALL                     1
                            336 GET_AWAITABLE            0
                            338 LOAD_CONST               1 (None)
                        >>  340 SEND                     3 (to 348)
                            342 YIELD_VALUE
                            344 RESUME                   3
                            346 JUMP_BACKWARD_NO_INTERRUPT     4 (to 340)
                        >>  348 POP_JUMP_FORWARD_IF_TRUE   189 (to 728)
                
-               538         350 LOAD_FAST                0 (self)
+               539         350 LOAD_FAST                0 (self)
                            352 LOAD_ATTR                7 (log)
                            362 LOAD_METHOD             10 (error)
                            384 LOAD_CONST               3 ('⚠ Failed spawning %s as proc %s')
                            386 LOAD_FAST                2 (uid)
                            388 LOAD_FAST                1 (item)
                            390 LOAD_ATTR               11 (pid)
                            400 PRECALL                  3
                            404 CALL                     3
                            414 POP_TOP
                
-               539         416 LOAD_FAST                1 (item)
+               540         416 LOAD_FAST                1 (item)
                            418 LOAD_METHOD             12 (isAlive)
                            440 PRECALL                  0
                            444 CALL                     0
                            454 GET_AWAITABLE            0
                            456 LOAD_CONST               1 (None)
                        >>  458 SEND                     3 (to 466)
                            460 YIELD_VALUE
                            462 RESUME                   3
                            464 JUMP_BACKWARD_NO_INTERRUPT     4 (to 458)
                        >>  466 POP_JUMP_FORWARD_IF_FALSE     3 (to 474)
                
-               540         468 LOAD_CONST               4 ("The command didn't open a window")
+               541         468 LOAD_CONST               4 ("The command didn't open a window")
                            470 STORE_FAST               3 (error)
                            472 JUMP_FORWARD            65 (to 604)
                
-               542     >>  474 LOAD_FAST                0 (self)
+               543     >>  474 LOAD_FAST                0 (self)
                            476 LOAD_ATTR                1 (procs)
                            486 LOAD_FAST                2 (uid)
                            488 BINARY_SUBSCR
                            498 LOAD_METHOD             13 (communicate)
                            520 PRECALL                  0
                            524 CALL                     0
                            534 GET_AWAITABLE            0
                            536 LOAD_CONST               1 (None)
                        >>  538 SEND                     3 (to 546)
                            540 YIELD_VALUE
                            542 RESUME                   3
                            544 JUMP_BACKWARD_NO_INTERRUPT     4 (to 538)
                        >>  546 POP_TOP
                
-               543         548 LOAD_FAST                0 (self)
+               544         548 LOAD_FAST                0 (self)
                            550 LOAD_ATTR                1 (procs)
                            560 LOAD_FAST                2 (uid)
                            562 BINARY_SUBSCR
                            572 LOAD_ATTR               14 (returncode)
                            582 STORE_FAST               4 (code)
                
-               544         584 LOAD_FAST                4 (code)
+               545         584 LOAD_FAST                4 (code)
                            586 POP_JUMP_FORWARD_IF_FALSE     6 (to 600)
                
-               545         588 LOAD_CONST               5 ('The command failed with code ')
+               546         588 LOAD_CONST               5 ('The command failed with code ')
                            590 LOAD_FAST                4 (code)
                            592 FORMAT_VALUE             0
                            594 BUILD_STRING             2
                            596 STORE_FAST               3 (error)
                            598 JUMP_FORWARD             2 (to 604)
                
-               547     >>  600 LOAD_CONST               6 ('The command terminated sucessfully, is it already running?')
+               548     >>  600 LOAD_CONST               6 ('The command terminated sucessfully, is it already running?')
                            602 STORE_FAST               3 (error)
                
-               548     >>  604 LOAD_FAST                0 (self)
+               549     >>  604 LOAD_FAST                0 (self)
                            606 LOAD_ATTR                7 (log)
                            616 LOAD_METHOD             10 (error)
                            638 LOAD_CONST               7 ('"%s": %s')
                            640 LOAD_FAST                1 (item)
                            642 LOAD_ATTR               15 (conf)
                            652 LOAD_CONST               8 ('command')
                            654 BINARY_SUBSCR
                            664 LOAD_FAST                3 (error)
                            666 PRECALL                  3
                            670 CALL                     3
                            680 POP_TOP
                
-               549         682 LOAD_GLOBAL             33 (NULL + notify_error)
+               550         682 LOAD_GLOBAL             33 (NULL + notify_error)
                            694 LOAD_FAST                3 (error)
                            696 PRECALL                  1
                            700 CALL                     1
                            710 GET_AWAITABLE            0
                            712 LOAD_CONST               1 (None)
                        >>  714 SEND                     3 (to 722)
                            716 YIELD_VALUE
                            718 RESUME                   3
                            720 JUMP_BACKWARD_NO_INTERRUPT     4 (to 714)
                        >>  722 POP_TOP
                
-               550         724 LOAD_CONST               9 (False)
+               551         724 LOAD_CONST               9 (False)
                            726 RETURN_VALUE
                
-               551     >>  728 LOAD_CONST              10 (True)
+               552     >>  728 LOAD_CONST              10 (True)
                            730 RETURN_VALUE
                ExceptionTable:
                  40 to 100 -> 104 [0]
                  104 to 122 -> 130 [1] lasti
                  128 to 128 -> 130 [1] lasti
                consts
                   'Ensure alive, standard version'
@@ -4523,15 +4533,15 @@
                   True
                names      ('uid', 'procs', 'kill', 'ProcessLookupError', 'scratches', 'reset', 'start_scratch_command', 'log', 'info', '_Extension__wait_for_client', 'error', 'pid', 'isAlive', 'communicate', 'returncode', 'conf', 'notify_error')
                varnames   ('self', 'item', 'uid', 'error', 'code')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       '_start_scratch'
-               firstlineno 526
+               firstlineno 527
                lnotab
                   0x06020e01120102014201120104ff080234013601360136014201340106
                   024a01240104010c0204014e012a010401
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 5
@@ -4550,93 +4560,93 @@
                   0064057c01a6020000ab02000000000000000001007c00a0080000000000
                   0000000000000000000000000000007c02a6010000ab0100000000000000
                   00830064027b03560097038604732074130000000000000000000064067c
                   026a0a00000000000000009b0064079d03a6010000ab0100000000000000
                   00830064027b03560097038604010064085300640453007c00a00b000000
                   00000000000000000000000000000000007c02a6010000ab010000000000
                   000000830064027b035600970386045300
-               553           0 RETURN_GENERATOR
+               554           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               557           6 LOAD_FAST                0 (self)
+               558           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (scratches)
                             18 LOAD_METHOD              1 (get)
                             40 LOAD_FAST                1 (uid)
                             42 KW_NAMES                 1
                             44 PRECALL                  1
                             48 CALL                     1
                             58 STORE_FAST               2 (item)
                
-               558          60 LOAD_FAST                0 (self)
+               559          60 LOAD_FAST                0 (self)
                             62 LOAD_METHOD              2 (_configure_windowrules)
                             84 LOAD_FAST                2 (item)
                             86 PRECALL                  1
                             90 CALL                     1
                            100 GET_AWAITABLE            0
                            102 LOAD_CONST               2 (None)
                        >>  104 SEND                     3 (to 112)
                            106 YIELD_VALUE
                            108 RESUME                   3
                            110 JUMP_BACKWARD_NO_INTERRUPT     4 (to 104)
                        >>  112 POP_TOP
                
-               559         114 LOAD_FAST                2 (item)
+               560         114 LOAD_FAST                2 (item)
                            116 POP_JUMP_FORWARD_IF_TRUE     2 (to 122)
                            118 LOAD_ASSERTION_ERROR
                            120 RAISE_VARARGS            1
                
-               561     >>  122 LOAD_FAST                0 (self)
+               562     >>  122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD              3 (cast_bool)
                            146 LOAD_FAST                2 (item)
                            148 LOAD_ATTR                4 (conf)
                            158 LOAD_METHOD              1 (get)
                            180 LOAD_CONST               3 ('process_tracking')
                            182 PRECALL                  1
                            186 CALL                     1
                            196 LOAD_CONST               4 (True)
                            198 PRECALL                  2
                            202 CALL                     2
                            212 POP_JUMP_FORWARD_IF_FALSE   114 (to 442)
                
-               562         214 LOAD_FAST                2 (item)
+               563         214 LOAD_FAST                2 (item)
                            216 LOAD_METHOD              5 (isAlive)
                            238 PRECALL                  0
                            242 CALL                     0
                            252 GET_AWAITABLE            0
                            254 LOAD_CONST               2 (None)
                        >>  256 SEND                     3 (to 264)
                            258 YIELD_VALUE
                            260 RESUME                   3
                            262 JUMP_BACKWARD_NO_INTERRUPT     4 (to 256)
                        >>  264 POP_JUMP_FORWARD_IF_TRUE    86 (to 438)
                
-               563         266 LOAD_FAST                0 (self)
+               564         266 LOAD_FAST                0 (self)
                            268 LOAD_ATTR                6 (log)
                            278 LOAD_METHOD              7 (info)
                            300 LOAD_CONST               5 ('%s is not running, starting...')
                            302 LOAD_FAST                1 (uid)
                            304 PRECALL                  2
                            308 CALL                     2
                            318 POP_TOP
                
-               564         320 LOAD_FAST                0 (self)
+               565         320 LOAD_FAST                0 (self)
                            322 LOAD_METHOD              8 (_start_scratch)
                            344 LOAD_FAST                2 (item)
                            346 PRECALL                  1
                            350 CALL                     1
                            360 GET_AWAITABLE            0
                            362 LOAD_CONST               2 (None)
                        >>  364 SEND                     3 (to 372)
                            366 YIELD_VALUE
                            368 RESUME                   3
                            370 JUMP_BACKWARD_NO_INTERRUPT     4 (to 364)
                        >>  372 POP_JUMP_FORWARD_IF_TRUE    32 (to 438)
                
-               565         374 LOAD_GLOBAL             19 (NULL + notify_error)
+               566         374 LOAD_GLOBAL             19 (NULL + notify_error)
                            386 LOAD_CONST               6 ('Failed to show scratch "')
                            388 LOAD_FAST                2 (item)
                            390 LOAD_ATTR               10 (uid)
                            400 FORMAT_VALUE             0
                            402 LOAD_CONST               7 ('"')
                            404 BUILD_STRING             3
                            406 PRECALL                  1
@@ -4645,21 +4655,21 @@
                            422 LOAD_CONST               2 (None)
                        >>  424 SEND                     3 (to 432)
                            426 YIELD_VALUE
                            428 RESUME                   3
                            430 JUMP_BACKWARD_NO_INTERRUPT     4 (to 424)
                        >>  432 POP_TOP
                
-               566         434 LOAD_CONST               8 (False)
+               567         434 LOAD_CONST               8 (False)
                            436 RETURN_VALUE
                
-               567     >>  438 LOAD_CONST               4 (True)
+               568     >>  438 LOAD_CONST               4 (True)
                            440 RETURN_VALUE
                
-               569     >>  442 LOAD_FAST                0 (self)
+               570     >>  442 LOAD_FAST                0 (self)
                            444 LOAD_METHOD             11 (_start_scratch_classbased)
                            466 LOAD_FAST                2 (item)
                            468 PRECALL                  1
                            472 CALL                     1
                            482 GET_AWAITABLE            0
                            484 LOAD_CONST               2 (None)
                        >>  486 SEND                     3 (to 494)
@@ -4679,15 +4689,15 @@
                   False
                names      ('scratches', 'get', '_configure_windowrules', 'cast_bool', 'conf', 'isAlive', 'log', 'info', '_start_scratch', 'notify_error', 'uid', '_start_scratch_classbased')
                varnames   ('self', 'uid', 'item')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'ensure_alive'
-               firstlineno 553
+               firstlineno 554
                lnotab 0x06043601360108025c013401360136013c0104010402
             'name'
             code
                argcount  : 2
                nlocals   : 6
                stacksize : 7
                flags     : 131
@@ -4707,55 +4717,55 @@
                   0000007c027c05ac05a6020000ab02000000000000000001007c006a0a00
                   00000000000000a00b000000000000000000000000000000000000000064
                   067c026a0c00000000000000007c026a070000000000000000a001000000
                   00000000000000000000000000000000006403a6010000ab010000000000
                   0000007c05a6040000ab04000000000000000001007c03721d7c006a0000
                   00000000000000a00d00000000000000000000000000000000000000007c
                   03ac05a6010000ab01000000000000000001006404530064045300
-               571           0 RETURN_GENERATOR
+               572           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               573           6 LOAD_FAST                0 (self)
+               574           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (scratches)
                             18 LOAD_METHOD              1 (get)
                             40 LOAD_FAST                1 (name)
                             42 PRECALL                  1
                             46 CALL                     1
                             56 STORE_FAST               2 (scratch)
                
-               574          58 LOAD_FAST                2 (scratch)
+               575          58 LOAD_FAST                2 (scratch)
                             60 POP_JUMP_FORWARD_IF_TRUE     2 (to 66)
                             62 LOAD_ASSERTION_ERROR
                             64 RAISE_VARARGS            1
                
-               575     >>   66 LOAD_FAST                0 (self)
+               576     >>   66 LOAD_FAST                0 (self)
                             68 LOAD_ATTR                0 (scratches)
                             78 LOAD_METHOD              2 (setState)
                            100 LOAD_FAST                2 (scratch)
                            102 LOAD_CONST               1 ('respawned')
                            104 PRECALL                  2
                            108 CALL                     2
                            118 POP_TOP
                
-               576         120 LOAD_FAST                1 (name)
+               577         120 LOAD_FAST                1 (name)
                            122 LOAD_FAST                0 (self)
                            124 LOAD_ATTR                3 (procs)
                            134 CONTAINS_OP              0
                            136 POP_JUMP_FORWARD_IF_FALSE    18 (to 174)
                            138 LOAD_FAST                0 (self)
                            140 LOAD_ATTR                3 (procs)
                            150 LOAD_FAST                1 (name)
                            152 BINARY_SUBSCR
                            162 LOAD_ATTR                4 (pid)
                            172 JUMP_FORWARD             1 (to 176)
                        >>  174 LOAD_CONST               2 (0)
                        >>  176 STORE_FAST               3 (old_pid)
                
-               577         178 LOAD_GLOBAL             11 (NULL + asyncio)
+               578         178 LOAD_GLOBAL             11 (NULL + asyncio)
                            190 LOAD_ATTR                6 (create_subprocess_shell)
                            200 LOAD_FAST                2 (scratch)
                            202 LOAD_ATTR                7 (conf)
                            212 LOAD_CONST               3 ('command')
                            214 BINARY_SUBSCR
                            224 PRECALL                  1
                            228 CALL                     1
@@ -4763,75 +4773,75 @@
                            240 LOAD_CONST               4 (None)
                        >>  242 SEND                     3 (to 250)
                            244 YIELD_VALUE
                            246 RESUME                   3
                            248 JUMP_BACKWARD_NO_INTERRUPT     4 (to 242)
                        >>  250 STORE_FAST               4 (proc)
                
-               578         252 LOAD_FAST                4 (proc)
+               579         252 LOAD_FAST                4 (proc)
                            254 LOAD_FAST                0 (self)
                            256 LOAD_ATTR                3 (procs)
                            266 LOAD_FAST                1 (name)
                            268 STORE_SUBSCR
                
-               579         272 LOAD_FAST                4 (proc)
+               580         272 LOAD_FAST                4 (proc)
                            274 LOAD_ATTR                4 (pid)
                            284 STORE_FAST               5 (pid)
                
-               580         286 LOAD_FAST                2 (scratch)
+               581         286 LOAD_FAST                2 (scratch)
                            288 LOAD_METHOD              8 (reset)
                            310 LOAD_FAST                5 (pid)
                            312 PRECALL                  1
                            316 CALL                     1
                            326 POP_TOP
                
-               581         328 LOAD_FAST                0 (self)
+               582         328 LOAD_FAST                0 (self)
                            330 LOAD_ATTR                0 (scratches)
                            340 LOAD_METHOD              9 (register)
                            362 LOAD_FAST                2 (scratch)
                            364 LOAD_FAST                5 (pid)
                            366 KW_NAMES                 5
                            368 PRECALL                  2
                            372 CALL                     2
                            382 POP_TOP
                
-               582         384 LOAD_FAST                0 (self)
+               583         384 LOAD_FAST                0 (self)
                            386 LOAD_ATTR               10 (log)
                            396 LOAD_METHOD             11 (info)
                
-               583         418 LOAD_CONST               6 ('scratch %s (%s) has pid %s')
+               584         418 LOAD_CONST               6 ('scratch %s (%s) has pid %s')
                            420 LOAD_FAST                2 (scratch)
                            422 LOAD_ATTR               12 (uid)
                            432 LOAD_FAST                2 (scratch)
                            434 LOAD_ATTR                7 (conf)
                            444 LOAD_METHOD              1 (get)
                            466 LOAD_CONST               3 ('command')
                            468 PRECALL                  1
                            472 CALL                     1
                            482 LOAD_FAST                5 (pid)
                
-               582         484 PRECALL                  4
+               583         484 PRECALL                  4
                            488 CALL                     4
                            498 POP_TOP
                
-               585         500 LOAD_FAST                3 (old_pid)
+               586         500 LOAD_FAST                3 (old_pid)
                            502 POP_JUMP_FORWARD_IF_FALSE    29 (to 562)
                
-               586         504 LOAD_FAST                0 (self)
+               587         504 LOAD_FAST                0 (self)
                            506 LOAD_ATTR                0 (scratches)
                            516 LOAD_METHOD             13 (clear)
                            538 LOAD_FAST                3 (old_pid)
                            540 KW_NAMES                 5
                            542 PRECALL                  1
                            546 CALL                     1
                            556 POP_TOP
                            558 LOAD_CONST               4 (None)
                            560 RETURN_VALUE
                
-               585     >>  562 LOAD_CONST               4 (None)
+               586     >>  562 LOAD_CONST               4 (None)
                            564 RETURN_VALUE
                consts
                   "spawns a given scratchpad's process"
                   'respawned'
                   0
                   'command'
                   None
@@ -4839,15 +4849,15 @@
                   'scratch %s (%s) has pid %s'
                names      ('scratches', 'get', 'setState', 'procs', 'pid', 'asyncio', 'create_subprocess_shell', 'conf', 'reset', 'register', 'log', 'info', 'uid', 'clear')
                varnames   ('self', 'name', 'scratch', 'old_pid', 'proc', 'pid')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'start_scratch_command'
-               firstlineno 571
+               firstlineno 572
                lnotab
                   0x06023401080136013a014a0114010e012a013801220142ff100304013a
                   ff
             'orig_scratch'
             code
                argcount  : 2
                nlocals   : 5
@@ -4868,98 +4878,98 @@
                   047c0472487c006a040000000000000000a0060000000000000000000000
                   0000000000000000007c047c036404190000000000000000006405640185
                   0219000000000000000000ac06a6020000ab02000000000000000001007c
                   04a00700000000000000000000000000000000000000007c03a6010000ab
                   010000000000000000830064017b0356009703860401000100640153008c
                   c77c006a080000000000000000a009000000000000000000000000000000
                   000000000064087c00a6020000ab020000000000000000010064015300
-               588           0 RETURN_GENERATOR
+               589           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               591           6 LOAD_FAST                1 (orig_scratch)
+               592           6 LOAD_FAST                1 (orig_scratch)
                              8 POP_JUMP_FORWARD_IF_FALSE     7 (to 24)
                             10 LOAD_FAST                1 (orig_scratch)
                             12 LOAD_ATTR                0 (pid)
                             22 JUMP_FORWARD             1 (to 26)
                        >>   24 LOAD_CONST               1 (None)
                        >>   26 STORE_FAST               2 (pid)
                
-               592          28 LOAD_FAST                0 (self)
+               593          28 LOAD_FAST                0 (self)
                             30 LOAD_METHOD              1 (hyprctlJSON)
                             52 LOAD_CONST               2 ('clients')
                             54 PRECALL                  1
                             58 CALL                     1
                             68 GET_AWAITABLE            0
                             70 LOAD_CONST               1 (None)
                        >>   72 SEND                     3 (to 80)
                             74 YIELD_VALUE
                             76 RESUME                   3
                             78 JUMP_BACKWARD_NO_INTERRUPT     4 (to 72)
                        >>   80 GET_ITER
                        >>   82 FOR_ITER               198 (to 480)
                             84 STORE_FAST               3 (client)
                
-               593          86 LOAD_GLOBAL              5 (NULL + isinstance)
+               594          86 LOAD_GLOBAL              5 (NULL + isinstance)
                             98 LOAD_FAST                3 (client)
                            100 LOAD_GLOBAL              6 (dict)
                            112 PRECALL                  2
                            116 CALL                     2
                            126 POP_JUMP_FORWARD_IF_TRUE     2 (to 132)
                            128 LOAD_ASSERTION_ERROR
                            130 RAISE_VARARGS            1
                
-               594     >>  132 LOAD_FAST                2 (pid)
+               595     >>  132 LOAD_FAST                2 (pid)
                            134 POP_JUMP_FORWARD_IF_FALSE    13 (to 162)
                            136 LOAD_FAST                2 (pid)
                            138 LOAD_FAST                3 (client)
                            140 LOAD_CONST               3 ('pid')
                            142 BINARY_SUBSCR
                            152 COMPARE_OP               3 (!=)
                            158 POP_JUMP_FORWARD_IF_FALSE     1 (to 162)
                
-               595         160 JUMP_BACKWARD           40 (to 82)
+               596         160 JUMP_BACKWARD           40 (to 82)
                
-               598     >>  162 LOAD_FAST                0 (self)
+               599     >>  162 LOAD_FAST                0 (self)
                            164 LOAD_ATTR                4 (scratches)
                            174 LOAD_METHOD              5 (get)
                            196 LOAD_FAST                3 (client)
                            198 LOAD_CONST               4 ('address')
                            200 BINARY_SUBSCR
                            210 LOAD_CONST               5 (2)
                            212 LOAD_CONST               1 (None)
                            214 BUILD_SLICE              2
                            216 BINARY_SUBSCR
                            226 KW_NAMES                 6
                            228 PRECALL                  1
                            232 CALL                     1
                            242 STORE_FAST               4 (scratch)
                
-               599         244 LOAD_FAST                4 (scratch)
+               600         244 LOAD_FAST                4 (scratch)
                            246 POP_JUMP_FORWARD_IF_TRUE    41 (to 330)
                            248 LOAD_FAST                3 (client)
                            250 LOAD_CONST               3 ('pid')
                            252 BINARY_SUBSCR
                            262 POP_JUMP_FORWARD_IF_FALSE    33 (to 330)
                
-               600         264 LOAD_FAST                0 (self)
+               601         264 LOAD_FAST                0 (self)
                            266 LOAD_ATTR                4 (scratches)
                            276 LOAD_METHOD              5 (get)
                            298 LOAD_FAST                3 (client)
                            300 LOAD_CONST               3 ('pid')
                            302 BINARY_SUBSCR
                            312 KW_NAMES                 7
                            314 PRECALL                  1
                            318 CALL                     1
                            328 STORE_FAST               4 (scratch)
                
-               601     >>  330 LOAD_FAST                4 (scratch)
+               602     >>  330 LOAD_FAST                4 (scratch)
                            332 POP_JUMP_FORWARD_IF_FALSE    72 (to 478)
                
-               602         334 LOAD_FAST                0 (self)
+               603         334 LOAD_FAST                0 (self)
                            336 LOAD_ATTR                4 (scratches)
                            346 LOAD_METHOD              6 (register)
                            368 LOAD_FAST                4 (scratch)
                            370 LOAD_FAST                3 (client)
                            372 LOAD_CONST               4 ('address')
                            374 BINARY_SUBSCR
                            384 LOAD_CONST               5 (2)
@@ -4967,34 +4977,34 @@
                            388 BUILD_SLICE              2
                            390 BINARY_SUBSCR
                            400 KW_NAMES                 6
                            402 PRECALL                  2
                            406 CALL                     2
                            416 POP_TOP
                
-               603         418 LOAD_FAST                4 (scratch)
+               604         418 LOAD_FAST                4 (scratch)
                            420 LOAD_METHOD              7 (updateClientInfo)
                            442 LOAD_FAST                3 (client)
                            444 PRECALL                  1
                            448 CALL                     1
                            458 GET_AWAITABLE            0
                            460 LOAD_CONST               1 (None)
                        >>  462 SEND                     3 (to 470)
                            464 YIELD_VALUE
                            466 RESUME                   3
                            468 JUMP_BACKWARD_NO_INTERRUPT     4 (to 462)
                        >>  470 POP_TOP
                
-               604         472 POP_TOP
+               605         472 POP_TOP
                            474 LOAD_CONST               1 (None)
                            476 RETURN_VALUE
                
-               601     >>  478 JUMP_BACKWARD          199 (to 82)
+               602     >>  478 JUMP_BACKWARD          199 (to 82)
                
-               606     >>  480 LOAD_FAST                0 (self)
+               607     >>  480 LOAD_FAST                0 (self)
                            482 LOAD_ATTR                8 (log)
                            492 LOAD_METHOD              9 (info)
                            514 LOAD_CONST               8 ("Didn't update scratch info %s")
                            516 LOAD_FAST                0 (self)
                            518 PRECALL                  2
                            522 CALL                     2
                            532 POP_TOP
@@ -5012,48 +5022,48 @@
                   "Didn't update scratch info %s"
                names      ('pid', 'hyprctlJSON', 'isinstance', 'dict', 'scratches', 'get', 'register', 'updateClientInfo', 'log', 'info')
                varnames   ('self', 'orig_scratch', 'pid', 'client', 'scratch')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'updateScratchInfo'
-               firstlineno 588
+               firstlineno 589
                lnotab 0x060316013a012e011c01020352011401420104015401360106fd0205
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 5
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   0000000000000000000000a6000000ab00000000000000000044005d2f7d
                   027c026a0200000000000000007c016b020000000072227c00a003000000
                   00000000000000000000000000000000007c026a04000000000000000064
                   01ac02a6020000ab020000000000000000830064037b0356009703860401
                   008c3064035300
-               609           0 RETURN_GENERATOR
+               610           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               611           6 LOAD_FAST                0 (self)
+               612           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (scratches)
                             18 LOAD_METHOD              1 (values)
                             40 PRECALL                  0
                             44 CALL                     0
                             54 GET_ITER
                        >>   56 FOR_ITER                47 (to 152)
                             58 STORE_FAST               2 (scratch)
                
-               612          60 LOAD_FAST                2 (scratch)
+               613          60 LOAD_FAST                2 (scratch)
                             62 LOAD_ATTR                2 (monitor)
                             72 LOAD_FAST                1 (monitor_name)
                             74 COMPARE_OP               2 (==)
                             80 POP_JUMP_FORWARD_IF_FALSE    34 (to 150)
                
-               613          82 LOAD_FAST                0 (self)
+               614          82 LOAD_FAST                0 (self)
                             84 LOAD_METHOD              3 (run_hide)
                            106 LOAD_FAST                2 (scratch)
                            108 LOAD_ATTR                4 (uid)
                            118 LOAD_CONST               1 (True)
                            120 KW_NAMES                 2
                            122 PRECALL                  2
                            126 CALL                     2
@@ -5062,95 +5072,95 @@
                        >>  140 SEND                     3 (to 148)
                            142 YIELD_VALUE
                            144 RESUME                   3
                            146 JUMP_BACKWARD_NO_INTERRUPT     4 (to 140)
                        >>  148 POP_TOP
                        >>  150 JUMP_BACKWARD           48 (to 56)
                
-               611     >>  152 LOAD_CONST               3 (None)
+               612     >>  152 LOAD_CONST               3 (None)
                            154 RETURN_VALUE
                consts
                   'Hides scratchpads on the removed screen'
                   True
                   ('autohide',)
                   None
                names      ('scratches', 'values', 'monitor', 'run_hide', 'uid')
                varnames   ('self', 'monitor_name', 'scratch')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'event_monitorremoved'
-               firstlineno 609
+               firstlineno 610
                lnotab 0x06023601160146fe
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 5
                flags     : 131
                code
                   0x4b00010097007401000000000000000000007c006a0100000000000000
                   00a00200000000000000000000000000000000000000006401a6010000ab
                   010000000000000000a6010000ab01000000000000000044005d387d027c
                   006a010000000000000000a0030000000000000000000000000000000000
                   0000007c026401a6020000ab02000000000000000001007c00a004000000
                   00000000000000000000000000000000007c02a6010000ab010000000000
                   000000830064027b0356009703860401008c3964025300
-               615           0 RETURN_GENERATOR
+               616           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               617           6 LOAD_GLOBAL              1 (NULL + list)
+               618           6 LOAD_GLOBAL              1 (NULL + list)
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (scratches)
                             30 LOAD_METHOD              2 (getByState)
                             52 LOAD_CONST               1 ('configured')
                             54 PRECALL                  1
                             58 CALL                     1
                             68 PRECALL                  1
                             72 CALL                     1
                             82 GET_ITER
                        >>   84 FOR_ITER                56 (to 198)
                             86 STORE_FAST               2 (scratch)
                
-               618          88 LOAD_FAST                0 (self)
+               619          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                1 (scratches)
                            100 LOAD_METHOD              3 (clearState)
                            122 LOAD_FAST                2 (scratch)
                            124 LOAD_CONST               1 ('configured')
                            126 PRECALL                  2
                            130 CALL                     2
                            140 POP_TOP
                
-               619         142 LOAD_FAST                0 (self)
+               620         142 LOAD_FAST                0 (self)
                            144 LOAD_METHOD              4 (_configure_windowrules)
                            166 LOAD_FAST                2 (scratch)
                            168 PRECALL                  1
                            172 CALL                     1
                            182 GET_AWAITABLE            0
                            184 LOAD_CONST               2 (None)
                        >>  186 SEND                     3 (to 194)
                            188 YIELD_VALUE
                            190 RESUME                   3
                            192 JUMP_BACKWARD_NO_INTERRUPT     4 (to 186)
                        >>  194 POP_TOP
                            196 JUMP_BACKWARD           57 (to 84)
                
-               617     >>  198 LOAD_CONST               2 (None)
+               618     >>  198 LOAD_CONST               2 (None)
                            200 RETURN_VALUE
                consts
                   'Re-apply windowrules when hyprland is restarted'
                   'configured'
                   None
                names      ('list', 'scratches', 'getByState', 'clearState', '_configure_windowrules')
                varnames   ('self', '_nothing', 'scratch')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'event_configreloaded'
-               firstlineno 615
+               firstlineno 616
                lnotab 0x06025201360138fe
             code
                argcount  : 2
                nlocals   : 8
                stacksize : 7
                flags     : 131
                code
@@ -5189,218 +5199,218 @@
                   00a6010000ab010000000000000000010090018ccd89006a080000000000
                   000000a009000000000000000000000000000000000000000064097c02a6
                   020000ab02000000000000000001008900a0130000000000000000000000
                   0000000000000000007c02640aac0ba6020000ab02000000000000000083
                   00640c7b03560097038604010090028c07640c5300
                              0 MAKE_CELL                0 (self)
                
-               621           2 RETURN_GENERATOR
+               622           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                
-               623           8 LOAD_DEREF               0 (self)
+               624           8 LOAD_DEREF               0 (self)
                             10 LOAD_ATTR                0 (scratches)
                             20 LOAD_METHOD              1 (items)
                             42 PRECALL                  0
                             46 CALL                     0
                             56 GET_ITER
                        >>   58 EXTENDED_ARG             2
                             60 FOR_ITER               517 (to 1096)
                             62 UNPACK_SEQUENCE          2
                             66 STORE_FAST               2 (uid)
                             68 STORE_FAST               3 (scratch)
                
-               624          70 LOAD_FAST                3 (scratch)
+               625          70 LOAD_FAST                3 (scratch)
                             72 LOAD_ATTR                2 (client_info)
                             82 POP_JUMP_FORWARD_IF_TRUE     1 (to 86)
                
-               625          84 JUMP_BACKWARD           14 (to 58)
+               626          84 JUMP_BACKWARD           14 (to 58)
                
-               626     >>   86 LOAD_FAST                3 (scratch)
+               627     >>   86 LOAD_FAST                3 (scratch)
                             88 LOAD_ATTR                3 (address)
                             98 LOAD_FAST                1 (addr)
                            100 COMPARE_OP               2 (==)
                            106 POP_JUMP_FORWARD_IF_FALSE   108 (to 324)
                
-               627         108 LOAD_DEREF               0 (self)
+               628         108 LOAD_DEREF               0 (self)
                            110 LOAD_ATTR                4 (_hysteresis_tasks)
                            120 LOAD_METHOD              5 (get)
                            142 LOAD_FAST                3 (scratch)
                            144 LOAD_ATTR                6 (uid)
                            154 PRECALL                  1
                            158 CALL                     1
                            168 STORE_FAST               4 (task)
                
-               628         170 LOAD_FAST                4 (task)
+               629         170 LOAD_FAST                4 (task)
                            172 POP_JUMP_FORWARD_IF_FALSE    74 (to 322)
                
-               629         174 LOAD_FAST                4 (task)
+               630         174 LOAD_FAST                4 (task)
                            176 LOAD_METHOD              7 (cancel)
                            198 PRECALL                  0
                            202 CALL                     0
                            212 POP_TOP
                
-               630         214 LOAD_FAST                3 (scratch)
+               631         214 LOAD_FAST                3 (scratch)
                            216 LOAD_ATTR                6 (uid)
                            226 LOAD_DEREF               0 (self)
                            228 LOAD_ATTR                4 (_hysteresis_tasks)
                            238 CONTAINS_OP              0
                            240 POP_JUMP_FORWARD_IF_FALSE    13 (to 268)
                
-               631         242 LOAD_DEREF               0 (self)
+               632         242 LOAD_DEREF               0 (self)
                            244 LOAD_ATTR                4 (_hysteresis_tasks)
                            254 LOAD_FAST                3 (scratch)
                            256 LOAD_ATTR                6 (uid)
                            266 DELETE_SUBSCR
                
-               632     >>  268 LOAD_DEREF               0 (self)
+               633     >>  268 LOAD_DEREF               0 (self)
                            270 LOAD_ATTR                8 (log)
                            280 LOAD_METHOD              9 (debug)
                            302 LOAD_CONST               1 ('Canceled previous task for %s')
                            304 LOAD_FAST                2 (uid)
                            306 PRECALL                  2
                            310 CALL                     2
                            320 POP_TOP
                        >>  322 JUMP_BACKWARD          133 (to 58)
                
-               634     >>  324 LOAD_FAST                3 (scratch)
+               635     >>  324 LOAD_FAST                3 (scratch)
                            326 LOAD_ATTR               10 (visible)
                            336 EXTENDED_ARG             1
                            338 POP_JUMP_FORWARD_IF_FALSE   376 (to 1092)
                            340 LOAD_FAST                3 (scratch)
                            342 LOAD_ATTR               11 (conf)
                            352 LOAD_METHOD              5 (get)
                            374 LOAD_CONST               2 ('unfocus')
                            376 PRECALL                  1
                            380 CALL                     1
                            390 LOAD_CONST               3 ('hide')
                            392 COMPARE_OP               2 (==)
                            398 EXTENDED_ARG             1
                            400 POP_JUMP_FORWARD_IF_FALSE   345 (to 1092)
                
-               635         402 LOAD_FAST                3 (scratch)
+               636         402 LOAD_FAST                3 (scratch)
                            404 LOAD_ATTR               12 (meta)
                            414 LOAD_METHOD              5 (get)
                            436 LOAD_CONST               4 ('last_shown')
                            438 LOAD_CONST               5 (0)
                            440 PRECALL                  2
                            444 CALL                     2
                            454 STORE_FAST               5 (last_shown)
                
-               636         456 LOAD_FAST                5 (last_shown)
+               637         456 LOAD_FAST                5 (last_shown)
                            458 LOAD_GLOBAL             26 (AFTER_SHOW_INHIBITION)
                            470 BINARY_OP                0 (+)
                            474 LOAD_GLOBAL             29 (NULL + time)
                            486 LOAD_ATTR               14 (time)
                            496 PRECALL                  0
                            500 CALL                     0
                            510 COMPARE_OP               4 (>)
                            516 POP_JUMP_FORWARD_IF_FALSE    29 (to 576)
                
-               637         518 LOAD_DEREF               0 (self)
+               638         518 LOAD_DEREF               0 (self)
                            520 LOAD_ATTR                8 (log)
                            530 LOAD_METHOD              9 (debug)
                
-               638         552 LOAD_CONST               6 ('(SKIPPED) hide %s because another client is active')
+               639         552 LOAD_CONST               6 ('(SKIPPED) hide %s because another client is active')
                
-               639         554 LOAD_FAST                2 (uid)
+               640         554 LOAD_FAST                2 (uid)
                
-               637         556 PRECALL                  2
+               638         556 PRECALL                  2
                            560 CALL                     2
                            570 POP_TOP
                
-               641         572 EXTENDED_ARG             1
+               642         572 EXTENDED_ARG             1
                            574 JUMP_BACKWARD          259 (to 58)
                
-               643     >>  576 LOAD_FAST                3 (scratch)
+               644     >>  576 LOAD_FAST                3 (scratch)
                            578 LOAD_ATTR               11 (conf)
                            588 LOAD_METHOD              5 (get)
                            610 LOAD_CONST               7 ('hysteresis')
                            612 LOAD_GLOBAL             30 (DEFAULT_HYSTERESIS)
                            624 PRECALL                  2
                            628 CALL                     2
                            638 STORE_FAST               6 (hysteresis)
                
-               644         640 LOAD_FAST                6 (hysteresis)
+               645         640 LOAD_FAST                6 (hysteresis)
                            642 POP_JUMP_FORWARD_IF_FALSE   168 (to 980)
                
-               645         644 LOAD_DEREF               0 (self)
+               646         644 LOAD_DEREF               0 (self)
                            646 LOAD_ATTR                4 (_hysteresis_tasks)
                            656 LOAD_METHOD              5 (get)
                            678 LOAD_FAST                3 (scratch)
                            680 LOAD_ATTR                6 (uid)
                            690 PRECALL                  1
                            694 CALL                     1
                            704 STORE_FAST               4 (task)
                
-               646         706 LOAD_FAST                4 (task)
+               647         706 LOAD_FAST                4 (task)
                            708 POP_JUMP_FORWARD_IF_FALSE    47 (to 804)
                
-               647         710 LOAD_FAST                4 (task)
+               648         710 LOAD_FAST                4 (task)
                            712 LOAD_METHOD              7 (cancel)
                            734 PRECALL                  0
                            738 CALL                     0
                            748 POP_TOP
                
-               648         750 LOAD_DEREF               0 (self)
+               649         750 LOAD_DEREF               0 (self)
                            752 LOAD_ATTR                8 (log)
                            762 LOAD_METHOD              9 (debug)
                            784 LOAD_CONST               1 ('Canceled previous task for %s')
                            786 LOAD_FAST                2 (uid)
                            788 PRECALL                  2
                            792 CALL                     2
                            802 POP_TOP
                
-               649     >>  804 LOAD_GLOBAL             33 (NULL + asyncio)
+               650     >>  804 LOAD_GLOBAL             33 (NULL + asyncio)
                            816 LOAD_ATTR               17 (create_task)
                
-               650         826 LOAD_GLOBAL             33 (NULL + asyncio)
+               651         826 LOAD_GLOBAL             33 (NULL + asyncio)
                            838 LOAD_ATTR               18 (sleep)
                            848 LOAD_FAST                6 (hysteresis)
                            850 PRECALL                  1
                            854 CALL                     1
                
-               649         864 PRECALL                  1
+               650         864 PRECALL                  1
                            868 CALL                     1
                            878 LOAD_DEREF               0 (self)
                            880 LOAD_ATTR                4 (_hysteresis_tasks)
                            890 LOAD_FAST                3 (scratch)
                            892 LOAD_ATTR                6 (uid)
                            902 STORE_SUBSCR
                
-               653         906 LOAD_CLOSURE             0 (self)
+               654         906 LOAD_CLOSURE             0 (self)
                            908 BUILD_TUPLE              1
-                           910 LOAD_CONST               8 (<code object _task, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 653>)
+                           910 LOAD_CONST               8 (<code object _task, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 654>)
                            912 MAKE_FUNCTION            8 (closure)
                            914 STORE_FAST               7 (_task)
                
-               668         916 LOAD_GLOBAL             33 (NULL + asyncio)
+               669         916 LOAD_GLOBAL             33 (NULL + asyncio)
                            928 LOAD_ATTR               17 (create_task)
                            938 PUSH_NULL
                            940 LOAD_FAST                7 (_task)
                            942 LOAD_FAST                3 (scratch)
                            944 LOAD_FAST                2 (uid)
                            946 PRECALL                  2
                            950 CALL                     2
                            960 PRECALL                  1
                            964 CALL                     1
                            974 POP_TOP
                            976 EXTENDED_ARG             1
                            978 JUMP_BACKWARD          461 (to 58)
                
-               670     >>  980 LOAD_DEREF               0 (self)
+               671     >>  980 LOAD_DEREF               0 (self)
                            982 LOAD_ATTR                8 (log)
                            992 LOAD_METHOD              9 (debug)
                           1014 LOAD_CONST               9 ('hide %s because another client is active')
                           1016 LOAD_FAST                2 (uid)
                           1018 PRECALL                  2
                           1022 CALL                     2
                           1032 POP_TOP
                
-               671        1034 LOAD_DEREF               0 (self)
+               672        1034 LOAD_DEREF               0 (self)
                           1036 LOAD_METHOD             19 (run_hide)
                           1058 LOAD_FAST                2 (uid)
                           1060 LOAD_CONST              10 (True)
                           1062 KW_NAMES                11
                           1064 PRECALL                  2
                           1068 CALL                     2
                           1078 GET_AWAITABLE            0
@@ -5409,15 +5419,15 @@
                           1084 YIELD_VALUE
                           1086 RESUME                   3
                           1088 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1082)
                        >> 1090 POP_TOP
                        >> 1092 EXTENDED_ARG             2
                           1094 JUMP_BACKWARD          519 (to 58)
                
-               623     >> 1096 LOAD_CONST              12 (None)
+               624     >> 1096 LOAD_CONST              12 (None)
                           1098 RETURN_VALUE
                consts
                   'active windows hook'
                   'Canceled previous task for %s'
                   'unfocus'
                   'hide'
                   'last_shown'
@@ -5439,78 +5449,78 @@
                         0000000000000064017c01a6020000ab0200000000000000000100640053
                         0089026a050000000000000000a006000000000000000000000000000000
                         000000000064027c01a6020000ab02000000000000000001008902a00700
                         000000000000000000000000000000000000007c016403ac04a6020000ab
                         020000000000000000830064007b03560097038604010064005300
                                    0 COPY_FREE_VARS           1
                      
-                     653           2 RETURN_GENERATOR
+                     654           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                      
-                     654           8 LOAD_FAST                0 (scratch)
+                     655           8 LOAD_FAST                0 (scratch)
                                   10 LOAD_ATTR                0 (uid)
                                   20 LOAD_DEREF               2 (self)
                                   22 LOAD_ATTR                1 (_hysteresis_tasks)
                                   32 CONTAINS_OP              0
                                   34 POP_JUMP_FORWARD_IF_FALSE    37 (to 110)
                      
-                     655          36 LOAD_DEREF               2 (self)
+                     656          36 LOAD_DEREF               2 (self)
                                   38 LOAD_ATTR                1 (_hysteresis_tasks)
                                   48 LOAD_FAST                0 (scratch)
                                   50 LOAD_ATTR                0 (uid)
                                   60 BINARY_SUBSCR
                                   70 GET_AWAITABLE            0
                                   72 LOAD_CONST               0 (None)
                              >>   74 SEND                     3 (to 82)
                                   76 YIELD_VALUE
                                   78 RESUME                   3
                                   80 JUMP_BACKWARD_NO_INTERRUPT     4 (to 74)
                              >>   82 POP_TOP
                      
-                     656          84 LOAD_DEREF               2 (self)
+                     657          84 LOAD_DEREF               2 (self)
                                   86 LOAD_ATTR                1 (_hysteresis_tasks)
                                   96 LOAD_FAST                0 (scratch)
                                   98 LOAD_ATTR                0 (uid)
                                  108 DELETE_SUBSCR
                      
-                     657     >>  110 LOAD_GLOBAL              4 (state)
+                     658     >>  110 LOAD_GLOBAL              4 (state)
                                  122 LOAD_ATTR                3 (active_window)
                                  132 LOAD_FAST                0 (scratch)
                                  134 LOAD_ATTR                4 (full_address)
                                  144 COMPARE_OP               2 (==)
                                  150 POP_JUMP_FORWARD_IF_FALSE    29 (to 210)
                      
-                     658         152 LOAD_DEREF               2 (self)
+                     659         152 LOAD_DEREF               2 (self)
                                  154 LOAD_ATTR                5 (log)
                                  164 LOAD_METHOD              6 (debug)
                      
-                     659         186 LOAD_CONST               1 ('Skipped hidding %s because client got the focus back')
+                     660         186 LOAD_CONST               1 ('Skipped hidding %s because client got the focus back')
                      
-                     660         188 LOAD_FAST                1 (uid)
+                     661         188 LOAD_FAST                1 (uid)
                      
-                     658         190 PRECALL                  2
+                     659         190 PRECALL                  2
                                  194 CALL                     2
                                  204 POP_TOP
                      
-                     662         206 LOAD_CONST               0 (None)
+                     663         206 LOAD_CONST               0 (None)
                                  208 RETURN_VALUE
                      
-                     663     >>  210 LOAD_DEREF               2 (self)
+                     664     >>  210 LOAD_DEREF               2 (self)
                                  212 LOAD_ATTR                5 (log)
                                  222 LOAD_METHOD              6 (debug)
                      
-                     664         244 LOAD_CONST               2 ('hide %s because another client is active')
+                     665         244 LOAD_CONST               2 ('hide %s because another client is active')
                                  246 LOAD_FAST                1 (uid)
                      
-                     663         248 PRECALL                  2
+                     664         248 PRECALL                  2
                                  252 CALL                     2
                                  262 POP_TOP
                      
-                     666         264 LOAD_DEREF               2 (self)
+                     667         264 LOAD_DEREF               2 (self)
                                  266 LOAD_METHOD              7 (run_hide)
                                  288 LOAD_FAST                1 (uid)
                                  290 LOAD_CONST               3 (True)
                                  292 KW_NAMES                 4
                                  294 PRECALL                  2
                                  298 CALL                     2
                                  308 GET_AWAITABLE            0
@@ -5530,27 +5540,27 @@
                         ('autohide',)
                      names      ('uid', '_hysteresis_tasks', 'state', 'active_window', 'full_address', 'log', 'debug', 'run_hide')
                      varnames   ('scratch', 'uid')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                      name       '_task'
-                     firstlineno 653
+                     firstlineno 654
                      lnotab 0x08011c0130011a012a012201020102fe10040401220104ff1003
                   'hide %s because another client is active'
                   True
                   ('autohide',)
                   None
                names      ('scratches', 'items', 'client_info', 'address', '_hysteresis_tasks', 'get', 'uid', 'cancel', 'log', 'debug', 'visible', 'conf', 'meta', 'AFTER_SHOW_INHIBITION', 'time', 'DEFAULT_HYSTERESIS', 'asyncio', 'create_task', 'sleep', 'run_hide')
                varnames   ('self', 'addr', 'uid', 'scratch', 'task', 'last_shown', 'hysteresis', '_task')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'event_activewindowv2'
-               firstlineno 621
+               firstlineno 622
                lnotab
                   0x08023e010e01020116013e01040128011c011a0138024e0136013e0122
                   01020102fe10040402400104013e01040128013601160126ff2a040a0f40
                   0236013ed0
             code
                argcount  : 1
                nlocals   : 4
@@ -5572,89 +5582,89 @@
                   000000000000000000ac0aa6020000ab020000000000000000010089006a
                   020000000000000000a00300000000000000000000000000000000000000
                   00640b7c02a6020000ab02000000000000000001007c03a0090000000000
                   0000000000000000000000000000007c02a6010000ab0100000000000000
                   00830064067b0356009703860401008c7a8c96640c5300
                              0 MAKE_CELL                0 (self)
                
-               673           2 RETURN_GENERATOR
+               674           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                
-               675           8 LOAD_CLOSURE             0 (self)
+               676           8 LOAD_CLOSURE             0 (self)
                             10 BUILD_TUPLE              1
-                            12 LOAD_CONST               1 (<code object <listcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 675>)
+                            12 LOAD_CONST               1 (<code object <listcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 676>)
                             14 MAKE_FUNCTION            8 (closure)
                
-               677          16 LOAD_DEREF               0 (self)
+               678          16 LOAD_DEREF               0 (self)
                             18 LOAD_ATTR                0 (scratches)
                             28 LOAD_METHOD              1 (getByState)
                             50 LOAD_CONST               2 ('respawned')
                             52 PRECALL                  1
                             56 CALL                     1
                
-               675          66 GET_ITER
+               676          66 GET_ITER
                             68 PRECALL                  0
                             72 CALL                     0
                             82 STORE_FAST               1 (class_lookup_hack)
                
-               680          84 LOAD_FAST                1 (class_lookup_hack)
+               681          84 LOAD_FAST                1 (class_lookup_hack)
                             86 POP_JUMP_FORWARD_IF_TRUE     2 (to 92)
                
-               681          88 LOAD_CONST               3 (False)
+               682          88 LOAD_CONST               3 (False)
                             90 RETURN_VALUE
                
-               682     >>   92 LOAD_DEREF               0 (self)
+               683     >>   92 LOAD_DEREF               0 (self)
                             94 LOAD_ATTR                2 (log)
                            104 LOAD_METHOD              3 (debug)
                            126 LOAD_CONST               4 ('Lookup hack triggered')
                            128 PRECALL                  1
                            132 CALL                     1
                            142 POP_TOP
                
-               684         144 LOAD_DEREF               0 (self)
+               685         144 LOAD_DEREF               0 (self)
                            146 LOAD_METHOD              4 (hyprctlJSON)
                            168 LOAD_CONST               5 ('clients')
                            170 PRECALL                  1
                            174 CALL                     1
                            184 GET_AWAITABLE            0
                            186 LOAD_CONST               6 (None)
                        >>  188 SEND                     3 (to 196)
                            190 YIELD_VALUE
                            192 RESUME                   3
                            194 JUMP_BACKWARD_NO_INTERRUPT     4 (to 188)
                        >>  196 GET_ITER
                        >>  198 FOR_ITER               149 (to 498)
                            200 STORE_FAST               2 (client)
                
-               685         202 LOAD_GLOBAL             11 (NULL + isinstance)
+               686         202 LOAD_GLOBAL             11 (NULL + isinstance)
                            214 LOAD_FAST                2 (client)
                            216 LOAD_GLOBAL             12 (dict)
                            228 PRECALL                  2
                            232 CALL                     2
                            242 POP_JUMP_FORWARD_IF_TRUE     2 (to 248)
                            244 LOAD_ASSERTION_ERROR
                            246 RAISE_VARARGS            1
                
-               686     >>  248 LOAD_FAST                1 (class_lookup_hack)
+               687     >>  248 LOAD_FAST                1 (class_lookup_hack)
                            250 GET_ITER
                        >>  252 FOR_ITER               121 (to 496)
                            254 STORE_FAST               3 (pending_scratch)
                
-               687         256 LOAD_FAST                3 (pending_scratch)
+               688         256 LOAD_FAST                3 (pending_scratch)
                            258 LOAD_ATTR                7 (conf)
                            268 LOAD_CONST               7 ('class')
                            270 BINARY_SUBSCR
                            280 LOAD_FAST                2 (client)
                            282 LOAD_CONST               7 ('class')
                            284 BINARY_SUBSCR
                            294 COMPARE_OP               2 (==)
                            300 POP_JUMP_FORWARD_IF_FALSE    96 (to 494)
                
-               688         302 LOAD_DEREF               0 (self)
+               689         302 LOAD_DEREF               0 (self)
                            304 LOAD_ATTR                0 (scratches)
                            314 LOAD_METHOD              8 (register)
                            336 LOAD_FAST                3 (pending_scratch)
                            338 LOAD_FAST                2 (client)
                            340 LOAD_CONST               8 ('address')
                            342 BINARY_SUBSCR
                            352 LOAD_CONST               9 (2)
@@ -5662,40 +5672,40 @@
                            356 BUILD_SLICE              2
                            358 BINARY_SUBSCR
                            368 KW_NAMES                10
                            370 PRECALL                  2
                            374 CALL                     2
                            384 POP_TOP
                
-               689         386 LOAD_DEREF               0 (self)
+               690         386 LOAD_DEREF               0 (self)
                            388 LOAD_ATTR                2 (log)
                            398 LOAD_METHOD              3 (debug)
                            420 LOAD_CONST              11 ('client class found: %s')
                            422 LOAD_FAST                2 (client)
                            424 PRECALL                  2
                            428 CALL                     2
                            438 POP_TOP
                
-               690         440 LOAD_FAST                3 (pending_scratch)
+               691         440 LOAD_FAST                3 (pending_scratch)
                            442 LOAD_METHOD              9 (updateClientInfo)
                            464 LOAD_FAST                2 (client)
                            466 PRECALL                  1
                            470 CALL                     1
                            480 GET_AWAITABLE            0
                            482 LOAD_CONST               6 (None)
                        >>  484 SEND                     3 (to 492)
                            486 YIELD_VALUE
                            488 RESUME                   3
                            490 JUMP_BACKWARD_NO_INTERRUPT     4 (to 484)
                        >>  492 POP_TOP
                        >>  494 JUMP_BACKWARD          122 (to 252)
                
-               686     >>  496 JUMP_BACKWARD          150 (to 198)
+               687     >>  496 JUMP_BACKWARD          150 (to 198)
                
-               691     >>  498 LOAD_CONST              12 (True)
+               692     >>  498 LOAD_CONST              12 (True)
                            500 RETURN_VALUE
                consts
                   'if class_match attribute is defined, use class matching and return True'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 7
@@ -5703,48 +5713,48 @@
                      code
                         0x9501970067007c005d317d018902a00000000000000000000000000000
                         000000000000007c016a010000000000000000a002000000000000000000
                         00000000000000000000006400a6010000ab010000000000000000a60100
                         00ab010000000000000000af2f7c0191028c325300
                                    0 COPY_FREE_VARS           1
                      
-                     675           2 RESUME                   0
+                     676           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                49 (to 108)
                      
-                     677          10 STORE_FAST               1 (s)
+                     678          10 STORE_FAST               1 (s)
                      
-                     678          12 LOAD_DEREF               2 (self)
+                     679          12 LOAD_DEREF               2 (self)
                                   14 LOAD_METHOD              0 (cast_bool)
                                   36 LOAD_FAST                1 (s)
                                   38 LOAD_ATTR                1 (conf)
                                   48 LOAD_METHOD              2 (get)
                                   70 LOAD_CONST               0 ('class_match')
                                   72 PRECALL                  1
                                   76 CALL                     1
                                   86 PRECALL                  1
                                   90 CALL                     1
                      
-                     675         100 POP_JUMP_BACKWARD_IF_FALSE    47 (to 8)
+                     676         100 POP_JUMP_BACKWARD_IF_FALSE    47 (to 8)
                      
-                     676         102 LOAD_FAST                1 (s)
+                     677         102 LOAD_FAST                1 (s)
                      
-                     675         104 LIST_APPEND              2
+                     676         104 LIST_APPEND              2
                                  106 JUMP_BACKWARD           50 (to 8)
                              >>  108 RETURN_VALUE
                      consts
                         'class_match'
                      names      ('cast_bool', 'conf', 'get')
                      varnames   ('.0', 's')
                      freevars   ('self',)
                      cellvars   ()
                      filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                      name       '<listcomp>'
-                     firstlineno 675
+                     firstlineno 676
                      lnotab 0x0a02020158fd020102ff
                   'respawned'
                   False
                   'Lookup hack triggered'
                   'clients'
                   None
                   'class'
@@ -5755,15 +5765,15 @@
                   True
                names      ('scratches', 'getByState', 'log', 'debug', 'hyprctlJSON', 'isinstance', 'dict', 'conf', 'register', 'updateClientInfo')
                varnames   ('self', 'class_lookup_hack', 'client', 'pending_scratch')
                freevars   ()
                cellvars   ('self',)
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       '_alternative_lookup'
-               firstlineno 673
+               firstlineno 674
                lnotab
                   0x0802080232fe12050401040134023a012e0108012e015401360138fc02
                   05
             code
                argcount  : 2
                nlocals   : 8
                stacksize : 5
@@ -5784,103 +5794,103 @@
                   010000000000000000a00200000000000000000000000000000000000000
                   007c02ac03a6010000ab0100000000000000007d067c0672297c066a0900
                   0000000000000072227c00a00a0000000000000000000000000000000000
                   0000007c066a0b00000000000000006407ac08a6020000ab020000000000
                   000000830064057b0356009703860401007c06721d7c06a00c0000000000
                   0000000000000000000000000000007c00a6010000ab0100000000000000
                   00830064057b0356009703860401006405530064055300
-               693           0 RETURN_GENERATOR
+               694           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               695           6 LOAD_FAST                1 (params)
+               696           6 LOAD_FAST                1 (params)
                              8 LOAD_METHOD              0 (split)
                             30 LOAD_CONST               1 (',')
                             32 LOAD_CONST               2 (3)
                             34 PRECALL                  2
                             38 CALL                     2
                             48 UNPACK_SEQUENCE          4
                             52 STORE_FAST               2 (addr)
                             54 STORE_FAST               3 (_wrkspc)
                             56 STORE_FAST               4 (_kls)
                             58 STORE_FAST               5 (_title)
                
-               696          60 LOAD_FAST                0 (self)
+               697          60 LOAD_FAST                0 (self)
                             62 LOAD_ATTR                1 (scratches)
                             72 LOAD_METHOD              2 (get)
                             94 LOAD_FAST                2 (addr)
                             96 KW_NAMES                 3
                             98 PRECALL                  1
                            102 CALL                     1
                            112 STORE_FAST               6 (item)
                
-               697         114 LOAD_GLOBAL              7 (NULL + list)
+               698         114 LOAD_GLOBAL              7 (NULL + list)
                            126 LOAD_FAST                0 (self)
                            128 LOAD_ATTR                1 (scratches)
                            138 LOAD_METHOD              4 (getByState)
                            160 LOAD_CONST               4 ('respawned')
                            162 PRECALL                  1
                            166 CALL                     1
                            176 PRECALL                  1
                            180 CALL                     1
                            190 STORE_FAST               7 (rs)
                
-               698         192 LOAD_FAST                7 (rs)
+               699         192 LOAD_FAST                7 (rs)
                            194 POP_JUMP_FORWARD_IF_FALSE   150 (to 496)
                            196 LOAD_FAST                6 (item)
                            198 POP_JUMP_FORWARD_IF_TRUE   148 (to 496)
                
-               700         200 LOAD_FAST                0 (self)
+               701         200 LOAD_FAST                0 (self)
                            202 LOAD_METHOD              5 (_alternative_lookup)
                            224 PRECALL                  0
                            228 CALL                     0
                            238 GET_AWAITABLE            0
                            240 LOAD_CONST               5 (None)
                        >>  242 SEND                     3 (to 250)
                            244 YIELD_VALUE
                            246 RESUME                   3
                            248 JUMP_BACKWARD_NO_INTERRUPT     4 (to 242)
                        >>  250 POP_JUMP_FORWARD_IF_TRUE    52 (to 356)
                
-               701         252 LOAD_FAST                0 (self)
+               702         252 LOAD_FAST                0 (self)
                            254 LOAD_ATTR                6 (log)
                            264 LOAD_METHOD              7 (info)
                            286 LOAD_CONST               6 ('Updating Scratch info')
                            288 PRECALL                  1
                            292 CALL                     1
                            302 POP_TOP
                
-               702         304 LOAD_FAST                0 (self)
+               703         304 LOAD_FAST                0 (self)
                            306 LOAD_METHOD              8 (updateScratchInfo)
                            328 PRECALL                  0
                            332 CALL                     0
                            342 GET_AWAITABLE            0
                            344 LOAD_CONST               5 (None)
                        >>  346 SEND                     3 (to 354)
                            348 YIELD_VALUE
                            350 RESUME                   3
                            352 JUMP_BACKWARD_NO_INTERRUPT     4 (to 346)
                        >>  354 POP_TOP
                
-               703     >>  356 LOAD_FAST                0 (self)
+               704     >>  356 LOAD_FAST                0 (self)
                            358 LOAD_ATTR                1 (scratches)
                            368 LOAD_METHOD              2 (get)
                            390 LOAD_FAST                2 (addr)
                            392 KW_NAMES                 3
                            394 PRECALL                  1
                            398 CALL                     1
                            408 STORE_FAST               6 (item)
                
-               704         410 LOAD_FAST                6 (item)
+               705         410 LOAD_FAST                6 (item)
                            412 POP_JUMP_FORWARD_IF_FALSE    41 (to 496)
                            414 LOAD_FAST                6 (item)
                            416 LOAD_ATTR                9 (should_hide)
                            426 POP_JUMP_FORWARD_IF_FALSE    34 (to 496)
                
-               705         428 LOAD_FAST                0 (self)
+               706         428 LOAD_FAST                0 (self)
                            430 LOAD_METHOD             10 (run_hide)
                            452 LOAD_FAST                6 (item)
                            454 LOAD_ATTR               11 (uid)
                            464 LOAD_CONST               7 (True)
                            466 KW_NAMES                 8
                            468 PRECALL                  2
                            472 CALL                     2
@@ -5888,33 +5898,33 @@
                            484 LOAD_CONST               5 (None)
                        >>  486 SEND                     3 (to 494)
                            488 YIELD_VALUE
                            490 RESUME                   3
                            492 JUMP_BACKWARD_NO_INTERRUPT     4 (to 486)
                        >>  494 POP_TOP
                
-               706     >>  496 LOAD_FAST                6 (item)
+               707     >>  496 LOAD_FAST                6 (item)
                            498 POP_JUMP_FORWARD_IF_FALSE    29 (to 558)
                
-               707         500 LOAD_FAST                6 (item)
+               708         500 LOAD_FAST                6 (item)
                            502 LOAD_METHOD             12 (initialize)
                            524 LOAD_FAST                0 (self)
                            526 PRECALL                  1
                            530 CALL                     1
                            540 GET_AWAITABLE            0
                            542 LOAD_CONST               5 (None)
                        >>  544 SEND                     3 (to 552)
                            546 YIELD_VALUE
                            548 RESUME                   3
                            550 JUMP_BACKWARD_NO_INTERRUPT     4 (to 544)
                        >>  552 POP_TOP
                            554 LOAD_CONST               5 (None)
                            556 RETURN_VALUE
                
-               706     >>  558 LOAD_CONST               5 (None)
+               707     >>  558 LOAD_CONST               5 (None)
                            560 RETURN_VALUE
                consts
                   'open windows hook'
                   ','
                   3
                   ('addr',)
                   'respawned'
@@ -5924,15 +5934,15 @@
                   ('force',)
                names      ('split', 'scratches', 'get', 'list', 'getByState', '_alternative_lookup', 'log', 'info', 'updateScratchInfo', 'should_hide', 'run_hide', 'uid', 'initialize')
                varnames   ('self', 'params', 'addr', '_wrkspc', '_kls', '_title', 'item', 'rs')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'event_openwindow'
-               firstlineno 693
+               firstlineno 694
                lnotab 0x0602360136014e01080234013401340136011201440104013aff
             'uid_or_uids'
             code
                argcount  : 2
                nlocals   : 8
                stacksize : 10
                flags     : 131
@@ -5968,24 +5978,24 @@
                   0000000000000000007c006a1500000000000000007c06a6020000ab0200
                   00000000000000a6010000ab01000000000000000001008ca17c05a01300
                   000000000000000000000000000000000000007429000000000000000000
                   007c006a1600000000000000007c06a6020000ab020000000000000000a6
                   010000ab01000000000000000001008cca742f000000000000000000006a
                   180000000000000000640a84007c054400a6000000ab0000000000000000
                   008e00830064067b03560097038604010064065300
-               711           0 RETURN_GENERATOR
+               712           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               713           6 LOAD_CONST               1 (' ')
+               714           6 LOAD_CONST               1 (' ')
                              8 LOAD_FAST                1 (uid_or_uids)
                             10 CONTAINS_OP              0
                             12 POP_JUMP_FORWARD_IF_FALSE    77 (to 168)
                
-               714          14 LOAD_GLOBAL              1 (NULL + list)
+               715          14 LOAD_GLOBAL              1 (NULL + list)
                             26 LOAD_GLOBAL              3 (NULL + filter)
                             38 LOAD_GLOBAL              4 (bool)
                             50 LOAD_GLOBAL              7 (NULL + map)
                             62 LOAD_GLOBAL              8 (str)
                             74 LOAD_ATTR                5 (strip)
                             84 LOAD_FAST                1 (uid_or_uids)
                             86 LOAD_METHOD              6 (split)
@@ -5996,185 +6006,185 @@
                            136 PRECALL                  2
                            140 CALL                     2
                            150 PRECALL                  1
                            154 CALL                     1
                            164 STORE_FAST               2 (uids)
                            166 JUMP_FORWARD            21 (to 210)
                
-               716     >>  168 LOAD_FAST                1 (uid_or_uids)
+               717     >>  168 LOAD_FAST                1 (uid_or_uids)
                            170 LOAD_METHOD              5 (strip)
                            192 PRECALL                  0
                            196 CALL                     0
                            206 BUILD_LIST               1
                            208 STORE_FAST               2 (uids)
                
-               718     >>  210 LOAD_GLOBAL             15 (NULL + len)
+               719     >>  210 LOAD_GLOBAL             15 (NULL + len)
                            222 LOAD_FAST                2 (uids)
                            224 PRECALL                  1
                            228 CALL                     1
                            238 LOAD_CONST               2 (0)
                            240 COMPARE_OP               4 (>)
                            246 POP_JUMP_FORWARD_IF_TRUE     2 (to 252)
                            248 LOAD_ASSERTION_ERROR
                            250 RAISE_VARARGS            1
                
-               719     >>  252 LOAD_FAST                0 (self)
+               720     >>  252 LOAD_FAST                0 (self)
                            254 LOAD_ATTR                8 (scratches)
                            264 LOAD_METHOD              9 (get)
                            286 LOAD_FAST                2 (uids)
                            288 LOAD_CONST               2 (0)
                            290 BINARY_SUBSCR
                            300 PRECALL                  1
                            304 CALL                     1
                            314 STORE_FAST               3 (first_scratch)
                
-               720         316 LOAD_FAST                3 (first_scratch)
+               721         316 LOAD_FAST                3 (first_scratch)
                            318 POP_JUMP_FORWARD_IF_TRUE    66 (to 452)
                
-               721         320 LOAD_FAST                0 (self)
+               722         320 LOAD_FAST                0 (self)
                            322 LOAD_ATTR               10 (log)
                            332 LOAD_METHOD             11 (warning)
                            354 LOAD_CONST               3 ("%s doesn't exist, can't toggle.")
                            356 LOAD_FAST                2 (uids)
                            358 LOAD_CONST               2 (0)
                            360 BINARY_SUBSCR
                            370 PRECALL                  2
                            374 CALL                     2
                            384 POP_TOP
                
-               722         386 LOAD_GLOBAL             25 (NULL + notify_error)
+               723         386 LOAD_GLOBAL             25 (NULL + notify_error)
                
-               723         398 LOAD_CONST               4 ("Scratchpad '")
+               724         398 LOAD_CONST               4 ("Scratchpad '")
                            400 LOAD_FAST                2 (uids)
                            402 LOAD_CONST               2 (0)
                            404 BINARY_SUBSCR
                            414 FORMAT_VALUE             0
                            416 LOAD_CONST               5 ("' not found, check your configuration or the toggle parameter")
                            418 BUILD_STRING             3
                
-               722         420 PRECALL                  1
+               723         420 PRECALL                  1
                            424 CALL                     1
                            434 GET_AWAITABLE            0
                            436 LOAD_CONST               6 (None)
                        >>  438 SEND                     3 (to 446)
                            440 YIELD_VALUE
                            442 RESUME                   3
                            444 JUMP_BACKWARD_NO_INTERRUPT     4 (to 438)
                        >>  446 POP_TOP
                
-               725         448 LOAD_CONST               6 (None)
+               726         448 LOAD_CONST               6 (None)
                            450 RETURN_VALUE
                
-               727     >>  452 LOAD_FAST                3 (first_scratch)
+               728     >>  452 LOAD_FAST                3 (first_scratch)
                            454 LOAD_ATTR               13 (visible)
                            464 JUMP_IF_FALSE_OR_POP    48 (to 562)
                
-               728         466 LOAD_FAST                3 (first_scratch)
+               729         466 LOAD_FAST                3 (first_scratch)
                            468 LOAD_ATTR               14 (conf)
                            478 LOAD_METHOD              9 (get)
                            500 LOAD_CONST               7 ('force_monitor')
                            502 PRECALL                  1
                            506 CALL                     1
                            516 JUMP_IF_TRUE_OR_POP     22 (to 562)
                
-               729         518 LOAD_FAST                3 (first_scratch)
+               730         518 LOAD_FAST                3 (first_scratch)
                            520 LOAD_ATTR               15 (space_identifier)
                            530 LOAD_GLOBAL             33 (NULL + get_space_identifier)
                            542 PRECALL                  0
                            546 CALL                     0
                            556 COMPARE_OP               2 (==)
                
-               727     >>  562 STORE_FAST               4 (is_visible)
+               728     >>  562 STORE_FAST               4 (is_visible)
                
-               731         564 BUILD_LIST               0
+               732         564 BUILD_LIST               0
                            566 STORE_FAST               5 (tasks)
                
-               733         568 LOAD_FAST                2 (uids)
+               734         568 LOAD_FAST                2 (uids)
                            570 GET_ITER
                        >>  572 FOR_ITER               201 (to 976)
                            574 STORE_FAST               6 (uid)
                
-               734         576 LOAD_FAST                0 (self)
+               735         576 LOAD_FAST                0 (self)
                            578 LOAD_ATTR                8 (scratches)
                            588 LOAD_METHOD              9 (get)
                            610 LOAD_FAST                6 (uid)
                            612 PRECALL                  1
                            616 CALL                     1
                            626 STORE_FAST               7 (item)
                
-               735         628 LOAD_FAST                7 (item)
+               736         628 LOAD_FAST                7 (item)
                            630 POP_JUMP_FORWARD_IF_TRUE    28 (to 688)
                
-               736         632 LOAD_FAST                0 (self)
+               737         632 LOAD_FAST                0 (self)
                            634 LOAD_ATTR               10 (log)
                            644 LOAD_METHOD             11 (warning)
                            666 LOAD_CONST               8 ('%s is not configured')
                            668 LOAD_FAST                6 (uid)
                            670 PRECALL                  2
                            674 CALL                     2
                            684 POP_TOP
                            686 JUMP_BACKWARD           58 (to 572)
                
-               738     >>  688 LOAD_FAST                0 (self)
+               739     >>  688 LOAD_FAST                0 (self)
                            690 LOAD_ATTR               10 (log)
                            700 LOAD_METHOD             17 (debug)
                
-               739         722 LOAD_CONST               9 ('%s is visible = %s (but %s)')
+               740         722 LOAD_CONST               9 ('%s is visible = %s (but %s)')
                            724 LOAD_FAST                6 (uid)
                            726 LOAD_FAST                7 (item)
                            728 LOAD_ATTR               13 (visible)
                            738 LOAD_FAST                4 (is_visible)
                
-               738         740 PRECALL                  4
+               739         740 PRECALL                  4
                            744 CALL                     4
                            754 POP_TOP
                
-               741         756 LOAD_FAST                4 (is_visible)
+               742         756 LOAD_FAST                4 (is_visible)
                            758 POP_JUMP_FORWARD_IF_FALSE    67 (to 894)
                            760 LOAD_FAST                7 (item)
                            762 LOAD_METHOD             18 (isAlive)
                            784 PRECALL                  0
                            788 CALL                     0
                            798 GET_AWAITABLE            0
                            800 LOAD_CONST               6 (None)
                        >>  802 SEND                     3 (to 810)
                            804 YIELD_VALUE
                            806 RESUME                   3
                            808 JUMP_BACKWARD_NO_INTERRUPT     4 (to 802)
                        >>  810 POP_JUMP_FORWARD_IF_FALSE    41 (to 894)
                
-               742         812 LOAD_FAST                5 (tasks)
+               743         812 LOAD_FAST                5 (tasks)
                            814 LOAD_METHOD             19 (append)
                            836 LOAD_GLOBAL             41 (NULL + partial)
                            848 LOAD_FAST                0 (self)
                            850 LOAD_ATTR               21 (run_hide)
                            860 LOAD_FAST                6 (uid)
                            862 PRECALL                  2
                            866 CALL                     2
                            876 PRECALL                  1
                            880 CALL                     1
                            890 POP_TOP
                            892 JUMP_BACKWARD          161 (to 572)
                
-               744     >>  894 LOAD_FAST                5 (tasks)
+               745     >>  894 LOAD_FAST                5 (tasks)
                            896 LOAD_METHOD             19 (append)
                            918 LOAD_GLOBAL             41 (NULL + partial)
                            930 LOAD_FAST                0 (self)
                            932 LOAD_ATTR               22 (run_show)
                            942 LOAD_FAST                6 (uid)
                            944 PRECALL                  2
                            948 CALL                     2
                            958 PRECALL                  1
                            962 CALL                     1
                            972 POP_TOP
                            974 JUMP_BACKWARD          202 (to 572)
                
-               745     >>  976 LOAD_GLOBAL             47 (NULL + asyncio)
+               746     >>  976 LOAD_GLOBAL             47 (NULL + asyncio)
                            988 LOAD_ATTR               24 (gather)
-                           998 LOAD_CONST              10 (<code object <genexpr>, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 745>)
+                           998 LOAD_CONST              10 (<code object <genexpr>, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 746>)
                           1000 MAKE_FUNCTION            0
                           1002 LOAD_FAST                5 (tasks)
                           1004 GET_ITER
                           1006 PRECALL                  0
                           1010 CALL                     0
                           1020 CALL_FUNCTION_EX         0
                           1022 GET_AWAITABLE            0
@@ -6202,15 +6212,15 @@
                      nlocals   : 2
                      stacksize : 5
                      flags     : 51
                      code
                         0x4b00010097007c005d207d017401000000000000000000006a01000000
                         000000000002007c01a6000000ab000000000000000000a6010000ab0100
                         000000000000005600970101008c2164005300
-                     745           0 RETURN_GENERATOR
+                     746           0 RETURN_GENERATOR
                                    2 POP_TOP
                                    4 RESUME                   0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                32 (to 74)
                                   10 STORE_FAST               1 (t)
                                   12 LOAD_GLOBAL              1 (NULL + asyncio)
                                   24 LOAD_ATTR                1 (create_task)
@@ -6230,58 +6240,58 @@
                         None
                      names      ('asyncio', 'create_task')
                      varnames   ('.0', 't')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                      name       '<genexpr>'
-                     firstlineno 745
+                     firstlineno 746
                      lnotab 0x
                names      ('list', 'filter', 'bool', 'map', 'str', 'strip', 'split', 'len', 'scratches', 'get', 'log', 'warning', 'notify_error', 'visible', 'conf', 'space_identifier', 'get_space_identifier', 'debug', 'isAlive', 'append', 'partial', 'run_hide', 'run_show', 'asyncio', 'gather')
                varnames   ('self', 'uid_or_uids', 'uids', 'first_scratch', 'is_visible', 'tasks', 'uid', 'item')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'run_toggle'
-               firstlineno 711
+               firstlineno 712
                lnotab
                   0x060208019a022a022a014001040142010c0116ff1c0304020e0134012c
                   fe020404020801340104013802220112ff1003380152025201
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 3
                flags     : 131
                code
                   0x4b00010097007c016a000000000000000000a001000000000000000000
                   00000000000000000000006401a6010000ab0100000000000000007d037c
                   0372047c037c03660253007c01a002000000000000000000000000000000
                   00000000007c02a6010000ab010000000000000000830064027b03560097
                   0386045300
-               747           0 RETURN_GENERATOR
+               748           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               749           6 LOAD_FAST                1 (scratch)
+               750           6 LOAD_FAST                1 (scratch)
                              8 LOAD_ATTR                0 (conf)
                             18 LOAD_METHOD              1 (get)
                             40 LOAD_CONST               1 ('offset')
                             42 PRECALL                  1
                             46 CALL                     1
                             56 STORE_FAST               3 (offset)
                
-               750          58 LOAD_FAST                3 (offset)
+               751          58 LOAD_FAST                3 (offset)
                             60 POP_JUMP_FORWARD_IF_FALSE     4 (to 70)
                
-               751          62 LOAD_FAST                3 (offset)
+               752          62 LOAD_FAST                3 (offset)
                             64 LOAD_FAST                3 (offset)
                             66 BUILD_TUPLE              2
                             68 RETURN_VALUE
                
-               752     >>   70 LOAD_FAST                1 (scratch)
+               753     >>   70 LOAD_FAST                1 (scratch)
                             72 LOAD_METHOD              2 (get_auto_offset)
                             94 LOAD_FAST                2 (monitor)
                             96 PRECALL                  1
                            100 CALL                     1
                            110 GET_AWAITABLE            0
                            112 LOAD_CONST               2 (None)
                        >>  114 SEND                     3 (to 122)
@@ -6295,89 +6305,116 @@
                   None
                names      ('conf', 'get', 'get_auto_offset')
                varnames   ('self', 'scratch', 'monitor', 'offset')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'get_offsets'
-               firstlineno 747
+               firstlineno 748
                lnotab 0x0602340104010801
             code
                argcount  : 3
-               nlocals   : 5
+               nlocals   : 6
                stacksize : 6
                flags     : 131
                code
-                  0x4b00010097007c00a00000000000000000000000000000000000000000
-                  007c02a6010000ab010000000000000000830064017b0356009703860401
-                  007c00a00100000000000000000000000000000000000000007c02a60100
-                  00ab010000000000000000830064017b035600970386045c0200007d037d
-                  047c00a00200000000000000000000000000000000000000007c017c027c
-                  037c04a6040000ab040000000000000000830064017b0356009703860401
-                  0064015300
-               754           0 RETURN_GENERATOR
+                  0x4b00010097007c016a000000000000000000a001000000000000000000
+                  000000000000000000000064016402a6020000ab020000000000000000a0
+                  020000000000000000000000000000000000000000a6000000ab00000000
+                  00000000007d037c037302640353007c00a0030000000000000000000000
+                  0000000000000000007c01a6010000ab010000000000000000830064047b
+                  0356009703860401007c00a0040000000000000000000000000000000000
+                  0000007c017c02a6020000ab020000000000000000830064047b03560097
+                  0386045c0200007d047d057c00a005000000000000000000000000000000
+                  00000000007c037c017c047c05a6040000ab040000000000000000830064
+                  047b03560097038604010064055300
+               755           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               757           6 LOAD_FAST                0 (self)
-                             8 LOAD_METHOD              0 (updateScratchInfo)
-                            30 LOAD_FAST                2 (scratch)
-                            32 PRECALL                  1
-                            36 CALL                     1
-                            46 GET_AWAITABLE            0
-                            48 LOAD_CONST               1 (None)
-                       >>   50 SEND                     3 (to 58)
-                            52 YIELD_VALUE
-                            54 RESUME                   3
-                            56 JUMP_BACKWARD_NO_INTERRUPT     4 (to 50)
-                       >>   58 POP_TOP
-               
-               759          60 LOAD_FAST                0 (self)
-                            62 LOAD_METHOD              1 (get_offsets)
-                            84 LOAD_FAST                2 (scratch)
-                            86 PRECALL                  1
-                            90 CALL                     1
-                           100 GET_AWAITABLE            0
-                           102 LOAD_CONST               1 (None)
-                       >>  104 SEND                     3 (to 112)
-                           106 YIELD_VALUE
-                           108 RESUME                   3
-                           110 JUMP_BACKWARD_NO_INTERRUPT     4 (to 104)
-                       >>  112 UNPACK_SEQUENCE          2
-                           116 STORE_FAST               3 (off_x)
-                           118 STORE_FAST               4 (off_y)
-               
-               760         120 LOAD_FAST                0 (self)
-                           122 LOAD_METHOD              2 (_slide_animation)
-                           144 LOAD_FAST                1 (animation_type)
-                           146 LOAD_FAST                2 (scratch)
-                           148 LOAD_FAST                3 (off_x)
-                           150 LOAD_FAST                4 (off_y)
-                           152 PRECALL                  4
-                           156 CALL                     4
-                           166 GET_AWAITABLE            0
-                           168 LOAD_CONST               1 (None)
-                       >>  170 SEND                     3 (to 178)
-                           172 YIELD_VALUE
-                           174 RESUME                   3
-                           176 JUMP_BACKWARD_NO_INTERRUPT     4 (to 170)
-                       >>  178 POP_TOP
-                           180 LOAD_CONST               1 (None)
-                           182 RETURN_VALUE
+               758           6 LOAD_FAST                1 (scratch)
+                             8 LOAD_ATTR                0 (conf)
+                            18 LOAD_METHOD              1 (get)
+                            40 LOAD_CONST               1 ('animation')
+                            42 LOAD_CONST               2 ('')
+                            44 PRECALL                  2
+                            48 CALL                     2
+                            58 LOAD_METHOD              2 (lower)
+                            80 PRECALL                  0
+                            84 CALL                     0
+                            94 STORE_FAST               3 (animation_type)
+               
+               759          96 LOAD_FAST                3 (animation_type)
+                            98 POP_JUMP_FORWARD_IF_TRUE     2 (to 104)
+               
+               760         100 LOAD_CONST               3 (False)
+                           102 RETURN_VALUE
+               
+               762     >>  104 LOAD_FAST                0 (self)
+                           106 LOAD_METHOD              3 (updateScratchInfo)
+                           128 LOAD_FAST                1 (scratch)
+                           130 PRECALL                  1
+                           134 CALL                     1
+                           144 GET_AWAITABLE            0
+                           146 LOAD_CONST               4 (None)
+                       >>  148 SEND                     3 (to 156)
+                           150 YIELD_VALUE
+                           152 RESUME                   3
+                           154 JUMP_BACKWARD_NO_INTERRUPT     4 (to 148)
+                       >>  156 POP_TOP
+               
+               764         158 LOAD_FAST                0 (self)
+                           160 LOAD_METHOD              4 (get_offsets)
+                           182 LOAD_FAST                1 (scratch)
+                           184 LOAD_FAST                2 (monitor)
+                           186 PRECALL                  2
+                           190 CALL                     2
+                           200 GET_AWAITABLE            0
+                           202 LOAD_CONST               4 (None)
+                       >>  204 SEND                     3 (to 212)
+                           206 YIELD_VALUE
+                           208 RESUME                   3
+                           210 JUMP_BACKWARD_NO_INTERRUPT     4 (to 204)
+                       >>  212 UNPACK_SEQUENCE          2
+                           216 STORE_FAST               4 (off_x)
+                           218 STORE_FAST               5 (off_y)
+               
+               765         220 LOAD_FAST                0 (self)
+                           222 LOAD_METHOD              5 (_slide_animation)
+                           244 LOAD_FAST                3 (animation_type)
+                           246 LOAD_FAST                1 (scratch)
+                           248 LOAD_FAST                4 (off_x)
+                           250 LOAD_FAST                5 (off_y)
+                           252 PRECALL                  4
+                           256 CALL                     4
+                           266 GET_AWAITABLE            0
+                           268 LOAD_CONST               4 (None)
+                       >>  270 SEND                     3 (to 278)
+                           272 YIELD_VALUE
+                           274 RESUME                   3
+                           276 JUMP_BACKWARD_NO_INTERRUPT     4 (to 270)
+                       >>  278 POP_TOP
+               
+               766         280 LOAD_CONST               5 (True)
+                           282 RETURN_VALUE
                consts
                   'animate hiding a scratchpad'
+                  'animation'
+                  ''
+                  False
                   None
-               names      ('updateScratchInfo', 'get_offsets', '_slide_animation')
-               varnames   ('self', 'animation_type', 'scratch', 'off_x', 'off_y')
+                  True
+               names      ('conf', 'get', 'lower', 'updateScratchInfo', 'get_offsets', '_slide_animation')
+               varnames   ('self', 'scratch', 'monitor', 'animation_type', 'off_x', 'off_y')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
-               name       '_anim_hide'
-               firstlineno 754
-               lnotab 0x060336023c01
+               name       '_hide_transition'
+               firstlineno 755
+               lnotab 0x06035a010401040236023e013c01
             code
                argcount  : 5
                nlocals   : 6
                stacksize : 6
                flags     : 131
                code
                   0x4b000100970064017c026a0000000000000000007a0000007d057c0164
@@ -6390,30 +6427,30 @@
                   00000000000000000000000000000064087c030b009b0064097c059b009d
                   04a6010000ab010000000000000000830064057b0356009703860401006e
                   277c01640a6b020000000072217c00a00100000000000000000000000000
                   0000000000000064087c039b0064097c059b009d04a6010000ab01000000
                   0000000000830064057b0356009703860401007405000000000000000000
                   006a030000000000000000640ba6010000ab010000000000000000830064
                   057b03560097038604010064055300
-               762           0 RETURN_GENERATOR
+               768           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               764           6 LOAD_CONST               1 ('address:')
+               770           6 LOAD_CONST               1 ('address:')
                              8 LOAD_FAST                2 (scratch)
                             10 LOAD_ATTR                0 (full_address)
                             20 BINARY_OP                0 (+)
                             24 STORE_FAST               5 (addr)
                
-               765          26 LOAD_FAST                1 (animation_type)
+               771          26 LOAD_FAST                1 (animation_type)
                             28 LOAD_CONST               2 ('fromtop')
                             30 COMPARE_OP               2 (==)
                             36 POP_JUMP_FORWARD_IF_FALSE    35 (to 108)
                
-               766          38 LOAD_FAST                0 (self)
+               772          38 LOAD_FAST                0 (self)
                             40 LOAD_METHOD              1 (hyprctl)
                             62 LOAD_CONST               3 ('movewindowpixel 0 ')
                             64 LOAD_FAST                4 (off_y)
                             66 UNARY_NEGATIVE
                             68 FORMAT_VALUE             0
                             70 LOAD_CONST               4 (',')
                             72 LOAD_FAST                5 (addr)
@@ -6426,20 +6463,20 @@
                        >>   96 SEND                     3 (to 104)
                             98 YIELD_VALUE
                            100 RESUME                   3
                            102 JUMP_BACKWARD_NO_INTERRUPT     4 (to 96)
                        >>  104 POP_TOP
                            106 JUMP_FORWARD           120 (to 348)
                
-               767     >>  108 LOAD_FAST                1 (animation_type)
+               773     >>  108 LOAD_FAST                1 (animation_type)
                            110 LOAD_CONST               6 ('frombottom')
                            112 COMPARE_OP               2 (==)
                            118 POP_JUMP_FORWARD_IF_FALSE    34 (to 188)
                
-               768         120 LOAD_FAST                0 (self)
+               774         120 LOAD_FAST                0 (self)
                            122 LOAD_METHOD              1 (hyprctl)
                            144 LOAD_CONST               3 ('movewindowpixel 0 ')
                            146 LOAD_FAST                4 (off_y)
                            148 FORMAT_VALUE             0
                            150 LOAD_CONST               4 (',')
                            152 LOAD_FAST                5 (addr)
                            154 FORMAT_VALUE             0
@@ -6451,20 +6488,20 @@
                        >>  176 SEND                     3 (to 184)
                            178 YIELD_VALUE
                            180 RESUME                   3
                            182 JUMP_BACKWARD_NO_INTERRUPT     4 (to 176)
                        >>  184 POP_TOP
                            186 JUMP_FORWARD            80 (to 348)
                
-               769     >>  188 LOAD_FAST                1 (animation_type)
+               775     >>  188 LOAD_FAST                1 (animation_type)
                            190 LOAD_CONST               7 ('fromleft')
                            192 COMPARE_OP               2 (==)
                            198 POP_JUMP_FORWARD_IF_FALSE    35 (to 270)
                
-               770         200 LOAD_FAST                0 (self)
+               776         200 LOAD_FAST                0 (self)
                            202 LOAD_METHOD              1 (hyprctl)
                            224 LOAD_CONST               8 ('movewindowpixel ')
                            226 LOAD_FAST                3 (off_x)
                            228 UNARY_NEGATIVE
                            230 FORMAT_VALUE             0
                            232 LOAD_CONST               9 (' 0,')
                            234 LOAD_FAST                5 (addr)
@@ -6477,20 +6514,20 @@
                        >>  258 SEND                     3 (to 266)
                            260 YIELD_VALUE
                            262 RESUME                   3
                            264 JUMP_BACKWARD_NO_INTERRUPT     4 (to 258)
                        >>  266 POP_TOP
                            268 JUMP_FORWARD            39 (to 348)
                
-               771     >>  270 LOAD_FAST                1 (animation_type)
+               777     >>  270 LOAD_FAST                1 (animation_type)
                            272 LOAD_CONST              10 ('fromright')
                            274 COMPARE_OP               2 (==)
                            280 POP_JUMP_FORWARD_IF_FALSE    33 (to 348)
                
-               772         282 LOAD_FAST                0 (self)
+               778         282 LOAD_FAST                0 (self)
                            284 LOAD_METHOD              1 (hyprctl)
                            306 LOAD_CONST               8 ('movewindowpixel ')
                            308 LOAD_FAST                3 (off_x)
                            310 FORMAT_VALUE             0
                            312 LOAD_CONST               9 (' 0,')
                            314 LOAD_FAST                5 (addr)
                            316 FORMAT_VALUE             0
@@ -6501,15 +6538,15 @@
                            336 LOAD_CONST               5 (None)
                        >>  338 SEND                     3 (to 346)
                            340 YIELD_VALUE
                            342 RESUME                   3
                            344 JUMP_BACKWARD_NO_INTERRUPT     4 (to 338)
                        >>  346 POP_TOP
                
-               774     >>  348 LOAD_GLOBAL              5 (NULL + asyncio)
+               780     >>  348 LOAD_GLOBAL              5 (NULL + asyncio)
                            360 LOAD_ATTR                3 (sleep)
                            370 LOAD_CONST              11 (0.2)
                            372 PRECALL                  1
                            376 CALL                     1
                            386 GET_AWAITABLE            0
                            388 LOAD_CONST               5 (None)
                        >>  390 SEND                     3 (to 398)
@@ -6534,15 +6571,15 @@
                   0.2
                names      ('full_address', 'hyprctl', 'asyncio', 'sleep')
                varnames   ('self', 'animation_type', 'scratch', 'off_x', 'off_y', 'addr')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       '_slide_animation'
-               firstlineno 762
+               firstlineno 768
                lnotab 0x060214010c0146010c0144010c0146010c014202
             code
                argcount  : 2
                nlocals   : 8
                stacksize : 5
                flags     : 131
                code
@@ -6581,165 +6618,165 @@
                   00830064047b035600970386047d077c0773024a0082017c026a15000000
                   0000000000730a4a00640ea6000000ab00000000000000000082017c00a0
                   1600000000000000000000000000000000000000007c027c077c03a60300
                   00ab030000000000000000830064047b0356009703860401007c07640f19
                   0000000000000000007c025f17000000000000000064045300
                              0 MAKE_CELL                1 (uid)
                
-               776           2 RETURN_GENERATOR
+               782           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                
-               778           8 LOAD_FAST                0 (self)
+               784           8 LOAD_FAST                0 (self)
                             10 LOAD_ATTR                0 (scratches)
                             20 LOAD_METHOD              1 (get)
                             42 LOAD_DEREF               1 (uid)
                             44 PRECALL                  1
                             48 CALL                     1
                             58 STORE_FAST               2 (item)
                
-               780          60 LOAD_FAST                2 (item)
+               786          60 LOAD_FAST                2 (item)
                             62 POP_JUMP_FORWARD_IF_TRUE    54 (to 172)
                
-               781          64 LOAD_FAST                0 (self)
+               787          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                2 (log)
                             76 LOAD_METHOD              3 (warning)
                             98 LOAD_CONST               1 ("%s doesn't exist, can't hide.")
                            100 LOAD_DEREF               1 (uid)
                            102 PRECALL                  2
                            106 CALL                     2
                            116 POP_TOP
                
-               782         118 LOAD_GLOBAL              9 (NULL + notify_error)
+               788         118 LOAD_GLOBAL              9 (NULL + notify_error)
                
-               783         130 LOAD_CONST               2 ("Scratchpad '")
+               789         130 LOAD_CONST               2 ("Scratchpad '")
                            132 LOAD_DEREF               1 (uid)
                            134 FORMAT_VALUE             0
                            136 LOAD_CONST               3 ("' not found, check your configuration or the show parameter")
                            138 BUILD_STRING             3
                
-               782         140 PRECALL                  1
+               788         140 PRECALL                  1
                            144 CALL                     1
                            154 GET_AWAITABLE            0
                            156 LOAD_CONST               4 (None)
                        >>  158 SEND                     3 (to 166)
                            160 YIELD_VALUE
                            162 RESUME                   3
                            164 JUMP_BACKWARD_NO_INTERRUPT     4 (to 158)
                        >>  166 POP_TOP
                
-               785         168 LOAD_CONST               4 (None)
+               791         168 LOAD_CONST               4 (None)
                            170 RETURN_VALUE
                
-               787     >>  172 LOAD_GLOBAL             10 (state)
+               793     >>  172 LOAD_GLOBAL             10 (state)
                            184 LOAD_ATTR                6 (active_window)
                            194 LOAD_FAST                0 (self)
                            196 LOAD_ATTR                7 (focused_window_tracking)
                            206 LOAD_DEREF               1 (uid)
                            208 STORE_SUBSCR
                
-               789         212 LOAD_FAST                0 (self)
+               795         212 LOAD_FAST                0 (self)
                            214 LOAD_ATTR                2 (log)
                            224 LOAD_METHOD              8 (info)
                            246 LOAD_CONST               5 ('Showing %s')
                            248 LOAD_DEREF               1 (uid)
                            250 PRECALL                  2
                            254 CALL                     2
                            264 POP_TOP
                
-               790         266 LOAD_FAST                2 (item)
+               796         266 LOAD_FAST                2 (item)
                            268 LOAD_METHOD              9 (isAlive)
                            290 PRECALL                  0
                            294 CALL                     0
                            304 GET_AWAITABLE            0
                            306 LOAD_CONST               4 (None)
                        >>  308 SEND                     3 (to 316)
                            310 YIELD_VALUE
                            312 RESUME                   3
                            314 JUMP_BACKWARD_NO_INTERRUPT     4 (to 308)
                        >>  316 STORE_FAST               3 (was_alive)
                
-               791         318 LOAD_FAST                0 (self)
+               797         318 LOAD_FAST                0 (self)
                            320 LOAD_METHOD             10 (ensure_alive)
                            342 LOAD_DEREF               1 (uid)
                            344 PRECALL                  1
                            348 CALL                     1
                            358 GET_AWAITABLE            0
                            360 LOAD_CONST               4 (None)
                        >>  362 SEND                     3 (to 370)
                            364 YIELD_VALUE
                            366 RESUME                   3
                            368 JUMP_BACKWARD_NO_INTERRUPT     4 (to 362)
                        >>  370 POP_JUMP_FORWARD_IF_TRUE    29 (to 430)
                
-               792         372 LOAD_FAST                0 (self)
+               798         372 LOAD_FAST                0 (self)
                            374 LOAD_ATTR                2 (log)
                            384 LOAD_METHOD             11 (error)
                            406 LOAD_CONST               6 ('Failed to show %s, aborting.')
                            408 LOAD_DEREF               1 (uid)
                            410 PRECALL                  2
                            414 CALL                     2
                            424 POP_TOP
                
-               793         426 LOAD_CONST               4 (None)
+               799         426 LOAD_CONST               4 (None)
                            428 RETURN_VALUE
                
-               795     >>  430 LOAD_FAST                2 (item)
+               801     >>  430 LOAD_FAST                2 (item)
                            432 LOAD_ATTR               12 (conf)
                            442 LOAD_METHOD              1 (get)
                            464 LOAD_CONST               7 ('excludes')
                            466 BUILD_LIST               0
                            468 PRECALL                  2
                            472 CALL                     2
                            482 STORE_FAST               4 (excluded)
                
-               796         484 LOAD_FAST                4 (excluded)
+               802         484 LOAD_FAST                4 (excluded)
                            486 LOAD_CONST               8 ('*')
                            488 COMPARE_OP               2 (==)
                            494 POP_JUMP_FORWARD_IF_FALSE    37 (to 570)
                
-               797         496 LOAD_CLOSURE             1 (uid)
+               803         496 LOAD_CLOSURE             1 (uid)
                            498 BUILD_TUPLE              1
-                           500 LOAD_CONST               9 (<code object <listcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 797>)
+                           500 LOAD_CONST               9 (<code object <listcomp>, file "/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py", line 803>)
                            502 MAKE_FUNCTION            8 (closure)
                
-               798         504 LOAD_FAST                0 (self)
+               804         504 LOAD_FAST                0 (self)
                            506 LOAD_ATTR                0 (scratches)
                            516 LOAD_METHOD             13 (values)
                            538 PRECALL                  0
                            542 CALL                     0
                
-               797         552 GET_ITER
+               803         552 GET_ITER
                            554 PRECALL                  0
                            558 CALL                     0
                            568 STORE_FAST               4 (excluded)
                
-               800     >>  570 LOAD_FAST                4 (excluded)
+               806     >>  570 LOAD_FAST                4 (excluded)
                            572 GET_ITER
                        >>  574 FOR_ITER                68 (to 712)
                            576 STORE_FAST               5 (e_uid)
                
-               801         578 LOAD_FAST                0 (self)
+               807         578 LOAD_FAST                0 (self)
                            580 LOAD_ATTR                0 (scratches)
                            590 LOAD_METHOD              1 (get)
                            612 LOAD_FAST                5 (e_uid)
                            614 PRECALL                  1
                            618 CALL                     1
                            628 STORE_FAST               6 (scratch)
                
-               802         630 LOAD_FAST                6 (scratch)
+               808         630 LOAD_FAST                6 (scratch)
                            632 POP_JUMP_FORWARD_IF_TRUE     2 (to 638)
                            634 LOAD_ASSERTION_ERROR
                            636 RAISE_VARARGS            1
                
-               803     >>  638 LOAD_FAST                6 (scratch)
+               809     >>  638 LOAD_FAST                6 (scratch)
                            640 LOAD_ATTR               14 (visible)
                            650 POP_JUMP_FORWARD_IF_FALSE    29 (to 710)
                
-               804         652 LOAD_FAST                0 (self)
+               810         652 LOAD_FAST                0 (self)
                            654 LOAD_METHOD             15 (run_hide)
                            676 LOAD_FAST                5 (e_uid)
                            678 LOAD_CONST              10 (True)
                            680 KW_NAMES                11
                            682 PRECALL                  2
                            686 CALL                     2
                            696 GET_AWAITABLE            0
@@ -6747,100 +6784,100 @@
                        >>  700 SEND                     3 (to 708)
                            702 YIELD_VALUE
                            704 RESUME                   3
                            706 JUMP_BACKWARD_NO_INTERRUPT     4 (to 700)
                        >>  708 POP_TOP
                        >>  710 JUMP_BACKWARD           69 (to 574)
                
-               805     >>  712 LOAD_FAST                2 (item)
+               811     >>  712 LOAD_FAST                2 (item)
                            714 LOAD_METHOD             16 (updateClientInfo)
                            736 PRECALL                  0
                            740 CALL                     0
                            750 GET_AWAITABLE            0
                            752 LOAD_CONST               4 (None)
                        >>  754 SEND                     3 (to 762)
                            756 YIELD_VALUE
                            758 RESUME                   3
                            760 JUMP_BACKWARD_NO_INTERRUPT     4 (to 754)
                        >>  762 POP_TOP
                
-               806         764 LOAD_FAST                2 (item)
+               812         764 LOAD_FAST                2 (item)
                            766 LOAD_METHOD             17 (initialize)
                            788 LOAD_FAST                0 (self)
                            790 PRECALL                  1
                            794 CALL                     1
                            804 GET_AWAITABLE            0
                            806 LOAD_CONST               4 (None)
                        >>  808 SEND                     3 (to 816)
                            810 YIELD_VALUE
                            812 RESUME                   3
                            814 JUMP_BACKWARD_NO_INTERRUPT     4 (to 808)
                        >>  816 POP_TOP
                
-               808         818 LOAD_CONST              10 (True)
+               814         818 LOAD_CONST              10 (True)
                            820 LOAD_FAST                2 (item)
                            822 STORE_ATTR              14 (visible)
                
-               809         832 LOAD_GLOBAL             37 (NULL + get_space_identifier)
+               815         832 LOAD_GLOBAL             37 (NULL + get_space_identifier)
                            844 PRECALL                  0
                            848 CALL                     0
                            858 LOAD_FAST                2 (item)
                            860 STORE_ATTR              19 (space_identifier)
                
-               810         870 LOAD_FAST                0 (self)
+               816         870 LOAD_FAST                0 (self)
                            872 LOAD_METHOD             20 (get_focused_monitor_props)
                
-               811         894 LOAD_FAST                2 (item)
+               817         894 LOAD_FAST                2 (item)
                            896 LOAD_ATTR               12 (conf)
                            906 LOAD_METHOD              1 (get)
                            928 LOAD_CONST              12 ('force_monitor')
                            930 PRECALL                  1
                            934 CALL                     1
                
-               810         944 KW_NAMES                13
+               816         944 KW_NAMES                13
                            946 PRECALL                  1
                            950 CALL                     1
                            960 GET_AWAITABLE            0
                            962 LOAD_CONST               4 (None)
                        >>  964 SEND                     3 (to 972)
                            966 YIELD_VALUE
                            968 RESUME                   3
                            970 JUMP_BACKWARD_NO_INTERRUPT     4 (to 964)
                        >>  972 STORE_FAST               7 (monitor)
                
-               814         974 LOAD_FAST                7 (monitor)
+               820         974 LOAD_FAST                7 (monitor)
                            976 POP_JUMP_FORWARD_IF_TRUE     2 (to 982)
                            978 LOAD_ASSERTION_ERROR
                            980 RAISE_VARARGS            1
                
-               815     >>  982 LOAD_FAST                2 (item)
+               821     >>  982 LOAD_FAST                2 (item)
                            984 LOAD_ATTR               21 (full_address)
                            994 POP_JUMP_FORWARD_IF_TRUE    10 (to 1016)
                            996 LOAD_ASSERTION_ERROR
                            998 LOAD_CONST              14 ('No address !')
                           1000 PRECALL                  0
                           1004 CALL                     0
                           1014 RAISE_VARARGS            1
                
-               817     >> 1016 LOAD_FAST                0 (self)
+               823     >> 1016 LOAD_FAST                0 (self)
                           1018 LOAD_METHOD             22 (_show_transition)
                           1040 LOAD_FAST                2 (item)
                           1042 LOAD_FAST                7 (monitor)
                           1044 LOAD_FAST                3 (was_alive)
                           1046 PRECALL                  3
                           1050 CALL                     3
                           1060 GET_AWAITABLE            0
                           1062 LOAD_CONST               4 (None)
                        >> 1064 SEND                     3 (to 1072)
                           1066 YIELD_VALUE
                           1068 RESUME                   3
                           1070 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1064)
                        >> 1072 POP_TOP
                
-               818        1074 LOAD_FAST                7 (monitor)
+               824        1074 LOAD_FAST                7 (monitor)
                           1076 LOAD_CONST              15 ('name')
                           1078 BINARY_SUBSCR
                           1088 LOAD_FAST                2 (item)
                           1090 STORE_ATTR              23 (monitor)
                           1100 LOAD_CONST               4 (None)
                           1102 RETURN_VALUE
                consts
@@ -6859,20 +6896,20 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x9501970067007c005d147d017c016a00000000000000000089026b0300
                         000000af0d7c016a00000000000000000091028c155300
                                    0 COPY_FREE_VARS           1
                      
-                     797           2 RESUME                   0
+                     803           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                20 (to 50)
                      
-                     798          10 STORE_FAST               1 (scratch)
+                     804          10 STORE_FAST               1 (scratch)
                                   12 LOAD_FAST                1 (scratch)
                                   14 LOAD_ATTR                0 (uid)
                                   24 LOAD_DEREF               2 (uid)
                                   26 COMPARE_OP               3 (!=)
                                   32 POP_JUMP_BACKWARD_IF_FALSE    13 (to 8)
                                   34 LOAD_FAST                1 (scratch)
                                   36 LOAD_ATTR                0 (uid)
@@ -6882,29 +6919,29 @@
                      consts
                      names      ('uid',)
                      varnames   ('.0', 'scratch')
                      freevars   ('uid',)
                      cellvars   ()
                      filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                      name       '<listcomp>'
-                     firstlineno 797
+                     firstlineno 803
                      lnotab 0x0a01
                   True
                   ('autohide',)
                   'force_monitor'
                   ('name',)
                   'No address !'
                   'name'
                names      ('scratches', 'get', 'log', 'warning', 'notify_error', 'state', 'active_window', 'focused_window_tracking', 'info', 'isAlive', 'ensure_alive', 'error', 'conf', 'values', 'visible', 'run_hide', 'updateClientInfo', 'initialize', 'get_space_identifier', 'space_identifier', 'get_focused_monitor_props', 'full_address', '_show_transition', 'monitor')
                varnames   ('self', 'uid', 'item', 'was_alive', 'excluded', 'e_uid', 'scratch', 'monitor')
                freevars   ()
                cellvars   ('uid',)
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'run_show'
-               firstlineno 776
+               firstlineno 782
                lnotab
                   0x08023402040136010c010aff1c03040228023601340136013601040236
                   010c01080130ff12030801340108010e013c01340136020e012601180132
                   ff1e04080122023a01
             code
                argcount  : 4
                nlocals   : 14
@@ -6948,195 +6985,196 @@
                   000000000000000000000000007c0da6010000ab01000000000000000083
                   00640c7b0356009703860401006e207c006a160000000000000000a01700
                   0000000000000000000000000000000000000064127c016a060000000000
                   000000a6020000ab02000000000000000001007c00a00500000000000000
                   0000000000000000000000000064137c016a0700000000000000009b009d
                   02a6010000ab0100000000000000008300640c7b03560097038604010074
                   07000000000000000000006a030000000000000000a6000000ab00000000
-                  00000000007c016a04000000000000000064053c000000640c5300
-               820           0 RETURN_GENERATOR
+                  00000000007c016a04000000000000000064053c0000007c027c016a0400
+                  0000000000000064143c000000640c5300
+               826           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               822           6 LOAD_FAST                1 (item)
+               828           6 LOAD_FAST                1 (item)
                              8 LOAD_ATTR                0 (conf)
                             18 LOAD_METHOD              1 (get)
                             40 LOAD_CONST               1 ('animation')
                             42 LOAD_CONST               2 ('')
                             44 PRECALL                  2
                             48 CALL                     2
                             58 LOAD_METHOD              2 (lower)
                             80 PRECALL                  0
                             84 CALL                     0
                             94 STORE_FAST               4 (animation_type)
                
-               823          96 LOAD_FAST                2 (monitor)
+               829          96 LOAD_FAST                2 (monitor)
                             98 LOAD_CONST               3 ('activeWorkspace')
                            100 BINARY_SUBSCR
                            110 LOAD_CONST               4 ('id')
                            112 BINARY_SUBSCR
                            122 STORE_FAST               5 (wrkspc)
                
-               824         124 LOAD_GLOBAL              7 (NULL + time)
+               830         124 LOAD_GLOBAL              7 (NULL + time)
                            136 LOAD_ATTR                3 (time)
                            146 PRECALL                  0
                            150 CALL                     0
                            160 LOAD_FAST                1 (item)
                            162 LOAD_ATTR                4 (meta)
                            172 LOAD_CONST               5 ('last_shown')
                            174 STORE_SUBSCR
                
-               826         178 LOAD_FAST                0 (self)
+               832         178 LOAD_FAST                0 (self)
                            180 LOAD_METHOD              5 (hyprctl)
                
-               828         202 LOAD_CONST               6 ('moveworkspacetomonitor special:scratch_')
+               834         202 LOAD_CONST               6 ('moveworkspacetomonitor special:scratch_')
                            204 LOAD_FAST                1 (item)
                            206 LOAD_ATTR                6 (uid)
                            216 FORMAT_VALUE             0
                            218 LOAD_CONST               7 (' ')
                            220 LOAD_FAST                2 (monitor)
                            222 LOAD_CONST               8 ('name')
                            224 BINARY_SUBSCR
                            234 FORMAT_VALUE             0
                            236 BUILD_STRING             4
                
-               829         238 LOAD_CONST               9 ('movetoworkspacesilent ')
+               835         238 LOAD_CONST               9 ('movetoworkspacesilent ')
                            240 LOAD_FAST                5 (wrkspc)
                            242 FORMAT_VALUE             0
                            244 LOAD_CONST              10 (',address:')
                            246 LOAD_FAST                1 (item)
                            248 LOAD_ATTR                7 (full_address)
                            258 FORMAT_VALUE             0
                            260 BUILD_STRING             4
                
-               830         262 LOAD_CONST              11 ('alterzorder top,address:')
+               836         262 LOAD_CONST              11 ('alterzorder top,address:')
                            264 LOAD_FAST                1 (item)
                            266 LOAD_ATTR                7 (full_address)
                            276 FORMAT_VALUE             0
                            278 BUILD_STRING             2
                
-               827         280 BUILD_LIST               3
+               833         280 BUILD_LIST               3
                
-               826         282 PRECALL                  1
+               832         282 PRECALL                  1
                            286 CALL                     1
                            296 GET_AWAITABLE            0
                            298 LOAD_CONST              12 (None)
                        >>  300 SEND                     3 (to 308)
                            302 YIELD_VALUE
                            304 RESUME                   3
                            306 JUMP_BACKWARD_NO_INTERRUPT     4 (to 300)
                        >>  308 POP_TOP
                
-               833         310 LOAD_FAST                0 (self)
+               839         310 LOAD_FAST                0 (self)
                            312 LOAD_METHOD              8 (cast_bool)
                            334 LOAD_FAST                1 (item)
                            336 LOAD_ATTR                0 (conf)
                            346 LOAD_METHOD              1 (get)
                            368 LOAD_CONST              13 ('preserve_aspect')
                            370 PRECALL                  1
                            374 CALL                     1
                            384 PRECALL                  1
                            388 CALL                     1
                            398 STORE_FAST               6 (preserve_aspect)
                
-               835         400 LOAD_FAST                6 (preserve_aspect)
+               841         400 LOAD_FAST                6 (preserve_aspect)
                            402 JUMP_IF_FALSE_OR_POP     1 (to 406)
                            404 LOAD_FAST                3 (was_alive)
                        >>  406 UNARY_NOT
                            408 JUMP_IF_TRUE_OR_POP     20 (to 450)
                            410 LOAD_FAST                1 (item)
                            412 LOAD_ATTR                9 (monitor)
                            422 LOAD_GLOBAL             20 (state)
                            434 LOAD_ATTR               11 (active_monitor)
                            444 COMPARE_OP               3 (!=)
                
-               834     >>  450 STORE_FAST               7 (should_set_aspect)
+               840     >>  450 STORE_FAST               7 (should_set_aspect)
                
-               837         452 LOAD_FAST                7 (should_set_aspect)
+               843         452 LOAD_FAST                7 (should_set_aspect)
                            454 POP_JUMP_FORWARD_IF_FALSE    28 (to 512)
                
-               838         456 LOAD_FAST                0 (self)
+               844         456 LOAD_FAST                0 (self)
                            458 LOAD_METHOD             12 (_fix_size)
                            480 LOAD_FAST                1 (item)
                            482 LOAD_FAST                2 (monitor)
                            484 PRECALL                  2
                            488 CALL                     2
                            498 GET_AWAITABLE            0
                            500 LOAD_CONST              12 (None)
                        >>  502 SEND                     3 (to 510)
                            504 YIELD_VALUE
                            506 RESUME                   3
                            508 JUMP_BACKWARD_NO_INTERRUPT     4 (to 502)
                        >>  510 POP_TOP
                
-               839     >>  512 LOAD_FAST                1 (item)
+               845     >>  512 LOAD_FAST                1 (item)
                            514 LOAD_METHOD             13 (updateClientInfo)
                            536 PRECALL                  0
                            540 CALL                     0
                            550 GET_AWAITABLE            0
                            552 LOAD_CONST              12 (None)
                        >>  554 SEND                     3 (to 562)
                            556 YIELD_VALUE
                            558 RESUME                   3
                            560 JUMP_BACKWARD_NO_INTERRUPT     4 (to 554)
                        >>  562 POP_TOP
                
-               840         564 LOAD_CONST              14 (False)
+               846         564 LOAD_CONST              14 (False)
                            566 STORE_FAST               8 (position_fixed)
                
-               841         568 LOAD_FAST                7 (should_set_aspect)
+               847         568 LOAD_FAST                7 (should_set_aspect)
                            570 POP_JUMP_FORWARD_IF_FALSE    28 (to 628)
                
-               842         572 LOAD_FAST                0 (self)
+               848         572 LOAD_FAST                0 (self)
                            574 LOAD_METHOD             14 (_fix_position)
                            596 LOAD_FAST                1 (item)
                            598 LOAD_FAST                2 (monitor)
                            600 PRECALL                  2
                            604 CALL                     2
                            614 GET_AWAITABLE            0
                            616 LOAD_CONST              12 (None)
                        >>  618 SEND                     3 (to 626)
                            620 YIELD_VALUE
                            622 RESUME                   3
                            624 JUMP_BACKWARD_NO_INTERRUPT     4 (to 618)
                        >>  626 STORE_FAST               8 (position_fixed)
                
-               843     >>  628 LOAD_FAST                8 (position_fixed)
+               849     >>  628 LOAD_FAST                8 (position_fixed)
                            630 POP_JUMP_FORWARD_IF_TRUE   248 (to 1128)
                
-               844         632 LOAD_FAST                4 (animation_type)
+               850         632 LOAD_FAST                4 (animation_type)
                            634 POP_JUMP_FORWARD_IF_FALSE   214 (to 1064)
                
-               846         636 LOAD_FAST                6 (preserve_aspect)
+               852         636 LOAD_FAST                6 (preserve_aspect)
                            638 POP_JUMP_FORWARD_IF_FALSE   104 (to 848)
                            640 LOAD_FAST                3 (was_alive)
                            642 POP_JUMP_FORWARD_IF_FALSE   102 (to 848)
                            644 LOAD_FAST                7 (should_set_aspect)
                            646 POP_JUMP_FORWARD_IF_TRUE   100 (to 848)
                
-               847         648 LOAD_CONST              15 ('size')
+               853         648 LOAD_CONST              15 ('size')
                            650 LOAD_FAST                1 (item)
                            652 LOAD_ATTR               15 (client_info)
                            662 CONTAINS_OP              1
                            664 POP_JUMP_FORWARD_IF_FALSE    27 (to 720)
                
-               848         666 LOAD_FAST                0 (self)
+               854         666 LOAD_FAST                0 (self)
                            668 LOAD_METHOD             16 (updateScratchInfo)
                            690 LOAD_FAST                1 (item)
                            692 PRECALL                  1
                            696 CALL                     1
                            706 GET_AWAITABLE            0
                            708 LOAD_CONST              12 (None)
                        >>  710 SEND                     3 (to 718)
                            712 YIELD_VALUE
                            714 RESUME                   3
                            716 JUMP_BACKWARD_NO_INTERRUPT     4 (to 710)
                        >>  718 POP_TOP
                
-               850     >>  720 LOAD_FAST                0 (self)
+               856     >>  720 LOAD_FAST                0 (self)
                            722 LOAD_METHOD             17 (get_offsets)
                            744 LOAD_FAST                1 (item)
                            746 LOAD_FAST                2 (monitor)
                            748 PRECALL                  2
                            752 CALL                     2
                            762 GET_AWAITABLE            0
                            764 LOAD_CONST              12 (None)
@@ -7144,15 +7182,15 @@
                            768 YIELD_VALUE
                            770 RESUME                   3
                            772 JUMP_BACKWARD_NO_INTERRUPT     4 (to 766)
                        >>  774 UNPACK_SEQUENCE          2
                            778 STORE_FAST               9 (ox)
                            780 STORE_FAST              10 (oy)
                
-               851         782 LOAD_FAST                0 (self)
+               857         782 LOAD_FAST                0 (self)
                            784 LOAD_METHOD             18 (_slide_animation)
                            806 LOAD_FAST                4 (animation_type)
                            808 LOAD_FAST                1 (item)
                            810 LOAD_FAST                9 (ox)
                            812 UNARY_NEGATIVE
                            814 LOAD_FAST               10 (oy)
                            816 UNARY_NEGATIVE
@@ -7163,77 +7201,77 @@
                        >>  836 SEND                     3 (to 844)
                            838 YIELD_VALUE
                            840 RESUME                   3
                            842 JUMP_BACKWARD_NO_INTERRUPT     4 (to 836)
                        >>  844 POP_TOP
                            846 JUMP_FORWARD           140 (to 1128)
                
-               853     >>  848 LOAD_FAST                1 (item)
+               859     >>  848 LOAD_FAST                1 (item)
                            850 LOAD_ATTR                0 (conf)
                            860 LOAD_METHOD              1 (get)
                            882 LOAD_CONST              16 ('margin')
                            884 LOAD_GLOBAL             38 (DEFAULT_MARGIN)
                            896 PRECALL                  2
                            900 CALL                     2
                            910 STORE_FAST              11 (margin)
                
-               854         912 LOAD_GLOBAL             41 (NULL + getattr)
+               860         912 LOAD_GLOBAL             41 (NULL + getattr)
                            924 LOAD_GLOBAL             42 (Animations)
                            936 LOAD_FAST                4 (animation_type)
                            938 PRECALL                  2
                            942 CALL                     2
                            952 STORE_FAST              12 (fn)
                
-               855         954 PUSH_NULL
+               861         954 PUSH_NULL
                            956 LOAD_FAST               12 (fn)
                
-               856         958 LOAD_FAST                2 (monitor)
+               862         958 LOAD_FAST                2 (monitor)
                
-               857         960 LOAD_FAST                1 (item)
+               863         960 LOAD_FAST                1 (item)
                            962 LOAD_ATTR               15 (client_info)
                
-               858         972 LOAD_CONST              17 ('address:')
+               864         972 LOAD_CONST              17 ('address:')
                            974 LOAD_FAST                1 (item)
                            976 LOAD_ATTR                7 (full_address)
                            986 BINARY_OP                0 (+)
                
-               859         990 LOAD_FAST               11 (margin)
+               865         990 LOAD_FAST               11 (margin)
                
-               855         992 PRECALL                  4
+               861         992 PRECALL                  4
                            996 CALL                     4
                           1006 STORE_FAST              13 (command)
                
-               861        1008 LOAD_FAST                0 (self)
+               867        1008 LOAD_FAST                0 (self)
                           1010 LOAD_METHOD              5 (hyprctl)
                           1032 LOAD_FAST               13 (command)
                           1034 PRECALL                  1
                           1038 CALL                     1
                           1048 GET_AWAITABLE            0
                           1050 LOAD_CONST              12 (None)
                        >> 1052 SEND                     3 (to 1060)
                           1054 YIELD_VALUE
                           1056 RESUME                   3
                           1058 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1052)
                        >> 1060 POP_TOP
                           1062 JUMP_FORWARD            32 (to 1128)
                
-               863     >> 1064 LOAD_FAST                0 (self)
+               869     >> 1064 LOAD_FAST                0 (self)
                           1066 LOAD_ATTR               22 (log)
                           1076 LOAD_METHOD             23 (warning)
                
-               864        1098 LOAD_CONST              18 ("No position and no animation provided for %s, don't know where to place it.")
+               870        1098 LOAD_CONST              18 ("No position and no animation provided for %s, don't know where to place it.")
                
-               865        1100 LOAD_FAST                1 (item)
+               871        1100 LOAD_FAST                1 (item)
                           1102 LOAD_ATTR                6 (uid)
                
-               863        1112 PRECALL                  2
+               869        1112 PRECALL                  2
                           1116 CALL                     2
                           1126 POP_TOP
                
-               868     >> 1128 LOAD_FAST                0 (self)
+               874     >> 1128 LOAD_FAST                0 (self)
                           1130 LOAD_METHOD              5 (hyprctl)
                           1152 LOAD_CONST              19 ('focuswindow address:')
                           1154 LOAD_FAST                1 (item)
                           1156 LOAD_ATTR                7 (full_address)
                           1166 FORMAT_VALUE             0
                           1168 BUILD_STRING             2
                           1170 PRECALL                  1
@@ -7242,24 +7280,30 @@
                           1186 LOAD_CONST              12 (None)
                        >> 1188 SEND                     3 (to 1196)
                           1190 YIELD_VALUE
                           1192 RESUME                   3
                           1194 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1188)
                        >> 1196 POP_TOP
                
-               869        1198 LOAD_GLOBAL              7 (NULL + time)
+               875        1198 LOAD_GLOBAL              7 (NULL + time)
                           1210 LOAD_ATTR                3 (time)
                           1220 PRECALL                  0
                           1224 CALL                     0
                           1234 LOAD_FAST                1 (item)
                           1236 LOAD_ATTR                4 (meta)
                           1246 LOAD_CONST               5 ('last_shown')
                           1248 STORE_SUBSCR
-                          1252 LOAD_CONST              12 (None)
-                          1254 RETURN_VALUE
+               
+               876        1252 LOAD_FAST                2 (monitor)
+                          1254 LOAD_FAST                1 (item)
+                          1256 LOAD_ATTR                4 (meta)
+                          1266 LOAD_CONST              20 ('monitor_info')
+                          1268 STORE_SUBSCR
+                          1272 LOAD_CONST              12 (None)
+                          1274 RETURN_VALUE
                consts
                   'perfoms the transition to visible state'
                   'animation'
                   ''
                   'activeWorkspace'
                   'id'
                   'last_shown'
@@ -7273,25 +7317,26 @@
                   'preserve_aspect'
                   False
                   'size'
                   'margin'
                   'address:'
                   "No position and no animation provided for %s, don't know where to place it."
                   'focuswindow address:'
+                  'monitor_info'
                names      ('conf', 'get', 'lower', 'time', 'meta', 'hyprctl', 'uid', 'full_address', 'cast_bool', 'monitor', 'state', 'active_monitor', '_fix_size', 'updateClientInfo', '_fix_position', 'client_info', 'updateScratchInfo', 'get_offsets', '_slide_animation', 'DEFAULT_MARGIN', 'getattr', 'Animations', 'log', 'warning')
                varnames   ('self', 'item', 'monitor', 'was_alive', 'animation_type', 'wrkspc', 'preserve_aspect', 'should_set_aspect', 'position_fixed', 'ox', 'oy', 'margin', 'fn', 'command')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       '_show_transition'
-               firstlineno 820
+               firstlineno 826
                lnotab
                   0x06025a011c01360218022401180112fd02ff1c075a0232ff0203040138
                   013401040104013801040104020c01120136023e01420240012a01040102
-                  010c01120102fc10063802220102010cfe10054601
+                  010c01120102fc10063802220102010cfe100546013601
             code
                argcount  : 3
                nlocals   : 9
                stacksize : 8
                flags     : 131
                code
                   0x4b00010097007c016a000000000000000000a001000000000000000000
@@ -7303,104 +7348,104 @@
                   007c006a0300000000000000007c067c02a6030000ab0300000000000000
                   005c0200007d077d087409000000000000000000007c077c04a6020000ab
                   0200000000000000007d047409000000000000000000007c087c05a60200
                   00ab0200000000000000007d057c00a00500000000000000000000000000
                   0000000000000064037c049b0064047c059b0064057c016a060000000000
                   0000009b009d06a6010000ab010000000000000000830064067b03560097
                   03860401006406530064065300
-               871           0 RETURN_GENERATOR
+               878           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               874           6 LOAD_FAST                1 (item)
+               881           6 LOAD_FAST                1 (item)
                              8 LOAD_ATTR                0 (conf)
                             18 LOAD_METHOD              1 (get)
                             40 LOAD_CONST               1 ('size')
                             42 PRECALL                  1
                             46 CALL                     1
                             56 STORE_FAST               3 (size)
                
-               875          58 LOAD_FAST                3 (size)
+               882          58 LOAD_FAST                3 (size)
                             60 POP_JUMP_FORWARD_IF_FALSE   153 (to 368)
                
-               876          62 LOAD_GLOBAL              5 (NULL + convert_coords)
+               883          62 LOAD_GLOBAL              5 (NULL + convert_coords)
                             74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                3 (log)
                             86 LOAD_FAST                3 (size)
                             88 LOAD_FAST                2 (monitor)
                             90 PRECALL                  3
                             94 CALL                     3
                            104 UNPACK_SEQUENCE          2
                            108 STORE_FAST               4 (width)
                            110 STORE_FAST               5 (height)
                
-               877         112 LOAD_FAST                1 (item)
+               884         112 LOAD_FAST                1 (item)
                            114 LOAD_ATTR                0 (conf)
                            124 LOAD_METHOD              1 (get)
                            146 LOAD_CONST               2 ('max_size')
                            148 PRECALL                  1
                            152 CALL                     1
                            162 STORE_FAST               6 (max_size)
                
-               878         164 LOAD_FAST                6 (max_size)
+               885         164 LOAD_FAST                6 (max_size)
                            166 POP_JUMP_FORWARD_IF_FALSE    57 (to 282)
                
-               879         168 LOAD_GLOBAL              5 (NULL + convert_coords)
+               886         168 LOAD_GLOBAL              5 (NULL + convert_coords)
                            180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                3 (log)
                            192 LOAD_FAST                6 (max_size)
                            194 LOAD_FAST                2 (monitor)
                            196 PRECALL                  3
                            200 CALL                     3
                            210 UNPACK_SEQUENCE          2
                            214 STORE_FAST               7 (max_width)
                            216 STORE_FAST               8 (max_height)
                
-               880         218 LOAD_GLOBAL              9 (NULL + min)
+               887         218 LOAD_GLOBAL              9 (NULL + min)
                            230 LOAD_FAST                7 (max_width)
                            232 LOAD_FAST                4 (width)
                            234 PRECALL                  2
                            238 CALL                     2
                            248 STORE_FAST               4 (width)
                
-               881         250 LOAD_GLOBAL              9 (NULL + min)
+               888         250 LOAD_GLOBAL              9 (NULL + min)
                            262 LOAD_FAST                8 (max_height)
                            264 LOAD_FAST                5 (height)
                            266 PRECALL                  2
                            270 CALL                     2
                            280 STORE_FAST               5 (height)
                
-               882     >>  282 LOAD_FAST                0 (self)
+               889     >>  282 LOAD_FAST                0 (self)
                            284 LOAD_METHOD              5 (hyprctl)
                
-               883         306 LOAD_CONST               3 ('resizewindowpixel exact ')
+               890         306 LOAD_CONST               3 ('resizewindowpixel exact ')
                            308 LOAD_FAST                4 (width)
                            310 FORMAT_VALUE             0
                            312 LOAD_CONST               4 (' ')
                            314 LOAD_FAST                5 (height)
                            316 FORMAT_VALUE             0
                            318 LOAD_CONST               5 (',address:')
                            320 LOAD_FAST                1 (item)
                            322 LOAD_ATTR                6 (full_address)
                            332 FORMAT_VALUE             0
                            334 BUILD_STRING             6
                
-               882         336 PRECALL                  1
+               889         336 PRECALL                  1
                            340 CALL                     1
                            350 GET_AWAITABLE            0
                            352 LOAD_CONST               6 (None)
                        >>  354 SEND                     3 (to 362)
                            356 YIELD_VALUE
                            358 RESUME                   3
                            360 JUMP_BACKWARD_NO_INTERRUPT     4 (to 354)
                        >>  362 POP_TOP
                            364 LOAD_CONST               6 (None)
                            366 RETURN_VALUE
                
-               875     >>  368 LOAD_CONST               6 (None)
+               882     >>  368 LOAD_CONST               6 (None)
                            370 RETURN_VALUE
                consts
                   'apply the `size` config parameter'
                   'size'
                   'max_size'
                   'resizewindowpixel exact '
                   ' '
@@ -7408,15 +7453,15 @@
                   None
                names      ('conf', 'get', 'convert_coords', 'log', 'min', 'hyprctl', 'full_address')
                varnames   ('self', 'item', 'monitor', 'size', 'width', 'height', 'max_size', 'max_width', 'max_height')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       '_fix_size'
-               firstlineno 871
+               firstlineno 878
                lnotab 0x06033401040132013401040132012001200118011eff20f9
             code
                argcount  : 3
                nlocals   : 8
                stacksize : 8
                flags     : 131
                code
@@ -7425,82 +7470,82 @@
                   03725a7405000000000000000000007c006a0300000000000000007c037c
                   02a6030000ab0300000000000000005c0200007d047d057c047c02640219
                   0000000000000000007a0000007c057c026403190000000000000000007a
                   0000007d077d067c00a00400000000000000000000000000000000000000
                   0064047c069b0064057c079b0064067c016a0500000000000000009b009d
                   06a6010000ab010000000000000000830064077b03560097038604010064
                   08530064095300
-               886           0 RETURN_GENERATOR
+               893           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               889           6 LOAD_FAST                1 (item)
+               896           6 LOAD_FAST                1 (item)
                              8 LOAD_ATTR                0 (conf)
                             18 LOAD_METHOD              1 (get)
                             40 LOAD_CONST               1 ('position')
                             42 PRECALL                  1
                             46 CALL                     1
                             56 STORE_FAST               3 (position)
                
-               890          58 LOAD_FAST                3 (position)
+               897          58 LOAD_FAST                3 (position)
                             60 POP_JUMP_FORWARD_IF_FALSE    90 (to 242)
                
-               891          62 LOAD_GLOBAL              5 (NULL + convert_coords)
+               898          62 LOAD_GLOBAL              5 (NULL + convert_coords)
                             74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                3 (log)
                             86 LOAD_FAST                3 (position)
                             88 LOAD_FAST                2 (monitor)
                             90 PRECALL                  3
                             94 CALL                     3
                            104 UNPACK_SEQUENCE          2
                            108 STORE_FAST               4 (x_pos)
                            110 STORE_FAST               5 (y_pos)
                
-               892         112 LOAD_FAST                4 (x_pos)
+               899         112 LOAD_FAST                4 (x_pos)
                            114 LOAD_FAST                2 (monitor)
                            116 LOAD_CONST               2 ('x')
                            118 BINARY_SUBSCR
                            128 BINARY_OP                0 (+)
                            132 LOAD_FAST                5 (y_pos)
                            134 LOAD_FAST                2 (monitor)
                            136 LOAD_CONST               3 ('y')
                            138 BINARY_SUBSCR
                            148 BINARY_OP                0 (+)
                            152 STORE_FAST               7 (y_pos_abs)
                            154 STORE_FAST               6 (x_pos_abs)
                
-               893         156 LOAD_FAST                0 (self)
+               900         156 LOAD_FAST                0 (self)
                            158 LOAD_METHOD              4 (hyprctl)
                
-               894         180 LOAD_CONST               4 ('movewindowpixel exact ')
+               901         180 LOAD_CONST               4 ('movewindowpixel exact ')
                            182 LOAD_FAST                6 (x_pos_abs)
                            184 FORMAT_VALUE             0
                            186 LOAD_CONST               5 (' ')
                            188 LOAD_FAST                7 (y_pos_abs)
                            190 FORMAT_VALUE             0
                            192 LOAD_CONST               6 (',address:')
                            194 LOAD_FAST                1 (item)
                            196 LOAD_ATTR                5 (full_address)
                            206 FORMAT_VALUE             0
                            208 BUILD_STRING             6
                
-               893         210 PRECALL                  1
+               900         210 PRECALL                  1
                            214 CALL                     1
                            224 GET_AWAITABLE            0
                            226 LOAD_CONST               7 (None)
                        >>  228 SEND                     3 (to 236)
                            230 YIELD_VALUE
                            232 RESUME                   3
                            234 JUMP_BACKWARD_NO_INTERRUPT     4 (to 228)
                        >>  236 POP_TOP
                
-               896         238 LOAD_CONST               8 (True)
+               903         238 LOAD_CONST               8 (True)
                            240 RETURN_VALUE
                
-               897     >>  242 LOAD_CONST               9 (False)
+               904     >>  242 LOAD_CONST               9 (False)
                            244 RETURN_VALUE
                consts
                   'apply the `position` config parameter'
                   'position'
                   'x'
                   'y'
                   'movewindowpixel exact '
@@ -7511,15 +7556,15 @@
                   False
                names      ('conf', 'get', 'convert_coords', 'log', 'hyprctl', 'full_address')
                varnames   ('self', 'item', 'monitor', 'position', 'x_pos', 'y_pos', 'x_pos_abs', 'y_pos_abs')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       '_fix_position'
-               firstlineno 886
+               firstlineno 893
                lnotab 0x06033401040132012c0118011eff1c030401
             False
             'uid'
             code
                argcount  : 4
                nlocals   : 6
                stacksize : 6
@@ -7533,84 +7578,82 @@
                   01a6020000ab0200000000000000000100640353007c046a050000000000
                   000000733a7c0273387c03733674050000000000000000000064017c019b
                   0064059d03a6010000ab010000000000000000830064037b035600970386
                   0401007c006a030000000000000000a00400000000000000000000000000
                   0000000000000064067c01a6020000ab0200000000000000000100640353
                   0064077c045f0500000000000000007c006a030000000000000000a00600
                   0000000000000000000000000000000000000064087c01a6020000ab0200
-                  0000000000000001007c046a070000000000000000a00100000000000000
-                  000000000000000000000000006409640aa6020000ab0200000000000000
-                  00a0080000000000000000000000000000000000000000a6000000ab0000
-                  000000000000007d057c05721c7c00a00900000000000000000000000000
-                  000000000000007c057c04a6020000ab020000000000000000830064037b
-                  0356009703860401007c00a00a0000000000000000000000000000000000
-                  000000640b7c019b00640c7c046a0b00000000000000009b009d04a60100
-                  00ab010000000000000000830064037b0356009703860401007c03736c7c
-                  05726c7c017c006a0c0000000000000000760072657c00a00d0000000000
-                  0000000000000000000000000000007c046a070000000000000000a00100
-                  00000000000000000000000000000000000000640da6010000ab01000000
-                  0000000000640ea6020000ab02000000000000000072397c00a00a000000
-                  0000000000000000000000000000000000640f7c006a0c00000000000000
-                  007c01190000000000000000009b009d02a6010000ab0100000000000000
-                  00830064037b0356009703860401007c006a0c00000000000000007c013d
-                  006403530064035300640353006403530064035300
-               899           0 RETURN_GENERATOR
+                  0000000000000001007c00a0070000000000000000000000000000000000
+                  0000007c047c046a080000000000000000640919000000000000000000a6
+                  020000ab020000000000000000830064037b035600970386047d057c00a0
+                  090000000000000000000000000000000000000000640a7c019b00640b7c
+                  046a0a00000000000000009b009d04a6010000ab01000000000000000083
+                  0064037b0356009703860401007c03736c7c05726c7c017c006a0b000000
+                  0000000000760072657c00a00c0000000000000000000000000000000000
+                  0000007c046a0d0000000000000000a00100000000000000000000000000
+                  00000000000000640ca6010000ab010000000000000000640da6020000ab
+                  02000000000000000072397c00a009000000000000000000000000000000
+                  0000000000640e7c006a0b00000000000000007c01190000000000000000
+                  009b009d02a6010000ab010000000000000000830064037b035600970386
+                  0401007c006a0b00000000000000007c013d006403530064035300640353
+                  006403530064035300
+               906           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               903           6 LOAD_FAST                0 (self)
+               910           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (scratches)
                             18 LOAD_METHOD              1 (get)
                             40 LOAD_FAST                1 (uid)
                             42 PRECALL                  1
                             46 CALL                     1
                             56 STORE_FAST               4 (scratch)
                
-               905          58 LOAD_FAST                4 (scratch)
+               912          58 LOAD_FAST                4 (scratch)
                             60 POP_JUMP_FORWARD_IF_TRUE    54 (to 170)
                
-               906          62 LOAD_GLOBAL              5 (NULL + notify_error)
+               913          62 LOAD_GLOBAL              5 (NULL + notify_error)
                
-               907          74 LOAD_CONST               1 ("Scratchpad '")
+               914          74 LOAD_CONST               1 ("Scratchpad '")
                             76 LOAD_FAST                1 (uid)
                             78 FORMAT_VALUE             0
                             80 LOAD_CONST               2 ("' not found, check your configuration or the hide parameter")
                             82 BUILD_STRING             3
                
-               906          84 PRECALL                  1
+               913          84 PRECALL                  1
                             88 CALL                     1
                             98 GET_AWAITABLE            0
                            100 LOAD_CONST               3 (None)
                        >>  102 SEND                     3 (to 110)
                            104 YIELD_VALUE
                            106 RESUME                   3
                            108 JUMP_BACKWARD_NO_INTERRUPT     4 (to 102)
                        >>  110 POP_TOP
                
-               909         112 LOAD_FAST                0 (self)
+               916         112 LOAD_FAST                0 (self)
                            114 LOAD_ATTR                3 (log)
                            124 LOAD_METHOD              4 (warning)
                            146 LOAD_CONST               4 ('%s is not configured')
                            148 LOAD_FAST                1 (uid)
                            150 PRECALL                  2
                            154 CALL                     2
                            164 POP_TOP
                
-               910         166 LOAD_CONST               3 (None)
+               917         166 LOAD_CONST               3 (None)
                            168 RETURN_VALUE
                
-               911     >>  170 LOAD_FAST                4 (scratch)
+               918     >>  170 LOAD_FAST                4 (scratch)
                            172 LOAD_ATTR                5 (visible)
                            182 POP_JUMP_FORWARD_IF_TRUE    58 (to 300)
                            184 LOAD_FAST                2 (force)
                            186 POP_JUMP_FORWARD_IF_TRUE    56 (to 300)
                            188 LOAD_FAST                3 (autohide)
                            190 POP_JUMP_FORWARD_IF_TRUE    54 (to 300)
                
-               912         192 LOAD_GLOBAL              5 (NULL + notify_error)
+               919         192 LOAD_GLOBAL              5 (NULL + notify_error)
                            204 LOAD_CONST               1 ("Scratchpad '")
                            206 LOAD_FAST                1 (uid)
                            208 FORMAT_VALUE             0
                            210 LOAD_CONST               5 ("' is not visible, will not hide.")
                            212 BUILD_STRING             3
                            214 PRECALL                  1
                            218 CALL                     1
@@ -7618,197 +7661,184 @@
                            230 LOAD_CONST               3 (None)
                        >>  232 SEND                     3 (to 240)
                            234 YIELD_VALUE
                            236 RESUME                   3
                            238 JUMP_BACKWARD_NO_INTERRUPT     4 (to 232)
                        >>  240 POP_TOP
                
-               913         242 LOAD_FAST                0 (self)
+               920         242 LOAD_FAST                0 (self)
                            244 LOAD_ATTR                3 (log)
                            254 LOAD_METHOD              4 (warning)
                            276 LOAD_CONST               6 ('%s is already hidden')
                            278 LOAD_FAST                1 (uid)
                            280 PRECALL                  2
                            284 CALL                     2
                            294 POP_TOP
                
-               914         296 LOAD_CONST               3 (None)
+               921         296 LOAD_CONST               3 (None)
                            298 RETURN_VALUE
                
-               915     >>  300 LOAD_CONST               7 (False)
+               922     >>  300 LOAD_CONST               7 (False)
                            302 LOAD_FAST                4 (scratch)
                            304 STORE_ATTR               5 (visible)
                
-               916         314 LOAD_FAST                0 (self)
+               923         314 LOAD_FAST                0 (self)
                            316 LOAD_ATTR                3 (log)
                            326 LOAD_METHOD              6 (info)
                            348 LOAD_CONST               8 ('Hiding %s')
                            350 LOAD_FAST                1 (uid)
                            352 PRECALL                  2
                            356 CALL                     2
                            366 POP_TOP
                
-               917         368 LOAD_FAST                4 (scratch)
-                           370 LOAD_ATTR                7 (conf)
-                           380 LOAD_METHOD              1 (get)
-                           402 LOAD_CONST               9 ('animation')
-                           404 LOAD_CONST              10 ('')
-                           406 PRECALL                  2
-                           410 CALL                     2
-                           420 LOAD_METHOD              8 (lower)
-                           442 PRECALL                  0
-                           446 CALL                     0
-                           456 STORE_FAST               5 (animation_type)
-               
-               918         458 LOAD_FAST                5 (animation_type)
-                           460 POP_JUMP_FORWARD_IF_FALSE    28 (to 518)
-               
-               919         462 LOAD_FAST                0 (self)
-                           464 LOAD_METHOD              9 (_anim_hide)
-                           486 LOAD_FAST                5 (animation_type)
-                           488 LOAD_FAST                4 (scratch)
-                           490 PRECALL                  2
-                           494 CALL                     2
-                           504 GET_AWAITABLE            0
-                           506 LOAD_CONST               3 (None)
-                       >>  508 SEND                     3 (to 516)
-                           510 YIELD_VALUE
-                           512 RESUME                   3
-                           514 JUMP_BACKWARD_NO_INTERRUPT     4 (to 508)
-                       >>  516 POP_TOP
-               
-               921     >>  518 LOAD_FAST                0 (self)
-                           520 LOAD_METHOD             10 (hyprctl)
-               
-               922         542 LOAD_CONST              11 ('movetoworkspacesilent special:scratch_')
-                           544 LOAD_FAST                1 (uid)
-                           546 FORMAT_VALUE             0
-                           548 LOAD_CONST              12 (',address:')
-                           550 LOAD_FAST                4 (scratch)
-                           552 LOAD_ATTR               11 (full_address)
-                           562 FORMAT_VALUE             0
-                           564 BUILD_STRING             4
-               
-               921         566 PRECALL                  1
-                           570 CALL                     1
-                           580 GET_AWAITABLE            0
-                           582 LOAD_CONST               3 (None)
-                       >>  584 SEND                     3 (to 592)
-                           586 YIELD_VALUE
-                           588 RESUME                   3
-                           590 JUMP_BACKWARD_NO_INTERRUPT     4 (to 584)
-                       >>  592 POP_TOP
-               
-               926         594 LOAD_FAST                3 (autohide)
-               
-               925         596 POP_JUMP_FORWARD_IF_TRUE   108 (to 814)
-               
-               927         598 LOAD_FAST                5 (animation_type)
-               
-               925         600 POP_JUMP_FORWARD_IF_FALSE   108 (to 818)
-               
-               928         602 LOAD_FAST                1 (uid)
-                           604 LOAD_FAST                0 (self)
-                           606 LOAD_ATTR               12 (focused_window_tracking)
-                           616 CONTAINS_OP              0
-                           618 POP_JUMP_FORWARD_IF_FALSE   101 (to 822)
-               
-               929         620 LOAD_FAST                0 (self)
-                           622 LOAD_METHOD             13 (cast_bool)
-                           644 LOAD_FAST                4 (scratch)
-                           646 LOAD_ATTR                7 (conf)
-                           656 LOAD_METHOD              1 (get)
-                           678 LOAD_CONST              13 ('restore_focus')
-                           680 PRECALL                  1
-                           684 CALL                     1
-                           694 LOAD_CONST              14 (True)
-                           696 PRECALL                  2
-                           700 CALL                     2
-               
-               928         710 POP_JUMP_FORWARD_IF_FALSE    57 (to 826)
-               
-               931         712 LOAD_FAST                0 (self)
-                           714 LOAD_METHOD             10 (hyprctl)
-               
-               932         736 LOAD_CONST              15 ('focuswindow address:')
-                           738 LOAD_FAST                0 (self)
-                           740 LOAD_ATTR               12 (focused_window_tracking)
-                           750 LOAD_FAST                1 (uid)
-                           752 BINARY_SUBSCR
-                           762 FORMAT_VALUE             0
-                           764 BUILD_STRING             2
-               
-               931         766 PRECALL                  1
-                           770 CALL                     1
-                           780 GET_AWAITABLE            0
-                           782 LOAD_CONST               3 (None)
-                       >>  784 SEND                     3 (to 792)
-                           786 YIELD_VALUE
-                           788 RESUME                   3
-                           790 JUMP_BACKWARD_NO_INTERRUPT     4 (to 784)
-                       >>  792 POP_TOP
-               
-               934         794 LOAD_FAST                0 (self)
-                           796 LOAD_ATTR               12 (focused_window_tracking)
-                           806 LOAD_FAST                1 (uid)
-                           808 DELETE_SUBSCR
-                           810 LOAD_CONST               3 (None)
-                           812 RETURN_VALUE
-               
-               925     >>  814 LOAD_CONST               3 (None)
-                           816 RETURN_VALUE
-                       >>  818 LOAD_CONST               3 (None)
-                           820 RETURN_VALUE
-               
-               928     >>  822 LOAD_CONST               3 (None)
-                           824 RETURN_VALUE
-                       >>  826 LOAD_CONST               3 (None)
-                           828 RETURN_VALUE
+               924         368 LOAD_FAST                0 (self)
+                           370 LOAD_METHOD              7 (_hide_transition)
+                           392 LOAD_FAST                4 (scratch)
+                           394 LOAD_FAST                4 (scratch)
+                           396 LOAD_ATTR                8 (meta)
+                           406 LOAD_CONST               9 ('monitor_info')
+                           408 BINARY_SUBSCR
+                           418 PRECALL                  2
+                           422 CALL                     2
+                           432 GET_AWAITABLE            0
+                           434 LOAD_CONST               3 (None)
+                       >>  436 SEND                     3 (to 444)
+                           438 YIELD_VALUE
+                           440 RESUME                   3
+                           442 JUMP_BACKWARD_NO_INTERRUPT     4 (to 436)
+                       >>  444 STORE_FAST               5 (animated)
+               
+               926         446 LOAD_FAST                0 (self)
+                           448 LOAD_METHOD              9 (hyprctl)
+               
+               927         470 LOAD_CONST              10 ('movetoworkspacesilent special:scratch_')
+                           472 LOAD_FAST                1 (uid)
+                           474 FORMAT_VALUE             0
+                           476 LOAD_CONST              11 (',address:')
+                           478 LOAD_FAST                4 (scratch)
+                           480 LOAD_ATTR               10 (full_address)
+                           490 FORMAT_VALUE             0
+                           492 BUILD_STRING             4
+               
+               926         494 PRECALL                  1
+                           498 CALL                     1
+                           508 GET_AWAITABLE            0
+                           510 LOAD_CONST               3 (None)
+                       >>  512 SEND                     3 (to 520)
+                           514 YIELD_VALUE
+                           516 RESUME                   3
+                           518 JUMP_BACKWARD_NO_INTERRUPT     4 (to 512)
+                       >>  520 POP_TOP
+               
+               931         522 LOAD_FAST                3 (autohide)
+               
+               930         524 POP_JUMP_FORWARD_IF_TRUE   108 (to 742)
+               
+               932         526 LOAD_FAST                5 (animated)
+               
+               930         528 POP_JUMP_FORWARD_IF_FALSE   108 (to 746)
+               
+               933         530 LOAD_FAST                1 (uid)
+                           532 LOAD_FAST                0 (self)
+                           534 LOAD_ATTR               11 (focused_window_tracking)
+                           544 CONTAINS_OP              0
+                           546 POP_JUMP_FORWARD_IF_FALSE   101 (to 750)
+               
+               934         548 LOAD_FAST                0 (self)
+                           550 LOAD_METHOD             12 (cast_bool)
+                           572 LOAD_FAST                4 (scratch)
+                           574 LOAD_ATTR               13 (conf)
+                           584 LOAD_METHOD              1 (get)
+                           606 LOAD_CONST              12 ('restore_focus')
+                           608 PRECALL                  1
+                           612 CALL                     1
+                           622 LOAD_CONST              13 (True)
+                           624 PRECALL                  2
+                           628 CALL                     2
+               
+               933         638 POP_JUMP_FORWARD_IF_FALSE    57 (to 754)
+               
+               936         640 LOAD_FAST                0 (self)
+                           642 LOAD_METHOD              9 (hyprctl)
+               
+               937         664 LOAD_CONST              14 ('focuswindow address:')
+                           666 LOAD_FAST                0 (self)
+                           668 LOAD_ATTR               11 (focused_window_tracking)
+                           678 LOAD_FAST                1 (uid)
+                           680 BINARY_SUBSCR
+                           690 FORMAT_VALUE             0
+                           692 BUILD_STRING             2
+               
+               936         694 PRECALL                  1
+                           698 CALL                     1
+                           708 GET_AWAITABLE            0
+                           710 LOAD_CONST               3 (None)
+                       >>  712 SEND                     3 (to 720)
+                           714 YIELD_VALUE
+                           716 RESUME                   3
+                           718 JUMP_BACKWARD_NO_INTERRUPT     4 (to 712)
+                       >>  720 POP_TOP
+               
+               939         722 LOAD_FAST                0 (self)
+                           724 LOAD_ATTR               11 (focused_window_tracking)
+                           734 LOAD_FAST                1 (uid)
+                           736 DELETE_SUBSCR
+                           738 LOAD_CONST               3 (None)
+                           740 RETURN_VALUE
+               
+               930     >>  742 LOAD_CONST               3 (None)
+                           744 RETURN_VALUE
+                       >>  746 LOAD_CONST               3 (None)
+                           748 RETURN_VALUE
+               
+               933     >>  750 LOAD_CONST               3 (None)
+                           752 RETURN_VALUE
+                       >>  754 LOAD_CONST               3 (None)
+                           756 RETURN_VALUE
                consts
                   '<name> hides scratchpad "name"\n        if `autohide` is True, skips focus tracking\n        `force` ignores the visibility check'
                   "Scratchpad '"
                   "' not found, check your configuration or the hide parameter"
                   None
                   '%s is not configured'
                   "' is not visible, will not hide."
                   '%s is already hidden'
                   False
                   'Hiding %s'
-                  'animation'
-                  ''
+                  'monitor_info'
                   'movetoworkspacesilent special:scratch_'
                   ',address:'
                   'restore_focus'
                   True
                   'focuswindow address:'
-               names      ('scratches', 'get', 'notify_error', 'log', 'warning', 'visible', 'info', 'conf', 'lower', '_anim_hide', 'hyprctl', 'full_address', 'focused_window_tracking', 'cast_bool')
-               varnames   ('self', 'uid', 'force', 'autohide', 'scratch', 'animation_type')
+               names      ('scratches', 'get', 'notify_error', 'log', 'warning', 'visible', 'info', '_hide_transition', 'meta', 'hyprctl', 'full_address', 'focused_window_tracking', 'cast_bool', 'conf')
+               varnames   ('self', 'uid', 'force', 'autohide', 'scratch', 'animated')
                freevars   ()
                cellvars   ()
                filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
                name       'run_hide'
-               firstlineno 899
+               firstlineno 906
                lnotab
-                  0x0604340204010c010aff1c033601040116013201360104010e0136015a
-                  0104013802180118ff1c0502ff020202fe020312015aff020318011eff1c
-                  0314f70803
+                  0x0604340204010c010aff1c033601040116013201360104010e0136014e
+                  02180118ff1c0502ff020202fe020312015aff020318011eff1c0314f708
+                  03
             ('return', None)
             (True,)
             (None,)
             (False, False)
-         names      ('__name__', '__module__', '__qualname__', 'procs', 'dict', 'str', 'asyncio', 'subprocess', 'Process', '__annotations__', 'ScratchDB', 'scratches', 'focused_window_tracking', 'workspace', 'monitor', 'Task', '__init__', 'exit', 'on_reload', '_configure_windowrules', 'bool', '_Extension__wait_for_client', '_start_scratch_classbased', '_start_scratch', 'ensure_alive', 'start_scratch_command', 'Scratch', 'updateScratchInfo', 'event_monitorremoved', 'event_configreloaded', 'event_activewindowv2', '_alternative_lookup', 'event_openwindow', 'run_toggle', 'get_offsets', '_anim_hide', '_slide_animation', 'run_show', '_show_transition', '_fix_size', '_fix_position', 'run_hide', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', 'procs', 'dict', 'str', 'asyncio', 'subprocess', 'Process', '__annotations__', 'ScratchDB', 'scratches', 'focused_window_tracking', 'workspace', 'monitor', 'Task', '__init__', 'exit', 'on_reload', '_configure_windowrules', 'bool', '_Extension__wait_for_client', '_start_scratch_classbased', '_start_scratch', 'ensure_alive', 'start_scratch_command', 'Scratch', 'updateScratchInfo', 'event_monitorremoved', 'event_configreloaded', 'event_activewindowv2', '_alternative_lookup', 'event_openwindow', 'run_toggle', 'get_offsets', '_hide_transition', '_slide_animation', 'run_show', '_show_transition', '_fix_size', '_fix_position', 'run_hide', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
          name       'Extension'
          firstlineno 367
          lnotab
-            0x0e01320114021e020401040224020a0908130820062c0e1e0c0e061b06
-            121011181508060606083406140812102408070608060e082c0633060f06
+            0x0e01320114021e020401040224020a0908130820062c0e1f0c0e061b06
+            12101118150806060608340614081210240807060d060e082c0634060f06
             0d
       'Extension'
    names      ('__doc__', 'os', 'time', 'logging', 'asyncio', 'typing', 'Any', 'cast', 'Callable', 'functools', 'partial', 'collections', 'defaultdict', 'aiofiles', 'aios', 'open', 'aiopen', 'ipc', 'notify_error', 'get_client_props', 'get_focused_monitor_props', 'interface', 'Plugin', 'common', 'state', 'CastBoolMixin', 'DEFAULT_MARGIN', 'AFTER_SHOW_INHIBITION', 'DEFAULT_HYSTERESIS', 'invert_dimension', 'get_space_identifier', 'convert_coords', 'Animations', 'OverridableConfig', 'Scratch', 'ScratchDB', 'Extension')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/fab/dev/std/pyprland/pyprland/plugins/scratchpads.py'
```

### Comparing `pyprland-2.1.1/pyprland/plugins/__pycache__/shift_monitors.cpython-311.pyc` & `pyprland-2.1.4/pyprland/plugins/__pycache__/shift_monitors.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/__pycache__/shortcuts_menu.cpython-311.pyc` & `pyprland-2.1.4/pyprland/plugins/__pycache__/shortcuts_menu.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/__pycache__/system_notifier.cpython-311.pyc` & `pyprland-2.1.4/pyprland/plugins/__pycache__/system_notifier.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/__pycache__/toggle_dpms.cpython-311.pyc` & `pyprland-2.1.4/pyprland/plugins/__pycache__/toggle_dpms.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/__pycache__/toggle_special.cpython-311.pyc` & `pyprland-2.1.4/pyprland/plugins/__pycache__/toggle_special.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/__pycache__/workspaces_follow_focus.cpython-311.pyc` & `pyprland-2.1.4/pyprland/plugins/__pycache__/workspaces_follow_focus.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/expose.py` & `pyprland-2.1.4/pyprland/plugins/expose.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/expose.py,cover` & `pyprland-2.1.4/pyprland/plugins/expose.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/fetch_client_menu.py` & `pyprland-2.1.4/pyprland/plugins/fetch_client_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/fetch_client_menu.py,cover` & `pyprland-2.1.4/pyprland/plugins/fetch_client_menu.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/interface.py` & `pyprland-2.1.4/pyprland/plugins/interface.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/interface.py,cover` & `pyprland-2.1.4/pyprland/plugins/interface.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/layout_center.py` & `pyprland-2.1.4/pyprland/plugins/layout_center.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/layout_center.py,cover` & `pyprland-2.1.4/pyprland/plugins/layout_center.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/lost_windows.py` & `pyprland-2.1.4/pyprland/plugins/lost_windows.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/lost_windows.py,cover` & `pyprland-2.1.4/pyprland/plugins/lost_windows.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/magnify.py,cover` & `pyprland-2.1.4/pyprland/plugins/magnify.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/monitors.py` & `pyprland-2.1.4/pyprland/plugins/monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/monitors.py,cover` & `pyprland-2.1.4/pyprland/plugins/monitors.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/monitors.py.orig` & `pyprland-2.1.4/pyprland/plugins/monitors.py.orig`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/monitors_v0.py` & `pyprland-2.1.4/pyprland/plugins/monitors_v0.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/pyprland.py` & `pyprland-2.1.4/pyprland/plugins/pyprland.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/pyprland.py,cover` & `pyprland-2.1.4/pyprland/plugins/pyprland.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/scratchpads.py` & `pyprland-2.1.4/pyprland/plugins/scratchpads.py`

 * *Files 2% similar despite different names*

```diff
@@ -480,16 +480,17 @@
             await self.hyprctl(ipc_commands, "keyword")
 
     async def __wait_for_client(self, item, use_proc=True) -> bool:
         """Waits for a client to be up and running
         if `class_match` is enabled, will use the class, else the process's PID will be used.
         """
         self.log.info("==> Wait for %s spawning", item.uid)
-        for loop_count in range(1, 8):
-            await asyncio.sleep(loop_count**2 / 10.0)
+        interval_range = [0.1] * 10 + [0.2] * 20 + [0.5] * 15
+        for interval in interval_range:
+            await asyncio.sleep(interval)
             is_alive = await item.isAlive()
 
             # skips the checks if the process isn't started (just wait)
             if is_alive or not use_proc:
                 if self.cast_bool(item.conf.get("class_match")):
                     info = await self.get_client_props(cls=item.conf.get("class"))
                 else:
@@ -747,21 +748,26 @@
     async def get_offsets(self, scratch, monitor=None):
         "Return offset from config or compute one"
         offset = scratch.conf.get("offset")
         if offset:
             return offset, offset
         return await scratch.get_auto_offset(monitor)
 
-    async def _anim_hide(self, animation_type, scratch):
+    async def _hide_transition(self, scratch, monitor):
         "animate hiding a scratchpad"
 
+        animation_type: str = scratch.conf.get("animation", "").lower()
+        if not animation_type:
+            return False
+
         await self.updateScratchInfo(scratch)
 
-        off_x, off_y = await self.get_offsets(scratch)
+        off_x, off_y = await self.get_offsets(scratch, monitor)
         await self._slide_animation(animation_type, scratch, off_x, off_y)
+        return True
 
     async def _slide_animation(self, animation_type, scratch, off_x, off_y):
         "Slides the window `offset` pixels respecting `animation_type`"
         addr = "address:" + scratch.full_address
         if animation_type == "fromtop":
             await self.hyprctl(f"movewindowpixel 0 {-off_y},{addr}")
         elif animation_type == "frombottom":
@@ -863,14 +869,15 @@
                 self.log.warning(
                     "No position and no animation provided for %s, don't know where to place it.",
                     item.uid,
                 )
 
         await self.hyprctl(f"focuswindow address:{item.full_address}")
         item.meta["last_shown"] = time.time()
+        item.meta["monitor_info"] = monitor
 
     async def _fix_size(self, item, monitor):
         "apply the `size` config parameter"
 
         size = item.conf.get("size")
         if size:
             width, height = convert_coords(self.log, size, monitor)
@@ -910,25 +917,23 @@
             return
         if not scratch.visible and not force and not autohide:
             await notify_error(f"Scratchpad '{uid}' is not visible, will not hide.")
             self.log.warning("%s is already hidden", uid)
             return
         scratch.visible = False
         self.log.info("Hiding %s", uid)
-        animation_type: str = scratch.conf.get("animation", "").lower()
-        if animation_type:
-            await self._anim_hide(animation_type, scratch)
+        animated = await self._hide_transition(scratch, scratch.meta["monitor_info"])
 
         await self.hyprctl(
             f"movetoworkspacesilent special:scratch_{uid},address:{scratch.full_address}"
         )
 
         if (
             not autohide
-            and animation_type
+            and animated
             and uid in self.focused_window_tracking
             and self.cast_bool(scratch.conf.get("restore_focus"), True)
         ):  # focus got lost when animating
             await self.hyprctl(
                 f"focuswindow address:{self.focused_window_tracking[uid]}"
             )
             del self.focused_window_tracking[uid]
```

### Comparing `pyprland-2.1.1/pyprland/plugins/scratchpads.py,cover` & `pyprland-2.1.4/pyprland/plugins/scratchpads.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/shift_monitors.py` & `pyprland-2.1.4/pyprland/plugins/shift_monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/shift_monitors.py,cover` & `pyprland-2.1.4/pyprland/plugins/shift_monitors.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/shortcuts_menu.py` & `pyprland-2.1.4/pyprland/plugins/shortcuts_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/shortcuts_menu.py,cover` & `pyprland-2.1.4/pyprland/plugins/shortcuts_menu.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/system_notifier.py` & `pyprland-2.1.4/pyprland/plugins/system_notifier.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/toggle_dpms.py` & `pyprland-2.1.4/pyprland/plugins/toggle_dpms.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/toggle_dpms.py,cover` & `pyprland-2.1.4/pyprland/plugins/toggle_dpms.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/toggle_special.py` & `pyprland-2.1.4/pyprland/plugins/toggle_special.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/toggle_special.py,cover` & `pyprland-2.1.4/pyprland/plugins/toggle_special.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/workspaces_follow_focus.py` & `pyprland-2.1.4/pyprland/plugins/workspaces_follow_focus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyprland/plugins/workspaces_follow_focus.py,cover` & `pyprland-2.1.4/pyprland/plugins/workspaces_follow_focus.py,cover`

 * *Files identical despite different names*

### Comparing `pyprland-2.1.1/pyproject.toml` & `pyprland-2.1.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyprland"
-version = "2.1.1"
+version = "2.1.4"
 description = "Hyperland plugin system - batteries included"
 authors = ["fdev31 <fdev31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pyprland"}]
 homepage = "https://github.com/hyprland-community/pyprland/"
```

### Comparing `pyprland-2.1.1/PKG-INFO` & `pyprland-2.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprland
-Version: 2.1.1
+Version: 2.1.4
 Summary: Hyperland plugin system - batteries included
 Home-page: https://github.com/hyprland-community/pyprland/
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -53,15 +53,15 @@
 ## Latest major changes
 
 Check the [Releases change log](https://github.com/hyprland-community/pyprland/releases) for more information
 
 
 ### 2.1
 
-- Requires Hyprland 0.37 or better
+- Requires Hyprland >= 0.37
 - [monitors](https://github.com/hyprland-community/pyprland/wiki//monitors)
   - Drops the `wlr-randr` dependency
   - simplified the syntax, no need for `()` around a screen name (will try matching the exact name first, then partial description)
 
 ### 2.0
 
 - New dependency: [aiofiles](https://pypi.org/project/aiofiles/)
@@ -113,7 +113,8 @@
   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline&theme=dark" />
     <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline" />
     <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=fdev31/pyprland&type=Timeline" />
   </picture>
 </a>
 
+
```

