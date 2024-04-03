# Comparing `tmp/discover-overlay-0.7.2.tar.gz` & `tmp/discover-overlay-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discover-overlay-0.7.2.tar", last modified: Wed Apr  3 18:39:47 2024, max compression
+gzip compressed data, was "discover-overlay-0.7.3.tar", last modified: Wed Apr  3 21:45:23 2024, max compression
```

## Comparing `discover-overlay-0.7.2.tar` & `discover-overlay-0.7.3.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover-overlay-default.png
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover-overlay-default.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover-overlay-tray.png
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover-overlay-tray.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover-overlay.png
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover-overlay.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/autostart.py
--rw-r--r--   0 runner    (1001) docker     (127)    29544 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/discord_connector.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22717 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/discover_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/draggable_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/draggable_window_wayland.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay/glade/
--rw-r--r--   0 runner    (1001) docker     (127)   135215 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/glade/settings.glade
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/image_getter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.011847 discover-overlay-0.7.2/discover_overlay/locales/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.007847 discover-overlay-0.7.2/discover_overlay/locales/cy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay/locales/cy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/locales/cy/LC_MESSAGES/default.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.011847 discover-overlay-0.7.2/discover_overlay/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/locales/de/LC_MESSAGES/default.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.011847 discover-overlay-0.7.2/discover_overlay/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/locales/en/LC_MESSAGES/default.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.011847 discover-overlay-0.7.2/discover_overlay/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     9407 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/locales/fr/LC_MESSAGES/default.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.011847 discover-overlay-0.7.2/discover_overlay/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/locales/tr/LC_MESSAGES/default.mo
--rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/notification_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    16056 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    48895 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/settings_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/text_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    41720 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/voice_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay.desktop
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-03 18:39:46.000000 discover-overlay-0.7.2/discover_overlay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-03 18:39:46.000000 discover-overlay-0.7.2/discover_overlay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:39:46.000000 discover-overlay-0.7.2/discover_overlay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 18:39:46.000000 discover-overlay-0.7.2/discover_overlay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 18:39:46.000000 discover-overlay-0.7.2/discover_overlay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 18:39:46.000000 discover-overlay-0.7.2/discover_overlay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay_configure.desktop
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.012823 discover-overlay-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-04-03 21:45:23.012823 discover-overlay-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover-overlay-default.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover-overlay-default.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover-overlay-tray.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover-overlay-tray.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover-overlay.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover-overlay.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.008823 discover-overlay-0.7.3/discover_overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/audio_assist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/autostart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30399 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/discord_connector.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23229 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/discover_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/draggable_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/draggable_window_wayland.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.008823 discover-overlay-0.7.3/discover_overlay/glade/
+-rw-r--r--   0 runner    (1001) docker     (127)   128883 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/glade/settings.glade
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/image_getter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.004823 discover-overlay-0.7.3/discover_overlay/locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.004823 discover-overlay-0.7.3/discover_overlay/locales/cy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.008823 discover-overlay-0.7.3/discover_overlay/locales/cy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/locales/cy/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.004823 discover-overlay-0.7.3/discover_overlay/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.008823 discover-overlay-0.7.3/discover_overlay/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/locales/de/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.004823 discover-overlay-0.7.3/discover_overlay/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.008823 discover-overlay-0.7.3/discover_overlay/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/locales/en/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.004823 discover-overlay-0.7.3/discover_overlay/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.012823 discover-overlay-0.7.3/discover_overlay/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/locales/fr/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.004823 discover-overlay-0.7.3/discover_overlay/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.012823 discover-overlay-0.7.3/discover_overlay/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/locales/tr/LC_MESSAGES/default.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    19938 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/notification_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16667 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55041 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/settings_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13788 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/text_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43733 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay/voice_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay.desktop
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:45:23.012823 discover-overlay-0.7.3/discover_overlay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-04-03 21:45:22.000000 discover-overlay-0.7.3/discover_overlay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-03 21:45:22.000000 discover-overlay-0.7.3/discover_overlay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:45:22.000000 discover-overlay-0.7.3/discover_overlay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 21:45:22.000000 discover-overlay-0.7.3/discover_overlay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 21:45:22.000000 discover-overlay-0.7.3/discover_overlay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 21:45:22.000000 discover-overlay-0.7.3/discover_overlay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/discover_overlay_configure.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:45:23.012823 discover-overlay-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-03 21:45:14.000000 discover-overlay-0.7.3/setup.py
```

### Comparing `discover-overlay-0.7.2/LICENSE` & `discover-overlay-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.2/PKG-INFO` & `discover-overlay-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discover-overlay
-Version: 0.7.2
+Version: 0.7.3
 Summary: Voice chat overlay
 Home-page: https://github.com/trigg/Discover
 Author: trigg
 Author-email: 
 License: GPLv3+
 Keywords: discord overlay voice linux
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,15 @@
 Requires-Dist: PyGObject>=3.22
 Requires-Dist: websocket-client
 Requires-Dist: pyxdg
 Requires-Dist: requests
 Requires-Dist: pillow
 Requires-Dist: python-xlib
 Requires-Dist: setuptools
+Requires-Dist: pulsectl-asyncio
 
 # Discover
 Yet another Discord overlay for Linux written in Python using GTK3.
 
 Discover-Overlay is a GTK3 overlay written in Python3. It can be configured to show who is currently talking on discord or it can be set to display text and images from a preconfigured channel. It is fully customisable and can be configured to display anywhere on the screen. We fully support X11 and wlroots based environments. We felt the need to make this project due to the shortcomings in support on Linux by the official discord client.
 
 Considerably lighter on system resources and less hack-and-slash included than discord-overlay.
```

### Comparing `discover-overlay-0.7.2/README.md` & `discover-overlay-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.2/discover-overlay-default.png` & `discover-overlay-0.7.3/discover-overlay-default.png`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.2/discover-overlay-default.svg` & `discover-overlay-0.7.3/discover-overlay-default.svg`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.2/discover-overlay-tray.png` & `discover-overlay-0.7.3/discover-overlay-tray.png`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.2/discover-overlay-tray.svg` & `discover-overlay-0.7.3/discover-overlay-tray.svg`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.2/discover-overlay.png` & `discover-overlay-0.7.3/discover-overlay.png`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.2/discover-overlay.svg` & `discover-overlay-0.7.3/discover-overlay.svg`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.2/discover_overlay/__init__.py` & `discover-overlay-0.7.3/discover_overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.2/discover_overlay/__main__.py` & `discover-overlay-0.7.3/discover_overlay/__main__.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.2/discover_overlay/autostart.py` & `discover-overlay-0.7.3/discover_overlay/autostart.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,18 +93,18 @@
             self.change_file("0")
         self.auto = enable
 
     def change_file(self, value):
         root = ''
         if shutil.which('pkexec'):
             root = 'pkexec'
-        else: 
+        else:
             log.error("No ability to request root privs. Cancel")
             return
-        command = " sed -i 's/AUTO_LAUNCH_DISCOVER_OVERLAY=./AUTO_LAUNCH_DISCOVER_OVERLAY=%s/g' /etc/default/discover-overlay" % (value)
+        command = " sed -i 's/AUTO_LAUNCH_DISCOVER_OVERLAY=./AUTO_LAUNCH_DISCOVER_OVERLAY=%s/g' /etc/default/discover-overlay" % (
+            value)
         command_with_permissions = root + command
         os.system(command_with_permissions)
 
-
     def is_auto(self):
         """Check if it's already set to auto-start"""
         return self.auto
```

### Comparing `discover-overlay-0.7.2/discover_overlay/discord_connector.py` & `discover-overlay-0.7.3/discover_overlay/discord_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,14 +343,27 @@
                 if self.current_text == j["data"]["channel_id"]:
                     self.delete_text(j["data"]["message"])
             elif j["evt"] == "CHANNEL_CREATE":
                 # We haven't been told what guild this is in
                 self.req_channel_details(j["data"]["id"], 'new')
             elif j["evt"] == "NOTIFICATION_CREATE":
                 self.discover.notification_overlay.add_notification_message(j)
+            elif j["evt"] == "VOICE_SETTINGS_UPDATE":
+                source = j['data']['input']['device_id']
+                sink = j['data']['output']['device_id']
+                if sink == 'default':
+                    for available_sink in j['data']['output']['available_devices']:
+                        if available_sink['id'] == 'default':
+                            sink = available_sink['name'][9:]
+                if source == 'default':
+                    for available_source in j['data']['input']['available_devices']:
+                        if available_source['id'] == 'default':
+                            source = available_source['name'][9:]
+                self.discover.audio_assist.set_devices(sink, source)
+
             else:
                 log.warning(j)
             return
         elif j["cmd"] == "AUTHENTICATE":
             if j["evt"] == "ERROR":
                 self.access_token = None
                 self.get_access_token_stage1()
@@ -585,14 +598,15 @@
         Subscribe to helpful events that report connectivity issues &
         when the user has intentionally changed channel
 
         Unfortunatly no event has been found to alert to being forcibly moved
         or that reports the users current location
         """
         self.sub_raw("VOICE_CHANNEL_SELECT", {}, "VOICE_CHANNEL_SELECT")
+        self.sub_raw("VOICE_SETTINGS_UPDATE", {}, "VOICE_SETTINGS_UPDATE")
         self.sub_raw("VOICE_CONNECTION_STATUS", {}, "VOICE_CONNECTION_STATUS")
         self.sub_raw("GUILD_CREATE", {}, "GUILD_CREATE")
         self.sub_raw("CHANNEL_CREATE", {}, "CHANNEL_CREATE")
         self.sub_raw("NOTIFICATION_CREATE", {}, "NOTIFICATION_CREATE")
 
     def sub_channel(self, event, channel):
         """
@@ -658,23 +672,25 @@
         cmd = {
             "cmd": "SET_VOICE_SETTINGS",
             "args": {"mute": muted},
             "nonce": "deadbeef"
         }
         if self.websocket:
             self.websocket.send(json.dumps(cmd))
+        return False
 
     def set_deaf(self, deaf):
         cmd = {
             "cmd": "SET_VOICE_SETTINGS",
             "args": {"deaf": deaf},
             "nonce": "deadbeef"
         }
         if self.websocket:
             self.websocket.send(json.dumps(cmd))
+        return False
 
     def change_voice_room(self, id):
         """
         Switch to another voice room
         """
         cmd = {
             "cmd": "SELECT_VOICE_CHANNEL",
```

### Comparing `discover-overlay-0.7.2/discover_overlay/discover_overlay.py` & `discover-overlay-0.7.3/discover_overlay/discover_overlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,24 @@
 import time
 import sys
 import re
 import traceback
 import logging
 import pkg_resources
 import json
+import signal
 import gi
 from configparser import ConfigParser
 
 from .settings_window import MainSettingsWindow
 from .voice_overlay import VoiceOverlayWindow
 from .text_overlay import TextOverlayWindow
 from .notification_overlay import NotificationOverlayWindow
 from .discord_connector import DiscordConnector
+from .audio_assist import DiscoverAudioAssist
 
 gi.require_version("Gtk", "3.0")
 # pylint: disable=wrong-import-position,wrong-import-order
 from gi.repository import Gtk, GLib, Gio, Gdk  # nopep8
 
 try:
     from xdg.BaseDirectory import xdg_config_home
@@ -74,14 +76,15 @@
                     "gtk-application-prefer-dark-theme", Gtk.true)
 
         self.create_gui()
 
         self.connection = DiscordConnector(self)
 
         self.connection.connect()
+        self.audio_assist = DiscoverAudioAssist(self)
 
         rpc_file = Gio.File.new_for_path(rpc_file)
         monitor = rpc_file.monitor_file(0, None)
         monitor.connect("changed", self.rpc_changed)
 
         config_file = Gio.File.new_for_path(config_file)
         monitor_config = config_file.monitor_file(0, None)
@@ -244,15 +247,15 @@
         floating_h = config.getint("main", "floating_h", fallback=400)
         self.voice_overlay.set_order(
             config.getint("main", "order", fallback=0))
         self.voice_overlay.set_hide_on_mouseover(
             config.getboolean("main", "autohide", fallback=False))
         self.voice_overlay.set_mouseover_timer(
             config.getint("main", "autohide_timer", fallback=1))
-    
+
         self.voice_overlay.set_horizontal(config.getboolean(
             "main", "horizontal", fallback=False))
         self.voice_overlay.set_guild_ids(self.parse_guild_ids(
             config.get("main", "guild_ids", fallback="")))
         self.voice_overlay.set_overflow(
             config.getint("main", "overflow", fallback=0))
         self.voice_overlay.set_show_connection(config.getboolean(
@@ -403,14 +406,16 @@
             config.getboolean("general", "xshape", fallback=False))
 
         hidden = config.getboolean("general", "hideoverlay", fallback=False)
         self.voice_overlay.set_hidden(hidden)
         self.text_overlay.set_hidden(hidden)
         self.notification_overlay.set_hidden(hidden)
 
+        self.audio_assist.set_enabled(config.getboolean(
+            "general", "audio_assist", fallback=False))
 
     def parse_guild_ids(self, guild_ids_str):
         """Parse the guild_ids from a str and return them in a list"""
         guild_ids = []
         for guild_id in guild_ids_str.split(","):
             guild_id = guild_id.strip()
             if guild_id != "":
@@ -464,28 +469,37 @@
         if self.voice_overlay:
             self.voice_overlay.set_task(visible)
         if self.text_overlay:
             self.text_overlay.set_task(visible)
         if self.notification_overlay:
             self.notification_overlay.set_task(visible)
 
+    def set_mute_async(self, mute):
+        if mute != None:
+            GLib.idle_add(self.connection.set_mute, mute)
+
+    def set_deaf_async(self, deaf):
+        if deaf != None:
+            GLib.idle_add(self.connection.set_deaf, deaf)
+
 
 def entrypoint():
     """
     Entry Point.
 
     Find all needed file locations and read args
 
     if '--rpc' simply pass them over the rpc file
 
     if '-c' or '--configure' start the config window only
 
     otherwise start overlay
     """
 
+    signal.signal(signal.SIGINT, signal.SIG_DFL)
     # Find Config directory
     config_dir = os.path.join(xdg_config_home, "discover_overlay")
     os.makedirs(config_dir, exist_ok=True)
 
     # Find RPC, Channel info, config and debug files
     rpc_file = os.path.join(config_dir, "discover_overlay.rpc")
     channel_file = os.path.join(config_dir, "channels.rpc")
```

### Comparing `discover-overlay-0.7.2/discover_overlay/draggable_window.py` & `discover-overlay-0.7.3/discover_overlay/draggable_window.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.2/discover_overlay/draggable_window_wayland.py` & `discover-overlay-0.7.3/discover_overlay/draggable_window_wayland.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.2/discover_overlay/glade/settings.glade` & `discover-overlay-0.7.3/discover_overlay/glade/settings.glade`

 * *Files 1% similar despite different names*

#### Comparing `discover-overlay-0.7.2/discover_overlay/glade/settings.glade` & `discover-overlay-0.7.3/discover_overlay/glade/settings.glade`

```diff
@@ -285,1415 +285,508 @@
             <property name="label" translatable="yes">Overview</property>
           </object>
           <packing>
             <property name="tab-fill">False</property>
           </packing>
         </child>
         <child>
-          <!-- n-columns=3 n-rows=2 -->
+          <!-- n-columns=8 n-rows=7 -->
           <object class="GtkGrid">
             <property name="name">voice_grid</property>
             <property name="visible">True</property>
             <property name="can-focus">False</property>
             <property name="halign">baseline</property>
             <property name="valign">baseline</property>
             <property name="margin-start">5</property>
             <property name="margin-end">5</property>
             <property name="margin-top">5</property>
             <property name="margin-bottom">5</property>
-            <property name="row-spacing">1</property>
-            <property name="column-spacing">1</property>
-            <property name="column-homogeneous">True</property>
+            <property name="row-spacing">3</property>
+            <property name="column-spacing">3</property>
             <child>
-              <!-- n-columns=1 n-rows=8 -->
-              <object class="GtkGrid">
-                <property name="name">voice_location_grid</property>
-                <property name="visible">True</property>
-                <property name="can-focus">False</property>
-                <property name="halign">center</property>
-                <property name="margin-bottom">40</property>
-                <property name="row-spacing">1</property>
-                <property name="column-spacing">1</property>
-                <property name="row-homogeneous">True</property>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_overlay_location_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Overlay Location</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">0</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkComboBoxText" id="voice_align_2">
-                    <property name="name">voice_align_2</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="active">0</property>
-                    <items>
-                      <item translatable="yes">Top</item>
-                      <item translatable="yes">Middle</item>
-                      <item translatable="yes">Bottom</item>
-                    </items>
-                    <signal name="changed" handler="voice_align_2_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">4</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkComboBoxText" id="voice_align_1">
-                    <property name="name">voice_align_1</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="active">0</property>
-                    <items>
-                      <item translatable="yes">Left</item>
-                      <item translatable="yes">Right</item>
-                    </items>
-                    <signal name="changed" handler="voice_align_1_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">3</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkComboBoxText" id="voice_monitor">
-                    <property name="name">voice_monitor</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <signal name="changed" handler="voice_monitor_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">2</property>
-                  </packing>
-                </child>
-                <child>
-                  <!-- n-columns=2 n-rows=1 -->
-                  <object class="GtkGrid">
-                    <property name="name">voice_location_grid_anchor</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <child>
-                      <object class="GtkRadioButton" id="anchortoedge">
-                        <property name="label" translatable="yes">Anchor To Edge</property>
-                        <property name="name">voice_anchor_to_edge_button</property>
-                        <property name="visible">True</property>
-                        <property name="can-focus">True</property>
-                        <property name="receives-default">False</property>
-                        <property name="active">True</property>
-                        <property name="draw-indicator">True</property>
-                        <signal name="toggled" handler="voice_anchor_to_edge_changed" swapped="no"/>
-                      </object>
-                      <packing>
-                        <property name="left-attach">0</property>
-                        <property name="top-attach">0</property>
-                      </packing>
-                    </child>
-                    <child>
-                      <object class="GtkRadioButton" id="anchorfloating">
-                        <property name="label" translatable="yes">Floating</property>
-                        <property name="name">voice_floating_button</property>
-                        <property name="visible">True</property>
-                        <property name="can-focus">True</property>
-                        <property name="receives-default">False</property>
-                        <property name="active">True</property>
-                        <property name="draw-indicator">True</property>
-                        <property name="group">anchortoedge</property>
-                        <signal name="toggled" handler="voice_floating_changed" swapped="no"/>
-                      </object>
-                      <packing>
-                        <property name="left-attach">1</property>
-                        <property name="top-attach">0</property>
-                      </packing>
-                    </child>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">1</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkButton" id="voice_show_advanced_options_button">
-                    <property name="label" translatable="yes">Show Advanced Options</property>
-                    <property name="name">voice_show_advanced_options_button</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <signal name="pressed" handler="voice_show_advanced_options_button_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">7</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkButton" id="voice_place_window_button">
-                    <property name="label" translatable="yes">Place Window</property>
-                    <property name="name">voice_place_window_button</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <signal name="pressed" handler="voice_place_window" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">6</property>
-                  </packing>
-                </child>
-                <child>
-                  <!-- n-columns=2 n-rows=1 -->
-                  <object class="GtkGrid">
-                    <property name="name">voice_location_grid_horizontal</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <child>
-                      <object class="GtkCheckButton">
-                        <property name="name">voice_display_horizontally</property>
-                        <property name="visible">True</property>
-                        <property name="can-focus">True</property>
-                        <property name="receives-default">False</property>
-                        <property name="draw-indicator">True</property>
-                        <signal name="toggled" handler="voice_display_horizontally_changed" swapped="no"/>
-                      </object>
-                      <packing>
-                        <property name="left-attach">1</property>
-                        <property name="top-attach">0</property>
-                      </packing>
-                    </child>
-                    <child>
-                      <object class="GtkLabel">
-                        <property name="name">voice_display_horizontally_label</property>
-                        <property name="visible">True</property>
-                        <property name="can-focus">False</property>
-                        <property name="margin-end">28</property>
-                        <property name="label" translatable="yes">Display Horizontally</property>
-                        <property name="xalign">0</property>
-                      </object>
-                      <packing>
-                        <property name="left-attach">0</property>
-                        <property name="top-attach">0</property>
-                      </packing>
-                    </child>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">5</property>
-                  </packing>
-                </child>
+              <object class="GtkLabel">
+                <property name="name">voice_display_horizontally_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="margin-right">28</property>
+                <property name="margin-end">28</property>
+                <property name="label" translatable="yes">Display Horizontally</property>
+                <property name="xalign">0</property>
               </object>
               <packing>
                 <property name="left-attach">0</property>
-                <property name="top-attach">0</property>
+                <property name="top-attach">5</property>
               </packing>
             </child>
             <child>
-              <!-- n-columns=4 n-rows=5 -->
-              <object class="GtkGrid">
-                <property name="name">voice_colour_grid</property>
-                <property name="visible">True</property>
-                <property name="can-focus">False</property>
-                <property name="halign">center</property>
-                <property name="margin-bottom">40</property>
-                <property name="row-spacing">1</property>
-                <property name="column-spacing">1</property>
-                <property name="row-homogeneous">True</property>
-                <property name="column-homogeneous">True</property>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_foreground_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="margin-start">4</property>
-                    <property name="margin-end">4</property>
-                    <property name="label" translatable="yes">Foreground</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">0</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_background_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="margin-start">4</property>
-                    <property name="margin-end">4</property>
-                    <property name="label" translatable="yes">Background</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">0</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_border_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="margin-start">4</property>
-                    <property name="margin-end">4</property>
-                    <property name="label" translatable="yes">Border</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">0</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_talking_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Talking</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">1</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_idle_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Idle</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">2</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_mute_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Mute</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">3</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_avatar_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Avatar</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">4</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkColorButton">
-                    <property name="name">voice_talking_foreground</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <property name="use-alpha">True</property>
-                    <signal name="color-set" handler="voice_talking_foreground_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">1</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkColorButton">
-                    <property name="name">voice_talking_background</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <property name="use-alpha">True</property>
-                    <signal name="color-set" handler="voice_talking_background_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">1</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkColorButton">
-                    <property name="name">voice_talking_border</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <property name="use-alpha">True</property>
-                    <signal name="color-set" handler="voice_talking_border_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">1</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkColorButton">
-                    <property name="name">voice_idle_foreground</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <property name="use-alpha">True</property>
-                    <signal name="color-set" handler="voice_idle_foreground_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">2</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkColorButton">
-                    <property name="name">voice_idle_background</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <property name="use-alpha">True</property>
-                    <signal name="color-set" handler="voice_idle_background_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">2</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkColorButton">
-                    <property name="name">voice_idle_border</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <property name="use-alpha">True</property>
-                    <signal name="color-set" handler="voice_idle_border_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">2</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkColorButton">
-                    <property name="name">voice_mute_foreground</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <property name="use-alpha">True</property>
-                    <signal name="color-set" handler="voice_mute_foreground_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">3</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkColorButton">
-                    <property name="name">voice_mute_background</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <property name="use-alpha">True</property>
-                    <signal name="color-set" handler="voice_mute_background_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">3</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkColorButton">
-                    <property name="name">voice_avatar_background</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <property name="use-alpha">True</property>
-                    <signal name="color-set" handler="voice_avatar_background_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">4</property>
-                  </packing>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
+              <object class="GtkCheckButton">
+                <property name="name">voice_display_horizontally</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">False</property>
+                <property name="draw-indicator">True</property>
+                <signal name="toggled" handler="voice_display_horizontally_changed" swapped="no"/>
               </object>
               <packing>
                 <property name="left-attach">1</property>
-                <property name="top-attach">0</property>
+                <property name="top-attach">5</property>
               </packing>
             </child>
             <child>
-              <!-- n-columns=6 n-rows=13 -->
-              <object class="GtkGrid">
-                <property name="name">voice_advanced_grid</property>
-                <property name="visible">True</property>
-                <property name="can-focus">False</property>
-                <property name="row-spacing">1</property>
-                <property name="column-spacing">5</property>
-                <property name="column-homogeneous">True</property>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_display_icon_only_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Show Names</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">0</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_display_icon_only</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_display_icon_only_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">0</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_font_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Font</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">1</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkFontButton">
-                    <property name="name">voice_font</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <property name="font">Sans 12</property>
-                    <property name="language">en-us</property>
-                    <property name="preview-text"/>
-                    <signal name="font-set" handler="voice_font_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">1</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_text_padding_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Text Padding</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">2</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_text_padding</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="text">0</property>
-                    <property name="adjustment">text_padding_adj</property>
-                    <signal name="value-changed" handler="voice_text_padding_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">2</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_text_vertical_offset_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Text Vertical Offset</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">3</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_text_vertical_offset</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="text">0</property>
-                    <property name="adjustment">voice_text_offset</property>
-                    <signal name="value-changed" handler="voice_text_vertical_offset_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">3</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_show_title_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Show Title</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">0</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_show_title</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_show_title_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">0</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_show_connection_status_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Show Connection Status</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">2</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_show_connection_status</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_show_connection_status_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">2</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkFontButton">
-                    <property name="name">voice_title_font</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <property name="font">Sans 12</property>
-                    <property name="language">en-us</property>
-                    <property name="preview-text"/>
-                    <signal name="font-set" handler="voice_title_font_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">1</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_title_font_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Title Font</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">1</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_vertical_padding</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="text">0</property>
-                    <property name="adjustment">voice_vertical_padding_adj</property>
-                    <signal name="value-changed" handler="voice_vertical_padding_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">4</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_horizontal_padding_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Horizontal Edge Padding</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">5</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_horizontal_padding</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="text">0</property>
-                    <property name="adjustment">voice_horizontal_padding_adj</property>
-                    <signal name="value-changed" handler="voice_horizontal_padding_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">5</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_show_test_content_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Show Test Content</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">7</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_show_test_content</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_toggle_test_content" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">7</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_dummy_count_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Test Data Count</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">8</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_dummy_count</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="text">50</property>
-                    <property name="adjustment">voice_dummy_count_adj</property>
-                    <property name="value">50</property>
-                    <signal name="value-changed" handler="voice_dummy_count_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">8</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_show_disconnected_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Show While Disconnected</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">9</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_show_disconnected</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_show_disconnected_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">9</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voce_vertical_padding_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Verticle Edge Padding</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">4</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_nick_length_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Limit text length</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">4</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_nick_length</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="text">32</property>
-                    <property name="adjustment">voice_nick_lenght_adj</property>
-                    <property name="value">32</property>
-                    <signal name="value-changed" handler="voice_nick_length_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">4</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_avatar_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Show Avatar</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">5</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_show_avatar</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_show_avatar_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">5</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_square_avatar_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Square Avatar</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">6</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_square_avatar</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_square_avatar_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">6</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_fancy_avatar_shapes_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Fancy Avatar Shapes</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">7</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_fancy_avatar_shapes</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_fancy_avatar_shapes_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">7</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_avatar_size_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Avatar Size</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">8</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_avatar_size</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="text">48</property>
-                    <property name="adjustment">avatar_size_adj</property>
-                    <property name="value">48</property>
-                    <signal name="value-changed" handler="voice_avatar_size_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">8</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_avatar_opacity_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Avatar Opacity</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">2</property>
-                    <property name="top-attach">9</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkScale">
-                    <property name="name">voice_avatar_opacity</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="adjustment">ava_opacity_adj</property>
-                    <property name="round-digits">1</property>
-                    <signal name="value-changed" handler="voice_avatar_opacity_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">3</property>
-                    <property name="top-attach">9</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_display_speakers_only_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Display Speakers Only</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">4</property>
-                    <property name="top-attach">0</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_display_speakers_only</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_display_speakers_only" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">0</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_display_speakers_grace_period_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Speakers Grace Period</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">4</property>
-                    <property name="top-attach">1</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_display_speakers_grace_period</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="text">0</property>
-                    <property name="adjustment">voice_display_speakers_grace_period_adj</property>
-                    <signal name="value-changed" handler="voice_display_speakers_grace_period" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">1</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_overflow_style_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Overflow Style</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">4</property>
-                    <property name="top-attach">2</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkComboBoxText" id="voice_overflow_style">
-                    <property name="name">voice_overflow_style</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <items>
-                      <item translatable="yes">None</item>
-                      <item translatable="yes">Wrap</item>
-                      <item translatable="yes">Shrink</item>
-                    </items>
-                    <signal name="changed" handler="voice_overflow_style_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">2</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_order_avatars_by_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Order Users By</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">4</property>
-                    <property name="top-attach">3</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkComboBoxText" id="voice_order_avatars_by">
-                    <property name="name">voice_order_avatars_by</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <items>
-                      <item translatable="yes">Alphabetically</item>
-                      <item translatable="yes">ID</item>
-                      <item translatable="yes">Last Spoken</item>
-                    </items>
-                    <signal name="changed" handler="voice_order_avatars_by_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">3</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_highlight_self_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Highlight Self</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">4</property>
-                    <property name="top-attach">4</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_highlight_self</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_highlight_self_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">4</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_border_width_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Border width</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">4</property>
-                    <property name="top-attach">5</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_border_width</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="text">1</property>
-                    <property name="adjustment">border_width_adj</property>
-                    <property name="value">1</property>
-                    <signal name="value-changed" handler="voice_border_width_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">5</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_icon_spacing_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Padding between users</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">4</property>
-                    <property name="top-attach">6</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_icon_spacing</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="text">0</property>
-                    <property name="adjustment">icon_spacing_adj</property>
-                    <signal name="value-changed" handler="voice_icon_spacing_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">6</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkButton">
-                    <property name="label" translatable="yes">Reset Voice Settings</property>
-                    <property name="name">voice_reset_all</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">True</property>
-                    <signal name="pressed" handler="voice_reset_all" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">12</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_inactive_fade_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Fade out when Inactive</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">4</property>
-                    <property name="top-attach">7</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_inactive_opacity_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Inactive Opacity</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">4</property>
-                    <property name="top-attach">8</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_inactive_time_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Time before Inactive</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">4</property>
-                    <property name="top-attach">9</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_inactive_fade_time_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Time Fading out</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">4</property>
-                    <property name="top-attach">10</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_inactive_fade</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="inactive_fade_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">7</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkScale">
-                    <property name="name">voice_inactive_opacity</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="adjustment">voice_inactive_fade_opacity</property>
-                    <property name="round-digits">1</property>
-                    <signal name="value-changed" handler="inactive_fade_opacity_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">8</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_inactive_time</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="text">0</property>
-                    <property name="adjustment">voice_inactive_time_range</property>
-                    <signal name="value-changed" handler="inactive_time_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">9</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_inactive_fade_time</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="text">0</property>
-                    <property name="adjustment">voice_inactive_fade_time_range</property>
-                    <signal name="value-changed" handler="inactive_fade_time_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">5</property>
-                    <property name="top-attach">10</property>
-                  </packing>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
-                <child>
-                  <placeholder/>
-                </child>
+              <object class="GtkLabel">
+                <property name="name">voice_talking_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Talking</property>
               </object>
               <packing>
-                <property name="left-attach">0</property>
+                <property name="left-attach">2</property>
                 <property name="top-attach">1</property>
-                <property name="width">3</property>
               </packing>
             </child>
             <child>
-              <!-- n-columns=2 n-rows=2 -->
-              <object class="GtkGrid">
-                <property name="name">voice_mouseover_grid</property>
-                <property name="visible">True</property>
-                <property name="can-focus">False</property>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_hide_mouseover_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Hide Overlay on Mouseover</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">0</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkLabel">
-                    <property name="name">voice_show_mouseover_label</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">False</property>
-                    <property name="label" translatable="yes">Show again after (seconds)</property>
-                    <property name="xalign">0</property>
-                  </object>
-                  <packing>
-                    <property name="left-attach">0</property>
-                    <property name="top-attach">1</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkCheckButton">
-                    <property name="name">voice_hide_mouseover</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="receives-default">False</property>
-                    <property name="draw-indicator">True</property>
-                    <signal name="toggled" handler="voice_hide_mouseover_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">0</property>
-                  </packing>
-                </child>
-                <child>
-                  <object class="GtkSpinButton">
-                    <property name="name">voice_show_mouseover</property>
-                    <property name="visible">True</property>
-                    <property name="can-focus">True</property>
-                    <property name="adjustment">voice_show_mouseover_adj</property>
-                    <signal name="value-changed" handler="voice_mouseover_timeout_changed" swapped="no"/>
-                  </object>
-                  <packing>
-                    <property name="left-attach">1</property>
-                    <property name="top-attach">1</property>
-                  </packing>
-                </child>
+              <object class="GtkLabel">
+                <property name="name">voice_idle_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Idle</property>
               </object>
               <packing>
                 <property name="left-attach">2</property>
+                <property name="top-attach">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_mute_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Mute</property>
+              </object>
+              <packing>
+                <property name="left-attach">2</property>
+                <property name="top-attach">3</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_avatar_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Avatar</property>
+              </object>
+              <packing>
+                <property name="left-attach">2</property>
+                <property name="top-attach">4</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_foreground_label</property>
+                <property name="width-request">100</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="margin-left">4</property>
+                <property name="margin-right">4</property>
+                <property name="margin-start">4</property>
+                <property name="margin-end">4</property>
+                <property name="label" translatable="yes">Foreground</property>
+              </object>
+              <packing>
+                <property name="left-attach">3</property>
                 <property name="top-attach">0</property>
               </packing>
             </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_background_label</property>
+                <property name="width-request">100</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="margin-left">4</property>
+                <property name="margin-right">4</property>
+                <property name="margin-start">4</property>
+                <property name="margin-end">4</property>
+                <property name="label" translatable="yes">Background</property>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">0</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_border_label</property>
+                <property name="width-request">100</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="margin-left">4</property>
+                <property name="margin-right">4</property>
+                <property name="margin-start">4</property>
+                <property name="margin-end">4</property>
+                <property name="label" translatable="yes">Border</property>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">0</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkColorButton">
+                <property name="name">voice_talking_foreground</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">True</property>
+                <property name="use-alpha">True</property>
+                <signal name="color-set" handler="voice_talking_foreground_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">3</property>
+                <property name="top-attach">1</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkColorButton">
+                <property name="name">voice_talking_background</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">True</property>
+                <property name="use-alpha">True</property>
+                <signal name="color-set" handler="voice_talking_background_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">1</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkColorButton">
+                <property name="name">voice_talking_border</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">True</property>
+                <property name="use-alpha">True</property>
+                <signal name="color-set" handler="voice_talking_border_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">1</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkColorButton">
+                <property name="name">voice_idle_foreground</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">True</property>
+                <property name="use-alpha">True</property>
+                <signal name="color-set" handler="voice_idle_foreground_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">3</property>
+                <property name="top-attach">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkColorButton">
+                <property name="name">voice_idle_background</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">True</property>
+                <property name="use-alpha">True</property>
+                <signal name="color-set" handler="voice_idle_background_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkColorButton">
+                <property name="name">voice_idle_border</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">True</property>
+                <property name="use-alpha">True</property>
+                <signal name="color-set" handler="voice_idle_border_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkColorButton">
+                <property name="name">voice_mute_foreground</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">True</property>
+                <property name="use-alpha">True</property>
+                <signal name="color-set" handler="voice_mute_foreground_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">3</property>
+                <property name="top-attach">3</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkColorButton">
+                <property name="name">voice_mute_background</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">True</property>
+                <property name="use-alpha">True</property>
+                <signal name="color-set" handler="voice_mute_background_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">3</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkColorButton">
+                <property name="name">voice_avatar_background</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">True</property>
+                <property name="use-alpha">True</property>
+                <signal name="color-set" handler="voice_avatar_background_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">4</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_hide_mouseover_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Hide Overlay on Mouseover</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">6</property>
+                <property name="top-attach">1</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkCheckButton">
+                <property name="name">voice_hide_mouseover</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">False</property>
+                <property name="draw-indicator">True</property>
+                <signal name="toggled" handler="voice_hide_mouseover_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">7</property>
+                <property name="top-attach">1</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_show_mouseover_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Show again after (seconds)</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">6</property>
+                <property name="top-attach">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkSpinButton">
+                <property name="name">voice_show_mouseover</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="text">1</property>
+                <property name="adjustment">voice_show_mouseover_adj</property>
+                <property name="value">1</property>
+                <signal name="value-changed" handler="voice_mouseover_timeout_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">7</property>
+                <property name="top-attach">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_overlay_location_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Overlay Location</property>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">0</property>
+                <property name="width">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkComboBoxText" id="voice_anchor_float">
+                <property name="name">voice_anchor_float</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="active">0</property>
+                <items>
+                  <item translatable="yes">Floating</item>
+                  <item translatable="yes">Anchor to Edge</item>
+                </items>
+                <signal name="changed" handler="voice_anchor_float_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">1</property>
+                <property name="width">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkComboBoxText" id="voice_monitor">
+                <property name="name">voice_monitor</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <signal name="changed" handler="voice_monitor_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">2</property>
+                <property name="width">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkComboBoxText" id="voice_align_1">
+                <property name="name">voice_align_1</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="active">0</property>
+                <items>
+                  <item translatable="yes">Left</item>
+                  <item translatable="yes">Right</item>
+                </items>
+                <signal name="changed" handler="voice_align_1_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">3</property>
+                <property name="width">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkComboBoxText" id="voice_align_2">
+                <property name="name">voice_align_2</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="active">0</property>
+                <items>
+                  <item translatable="yes">Top</item>
+                  <item translatable="yes">Middle</item>
+                  <item translatable="yes">Bottom</item>
+                </items>
+                <signal name="changed" handler="voice_align_2_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">4</property>
+                <property name="width">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkButton" id="voice_place_window_button">
+                <property name="label" translatable="yes">Place Window</property>
+                <property name="name">voice_place_window_button</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">True</property>
+                <signal name="pressed" handler="voice_place_window" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">3</property>
+                <property name="width">2</property>
+              </packing>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
           </object>
           <packing>
             <property name="position">1</property>
+            <property name="tab-fill">False</property>
           </packing>
         </child>
         <child type="tab">
           <object class="GtkLabel" id="notebook_voice_label">
             <property name="name">notebook_voice_label</property>
             <property name="visible">True</property>
             <property name="can-focus">False</property>
@@ -1701,26 +794,919 @@
           </object>
           <packing>
             <property name="position">1</property>
             <property name="tab-fill">False</property>
           </packing>
         </child>
         <child>
+          <!-- n-columns=6 n-rows=13 -->
+          <object class="GtkGrid">
+            <property name="name">voice_advanced_grid</property>
+            <property name="visible">True</property>
+            <property name="can-focus">False</property>
+            <property name="row-spacing">1</property>
+            <property name="column-spacing">5</property>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_display_icon_only_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Show Names</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">2</property>
+                <property name="top-attach">0</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkCheckButton">
+                <property name="name">voice_display_icon_only</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">False</property>
+                <property name="draw-indicator">True</property>
+                <signal name="toggled" handler="voice_display_icon_only_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">3</property>
+                <property name="top-attach">0</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_font_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Font</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">2</property>
+                <property name="top-attach">1</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkFontButton">
+                <property name="name">voice_font</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">True</property>
+                <property name="font">Sans 12</property>
+                <property name="language">en-us</property>
+                <property name="preview-text"/>
+                <signal name="font-set" handler="voice_font_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">3</property>
+                <property name="top-attach">1</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_text_padding_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Text Padding</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">2</property>
+                <property name="top-attach">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkSpinButton">
+                <property name="name">voice_text_padding</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="text">0</property>
+                <property name="adjustment">text_padding_adj</property>
+                <signal name="value-changed" handler="voice_text_padding_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">3</property>
+                <property name="top-attach">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_text_vertical_offset_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Text Vertical Offset</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">2</property>
+                <property name="top-attach">3</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkSpinButton">
+                <property name="name">voice_text_vertical_offset</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="text">0</property>
+                <property name="adjustment">voice_text_offset</property>
+                <signal name="value-changed" handler="voice_text_vertical_offset_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">3</property>
+                <property name="top-attach">3</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_show_title_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Show Title</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">0</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkCheckButton">
+                <property name="name">voice_show_title</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">False</property>
+                <property name="draw-indicator">True</property>
+                <signal name="toggled" handler="voice_show_title_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">1</property>
+                <property name="top-attach">0</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_show_connection_status_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Show Connection Status</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkCheckButton">
+                <property name="name">voice_show_connection_status</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">False</property>
+                <property name="draw-indicator">True</property>
+                <signal name="toggled" handler="voice_show_connection_status_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">1</property>
+                <property name="top-attach">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkFontButton">
+                <property name="name">voice_title_font</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">True</property>
+                <property name="font">Sans 12</property>
+                <property name="language">en-us</property>
+                <property name="preview-text"/>
+                <signal name="font-set" handler="voice_title_font_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">1</property>
+                <property name="top-attach">1</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_title_font_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Title Font</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">1</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkSpinButton">
+                <property name="name">voice_vertical_padding</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="text">0</property>
+                <property name="adjustment">voice_vertical_padding_adj</property>
+                <signal name="value-changed" handler="voice_vertical_padding_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">1</property>
+                <property name="top-attach">4</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_horizontal_padding_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Horizontal Edge Padding</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">5</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkSpinButton">
+                <property name="name">voice_horizontal_padding</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="text">0</property>
+                <property name="adjustment">voice_horizontal_padding_adj</property>
+                <signal name="value-changed" handler="voice_horizontal_padding_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">1</property>
+                <property name="top-attach">5</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_show_test_content_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Show Test Content</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">7</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkCheckButton">
+                <property name="name">voice_show_test_content</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">False</property>
+                <property name="draw-indicator">True</property>
+                <signal name="toggled" handler="voice_toggle_test_content" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">1</property>
+                <property name="top-attach">7</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_dummy_count_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Test Data Count</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">8</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkSpinButton">
+                <property name="name">voice_dummy_count</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="text">50</property>
+                <property name="adjustment">voice_dummy_count_adj</property>
+                <property name="value">50</property>
+                <signal name="value-changed" handler="voice_dummy_count_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">1</property>
+                <property name="top-attach">8</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_show_disconnected_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Show While Disconnected</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">9</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkCheckButton">
+                <property name="name">voice_show_disconnected</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">False</property>
+                <property name="draw-indicator">True</property>
+                <signal name="toggled" handler="voice_show_disconnected_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">1</property>
+                <property name="top-attach">9</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voce_vertical_padding_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Verticle Edge Padding</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">4</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_nick_length_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Limit text length</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">2</property>
+                <property name="top-attach">4</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkSpinButton">
+                <property name="name">voice_nick_length</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="text">32</property>
+                <property name="adjustment">voice_nick_lenght_adj</property>
+                <property name="value">32</property>
+                <signal name="value-changed" handler="voice_nick_length_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">3</property>
+                <property name="top-attach">4</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_avatar_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Show Avatar</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">2</property>
+                <property name="top-attach">5</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkCheckButton">
+                <property name="name">voice_show_avatar</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">False</property>
+                <property name="draw-indicator">True</property>
+                <signal name="toggled" handler="voice_show_avatar_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">3</property>
+                <property name="top-attach">5</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_square_avatar_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Square Avatar</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">2</property>
+                <property name="top-attach">6</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkCheckButton">
+                <property name="name">voice_square_avatar</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">False</property>
+                <property name="draw-indicator">True</property>
+                <signal name="toggled" handler="voice_square_avatar_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">3</property>
+                <property name="top-attach">6</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_fancy_avatar_shapes_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Fancy Avatar Shapes</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">2</property>
+                <property name="top-attach">7</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkCheckButton">
+                <property name="name">voice_fancy_avatar_shapes</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">False</property>
+                <property name="draw-indicator">True</property>
+                <signal name="toggled" handler="voice_fancy_avatar_shapes_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">3</property>
+                <property name="top-attach">7</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_avatar_size_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Avatar Size</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">2</property>
+                <property name="top-attach">8</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkSpinButton">
+                <property name="name">voice_avatar_size</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="text">48</property>
+                <property name="adjustment">avatar_size_adj</property>
+                <property name="value">48</property>
+                <signal name="value-changed" handler="voice_avatar_size_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">3</property>
+                <property name="top-attach">8</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_avatar_opacity_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Avatar Opacity</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">2</property>
+                <property name="top-attach">9</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkScale">
+                <property name="name">voice_avatar_opacity</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="adjustment">ava_opacity_adj</property>
+                <property name="round-digits">1</property>
+                <signal name="value-changed" handler="voice_avatar_opacity_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">3</property>
+                <property name="top-attach">9</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_display_speakers_only_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Display Speakers Only</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">0</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkCheckButton">
+                <property name="name">voice_display_speakers_only</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">False</property>
+                <property name="draw-indicator">True</property>
+                <signal name="toggled" handler="voice_display_speakers_only" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">0</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_display_speakers_grace_period_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Speakers Grace Period</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">1</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkSpinButton">
+                <property name="name">voice_display_speakers_grace_period</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="text">0</property>
+                <property name="adjustment">voice_display_speakers_grace_period_adj</property>
+                <signal name="value-changed" handler="voice_display_speakers_grace_period" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">1</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_overflow_style_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Overflow Style</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkComboBoxText" id="voice_overflow_style">
+                <property name="name">voice_overflow_style</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <items>
+                  <item translatable="yes">None</item>
+                  <item translatable="yes">Wrap</item>
+                  <item translatable="yes">Shrink</item>
+                </items>
+                <signal name="changed" handler="voice_overflow_style_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">2</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_order_avatars_by_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Order Users By</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">3</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkComboBoxText" id="voice_order_avatars_by">
+                <property name="name">voice_order_avatars_by</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <items>
+                  <item translatable="yes">Alphabetically</item>
+                  <item translatable="yes">ID</item>
+                  <item translatable="yes">Last Spoken</item>
+                </items>
+                <signal name="changed" handler="voice_order_avatars_by_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">3</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_highlight_self_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Highlight Self</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">4</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkCheckButton">
+                <property name="name">voice_highlight_self</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">False</property>
+                <property name="draw-indicator">True</property>
+                <signal name="toggled" handler="voice_highlight_self_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">4</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_border_width_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Border width</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">5</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkSpinButton">
+                <property name="name">voice_border_width</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="text">1</property>
+                <property name="adjustment">border_width_adj</property>
+                <property name="value">1</property>
+                <signal name="value-changed" handler="voice_border_width_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">5</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_icon_spacing_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Padding between users</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">6</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkSpinButton">
+                <property name="name">voice_icon_spacing</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="text">0</property>
+                <property name="adjustment">icon_spacing_adj</property>
+                <signal name="value-changed" handler="voice_icon_spacing_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">6</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkButton">
+                <property name="label" translatable="yes">Reset Voice Settings</property>
+                <property name="name">voice_reset_all</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">True</property>
+                <signal name="pressed" handler="voice_reset_all" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">12</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_inactive_fade_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Fade out when Inactive</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">7</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_inactive_opacity_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Inactive Opacity</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">8</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_inactive_time_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Time before Inactive</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">9</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">voice_inactive_fade_time_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Time Fading out</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">4</property>
+                <property name="top-attach">10</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkCheckButton">
+                <property name="name">voice_inactive_fade</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">False</property>
+                <property name="draw-indicator">True</property>
+                <signal name="toggled" handler="inactive_fade_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">7</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkScale">
+                <property name="name">voice_inactive_opacity</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="adjustment">voice_inactive_fade_opacity</property>
+                <property name="round-digits">1</property>
+                <signal name="value-changed" handler="inactive_fade_opacity_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">8</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkSpinButton">
+                <property name="name">voice_inactive_time</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="text">0</property>
+                <property name="adjustment">voice_inactive_time_range</property>
+                <signal name="value-changed" handler="inactive_time_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">9</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkSpinButton">
+                <property name="name">voice_inactive_fade_time</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="text">0</property>
+                <property name="adjustment">voice_inactive_fade_time_range</property>
+                <signal name="value-changed" handler="inactive_fade_time_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">5</property>
+                <property name="top-attach">10</property>
+              </packing>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+            <child>
+              <placeholder/>
+            </child>
+          </object>
+          <packing>
+            <property name="position">2</property>
+            <property name="tab-fill">False</property>
+          </packing>
+        </child>
+        <child type="tab">
+          <object class="GtkLabel" id="notebook_voice_adv_label">
+            <property name="name">notebook_voice_adv_label</property>
+            <property name="visible">True</property>
+            <property name="can-focus">False</property>
+            <property name="label" translatable="yes">Voice - Advanced</property>
+          </object>
+          <packing>
+            <property name="position">2</property>
+            <property name="tab-fill">False</property>
+          </packing>
+        </child>
+        <child>
           <!-- n-columns=2 n-rows=16 -->
           <object class="GtkGrid">
             <property name="name">text_grid</property>
             <property name="visible">True</property>
             <property name="can-focus">False</property>
             <property name="margin-start">5</property>
             <property name="margin-end">5</property>
             <property name="margin-top">5</property>
             <property name="margin-bottom">5</property>
             <property name="row-spacing">1</property>
             <property name="column-spacing">1</property>
-            <property name="column-homogeneous">True</property>
             <child>
               <object class="GtkLabel">
                 <property name="name">text_enable_label</property>
                 <property name="visible">True</property>
                 <property name="can-focus">False</property>
                 <property name="label" translatable="yes">Enable</property>
                 <property name="xalign">0</property>
@@ -2112,26 +2098,27 @@
               <placeholder/>
             </child>
             <child>
               <placeholder/>
             </child>
           </object>
           <packing>
-            <property name="position">2</property>
+            <property name="position">3</property>
+            <property name="tab-fill">False</property>
           </packing>
         </child>
         <child type="tab">
           <object class="GtkLabel" id="notebook_text_label">
             <property name="name">notebook_text_label</property>
             <property name="visible">True</property>
             <property name="can-focus">False</property>
             <property name="label" translatable="yes">Text</property>
           </object>
           <packing>
-            <property name="position">2</property>
+            <property name="position">3</property>
             <property name="tab-fill">False</property>
           </packing>
         </child>
         <child>
           <!-- n-columns=2 n-rows=18 -->
           <object class="GtkGrid">
             <property name="name">notification_grid</property>
@@ -2139,15 +2126,14 @@
             <property name="can-focus">False</property>
             <property name="margin-start">5</property>
             <property name="margin-end">5</property>
             <property name="margin-top">5</property>
             <property name="margin-bottom">5</property>
             <property name="row-spacing">1</property>
             <property name="column-spacing">1</property>
-            <property name="column-homogeneous">True</property>
             <child>
               <object class="GtkLabel">
                 <property name="name">notification_enable_label</property>
                 <property name="visible">True</property>
                 <property name="can-focus">False</property>
                 <property name="label" translatable="yes">Enable</property>
                 <property name="xalign">0</property>
@@ -2600,31 +2586,32 @@
               </packing>
             </child>
             <child>
               <placeholder/>
             </child>
           </object>
           <packing>
-            <property name="position">3</property>
+            <property name="position">4</property>
+            <property name="tab-fill">False</property>
           </packing>
         </child>
         <child type="tab">
           <object class="GtkLabel" id="notebook_notification_label">
             <property name="name">notebook_notification_label</property>
             <property name="visible">True</property>
             <property name="can-focus">False</property>
             <property name="label" translatable="yes">Notification</property>
           </object>
           <packing>
-            <property name="position">3</property>
+            <property name="position">4</property>
             <property name="tab-fill">False</property>
           </packing>
         </child>
         <child>
-          <!-- n-columns=2 n-rows=7 -->
+          <!-- n-columns=2 n-rows=8 -->
           <object class="GtkGrid">
             <property name="name">core_grid</property>
             <property name="visible">True</property>
             <property name="can-focus">False</property>
             <property name="margin-start">5</property>
             <property name="margin-end">5</property>
             <property name="margin-top">5</property>
@@ -2799,34 +2786,62 @@
                 <property name="visible">True</property>
                 <property name="can-focus">True</property>
                 <property name="receives-default">True</property>
                 <signal name="pressed" handler="core_reset_all" swapped="no"/>
               </object>
               <packing>
                 <property name="left-attach">1</property>
+                <property name="top-attach">7</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkLabel">
+                <property name="name">core_audio_assist_label</property>
+                <property name="visible">True</property>
+                <property name="can-focus">False</property>
+                <property name="label" translatable="yes">Integrate with Pipewire/Pulseaudio</property>
+                <property name="xalign">0</property>
+              </object>
+              <packing>
+                <property name="left-attach">0</property>
+                <property name="top-attach">6</property>
+              </packing>
+            </child>
+            <child>
+              <object class="GtkCheckButton">
+                <property name="name">core_audio_assist</property>
+                <property name="visible">True</property>
+                <property name="can-focus">True</property>
+                <property name="receives-default">False</property>
+                <property name="draw-indicator">True</property>
+                <signal name="toggled" handler="core_audio_assist_changed" swapped="no"/>
+              </object>
+              <packing>
+                <property name="left-attach">1</property>
                 <property name="top-attach">6</property>
               </packing>
             </child>
             <child>
               <placeholder/>
             </child>
           </object>
           <packing>
-            <property name="position">4</property>
+            <property name="position">5</property>
+            <property name="tab-fill">False</property>
           </packing>
         </child>
         <child type="tab">
           <object class="GtkLabel" id="notebook_core_label">
             <property name="name">notebook_core_label</property>
             <property name="visible">True</property>
             <property name="can-focus">False</property>
             <property name="label" translatable="yes">Core</property>
           </object>
           <packing>
-            <property name="position">4</property>
+            <property name="position">5</property>
             <property name="tab-fill">False</property>
           </packing>
         </child>
       </object>
     </child>
   </object>
 </interface>
```

### Comparing `discover-overlay-0.7.2/discover_overlay/image_getter.py` & `discover-overlay-0.7.3/discover_overlay/image_getter.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 import cairo
 import PIL
 import PIL.Image as Image
 import os
 import io
 import copy
 gi.require_version('GdkPixbuf', '2.0')
+gi.require_version("Gtk", "3.0")
 # pylint: disable=wrong-import-position
-from gi.repository import Gio, GdkPixbuf  # nopep8
+from gi.repository import Gio, GdkPixbuf, Gtk  # nopep8
 
 log = logging.getLogger(__name__)
 
 
 class SurfaceGetter():
     """Download and decode image using PIL and store as a cairo surface"""
 
@@ -64,33 +65,58 @@
             log.error("Unable to read %s", self.url)
         except TypeError:
             log.error("Unable to read %s", self.url)
         except PIL.UnidentifiedImageError:
             log.error("Unknown image type:  %s", self.url)
 
     def get_file(self):
+        errors = []
+        # Grab icon from icon theme
+        icon_theme = Gtk.IconTheme.get_default()
+        icon = icon_theme.choose_icon(
+            [self.url, None], -1, Gtk.IconLookupFlags.NO_SVG)
+
+        if icon:
+            try:
+                image = Image.open(icon.get_filename())
+                (surface, mask) = from_pil(image)
+                if surface:
+                    self.func(self.identifier, surface, mask)
+                    return
+            except ValueError:
+                errors.append("Value Error - Unable to read %s" % (mixpath))
+            except TypeError:
+                errors.append("Type Error - Unable to read %s" % (mixpath))
+            except PIL.UnidentifiedImageError:
+                errors.append("Unknown image type: %s" % (mixpath))
+            except FileNotFoundError:
+                errors.append("File not found: %s" % (mixpath))
+        # Not found in theme, try some common locations
         locations = [os.path.expanduser('~/.local/'), '/usr/', '/app']
         for prefix in locations:
-            mixpath = os.path.join(prefix, self.url)
+            mixpath = os.path.join(os.path.join(
+                prefix, 'share/icons/hicolor/256x256/apps/'), self.url + ".png")
             image = None
             try:
                 image = Image.open(mixpath)
             except ValueError:
-                log.error("Value Erorr - Unable to read %s", mixpath)
+                errors.append("Value Error - Unable to read %s" % (mixpath))
             except TypeError:
-                log.error("Type Error - Unable to read %s", mixpath)
+                errors.append("Type Error - Unable to read %s" % (mixpath))
             except PIL.UnidentifiedImageError:
-                log.error("Unknown image type: %s", mixpath)
+                errors.append("Unknown image type: %s" % (mixpath))
             except FileNotFoundError:
-                log.error("File not found: %s", mixpath)
+                errors.append("File not found: %s" % (mixpath))
             if image:
                 (surface, mask) = from_pil(image)
                 if surface:
                     self.func(self.identifier, surface, mask)
                     return
+        for error in errors:
+            log.error(error)
 
 
 def from_pil(image, alpha=1.0, format='BGRa'):
     """
     :param im: Pillow Image
     :param alpha: 0..1 alpha to add to non-alpha images
     :param format: Pixel format for output surface
@@ -109,26 +135,27 @@
             if arr[idx] > 0:
                 mask[idx] = 255
             else:
                 mask[idx] = 0
             # Cairo expects the raw data to be pre-multiplied alpha
             # This means when we change the alpha level we need to change the RGB channels equally
             arr[idx] = int(arr[idx] * alpha)
-            idx +=1
+            idx += 1
     surface = cairo.ImageSurface.create_for_data(
         arr, cairo.FORMAT_ARGB32, image.width, image.height)
     mask = cairo.ImageSurface.create_for_data(
         mask, cairo.FORMAT_ARGB32, image.width, image.height)
     return (surface, mask)
 
 
 def to_pil(surface):
     if surface.get_format() == cairo.Format.ARGB32:
-        return Image.frombuffer('RGBA', (surface.get_width(), surface.get_height()), surface.get_data(),'raw',"BGRA",surface.get_stride())
-    return Image.frombuffer("RGB", (surface.get_width(), surface.get_height()), surface.get_data(),'raw', "BGRX", stride)
+        return Image.frombuffer('RGBA', (surface.get_width(), surface.get_height()), surface.get_data(), 'raw', "BGRA", surface.get_stride())
+    return Image.frombuffer("RGB", (surface.get_width(), surface.get_height()), surface.get_data(), 'raw', "BGRX", stride)
+
 
 def get_surface(func, identifier, ava, size):
     """Download to cairo surface"""
     image_getter = SurfaceGetter(func, identifier, ava, size)
     if identifier.startswith('http'):
         thread = threading.Thread(target=image_getter.get_url)
         thread.start()
@@ -160,14 +187,15 @@
         width = height * img_aspect
         if hanchor == 2:
             offset_x = offset_x + (old_width - width)
         if hanchor == 1:
             offset_x = offset_x + ((old_width - width) / 2)
     return (offset_x, offset_y, width, height)
 
+
 def draw_img_to_rect(img, ctx,
                      pos_x, pos_y,
                      width, height,
                      path=False, aspect=False,
                      anchor=0, hanchor=0, alpha=1.0):
     """Draw cairo surface onto context
 
@@ -183,36 +211,37 @@
     if aspect:
         (offset_x, offset_y, width, height) = get_aspected_size(
             img, width, height, anchor=anchor, hanchor=hanchor)
 
     ctx.translate(pos_x + offset_x, pos_y + offset_y)
     ctx.scale(width, height)
     ctx.scale(1 / img.get_width(), 1 / img.get_height())
-    
+
     if alpha != 1.0:
         # Honestly, couldn't find a 'use-image-with-modifier' option
         # Tried RasterSourcePattern but it appears... broken? in the python implementation
         # Or just lacking documentation.
 
         # Pass raw data to PIL and then back with an alpha modifier
         ctx.set_source_surface(
             from_pil(
                 to_pil(img),
                 alpha
             )[0],
-            0,0)
+            0, 0)
     else:
         ctx.set_source_surface(img, 0, 0)
 
     ctx.rectangle(0, 0, img.get_width(), img.get_height())
     if not path:
         ctx.fill()
     ctx.restore()
     return (width, height)
 
+
 def draw_img_to_mask(img, ctx,
                      pos_x, pos_y,
                      width, height,
                      path=False, aspect=False,
                      anchor=0, hanchor=0):
     """Draw cairo surface as mask into context
```

### Comparing `discover-overlay-0.7.2/discover_overlay/locales/cy/LC_MESSAGES/default.mo` & `discover-overlay-0.7.3/discover_overlay/locales/cy/LC_MESSAGES/default.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -15,16 +15,16 @@
 
 msgid "1"
 msgstr "1"
 
 msgid "Alphabetically"
 msgstr "Yn nhrefn yr wyddor"
 
-msgid "Anchor To Edge"
-msgstr "Angor i ymyl"
+msgid "Anchor to Edge"
+msgstr "Angor i Ymyl"
 
 msgid "Avatar"
 msgstr "Avatar"
 
 msgid "Avatar Opacity"
 msgstr "Anhryloywder Avatar"
 
@@ -152,14 +152,17 @@
 msgstr ""
 "If tray icon is enabled, start with only tray icon and no configuration "
 "window"
 
 msgid "Inactive Opacity"
 msgstr "Anweithgar Gormes"
 
+msgid "Integrate with Pipewire/Pulseaudio"
+msgstr "Integrate with Pipewire/Pulseaudio"
+
 msgid "Last Spoken"
 msgstr "Siaradwyd ddiwethaf"
 
 msgid "Left"
 msgstr "Chwith"
 
 msgid "Limit Popup Width"
@@ -272,17 +275,14 @@
 
 msgid "Set unmuted"
 msgstr "Gosod nid treiglo"
 
 msgid "Settings"
 msgstr "Gosodiadau"
 
-msgid "Show Advanced Options"
-msgstr "Dangos Mwy o Opsiynau"
-
 msgid "Show Attachments"
 msgstr "Dangos atodiadau"
 
 msgid "Show Avatar"
 msgstr "Dangos Avatar"
 
 msgid "Show Connection Status"
@@ -371,12 +371,15 @@
 
 msgid "Verticle Edge Padding"
 msgstr "Padio ymyl fertigol"
 
 msgid "Voice"
 msgstr "LLais"
 
+msgid "Voice - Advanced"
+msgstr "LLais - Uwch"
+
 msgid "Welcome to Discover Overlay"
 msgstr "Croeso i Discover Overlay"
 
 msgid "Wrap"
 msgstr "Lapio"
```

### Comparing `discover-overlay-0.7.2/discover_overlay/locales/de/LC_MESSAGES/default.mo` & `discover-overlay-0.7.3/discover_overlay/locales/de/LC_MESSAGES/default.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -21,15 +21,15 @@
 
 msgid "AWAITING_ENDPOINT"
 msgstr "ENDPUNKT_ABWARTEN"
 
 msgid "Alphabetically"
 msgstr "Alphabetisch"
 
-msgid "Anchor To Edge"
+msgid "Anchor to Edge"
 msgstr "An der Kante verankern"
 
 msgid "Avatar"
 msgstr "Avatar"
 
 msgid "Avatar Opacity"
 msgstr "Avatardurchsichtigkeit"
@@ -271,17 +271,14 @@
 
 msgid "Set unmuted"
 msgstr "Lautgeschaltet einstellen"
 
 msgid "Settings"
 msgstr "Einstellungen"
 
-msgid "Show Advanced Options"
-msgstr "Erweiterte Optionen anzeigen"
-
 msgid "Show Attachments"
 msgstr "Anhänge anzeigen"
 
 msgid "Show Connection Status"
 msgstr "Verbindungsstatus anzeigen"
 
 msgid "Show Icon"
```

### Comparing `discover-overlay-0.7.2/discover_overlay/locales/fr/LC_MESSAGES/default.mo` & `discover-overlay-0.7.3/discover_overlay/locales/fr/LC_MESSAGES/default.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: discover 0.7.2\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2024-03-23 00:10+0100\n"
+"PO-Revision-Date: 2024-04-03 22:46+0200\n"
 "Last-Translator: Noé Lopez <noelopez@free.fr>\n"
 "Language-Team: Noé Lopez <noelopez@free.fr>\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
@@ -21,15 +21,15 @@
 
 msgid "AWAITING_ENDPOINT"
 msgstr "AWAITING_ENDPOINT"
 
 msgid "Alphabetically"
 msgstr "Ordre alphabétique"
 
-msgid "Anchor To Edge"
+msgid "Anchor to Edge"
 msgstr "Ancré au bord"
 
 msgid "Avatar"
 msgstr "Avatar"
 
 msgid "Avatar Opacity"
 msgstr "Opacité des avatars"
@@ -174,14 +174,17 @@
 msgstr ""
 "Si le raccourci de la barre d’outils est activé, démarrer seulement avec le "
 "raccourci et sans fenêtre de configuration"
 
 msgid "Inactive Opacity"
 msgstr "Opacité à l’inactivité"
 
+msgid "Integrate with Pipewire/Pulseaudio"
+msgstr "Intégration avec Pipewire/Pulseaudio"
+
 msgid "Last Spoken"
 msgstr "Dernier à avoir parlé"
 
 msgid "Left"
 msgstr "Gauche"
 
 msgid "Limit Popup Width"
@@ -297,17 +300,14 @@
 
 msgid "Set unmuted"
 msgstr "Ne plus se rendre muet"
 
 msgid "Settings"
 msgstr "Paramètres"
 
-msgid "Show Advanced Options"
-msgstr "Afficher les options avancées"
-
 msgid "Show Attachments"
 msgstr "Afficher les pièce jointes"
 
 msgid "Show Avatar"
 msgstr "Afficher les avatars"
 
 msgid "Show Connection Status"
@@ -408,14 +408,17 @@
 
 msgid "Verticle Edge Padding"
 msgstr "Écart vertical avec le bord"
 
 msgid "Voice"
 msgstr "Voix"
 
+msgid "Voice - Advanced"
+msgstr "Voix — Avancé"
+
 msgid "Welcome to Discover Overlay"
 msgstr "Bienvenue sur le Discover Overlay"
 
 msgid "Wrap"
 msgstr "Retour à la ligne"
 
 msgid "from Discord client"
```

### Comparing `discover-overlay-0.7.2/discover_overlay/locales/tr/LC_MESSAGES/default.mo` & `discover-overlay-0.7.3/discover_overlay/locales/tr/LC_MESSAGES/default.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -12,15 +12,15 @@
 
 msgid " for support. Or open an issue on our GitHub "
 msgstr " sunucumuzu ziyaret edin. Veya Github'ta 'issue' açın."
 
 msgid "Alphabetically"
 msgstr "Alfabetik olarak"
 
-msgid "Anchor To Edge"
+msgid "Anchor to Edge"
 msgstr "Kenara Sabitle"
 
 msgid "Avatar"
 msgstr "Avatar"
 
 msgid "Avatar Opacity"
 msgstr "Avatar Saydamlığı"
@@ -245,17 +245,14 @@
 
 msgid "Set unmuted"
 msgstr "Sesi aç"
 
 msgid "Settings"
 msgstr "Ayarlar"
 
-msgid "Show Advanced Options"
-msgstr "Gelişmiş Ayarları Göster"
-
 msgid "Show Attachments"
 msgstr "Ekleri Göster"
 
 msgid "Show Avatar"
 msgstr "Avatarı Göster"
 
 msgid "Show Connection Status"
```

### Comparing `discover-overlay-0.7.2/discover_overlay/notification_overlay.py` & `discover-overlay-0.7.3/discover_overlay/notification_overlay.py`

 * *Files 10% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         # Iterate over and remove messages older than 30s
         for message in self.content:
             if message['time'] + self.text_time > now:
                 newlist.append(message)
         self.content = newlist
         # If the list is different than before
         if oldsize != len(newlist):
-            self.needsredraw = True
+            self.set_needs_redraw()
 
     def add_notification_message(self, data):
         noti = None
         data = data['data']
         message_id = data['message']['id']
         for message in self.content:
             if message['id'] == message_id:
@@ -100,63 +100,69 @@
             else:
                 noti = {"title": data['title'],
                         "body": data['body'], "time": time.time(),
                         "id": message_id}
 
         if noti:
             self.content.append(noti)
-            self.needsredraw = True
+            self.set_needs_redraw()
             self.get_all_images()
 
     def set_padding(self, padding):
         """
         Set the padding between notifications
         """
-        self.padding = padding
-        self.needsredraw = True
+        if self.padding != padding:
+            self.padding = padding
+            self.set_needs_redraw()
 
     def set_border_radius(self, radius):
         """
         Set the radius of the border
         """
-        self.border_radius = radius
-        self.needsredraw = True
+        if self.border_radius != radius:
+            self.border_radius = radius
+            self.set_needs_redraw()
 
     def set_icon_size(self, size):
         """
         Set Icon size
         """
-        self.icon_size = size
-        self.image_list = {}
-        self.get_all_images()
+        if self.icon_size != size:
+            self.icon_size = size
+            self.image_list = {}
+            self.get_all_images()
 
     def set_icon_pad(self, pad):
         """
         Set padding between icon and message
         """
-        self.icon_pad = pad
-        self.needsredraw = True
+        if self.icon_pad != pad:
+            self.icon_pad = pad
+            self.set_needs_redraw()
 
     def set_icon_left(self, left):
-        self.icon_left = left
-        self.needsredraw = True
+        if self.icon_left != left:
+            self.icon_left = left
+            self.set_needs_redraw()
 
     def set_text_time(self, timer):
         """
         Set the duration that a message will be visible for.
         """
         self.text_time = timer
         self.timer_after_draw = timer
 
     def set_limit_width(self, limit):
         """
         Set the word wrap limit in pixels
         """
-        self.limit_width = limit
-        self.needsredraw = True
+        if self.limit_width != limit:
+            self.limit_width = limit
+            self.set_needs_redraw()
 
     def get_all_images(self):
         the_list = self.content
         if self.testing:
             the_list = self.test_content
         for line in the_list:
             icon = line["icon"]
@@ -166,60 +172,65 @@
                             self.icon_size)
 
     def recv_icon(self, identifier, pix, mask):
         """
         Called when image_getter has downloaded an image
         """
         self.image_list[identifier] = pix
-        self.needsredraw = True
+        self.set_needs_redraw()
 
     def set_fg(self, fg_col):
         """
         Set default text colour
         """
-        self.fg_col = fg_col
-        self.needsredraw = True
+        if self.fg_col != fg_col:
+            self.fg_col = fg_col
+            self.set_needs_redraw()
 
     def set_bg(self, bg_col):
         """
         Set background colour
         """
-        self.bg_col = bg_col
-        self.needsredraw = True
+        if self.bg_col != bg_col:
+            self.bg_col = bg_col
+            self.set_needs_redraw()
 
     def set_show_icon(self, icon):
         """
         Set if icons should be shown inline
         """
-        self.show_icon = icon
-        self.needsredraw = True
-        self.get_all_images()
+        if self.show_icon != icon:
+            self.show_icon = icon
+            self.set_needs_redraw()
+            self.get_all_images()
 
     def set_reverse_order(self, rev):
-        self.reverse_order = rev
-        self.needsredraw = True
+        if self.reverse_order != rev:
+            self.reverse_order = rev
+            self.set_needs_redraw()
 
     def set_font(self, font):
         """
         Set font used to render text
         """
-        self.text_font = font
+        if self.text_font != font:
+            self.text_font = font
 
-        self.pango_rect = Pango.Rectangle()
-        font = Pango.FontDescription(self.text_font)
-        self.pango_rect.width = font.get_size() * Pango.SCALE
-        self.pango_rect.height = font.get_size() * Pango.SCALE
-        self.needsredraw = True
+            self.pango_rect = Pango.Rectangle()
+            font = Pango.FontDescription(self.text_font)
+            self.pango_rect.width = font.get_size() * Pango.SCALE
+            self.pango_rect.height = font.get_size() * Pango.SCALE
+            self.set_needs_redraw()
 
     def recv_attach(self, identifier, pix):
         """
         Called when an image has been downloaded by image_getter
         """
         self.icons[identifier] = pix
-        self.needsredraw = True
+        self.set_needs_redraw()
 
     def calc_all_height(self):
         h = 0
         my_list = self.content
         if self.testing:
             my_list = self.test_content
         for line in my_list:
@@ -512,9 +523,9 @@
         string = string .replace(">", "&gt;")
         string = string.replace("'", "&#39;")
         string = string.replace("\"", "&#34;")
         return string
 
     def set_testing(self, testing):
         self.testing = testing
-        self.needsredraw = True
+        self.set_needs_redraw()
         self.get_all_images()
```

### Comparing `discover-overlay-0.7.2/discover_overlay/overlay.py` & `discover-overlay-0.7.3/discover_overlay/overlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         if "Wayland" in screen_type:
             self.is_wayland = True
             return Gtk.WindowType.TOPLEVEL
         return Gtk.WindowType.POPUP
 
     def __init__(self, discover, piggyback=None):
         Gtk.Window.__init__(self, type=self.detect_type())
-        self.is_xatom_set=False
+        self.is_xatom_set = False
 
         self.discover = discover
         screen = self.get_screen()
         self.text_font = None
         self.text_size = None
         self.pos_x = None
         self.pos_y = None
@@ -110,15 +110,16 @@
         if piggyback:
             self.set_piggyback(piggyback)
 
         self.get_screen().connect("composited-changed", self.check_composite)
         self.get_screen().connect("monitors-changed", self.screen_changed)
         self.get_screen().connect("size-changed", self.screen_changed)
         if self.get_window():
-            self.get_window().set_events(self.get_window().get_events() | Gdk.EventMask.ENTER_NOTIFY_MASK)
+            self.get_window().set_events(self.get_window().get_events()
+                                         | Gdk.EventMask.ENTER_NOTIFY_MASK)
         self.connect("enter-notify-event", self.mouseover)
         self.connect("leave-notify-event", self.mouseout)
         self.mouse_over_timer = None
 
         # It shouldn't be possible, but let's not leave
         # this process hanging if it happens
         self.connect('destroy', self.window_exited)
@@ -198,44 +199,43 @@
                 surface = cairo.ImageSurface(
                     cairo.FORMAT_ARGB32, width, height)
                 surface_ctx = cairo.Context(surface)
                 self.overlay_draw(None, surface_ctx)
                 reg = Gdk.cairo_region_create_from_surface(surface)
                 self.input_shape_combine_region(reg)
 
-
-
         self.overlay_draw(_w, context, data)
 
     def overlay_draw(self, _w, context, data=None):
         """
         Draw overlay
         """
 
     def set_font(self, font):
         """
         Set the font used by the overlay
         """
-        self.text_font = font
-        self.set_needs_redraw()
+        if self.text_font != font:
+            self.text_font = font
+            self.set_needs_redraw()
 
     def set_floating(self, floating, pos_x, pos_y, width, height):
         """
         Set if the window is floating and what dimensions to use
         """
-
-        # Special case for Cinnamon desktop : see https://github.com/trigg/Discover/issues/322
-        if 'XDG_SESSION_DESKTOP' in os.environ and os.environ['XDG_SESSION_DESKTOP']=='cinnamon':
-            floating = True
-        self.floating = floating
-        self.pos_x = pos_x
-        self.pos_y = pos_y
-        self.width = width
-        self.height = height
-        self.force_location()
+        if self.floating != floating or self.pos_x != pos_x or self.pos_y != pos_y or self.width != width or self.height != height:
+            # Special case for Cinnamon desktop : see https://github.com/trigg/Discover/issues/322
+            if 'XDG_SESSION_DESKTOP' in os.environ and os.environ['XDG_SESSION_DESKTOP'] == 'cinnamon':
+                floating = True
+            self.floating = floating
+            self.pos_x = pos_x
+            self.pos_y = pos_y
+            self.width = width
+            self.height = height
+            self.force_location()
 
     def set_untouchable(self):
         """
         Create a custom input shape and tell it that all of the window is a cut-out
         This allows us to have a window above everything but that never gets clicked on
         """
         (width, height) = self.get_size()
@@ -244,19 +244,20 @@
         surface_ctx.set_source_rgba(0.0, 0.0, 0.0, 0.0)
         surface_ctx.set_operator(cairo.OPERATOR_SOURCE)
         surface_ctx.paint()
         reg = Gdk.cairo_region_create_from_surface(surface)
         self.input_shape_combine_region(reg)
 
     def set_hide_on_mouseover(self, hide):
-        self.hide_on_mouseover = hide
-        if self.hide_on_mouseover:
-            self.set_needs_redraw()
-        else:
-            self.set_untouchable()
+        if self.hide_on_mouseover != hide:
+            self.hide_on_mouseover = hide
+            if self.hide_on_mouseover:
+                self.set_needs_redraw()
+            else:
+                self.set_untouchable()
 
     def set_mouseover_timer(self, time):
         self.timeout_mouse_over = time
 
     def unset_shape(self):
         """
         Remove XShape (not input shape)
@@ -363,46 +364,49 @@
 
     def set_monitor(self, idx=None):
         """
         Set the monitor this overlay should display on.
         """
         if type(idx) is str:
             idx = 0
-        self.monitor = idx
-        if self.is_wayland:
-            display = Gdk.Display.get_default()
-            if "get_monitor" in dir(display):
-                monitor = display.get_monitor(self.monitor)
-                if monitor:
-                    GtkLayerShell.set_monitor(self, monitor)
+        if self.monitor != idx:
+            self.monitor = idx
+            if self.is_wayland:
+                display = Gdk.Display.get_default()
+                if "get_monitor" in dir(display):
+                    monitor = display.get_monitor(self.monitor)
+                    if monitor:
+                        GtkLayerShell.set_monitor(self, monitor)
+                    else:
+                        self.hide()
+                        self.set_wayland_state()
+                        self.show()
                 else:
-                    self.hide()
-                    self.set_wayland_state()
-                    self.show()
-            else:
-                log.error("No get_monitor in display")
-            self.set_untouchable()
-        self.force_location()
-        self.set_needs_redraw()
+                    log.error("No get_monitor in display")
+                self.set_untouchable()
+            self.force_location()
+            self.set_needs_redraw()
 
     def set_align_x(self, align_right):
         """
         Set the alignment (True for right, False for left)
         """
-        self.align_right = align_right
-        self.force_location()
-        self.set_needs_redraw()
+        if self.align_right != align_right:
+            self.align_right = align_right
+            self.force_location()
+            self.set_needs_redraw()
 
     def set_align_y(self, align_vert):
         """
         Set the veritcal alignment
         """
-        self.align_vert = align_vert
-        self.force_location()
-        self.set_needs_redraw()
+        if self.align_vert != align_vert:
+            self.align_vert = align_vert
+            self.force_location()
+            self.set_needs_redraw()
 
     def col(self, col, alpha=1.0):
         """
         Convenience function to set the cairo context next colour
         """
         self.context.set_source_rgba(col[0], col[1], col[2], col[3] * alpha)
 
@@ -432,25 +436,26 @@
             self.hide()
 
     def set_task(self, visible):
         self.set_skip_pager_hint(not visible)
         self.set_skip_taskbar_hint(not visible)
 
     def check_composite(self, _a=None, _b=None):
+        # Called when an X11 session switched compositing on or off
         self.redraw()
 
     def screen_changed(self, screen=None):
         self.set_monitor(self.monitor)
 
     def mouseover(self, a=None, b=None):
         self.draw_blank = True
         self.set_needs_redraw()
         return True
 
     def mouseout(self, a=None, b=None):
         GLib.timeout_add_seconds(self.timeout_mouse_over, self.mouseout_timed)
-
         return True
 
     def mouseout_timed(self, a=None, b=None):
         self.draw_blank = False
-        self.set_needs_redraw()
+        self.set_needs_redraw()
+        return False
```

### Comparing `discover-overlay-0.7.2/discover_overlay/settings_window.py` & `discover-overlay-0.7.3/discover_overlay/settings_window.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,18 +39,32 @@
     def __init__(self, config_file, rpc_file, channel_file, args):
         self.args = args
         # Detect Bazzite autostart
         self.alternative_autostart = os.path.exists(
             "/etc/default/discover-overlay")
         # Detect flatpak en
         self.disable_autostart = 'container' in os.environ
+        self.icon_name = "discover-overlay"
+        self.tray_icon_name = "discover-overlay-tray"
+
+        self.spinning_focus = None
+        self.scale_focus = None
+
+        icon_theme = Gtk.IconTheme.get_default()
+        icon_theme.add_resource_path(os.path.expanduser(
+            '~/.local/share/pipx/venvs/discover-overlay/share/icons'))
+        if not icon_theme.has_icon("discover-overlay"):
+            log.error("No icon found in theme")
+            self.icon_name = 'user-info'
+        if not icon_theme.has_icon(self.tray_icon_name):
+            log.error("No tray icon found in theme")
+            self.tray_icon_name = 'user-info'
         self.steamos = False
         self.voice_placement_window = None
         self.text_placement_window = None
-        self.voice_advanced = False
         self.tray = None  # Systemtray as fallback
         self.ind = None  # AppIndicator
         if self.alternative_autostart:
             self.autostart_helper = BazziteAutostart()
         else:
             self.autostart_helper = Autostart("discover_overlay")
 
@@ -110,29 +124,32 @@
             log.info(
                 "GameScope session detected. Enabling steam and gamescope integration")
             self.steamos = True
             settings = Gtk.Settings.get_default()
             if settings:
                 settings.set_property(
                     "gtk-application-prefer-dark-theme", Gtk.true)
-            self.widget['notebook'].set_tab_pos(Gtk.PositionType.LEFT)
             # TODO Not assume the display size. Probably poll it from GDK Display?
             window.set_default_size(1280, 800)
 
             # Larger fonts needed
             css = Gtk.CssProvider.new()
             css.load_from_data(bytes("* { font-size:18px; }", "utf-8"))
             window.get_style_context().add_provider(
                 css, Gtk.STYLE_PROVIDER_PRIORITY_USER)
-
-            # Space is premium. Sorry Craig
-            self.widget['voice_advanced_grid'].set_column_homogeneous(False)
         else:
             self.widget['overview_close_button'].hide()
 
+        self.super_focus = Gtk.CssProvider.new()
+        self.super_focus.load_from_data(
+            bytes(
+                """scale { background-color: rgba(100%, 0%, 0%, 0.3); background-image:unset; }
+                   spinbutton { background-color: rgba(100%, 0%, 0%, 0.3); background-image:unset;}
+                """, "utf-8"))
+
         screen = window.get_screen()
         screen_type = "%s" % (screen)
         self.is_wayland = False
         if "Wayland" in screen_type:
             self.is_wayland = True
         self.window = window
 
@@ -152,20 +169,113 @@
             'toggled', self.core_hide_overlay_changed)
 
         self.read_config()
 
         self.populate_guild_menu()
 
         builder.connect_signals(self)
+        window.connect('key-press-event', self.keypress_in_settings)
 
         if '--minimized' in self.args:
             self.start_minimized = True
         if not self.start_minimized or not self.show_sys_tray_icon:
             window.show()
 
+        if self.icon_name != 'discover-overlay':
+            self.widget['overview_image'].set_from_icon_name(
+                self.icon_name, Gtk.IconSize.DIALOG)
+            self.widget['window'].set_default_icon_name(self.icon_name)
+
+    def keypress_in_settings(self, window, event):
+        if self.spinning_focus:
+            match event.keyval:
+                case Gdk.KEY_Right:
+                    step = self.spinning_focus.get_increments().step
+                    value = self.spinning_focus.get_value()
+                    self.spinning_focus.set_value(value + step)
+                    pass
+                case Gdk.KEY_Left:
+                    step = self.spinning_focus.get_increments().step
+                    value = self.spinning_focus.get_value()
+                    self.spinning_focus.set_value(value - step)
+                    pass
+                case Gdk.KEY_Up:
+                    step = self.spinning_focus.get_increments().step
+                    value = self.spinning_focus.get_value()
+                    self.spinning_focus.set_value(value + step)
+                case Gdk.KEY_Down:
+                    step = self.spinning_focus.get_increments().step
+                    value = self.spinning_focus.get_value()
+                    self.spinning_focus.set_value(value - step)
+                case Gdk.KEY_space:
+                    self.spinning_focus.get_style_context().remove_provider(self.super_focus)
+                    self.spinning_focus = None
+                case Gdk.KEY_Escape:
+                    self.spinning_focus.get_style_context().remove_provider(self.super_focus)
+
+                    self.spinning_focus = None
+        elif self.scale_focus:
+            match event.keyval:
+                case Gdk.KEY_Right:
+                    value = self.scale_focus.get_value()
+                    self.scale_focus.set_value(value + 0.1)
+                    pass
+                case Gdk.KEY_Left:
+                    value = self.scale_focus.get_value()
+                    self.scale_focus.set_value(value - 0.1)
+                    pass
+                case Gdk.KEY_Up:
+                    value = self.scale_focus.get_value()
+                    self.scale_focus.set_value(value + 0.1)
+                case Gdk.KEY_Down:
+                    value = self.scale_focus.get_value()
+                    self.scale_focus.set_value(value - 0.1)
+                case Gdk.KEY_space:
+                    self.scale_focus.get_style_context().remove_provider(self.super_focus)
+                    self.scale_focus = None
+                case Gdk.KEY_Escape:
+                    self.scale_focus.get_style_context().remove_provider(self.super_focus)
+                    self.scale_focus = None
+        else:
+            match event.keyval:
+                case Gdk.KEY_Left:
+                    window.do_move_focus(window, Gtk.DirectionType.LEFT)
+                case Gdk.KEY_Right:
+                    window.do_move_focus(window, Gtk.DirectionType.RIGHT)
+                case Gdk.KEY_Up:
+                    window.do_move_focus(window, Gtk.DirectionType.UP)
+                case Gdk.KEY_Down:
+                    window.do_move_focus(window, Gtk.DirectionType.DOWN)
+                case Gdk.KEY_F1:
+                    self.widget['notebook'].prev_page()
+                case Gdk.KEY_F2:
+                    self.widget['notebook'].next_page()
+                case Gdk.KEY_Escape:
+                    return True
+                case Gdk.KEY_space:
+                    widget = self.window.get_focus()
+                    if widget:
+                        # I really want there to be a better way...
+                        widget_type = "%s" % (widget)
+                        if 'Gtk.SpinButton' in widget_type:
+                            self.spinning_focus = widget
+
+                            widget.get_style_context().add_provider(
+                                self.super_focus, Gtk.STYLE_PROVIDER_PRIORITY_APPLICATION)
+                            return True
+                        elif 'Gtk.Scale' in widget_type:
+                            self.scale_focus = widget
+                            widget.get_style_context().add_provider(
+                                self.super_focus, Gtk.STYLE_PROVIDER_PRIORITY_APPLICATION)
+                            return True
+                    return False
+                case _:
+                    return False
+        return True
+
     def request_channels_from_guild(self, guild_id):
         with open(self.rpc_file, 'w') as f:
             f.write('--rpc --guild-request=%s' % (guild_id))
 
     def populate_guild_menu(self, _a=None, _b=None, _c=None, _d=None):
         g = self.widget['text_server']
         c = self.widget['text_channel']
@@ -263,33 +373,32 @@
             i2 = m2.iter_next(i2)
             m2.set_value(i2, 0, _("Middle"))
             i2 = m2.iter_next(i2)
             m2.set_value(i2, 0, _("Bottom"))
 
     def read_config(self):
         self.loading_config = True
-        self.widget['voice_advanced_grid'].hide()
 
         # Read config and put into gui
         config = ConfigParser(interpolation=None)
         config.read(self.config_file)
 
         # Read Voice section
 
         self.voice_floating_x = config.getint("main", "floating_x", fallback=0)
         self.voice_floating_y = config.getint("main", "floating_y", fallback=0)
         self.voice_floating_w = config.getint(
             "main", "floating_w", fallback=400)
         self.voice_floating_h = config.getint(
             "main", "floating_h", fallback=400)
 
-        if config.getboolean("main", "floating", fallback=False):
-            self.widget['voice_floating_button'].set_active(True)
-        else:
-            self.widget['voice_anchor_to_edge_button'].set_active(True)
+        self.widget['voice_anchor_float'].set_active(
+            0 if config.getboolean("main", "floating", fallback=False) else 1)
+        self.update_floating_ahchor()
+
         self.widget['voice_align_1'].set_active(
             config.getboolean("main", "rightalign", fallback=False))
         self.widget['voice_align_2'].set_active(
             config.getint("main", "topalign", fallback=1))
 
         monitor = 0
         try:
@@ -417,14 +526,20 @@
         )
         self.widget['voice_inactive_time'].set_value(
             config.getint("main", "inactive_time", fallback=10)
         )
         self.widget['voice_inactive_fade_time'].set_value(
             config.getint("main", "inactive_fade_time", fallback=30)
         )
+        self.widget['voice_hide_mouseover'].set_active(
+            config.getboolean("main", "autohide", fallback=False)
+        )
+        self.widget['voice_show_mouseover'].set_value(
+            config.getint("main", "autohide_timer", fallback=5)
+        )
 
         # Read Text section
 
         self.text_floating_x = config.getint("text", "floating_x", fallback=0)
         self.text_floating_y = config.getint("text", "floating_y", fallback=0)
         self.text_floating_w = config.getint(
             "text", "floating_w", fallback=400)
@@ -465,14 +580,21 @@
 
         self.widget['text_show_attachments'].set_active(config.getboolean(
             "text", "show_attach", fallback=True))
 
         self.widget['text_line_limit'].set_value(
             config.getint("text", "line_limit", fallback=20))
 
+        self.widget['text_hide_mouseover'].set_active(
+            config.getboolean("text", "autohide", fallback=False)
+        )
+        self.widget['text_show_mouseover'].set_value(
+            config.getint("text", "autohide_timer", fallback=5)
+        )
+
         # Read Notification section
         self.widget['notification_enable'].set_active(
             config.getboolean("notification", "enabled", fallback=False))
 
         self.widget['notification_reverse_order'].set_active(
             config.getboolean("notification", "rev", fallback=False))
 
@@ -548,21 +670,25 @@
 
         self.hidden_overlay = config.getboolean(
             "general", "hideoverlay", fallback=False)
         self.update_toggle_overlay()
 
         self.start_minimized = config.getboolean(
             "general", "start_min", fallback=False)
+
         self.widget['core_settings_min'].set_active(self.start_minimized)
 
         self.widget['core_settings_min'].set_sensitive(self.show_sys_tray_icon)
-    
-        if 'XDG_SESSION_DESKTOP' in os.environ and os.environ['XDG_SESSION_DESKTOP']=='cinnamon':
+
+        if 'XDG_SESSION_DESKTOP' in os.environ and os.environ['XDG_SESSION_DESKTOP'] == 'cinnamon':
             self.widget['voice_anchor_to_edge_button'].set_sensitive(False)
 
+        self.widget['core_audio_assist'].set_active(
+            config.getboolean("general", "audio_assist", fallback=False))
+
         self.loading_config = False
 
     def make_colour(self, col):
         col = json.loads(col)
         return Gdk.RGBA(col[0], col[1], col[2], col[3])
 
     def parse_guild_ids(self, guild_ids_str):
@@ -588,24 +714,24 @@
         """
         try:
             gi.require_version('AppIndicator3', '0.1')
             # pylint: disable=import-outside-toplevel
             from gi.repository import AppIndicator3
             self.ind = AppIndicator3.Indicator.new(
                 "discover_overlay",
-                "discover-overlay-tray",
+                self.tray_icon_name,
                 AppIndicator3.IndicatorCategory.APPLICATION_STATUS)
             # Hide for now since we don't know if it should be shown yet
             self.ind.set_status(AppIndicator3.IndicatorStatus.PASSIVE)
             self.ind.set_menu(menu)
         except (ImportError, ValueError) as exception:
             # Create System Tray
             log.info("Falling back to Systray : %s", exception)
             self.tray = Gtk.StatusIcon.new_from_icon_name(
-                "discover-overlay-tray")
+                self.tray_icon_name)
             self.tray.connect('popup-menu', self.show_menu)
             # Hide for now since we don't know if it should be shown yet
             self.tray.set_visible(False)
 
     def show_menu(self, obj, button, time):
         """
         Show menu when System Tray icon is clicked
@@ -804,36 +930,38 @@
         if context in config.sections():
             config.remove_section(context)
         else:
             log.error("Unable to remove section %s" % (context))
         with open(self.config_file, 'w') as file:
             config.write(file)
 
-    def voice_anchor_to_edge_changed(self, button):
-        self.config_set("main", "floating", "False")
-
-    def voice_floating_changed(self, button):
-        self.config_set("main", "floating", "True")
+    def voice_anchor_float_changed(self, button):
+        self.config_set("main", "floating", "%s" % (button.get_active() == 0))
+        self.update_floating_ahchor()
+
+    def update_floating_ahchor(self):
+        floating = self.widget['voice_anchor_float'].get_active() == 0
+        if floating:
+            self.widget['voice_align_1'].hide()
+            self.widget['voice_align_2'].hide()
+            self.widget['voice_place_window_button'].show()
+        else:
+            self.widget['voice_align_1'].show()
+            self.widget['voice_align_2'].show()
+            self.widget['voice_place_window_button'].hide()
 
     def voice_monitor_changed(self, button):
         self.config_set("main", "monitor", "%s" % (button.get_active()))
 
     def voice_align_1_changed(self, button):
         self.config_set("main", "rightalign", "%s" % (button.get_active()))
 
     def voice_align_2_changed(self, button):
         self.config_set("main", "topalign", "%s" % (button.get_active()))
 
-    def voice_show_advanced_options_button_changed(self, button):
-        self.voice_advanced = not self.voice_advanced
-        if self.voice_advanced:
-            self.widget['voice_advanced_grid'].show()
-        else:
-            self.widget['voice_advanced_grid'].hide()
-
     def voice_font_changed(self, button):
         self.config_set("main", "font", button.get_font())
 
     def voice_title_font_changed(self, button):
         self.config_set("main", "title_font", button.get_font())
 
     def voice_icon_spacing_changed(self, button):
@@ -1150,32 +1278,37 @@
     def notification_reset_all(self, button):
         self.config_remove_section("notification")
         self.read_config()
 
     def voice_hide_mouseover_changed(self, button):
         self.config_set("main", "autohide", "%s" % (button.get_active()))
 
-    def text_hide_mouseover_changed(self,button):
+    def text_hide_mouseover_changed(self, button):
         self.config_set("text", "autohide", "%s" % (button.get_active()))
 
     def voice_mouseover_timeout_changed(self, button):
         self.config_set("main", "autohide_timer", "%s" %
                         (int(button.get_value())))
 
     def text_mouseover_timeout_changed(self, button):
         self.config_set("text", "autohide_timer", "%s" %
                         (int(button.get_value())))
 
     def inactive_fade_changed(self, button):
-        self.config_set("main", "fade_out_inactive", "%s" % (button.get_active()))
+        self.config_set("main", "fade_out_inactive", "%s" %
+                        (button.get_active()))
 
     def inactive_fade_opacity_changed(self, button):
         self.config_set("main", "fade_out_limit", "%.2f" %
                         (button.get_value()))
 
     def inactive_time_changed(self, button):
         self.config_set("main", "inactive_time", "%s" %
-                (int(button.get_value())))
+                        (int(button.get_value())))
 
-    def inactive_fade_time_changed(self,button):
+    def inactive_fade_time_changed(self, button):
         self.config_set("main", "inactive_fade_time", "%s" %
-                (int(button.get_value())))
+                        (int(button.get_value())))
+
+    def core_audio_assist_changed(self, button):
+        self.config_set("general", "audio_assist", "%s" %
+                        (button.get_active()))
```

### Comparing `discover-overlay-0.7.2/discover_overlay/text_overlay.py` & `discover-overlay-0.7.3/discover_overlay/text_overlay.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,70 +71,77 @@
                     log.info("keeping %s", url)
                     self.attachment[url] = oldlist[url]
 
     def set_text_time(self, timer):
         """
         Set the duration that a message will be visible for.
         """
-        self.text_time = timer
-        self.timer_after_draw = timer
-        self.set_needs_redraw()
+        if self.text_time != timer or self.timer_after_draw != timer:
+            self.text_time = timer
+            self.timer_after_draw = timer
+            self.set_needs_redraw()
 
     def set_text_list(self, tlist, altered):
         """
         Update the list of text messages to show
         """
         self.content = tlist[-self.line_limit:]
         if altered:
             self.set_needs_redraw()
 
     def set_fg(self, fg_col):
         """
         Set default text colour
         """
-        self.fg_col = fg_col
-        self.set_needs_redraw()
+        if self.fg_col != fg_col:
+            self.fg_col = fg_col
+            self.set_needs_redraw()
 
     def set_bg(self, bg_col):
         """
         Set background colour
         """
-        self.bg_col = bg_col
-        self.set_needs_redraw()
+        if self.bg_col != bg_col:
+            self.bg_col = bg_col
+            self.set_needs_redraw()
 
     def set_show_attach(self, attachment):
         """
         Set if attachments should be shown inline
         """
-        self.show_attach = attachment
-        self.set_needs_redraw()
+        if self.attachment != attachment:
+            self.show_attach = attachment
+            self.set_needs_redraw()
 
     def set_popup_style(self, boolean):
         """
         Set if message disappear after a certain duration
         """
-        self.popup_style = boolean
+        if self.popup_style != boolean:
+            self.popup_style = boolean
 
     def set_font(self, font):
         """
         Set font used to render text
         """
-        self.text_font = font
+        if self.text_font != font:
+            self.text_font = font
 
-        self.pango_rect = Pango.Rectangle()
-        font = Pango.FontDescription(self.text_font)
-        self.pango_rect.width = font.get_size() * Pango.SCALE
-        self.pango_rect.height = font.get_size() * Pango.SCALE
-        self.set_needs_redraw()
+            self.pango_rect = Pango.Rectangle()
+            font = Pango.FontDescription(self.text_font)
+            self.pango_rect.width = font.get_size() * Pango.SCALE
+            self.pango_rect.height = font.get_size() * Pango.SCALE
+            self.set_needs_redraw()
 
     def set_line_limit(self, limit):
         """
         Change maximum number of lines in overlay
         """
-        self.line_limit = limit
+        if self.line_limit != limit:
+            self.line_limit = limit
 
     def make_line(self, message):
         """
         Decode a recursive JSON object into pango markup.
         """
         ret = ""
         if isinstance(message, list):
```

### Comparing `discover-overlay-0.7.2/discover_overlay/voice_overlay.py` & `discover-overlay-0.7.3/discover_overlay/voice_overlay.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,16 +94,16 @@
         self.channel_title = ""
         self.border_width = 2
         self.icon_transparency = 0.0
         self.fancy_border = False
 
         self.fade_out_inactive = True
         self.fade_out_limit = 0.1
-        self.inactive_time = 10 # Seconds
-        self.inactive_fade_time = 20 # Seconds
+        self.inactive_time = 10  # Seconds
+        self.inactive_fade_time = 20  # Seconds
         self.fade_opacity = 1.0
         self.fade_start = 0
 
         self.inactive_timeout = None
         self.fadeout_timeout = None
 
         self.round_avatar = True
@@ -120,296 +120,330 @@
         self.avatar_bg_col = [0.0, 0.0, 1.0, 1.0]
         self.userlist = []
         self.connection_status = "DISCONNECTED"
         self.horizontal = False
         self.guild_ids = tuple()
         self.force_location()
         get_surface(self.recv_avatar,
-                    "share/icons/hicolor/256x256/apps/discover-overlay-default.png",
+                    "discover-overlay-default",
                     'def', self.avatar_size)
         self.set_title("Discover Voice")
         self.redraw()
 
     def reset_action_timer(self):
+        # Reset time since last voice activity
         self.fade_opacity = 1.0
+
+        # Remove both fading-out effect and timer set last time this happened
         if self.inactive_timeout:
             GLib.source_remove(self.inactive_timeout)
             self.inactive_timeout = None
         if self.fadeout_timeout:
             GLib.source_remove(self.fadeout_timeout)
             self.fadeout_timeout = None
 
+        # If we're using this feature, schedule a new iactivity timer
         if self.fade_out_inactive:
-            self.inactive_timeout = GLib.timeout_add_seconds(self.inactive_time, self.overlay_inactive)
+            self.inactive_timeout = GLib.timeout_add_seconds(
+                self.inactive_time, self.overlay_inactive)
 
     def overlay_inactive(self):
-        self.fade_start= perf_counter()
-        self.fadeout_timeout = GLib.timeout_add(self.inactive_fade_time/200 * 1000, self.overlay_fadeout)
+        # Inactivity has hit the first threshold, start fading out
+        self.fade_start = perf_counter()
+        # Fade out in 200 steps over X seconds.
+        self.fadeout_timeout = GLib.timeout_add(
+            self.inactive_fade_time/200 * 1000, self.overlay_fadeout)
         self.inactive_timeout = None
         return False
 
     def overlay_fadeout(self):
         self.set_needs_redraw()
+        # There's no guarantee over the granularity of the callback here, so use our time-since to work out how faded out we should be
+        # Might look choppy on systems under high cpu usage but that's just how it's going to be
         now = perf_counter()
         time_percent = (now - self.fade_start) / self.inactive_fade_time
-        if time_percent>=1.0:
+        if time_percent >= 1.0:
             self.fade_opacity = self.fade_out_limit
             self.fadeout_timeout = None
             return False
 
-        self.fade_opacity = self.fade_out_limit + ((1.0 - self.fade_out_limit) * (1.0 - time_percent))
+        self.fade_opacity = self.fade_out_limit + \
+            ((1.0 - self.fade_out_limit) * (1.0 - time_percent))
         return True
 
     def col(self, col, alpha=1.0):
         """
         Convenience function to set the cairo context next colour. Altered to account for fade-out function
         """
         if alpha == None:
             self.context.set_source_rgba(col[0], col[1], col[2], col[3])
         else:
-            self.context.set_source_rgba(col[0], col[1], col[2], col[3] * alpha * self.fade_opacity)
+            self.context.set_source_rgba(
+                col[0], col[1], col[2], col[3] * alpha * self.fade_opacity)
 
     def set_icon_transparency(self, trans):
-        if self.icon_transparency == trans:
-            return
-        self.icon_transparency = trans
-        #get_surface(self.recv_avatar,
-        #            "share/icons/hicolor/256x256/apps/discover-overlay-default.png",
-        #            'def', self.avatar_size)
-
-        #self.avatars = {}
-        #self.avatar_masks = {}
-
-        #self.channel_icon = None
-        #self.channel_mask = None
-
-        self.set_needs_redraw()
+        if self.icon_transparency != trans:
+            self.icon_transparency = trans
+            self.set_needs_redraw()
 
     def set_blank(self):
         self.userlist = []
         self.channel_icon = None
         self.channel_icon_url = None
         self.channel_title = None
         self.connection_status = "DISCONNECTED"
         self.set_needs_redraw()
 
     def set_fade_out_inactive(self, enabled, fade_time, fade_duration, fade_to):
-        if self.fade_out_inactive == enabled and self.inactive_time == fade_time and self.inactive_fade_time == fade_duration and self.fade_out_limit == fade_to:
-            return
-        self.fade_out_inactive = enabled
-        self.inactive_time = fade_time
-        self.inactive_fade_time = fade_duration
-        self.fade_out_limit = fade_to
-        self.reset_action_timer()
+        if self.fade_out_inactive != enabled or self.inactive_time != fade_time or self.inactive_fade_time != fade_duration or self.fade_out_limit != fade_to:
+            self.fade_out_inactive = enabled
+            self.inactive_time = fade_time
+            self.inactive_fade_time = fade_duration
+            self.fade_out_limit = fade_to
+            self.reset_action_timer()
 
     def set_title_font(self, font):
-        self.title_font = font
-        self.set_needs_redraw()
+        if self.title_font != font:
+            self.title_font = font
+            self.set_needs_redraw()
 
     def set_show_connection(self, show_connection):
-        self.show_connection = show_connection
-        self.set_needs_redraw()
+        if self.show_connection != show_connection:
+            self.show_connection = show_connection
+            self.set_needs_redraw()
 
     def set_show_avatar(self, show_avatar):
-        self.show_avatar = show_avatar
-        self.set_needs_redraw()
+        if self.show_avatar != show_avatar:
+            self.show_avatar = show_avatar
+            self.set_needs_redraw()
 
     def set_show_title(self, show_title):
-        self.show_title = show_title
-        self.set_needs_redraw()
+        if self.show_title != show_title:
+            self.show_title = show_title
+            self.set_needs_redraw()
 
     def set_show_disconnected(self, show_disconnected):
-        self.show_disconnected = show_disconnected
-        self.set_needs_redraw()
+        if self.show_disconnected != show_disconnected:
+            self.show_disconnected = show_disconnected
+            self.set_needs_redraw()
 
     def set_show_dummy(self, show_dummy):
         """
         Toggle use of dummy userdata to help choose settings
         """
-        self.use_dummy = show_dummy
-        self.set_needs_redraw()
+        if self.use_dummy != show_dummy:
+            self.use_dummy = show_dummy
+            self.set_needs_redraw()
 
     def set_dummy_count(self, dummy_count):
-        self.dummy_count = dummy_count
-        self.set_needs_redraw()
+        if self.dummy_count != dummy_count:
+            self.dummy_count = dummy_count
+            self.set_needs_redraw()
 
     def set_overflow(self, overflow):
         """
         How should excessive numbers of users be dealt with?
         """
-        self.overflow = overflow
-        self.set_needs_redraw()
+        if self.overflow != overflow:
+            self.overflow = overflow
+            self.set_needs_redraw()
 
     def set_bg(self, background_colour):
         """
         Set the background colour
         """
-        self.norm_col = background_colour
-        self.set_needs_redraw()
+        if self.norm_col != background_colour:
+            self.norm_col = background_colour
+            self.set_needs_redraw()
 
     def set_fg(self, foreground_colour):
         """
         Set the text colour
         """
-        self.text_col = foreground_colour
-        self.set_needs_redraw()
+        if self.text_col != foreground_colour:
+            self.text_col = foreground_colour
+            self.set_needs_redraw()
 
     def set_tk(self, talking_colour):
         """
         Set the border colour for users who are talking
         """
-        self.talk_col = talking_colour
-        self.set_needs_redraw()
+        if self.talk_col != talking_colour:
+            self.talk_col = talking_colour
+            self.set_needs_redraw()
 
     def set_mt(self, mute_colour):
         """
         Set the colour of mute and deafen logos
         """
-        self.mute_col = mute_colour
-        self.set_needs_redraw()
+        if self.mute_col != mute_colour:
+            self.mute_col = mute_colour
+            self.set_needs_redraw()
 
     def set_mute_bg(self, mute_bg_col):
         """
         Set the background colour for mute/deafen icon
         """
-        self.mute_bg_col = mute_bg_col
-        self.set_needs_redraw()
+        if self.mute_bg_col != mute_bg_col:
+            self.mute_bg_col = mute_bg_col
+            self.set_needs_redraw()
 
     def set_avatar_bg_col(self, avatar_bg_col):
         """
         Set Avatar background colour
         """
-        self.avatar_bg_col = avatar_bg_col
-        self.set_needs_redraw()
+        if self.avatar_bg_col != avatar_bg_col:
+            self.avatar_bg_col = avatar_bg_col
+            self.set_needs_redraw()
 
     def set_hi(self, highlight_colour):
         """
         Set the colour of background for speaking users
         """
-        self.hili_col = highlight_colour
-        self.set_needs_redraw()
+        if self.hili_col != highlight_colour:
+            self.hili_col = highlight_colour
+            self.set_needs_redraw()
 
     def set_fg_hi(self, highlight_colour):
         """
         Set the colour of background for speaking users
         """
-        self.text_hili_col = highlight_colour
-        self.set_needs_redraw()
+        if self.text_hili_col != highlight_colour:
+            self.text_hili_col = highlight_colour
+            self.set_needs_redraw()
 
     def set_bo(self, border_colour):
         """
         Set the colour for idle border
         """
-        self.border_col = border_colour
-        self.set_needs_redraw()
+        if self.border_col != border_colour:
+            self.border_col = border_colour
+            self.set_needs_redraw()
 
     def set_avatar_size(self, size):
         """
         Set the size of the avatar icons
         """
-        self.avatar_size = size
-        self.set_needs_redraw()
+        if self.avatar_size != size:
+            self.avatar_size = size
+            self.set_needs_redraw()
 
     def set_nick_length(self, size):
         """
         Set the length of nickname
         """
-        self.nick_length = size
-        self.set_needs_redraw()
+        if self.nick_length != size:
+            self.nick_length = size
+            self.set_needs_redraw()
 
     def set_icon_spacing(self, i):
         """
         Set the spacing between avatar icons
         """
-        self.icon_spacing = i
-        self.set_needs_redraw()
+        if self.icon_spacing != i:
+            self.icon_spacing = i
+            self.set_needs_redraw()
 
     def set_text_padding(self, i):
         """
         Set padding between text and border
         """
-        self.text_pad = i
-        self.set_needs_redraw()
+        if self.text_pad != i:
+            self.text_pad = i
+            self.set_needs_redraw()
 
     def set_text_baseline_adj(self, i):
         """
         Set padding between text and border
         """
-        self.text_baseline_adj = i
-        self.set_needs_redraw()
+        if self.text_baseline_adj != i:
+            self.text_baseline_adj = i
+            self.set_needs_redraw()
 
     def set_vert_edge_padding(self, i):
         """
         Set padding between top/bottom of screen and overlay contents
         """
-        self.vert_edge_padding = i
-        self.set_needs_redraw()
+        if self.vert_edge_padding != i:
+            self.vert_edge_padding = i
+            self.set_needs_redraw()
 
     def set_horz_edge_padding(self, i):
         """
         Set padding between left/right of screen and overlay contents
         """
-        self.horz_edge_padding = i
-        self.set_needs_redraw()
+        if self.horz_edge_padding != i:
+            self.horz_edge_padding = i
+            self.set_needs_redraw()
 
     def set_square_avatar(self, i):
         """
         Set if the overlay should crop avatars to a circle or show full square image
         """
-        self.round_avatar = not i
-        self.set_needs_redraw()
+        if self.round_avatar == i:
+            self.round_avatar = not i
+            self.set_needs_redraw()
 
     def set_fancy_border(self, border):
         """
         Sets if border should wrap around non-square avatar images
         """
-        self.fancy_border = border
-        self.set_needs_redraw()
+        if self.fancy_border != border:
+            self.fancy_border = border
+            self.set_needs_redraw()
 
     def set_only_speaking(self, only_speaking):
         """
         Set if overlay should only show people who are talking
         """
-        self.only_speaking = only_speaking
+        if self.only_speaking != only_speaking:
+            self.only_speaking = only_speaking
+            self.set_needs_redraw()
 
     def set_only_speaking_grace_period(self, grace_period):
         """
         Set grace period before hiding people who are not talking
         """
         self.only_speaking_grace_period = grace_period
         self.timer_after_draw = grace_period
 
     def set_highlight_self(self, highlight_self):
         """
         Set if the overlay should highlight the user
         """
-        self.highlight_self = highlight_self
+        if self.highlight_self != highlight_self:
+            self.highlight_self = highlight_self
+            self.set_needs_redraw()
 
     def set_order(self, i):
         """
         Set the method used to order avatar icons & names
         """
-        self.order = i
-        self.sort_list(self.userlist)
-        self.set_needs_redraw()
+        if self.order != i:
+            self.order = i
+            self.sort_list(self.userlist)
+            self.set_needs_redraw()
 
     def set_icon_only(self, i):
         """
         Set if the overlay should draw only the icon
         """
-        self.icon_only = i
-        self.set_needs_redraw()
+        if self.icon_only != i:
+            self.icon_only = i
+            self.set_needs_redraw()
 
     def set_border_width(self, width):
-        self.border_width = width
-        self.set_needs_redraw()
+        if self.border_width != width:
+            self.border_width = width
+            self.set_needs_redraw()
 
     def set_horizontal(self, horizontal=False):
-        self.horizontal = horizontal
-        self.set_needs_redraw()
+        if self.horizontal != horizontal:
+            self.horizontal = horizontal
+            self.set_needs_redraw()
 
     def set_guild_ids(self, guild_ids=tuple()):
         if self.discover.connection:
             for _id in guild_ids:
                 if _id not in self.guild_ids:
                     self.discover.connection.req_channels(_id)
         self.guild_ids = guild_ids
@@ -438,15 +472,17 @@
         """
         self.col(self.mute_col)
 
     def set_channel_title(self, channel_title):
         """
         Set title above voice list
         """
-        self.channel_title = channel_title
+        if self.channel_title != channel_title:
+            self.channel_title = channel_title
+            self.set_needs_redraw()
 
     def set_channel_icon(self, url):
         """
         Change the icon for channel
         """
         if not url:
             self.channel_icon = None
@@ -1011,15 +1047,15 @@
         if self.round_avatar:
             context.new_path()
             context.arc(pos_x + (avatar_size / 2), pos_y +
                         (avatar_size / 2), avatar_size / 2, 0, 2 * math.pi)
             context.clip()
         context.set_operator(cairo.OPERATOR_OVER)
         draw_img_to_rect(pixbuf, context, pos_x, pos_y,
-                         avatar_size, avatar_size, False, False, 0,0,self.fade_opacity * self.icon_transparency)
+                         avatar_size, avatar_size, False, False, 0, 0, self.fade_opacity * self.icon_transparency)
         context.restore()
 
     def draw_mute(self, context, pos_x, pos_y, bg_col, avatar_size):
         """
         Draw Mute logo
         """
         if avatar_size <= 0:
@@ -1096,15 +1132,15 @@
         context.save()
         context.translate(pos_x, pos_y)
         context.scale(avatar_size, avatar_size)
 
         # Add a dark background
         context.set_operator(cairo.OPERATOR_ATOP)
         context.rectangle(0.0, 0.0, 1.0, 1.0)
-        self.col(bg_col,None)
+        self.col(bg_col, None)
         context.fill()
         context.set_operator(cairo.OPERATOR_OVER)
 
         self.set_mute_col()
         context.save()
 
         # Clip Strike-through
```

### Comparing `discover-overlay-0.7.2/discover_overlay.egg-info/PKG-INFO` & `discover-overlay-0.7.3/discover_overlay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discover-overlay
-Version: 0.7.2
+Version: 0.7.3
 Summary: Voice chat overlay
 Home-page: https://github.com/trigg/Discover
 Author: trigg
 Author-email: 
 License: GPLv3+
 Keywords: discord overlay voice linux
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,15 @@
 Requires-Dist: PyGObject>=3.22
 Requires-Dist: websocket-client
 Requires-Dist: pyxdg
 Requires-Dist: requests
 Requires-Dist: pillow
 Requires-Dist: python-xlib
 Requires-Dist: setuptools
+Requires-Dist: pulsectl-asyncio
 
 # Discover
 Yet another Discord overlay for Linux written in Python using GTK3.
 
 Discover-Overlay is a GTK3 overlay written in Python3. It can be configured to show who is currently talking on discord or it can be set to display text and images from a preconfigured channel. It is fully customisable and can be configured to display anywhere on the screen. We fully support X11 and wlroots based environments. We felt the need to make this project due to the shortcomings in support on Linux by the official discord client.
 
 Considerably lighter on system resources and less hack-and-slash included than discord-overlay.
```

### Comparing `discover-overlay-0.7.2/discover_overlay.egg-info/SOURCES.txt` & `discover-overlay-0.7.3/discover_overlay.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 discover-overlay.png
 discover-overlay.svg
 discover_overlay.desktop
 discover_overlay_configure.desktop
 setup.py
 discover_overlay/__init__.py
 discover_overlay/__main__.py
+discover_overlay/audio_assist.py
 discover_overlay/autostart.py
 discover_overlay/discord_connector.py
 discover_overlay/discover_overlay.py
 discover_overlay/draggable_window.py
 discover_overlay/draggable_window_wayland.py
 discover_overlay/image_getter.py
 discover_overlay/notification_overlay.py
```

### Comparing `discover-overlay-0.7.2/discover_overlay_configure.desktop` & `discover-overlay-0.7.3/discover_overlay_configure.desktop`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.2/setup.py` & `discover-overlay-0.7.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     return open('README.md', 'r').read()
 
 
 setup(
     name='discover-overlay',
     author='trigg',
     author_email='',
-    version='0.7.2',
+    version='0.7.3',
     description='Voice chat overlay',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/trigg/Discover',
     packages=find_namespace_packages(),
     include_package_data=True,
     data_files=[
@@ -28,15 +28,16 @@
     install_requires=[
         'PyGObject>=3.22',
         'websocket-client',
         'pyxdg',
         'requests',
         'pillow',
         'python-xlib',
-        'setuptools'
+        'setuptools',
+        'pulsectl-asyncio'
     ],
     entry_points={
         'console_scripts': [
             'discover-overlay = discover_overlay.discover_overlay:entrypoint',
         ]
     },
     classifiers=[
```

