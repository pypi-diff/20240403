# Comparing `tmp/discover-overlay-0.7.1.tar.gz` & `tmp/discover-overlay-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discover-overlay-0.7.1.tar", last modified: Tue Mar 19 16:52:24 2024, max compression
+gzip compressed data, was "discover-overlay-0.7.2.tar", last modified: Wed Apr  3 18:39:47 2024, max compression
```

## Comparing `discover-overlay-0.7.1.tar` & `discover-overlay-0.7.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.084771 discover-overlay-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-03-19 16:52:24.084771 discover-overlay-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover-overlay-default.png
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover-overlay-default.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover-overlay-tray.png
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover-overlay-tray.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover-overlay.png
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover-overlay.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.080771 discover-overlay-0.7.1/discover_overlay/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/autostart.py
--rw-r--r--   0 runner    (1001) docker     (127)    29544 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/discord_connector.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22376 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/discover_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/draggable_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/draggable_window_wayland.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.084771 discover-overlay-0.7.1/discover_overlay/glade/
--rw-r--r--   0 runner    (1001) docker     (127)   127962 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/glade/settings.glade
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/image_getter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.076771 discover-overlay-0.7.1/discover_overlay/locales/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.076771 discover-overlay-0.7.1/discover_overlay/locales/cy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.084771 discover-overlay-0.7.1/discover_overlay/locales/cy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/locales/cy/LC_MESSAGES/default.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.076771 discover-overlay-0.7.1/discover_overlay/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.084771 discover-overlay-0.7.1/discover_overlay/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/locales/de/LC_MESSAGES/default.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.076771 discover-overlay-0.7.1/discover_overlay/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.084771 discover-overlay-0.7.1/discover_overlay/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/locales/en/LC_MESSAGES/default.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.076771 discover-overlay-0.7.1/discover_overlay/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.084771 discover-overlay-0.7.1/discover_overlay/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/locales/fr/LC_MESSAGES/default.mo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.076771 discover-overlay-0.7.1/discover_overlay/locales/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.084771 discover-overlay-0.7.1/discover_overlay/locales/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/locales/tr/LC_MESSAGES/default.mo
--rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/notification_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    15597 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    47766 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/settings_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/text_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    39288 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay/voice_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay.desktop
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:52:24.084771 discover-overlay-0.7.1/discover_overlay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-03-19 16:52:24.000000 discover-overlay-0.7.1/discover_overlay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-19 16:52:24.000000 discover-overlay-0.7.1/discover_overlay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 16:52:24.000000 discover-overlay-0.7.1/discover_overlay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-19 16:52:24.000000 discover-overlay-0.7.1/discover_overlay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-19 16:52:24.000000 discover-overlay-0.7.1/discover_overlay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-19 16:52:24.000000 discover-overlay-0.7.1/discover_overlay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/discover_overlay_configure.desktop
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 16:52:24.084771 discover-overlay-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-19 16:52:13.000000 discover-overlay-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover-overlay-default.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover-overlay-default.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover-overlay-tray.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover-overlay-tray.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover-overlay.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover-overlay.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/autostart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29544 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/discord_connector.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22717 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/discover_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/draggable_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/draggable_window_wayland.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay/glade/
+-rw-r--r--   0 runner    (1001) docker     (127)   135215 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/glade/settings.glade
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/image_getter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.011847 discover-overlay-0.7.2/discover_overlay/locales/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.007847 discover-overlay-0.7.2/discover_overlay/locales/cy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay/locales/cy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/locales/cy/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.011847 discover-overlay-0.7.2/discover_overlay/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/locales/de/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.011847 discover-overlay-0.7.2/discover_overlay/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/locales/en/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.011847 discover-overlay-0.7.2/discover_overlay/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     9407 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/locales/fr/LC_MESSAGES/default.mo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.011847 discover-overlay-0.7.2/discover_overlay/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/locales/tr/LC_MESSAGES/default.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/notification_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16056 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48895 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/settings_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13428 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/text_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41720 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay/voice_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay.desktop
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/discover_overlay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7781 2024-04-03 18:39:46.000000 discover-overlay-0.7.2/discover_overlay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-03 18:39:46.000000 discover-overlay-0.7.2/discover_overlay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:39:46.000000 discover-overlay-0.7.2/discover_overlay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 18:39:46.000000 discover-overlay-0.7.2/discover_overlay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 18:39:46.000000 discover-overlay-0.7.2/discover_overlay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 18:39:46.000000 discover-overlay-0.7.2/discover_overlay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/discover_overlay_configure.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:39:47.015847 discover-overlay-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-03 18:39:38.000000 discover-overlay-0.7.2/setup.py
```

### Comparing `discover-overlay-0.7.1/LICENSE` & `discover-overlay-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/PKG-INFO` & `discover-overlay-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discover-overlay
-Version: 0.7.1
+Version: 0.7.2
 Summary: Voice chat overlay
 Home-page: https://github.com/trigg/Discover
 Author: trigg
 Author-email: 
 License: GPLv3+
 Keywords: discord overlay voice linux
 Classifier: Development Status :: 4 - Beta
```

### Comparing `discover-overlay-0.7.1/README.md` & `discover-overlay-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover-overlay-default.png` & `discover-overlay-0.7.2/discover-overlay-default.png`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover-overlay-default.svg` & `discover-overlay-0.7.2/discover-overlay-default.svg`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover-overlay-tray.png` & `discover-overlay-0.7.2/discover-overlay-tray.png`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover-overlay-tray.svg` & `discover-overlay-0.7.2/discover-overlay-tray.svg`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover-overlay.png` & `discover-overlay-0.7.2/discover-overlay.png`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover-overlay.svg` & `discover-overlay-0.7.2/discover-overlay.svg`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover_overlay/__init__.py` & `discover-overlay-0.7.2/discover_overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover_overlay/__main__.py` & `discover-overlay-0.7.2/discover_overlay/__main__.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover_overlay/autostart.py` & `discover-overlay-0.7.2/discover_overlay/autostart.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover_overlay/discord_connector.py` & `discover-overlay-0.7.2/discover_overlay/discord_connector.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover_overlay/discover_overlay.py` & `discover-overlay-0.7.2/discover_overlay/discover_overlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,14 +282,21 @@
             floating, floating_x, floating_y, floating_w, floating_h)
 
         if font:
             self.voice_overlay.set_font(font)
         if title_font:
             self.voice_overlay.set_title_font(title_font)
 
+        self.voice_overlay.set_fade_out_inactive(
+            config.getboolean("main", "fade_out_inactive", fallback=False),
+            config.getint("main", "inactive_time", fallback=10),
+            config.getint("main", "inactive_fade_time", fallback=30),
+            config.getfloat("main", "fade_out_limit", fallback=0.3)
+        )
+
         # Set Text overlay options
         self.text_overlay.set_enabled(config.getboolean(
             "text", "enabled", fallback=False))
         self.text_overlay.set_align_x(config.getboolean(
             "text", "rightalign", fallback=True))
         self.text_overlay.set_align_y(
             config.getint("text", "topalign", fallback=2))
@@ -396,14 +403,15 @@
             config.getboolean("general", "xshape", fallback=False))
 
         hidden = config.getboolean("general", "hideoverlay", fallback=False)
         self.voice_overlay.set_hidden(hidden)
         self.text_overlay.set_hidden(hidden)
         self.notification_overlay.set_hidden(hidden)
 
+
     def parse_guild_ids(self, guild_ids_str):
         """Parse the guild_ids from a str and return them in a list"""
         guild_ids = []
         for guild_id in guild_ids_str.split(","):
             guild_id = guild_id.strip()
             if guild_id != "":
                 guild_ids.append(guild_id)
```

### Comparing `discover-overlay-0.7.1/discover_overlay/draggable_window.py` & `discover-overlay-0.7.2/discover_overlay/draggable_window.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover_overlay/draggable_window_wayland.py` & `discover-overlay-0.7.2/discover_overlay/draggable_window_wayland.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover_overlay/glade/settings.glade` & `discover-overlay-0.7.2/discover_overlay/glade/settings.glade`

 * *Files 0% similar despite different names*

#### Comparing `discover-overlay-0.7.1/discover_overlay/glade/settings.glade` & `discover-overlay-0.7.2/discover_overlay/glade/settings.glade`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- Generated with glade 3.40.0 -->
 <interface>
   <requires lib="gtk+" version="3.24"/>
   <object class="GtkAdjustment" id="ava_opacity_adj">
-    <property name="lower">0.5</property>
+    <property name="lower">0.10</property>
     <property name="upper">1</property>
     <property name="value">0.5</property>
     <property name="step-increment">0.01</property>
     <property name="page-increment">0.10</property>
   </object>
   <object class="GtkAdjustment" id="avatar_size_adj">
     <property name="lower">8</property>
@@ -151,14 +151,33 @@
     <property name="page-increment">10</property>
   </object>
   <object class="GtkAdjustment" id="voice_horizontal_padding_adj">
     <property name="upper">4000</property>
     <property name="step-increment">1</property>
     <property name="page-increment">8</property>
   </object>
+  <object class="GtkAdjustment" id="voice_inactive_fade_opacity">
+    <property name="upper">1</property>
+    <property name="value">0.3</property>
+    <property name="step-increment">0.01</property>
+    <property name="page-increment">0.10</property>
+  </object>
+  <object class="GtkAdjustment" id="voice_inactive_fade_time_range">
+    <property name="lower">1</property>
+    <property name="upper">100</property>
+    <property name="value">1</property>
+    <property name="step-increment">1</property>
+    <property name="page-increment">10</property>
+  </object>
+  <object class="GtkAdjustment" id="voice_inactive_time_range">
+    <property name="lower">1</property>
+    <property name="upper">100</property>
+    <property name="step-increment">1</property>
+    <property name="page-increment">10</property>
+  </object>
   <object class="GtkAdjustment" id="voice_nick_lenght_adj">
     <property name="lower">10</property>
     <property name="upper">32</property>
     <property name="value">32</property>
     <property name="step-increment">1</property>
     <property name="page-increment">10</property>
   </object>
@@ -716,15 +735,15 @@
               </object>
               <packing>
                 <property name="left-attach">1</property>
                 <property name="top-attach">0</property>
               </packing>
             </child>
             <child>
-              <!-- n-columns=6 n-rows=10 -->
+              <!-- n-columns=6 n-rows=13 -->
               <object class="GtkGrid">
                 <property name="name">voice_advanced_grid</property>
                 <property name="visible">True</property>
                 <property name="can-focus">False</property>
                 <property name="row-spacing">1</property>
                 <property name="column-spacing">5</property>
                 <property name="column-homogeneous">True</property>
@@ -1424,18 +1443,156 @@
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
                     <property name="receives-default">True</property>
                     <signal name="pressed" handler="voice_reset_all" swapped="no"/>
                   </object>
                   <packing>
                     <property name="left-attach">5</property>
+                    <property name="top-attach">12</property>
+                  </packing>
+                </child>
+                <child>
+                  <object class="GtkLabel">
+                    <property name="name">voice_inactive_fade_label</property>
+                    <property name="visible">True</property>
+                    <property name="can-focus">False</property>
+                    <property name="label" translatable="yes">Fade out when Inactive</property>
+                    <property name="xalign">0</property>
+                  </object>
+                  <packing>
+                    <property name="left-attach">4</property>
+                    <property name="top-attach">7</property>
+                  </packing>
+                </child>
+                <child>
+                  <object class="GtkLabel">
+                    <property name="name">voice_inactive_opacity_label</property>
+                    <property name="visible">True</property>
+                    <property name="can-focus">False</property>
+                    <property name="label" translatable="yes">Inactive Opacity</property>
+                    <property name="xalign">0</property>
+                  </object>
+                  <packing>
+                    <property name="left-attach">4</property>
+                    <property name="top-attach">8</property>
+                  </packing>
+                </child>
+                <child>
+                  <object class="GtkLabel">
+                    <property name="name">voice_inactive_time_label</property>
+                    <property name="visible">True</property>
+                    <property name="can-focus">False</property>
+                    <property name="label" translatable="yes">Time before Inactive</property>
+                    <property name="xalign">0</property>
+                  </object>
+                  <packing>
+                    <property name="left-attach">4</property>
                     <property name="top-attach">9</property>
                   </packing>
                 </child>
                 <child>
+                  <object class="GtkLabel">
+                    <property name="name">voice_inactive_fade_time_label</property>
+                    <property name="visible">True</property>
+                    <property name="can-focus">False</property>
+                    <property name="label" translatable="yes">Time Fading out</property>
+                    <property name="xalign">0</property>
+                  </object>
+                  <packing>
+                    <property name="left-attach">4</property>
+                    <property name="top-attach">10</property>
+                  </packing>
+                </child>
+                <child>
+                  <object class="GtkCheckButton">
+                    <property name="name">voice_inactive_fade</property>
+                    <property name="visible">True</property>
+                    <property name="can-focus">True</property>
+                    <property name="receives-default">False</property>
+                    <property name="draw-indicator">True</property>
+                    <signal name="toggled" handler="inactive_fade_changed" swapped="no"/>
+                  </object>
+                  <packing>
+                    <property name="left-attach">5</property>
+                    <property name="top-attach">7</property>
+                  </packing>
+                </child>
+                <child>
+                  <object class="GtkScale">
+                    <property name="name">voice_inactive_opacity</property>
+                    <property name="visible">True</property>
+                    <property name="can-focus">True</property>
+                    <property name="adjustment">voice_inactive_fade_opacity</property>
+                    <property name="round-digits">1</property>
+                    <signal name="value-changed" handler="inactive_fade_opacity_changed" swapped="no"/>
+                  </object>
+                  <packing>
+                    <property name="left-attach">5</property>
+                    <property name="top-attach">8</property>
+                  </packing>
+                </child>
+                <child>
+                  <object class="GtkSpinButton">
+                    <property name="name">voice_inactive_time</property>
+                    <property name="visible">True</property>
+                    <property name="can-focus">True</property>
+                    <property name="text">0</property>
+                    <property name="adjustment">voice_inactive_time_range</property>
+                    <signal name="value-changed" handler="inactive_time_changed" swapped="no"/>
+                  </object>
+                  <packing>
+                    <property name="left-attach">5</property>
+                    <property name="top-attach">9</property>
+                  </packing>
+                </child>
+                <child>
+                  <object class="GtkSpinButton">
+                    <property name="name">voice_inactive_fade_time</property>
+                    <property name="visible">True</property>
+                    <property name="can-focus">True</property>
+                    <property name="text">0</property>
+                    <property name="adjustment">voice_inactive_fade_time_range</property>
+                    <signal name="value-changed" handler="inactive_fade_time_changed" swapped="no"/>
+                  </object>
+                  <packing>
+                    <property name="left-attach">5</property>
+                    <property name="top-attach">10</property>
+                  </packing>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
+                  <placeholder/>
+                </child>
+                <child>
                   <placeholder/>
                 </child>
                 <child>
                   <placeholder/>
                 </child>
                 <child>
                   <placeholder/>
```

### Comparing `discover-overlay-0.7.1/discover_overlay/image_getter.py` & `discover-overlay-0.7.2/discover_overlay/image_getter.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,26 +34,26 @@
 
     def __init__(self, func, url, identifier, size):
         self.func = func
         self.identifier = identifier
         self.url = url
         self.size = size
 
-    def get_url(self, alpha):
+    def get_url(self):
         """Downloads and decodes"""
         try:
             resp = requests.get(
                 self.url, stream=True, headers={
                     'Referer': 'https://streamkit.discord.com/overlay/voice',
                     'User-Agent': 'Mozilla/5.0'
                 }
             )
             raw = resp.raw
             image = Image.open(raw)
-            (surface, mask) = from_pil(image, alpha)
+            (surface, mask) = from_pil(image)
 
             self.func(self.identifier, surface, mask)
         except requests.HTTPError:
             log.error("Unable to open %s", self.url)
         except requests.TooManyRedirects:
             log.error("Unable to open %s - Too many redirects", self.url)
         except requests.Timeout:
@@ -63,15 +63,15 @@
         except ValueError:
             log.error("Unable to read %s", self.url)
         except TypeError:
             log.error("Unable to read %s", self.url)
         except PIL.UnidentifiedImageError:
             log.error("Unknown image type:  %s", self.url)
 
-    def get_file(self, alpha):
+    def get_file(self):
         locations = [os.path.expanduser('~/.local/'), '/usr/', '/app']
         for prefix in locations:
             mixpath = os.path.join(prefix, self.url)
             image = None
             try:
                 image = Image.open(mixpath)
             except ValueError:
@@ -79,58 +79,65 @@
             except TypeError:
                 log.error("Type Error - Unable to read %s", mixpath)
             except PIL.UnidentifiedImageError:
                 log.error("Unknown image type: %s", mixpath)
             except FileNotFoundError:
                 log.error("File not found: %s", mixpath)
             if image:
-                (surface, mask) = from_pil(image, alpha)
+                (surface, mask) = from_pil(image)
                 if surface:
                     self.func(self.identifier, surface, mask)
                     return
 
 
-def from_pil(image, alpha):
+def from_pil(image, alpha=1.0, format='BGRa'):
     """
     :param im: Pillow Image
     :param alpha: 0..1 alpha to add to non-alpha images
     :param format: Pixel format for output surface
     """
     arr = bytearray()
     mask = bytearray()
     if 'A' not in image.getbands():
         image.putalpha(int(alpha * 255.0))
-        arr = bytearray(image.tobytes('raw', 'BGRa'))
+        arr = bytearray(image.tobytes('raw', format))
         mask = arr
     else:
-        arr = bytearray(image.tobytes('raw', 'BGRa'))
+        arr = bytearray(image.tobytes('raw', format))
         mask = copy.deepcopy((arr))
-        idx = 3
+        idx = 0
         while idx < len(arr):
             if arr[idx] > 0:
                 mask[idx] = 255
             else:
                 mask[idx] = 0
+            # Cairo expects the raw data to be pre-multiplied alpha
+            # This means when we change the alpha level we need to change the RGB channels equally
             arr[idx] = int(arr[idx] * alpha)
-            idx += 4
+            idx +=1
     surface = cairo.ImageSurface.create_for_data(
         arr, cairo.FORMAT_ARGB32, image.width, image.height)
     mask = cairo.ImageSurface.create_for_data(
         mask, cairo.FORMAT_ARGB32, image.width, image.height)
     return (surface, mask)
 
 
-def get_surface(func, identifier, ava, size, alpha=1.0):
+def to_pil(surface):
+    if surface.get_format() == cairo.Format.ARGB32:
+        return Image.frombuffer('RGBA', (surface.get_width(), surface.get_height()), surface.get_data(),'raw',"BGRA",surface.get_stride())
+    return Image.frombuffer("RGB", (surface.get_width(), surface.get_height()), surface.get_data(),'raw', "BGRX", stride)
+
+def get_surface(func, identifier, ava, size):
     """Download to cairo surface"""
     image_getter = SurfaceGetter(func, identifier, ava, size)
     if identifier.startswith('http'):
-        thread = threading.Thread(target=image_getter.get_url, args=[alpha])
+        thread = threading.Thread(target=image_getter.get_url)
         thread.start()
     else:
-        thread = threading.Thread(target=image_getter.get_file, args=[alpha])
+        thread = threading.Thread(target=image_getter.get_file)
         thread.start()
 
 
 def get_aspected_size(img, width, height, anchor=0, hanchor=0):
     """Get dimensions of image keeping current aspect ratio"""
     pic_width = img.get_width()
     pic_height = img.get_height()
@@ -153,20 +160,19 @@
         width = height * img_aspect
         if hanchor == 2:
             offset_x = offset_x + (old_width - width)
         if hanchor == 1:
             offset_x = offset_x + ((old_width - width) / 2)
     return (offset_x, offset_y, width, height)
 
-
 def draw_img_to_rect(img, ctx,
                      pos_x, pos_y,
                      width, height,
                      path=False, aspect=False,
-                     anchor=0, hanchor=0):
+                     anchor=0, hanchor=0, alpha=1.0):
     """Draw cairo surface onto context
 
     Path - only add the path do not fill : True/False
     Aspect - keep aspect ratio : True/False
     Anchor - with aspect : 0=left 1=middle 2=right
     HAnchor - with apect : 0=bottom 1=middle 2=top
     """
@@ -177,23 +183,36 @@
     if aspect:
         (offset_x, offset_y, width, height) = get_aspected_size(
             img, width, height, anchor=anchor, hanchor=hanchor)
 
     ctx.translate(pos_x + offset_x, pos_y + offset_y)
     ctx.scale(width, height)
     ctx.scale(1 / img.get_width(), 1 / img.get_height())
-    ctx.set_source_surface(img, 0, 0)
+    
+    if alpha != 1.0:
+        # Honestly, couldn't find a 'use-image-with-modifier' option
+        # Tried RasterSourcePattern but it appears... broken? in the python implementation
+        # Or just lacking documentation.
+
+        # Pass raw data to PIL and then back with an alpha modifier
+        ctx.set_source_surface(
+            from_pil(
+                to_pil(img),
+                alpha
+            )[0],
+            0,0)
+    else:
+        ctx.set_source_surface(img, 0, 0)
 
     ctx.rectangle(0, 0, img.get_width(), img.get_height())
     if not path:
         ctx.fill()
     ctx.restore()
     return (width, height)
 
-
 def draw_img_to_mask(img, ctx,
                      pos_x, pos_y,
                      width, height,
                      path=False, aspect=False,
                      anchor=0, hanchor=0):
     """Draw cairo surface as mask into context
```

### Comparing `discover-overlay-0.7.1/discover_overlay/locales/cy/LC_MESSAGES/default.mo` & `discover-overlay-0.7.2/discover_overlay/locales/cy/LC_MESSAGES/default.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -91,14 +91,17 @@
 
 msgid "Display Speakers Only"
 msgstr "Dangos siaradwyr yn unig"
 
 msgid "Enable"
 msgstr "Galluogi"
 
+msgid "Fade out when Inactive"
+msgstr "Diffoddwch pan yn anweithgar"
+
 msgid "Fancy Avatar Shapes"
 msgstr "Siâp avatar ffansi"
 
 msgid "Floating"
 msgstr "Symudol"
 
 msgid "Font"
@@ -146,14 +149,17 @@
 msgid ""
 "If tray icon is enabled, start with only tray icon and no configuration "
 "window"
 msgstr ""
 "If tray icon is enabled, start with only tray icon and no configuration "
 "window"
 
+msgid "Inactive Opacity"
+msgstr "Anweithgar Gormes"
+
 msgid "Last Spoken"
 msgstr "Siaradwyd ddiwethaf"
 
 msgid "Left"
 msgstr "Chwith"
 
 msgid "Limit Popup Width"
@@ -335,14 +341,20 @@
 
 msgid "Text Padding"
 msgstr "Padio testun"
 
 msgid "Text Vertical Offset"
 msgstr "Gwrthbwysiad fertigol testun"
 
+msgid "Time Fading out"
+msgstr "Amser yn pylu"
+
+msgid "Time before Inactive"
+msgstr "Amser cyn anweithgar"
+
 msgid "Title Font"
 msgstr "Ffont teitl"
 
 msgid "Top"
 msgstr "Brig"
 
 msgid "Unknown"
```

### Comparing `discover-overlay-0.7.1/discover_overlay/locales/de/LC_MESSAGES/default.mo` & `discover-overlay-0.7.2/discover_overlay/locales/de/LC_MESSAGES/default.mo`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover_overlay/locales/fr/LC_MESSAGES/default.mo` & `discover-overlay-0.7.2/discover_overlay/locales/fr/LC_MESSAGES/default.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,23 +1,21 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: \n"
+"Project-Id-Version: discover 0.7.2\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2024-02-23 14:05+0100\n"
+"PO-Revision-Date: 2024-03-23 00:10+0100\n"
 "Last-Translator: Noé Lopez <noelopez@free.fr>\n"
-"Language-Team: English <kde-i18n-doc@kde.org>\n"
-"Language: en_US\n"
+"Language-Team: Noé Lopez <noelopez@free.fr>\n"
+"Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Lokalize 23.04.0\n"
 
 msgid " for support. Or open an issue on our GitHub "
-msgstr "pour avoir de l'aide ou ouvrez une issue sur notre GitHub"
+msgstr "pour avoir de l’aide ou ouvrez une issue sur notre GitHub"
 
 msgid "1"
 msgstr "1"
 
 msgid "AUTHENTICATING"
 msgstr "AUTHENTICATING"
 
@@ -39,15 +37,15 @@
 msgid "Avatar Size"
 msgstr "Taille des avatars"
 
 msgid "Background"
 msgstr "Arrière-plan"
 
 msgid "Background Colour"
-msgstr "Couleur de l'arrière-plan"
+msgstr "Couleur de l’arrière-plan"
 
 msgid "Border"
 msgstr "Bordure"
 
 msgid "Border Radius"
 msgstr "Arrondissement des bordures"
 
@@ -63,24 +61,24 @@
 msgid "CONNECTING"
 msgstr "CONNECTING"
 
 msgid "Channel"
 msgstr "Salon"
 
 msgid "Close Overlay"
-msgstr "Fermer l'overlay"
+msgstr "Fermer l’overlay"
 
 msgid "Close Settings"
 msgstr "Ouvrir les paramètres"
 
 msgid "Close currently running instance"
 msgstr "Fermer une instance ouverte"
 
 msgid "Close overlay"
-msgstr "Fermer l'overlay"
+msgstr "Fermer l’overlay"
 
 msgid "Core"
 msgstr "Noyau"
 
 msgid "DISCONNECTED"
 msgstr "DISCONNECTED"
 
@@ -93,91 +91,97 @@
 "and images from a preconfigured channel. It is fully customisable and can be "
 "configured to display anywhere on the screen. We fully support X11 and "
 "wlroots based environments. We felt the need to make this project due to the "
 "shortcomings in support on Linux by the official discord client."
 msgstr ""
 "Discover Overlay est un overlay GTK3 écris en Python3. Il peut être "
 "configuré pour afficher qui est en train de parler sur discord, ou pour "
-"afficher texte et images provenant d'un salon sélectionné. Il est "
-"complètement personnalisable et peut être configuré pour afficher n'importe "
+"afficher texte et images provenant d’un salon sélectionné. Il est "
+"complètement personnalisable et peut être configuré pour afficher n’importe "
 "où sur votre écran. Nous ressentions le besoin de créer ce projet à cause du "
 "manque de support du client officiel sur Linux."
 
 msgid "Display Horizontally"
 msgstr "Afficher horizontalement"
 
 msgid "Display Speakers Only"
 msgstr "Afficher seulement les parleurs"
 
 msgid "Enable"
 msgstr "Activer"
 
+msgid "Fade out when Inactive"
+msgstr "Cacher progressivement à l’inactivité"
+
 msgid "Fancy Avatar Shapes"
-msgstr "Formes d'avatar chic"
+msgstr "Formes d’avatar chic"
 
 msgid "Floating"
 msgstr "Flottant"
 
 msgid "Font"
 msgstr "Police"
 
 msgid "For gamescope compatibility ensure ENV has 'GDK_BACKEND=x11'"
 msgstr ""
-"Pour la compatibilité avec gamescope, assurez vous d'avoir la variable "
-"d'environnement « GDK_BACKEND=x11 »"
+"Pour la compatibilité avec gamescope, assurez vous d’avoir défini la "
+"variable d’environnement « GDK_BACKEND=x11 »"
 
 msgid "Force XShape"
 msgstr "Forcer la XShape"
 
 msgid "Foreground"
 msgstr "Texte"
 
 msgid "Hide Overlay on Mouseover"
-msgstr "Cacher l'overlay au survolement de la souris"
+msgstr "Cacher l’overlay au survolement de la souris"
 
 msgid "Hide Overlays"
 msgstr "Cacher les overlays"
 
 msgid "Hide overlay"
-msgstr "Cacher l'overlay"
+msgstr "Cacher l’overlay"
 
 msgid "Highlight Self"
 msgstr "Surbrillance de soi-même"
 
 msgid "Horizontal Edge Padding"
 msgstr "Écart horizontal avec le bord"
 
 msgid "ICE_CHECKING"
 msgstr "ICE_CHECKING"
 
 msgid "ID"
 msgstr "ID"
 
 msgid "INTRO TEXT"
-msgstr "TEXT D'INTRO"
+msgstr "TEXT D’INTRO"
 
 msgid "Icon Padding"
 msgstr "Espace entre icônes"
 
 msgid "Icon Position"
-msgstr "Position de l'icône"
+msgstr "Position de l’icône"
 
 msgid "Icon Size"
 msgstr "Taille des icônes"
 
 msgid "Idle"
 msgstr "Silencieux"
 
 msgid ""
 "If tray icon is enabled, start with only tray icon and no configuration "
 "window"
 msgstr ""
-"Si le raccourci de la barre d'outils est activé, démarrer seulement avec le "
+"Si le raccourci de la barre d’outils est activé, démarrer seulement avec le "
 "raccourci et sans fenêtre de configuration"
 
+msgid "Inactive Opacity"
+msgstr "Opacité à l’inactivité"
+
 msgid "Last Spoken"
 msgstr "Dernier à avoir parlé"
 
 msgid "Left"
 msgstr "Gauche"
 
 msgid "Limit Popup Width"
@@ -213,15 +217,15 @@
 msgid "Order Users By"
 msgstr "Ordre des utilisateurs"
 
 msgid "Overflow Style"
 msgstr "Style de débordement"
 
 msgid "Overlay Location"
-msgstr "Position de l'overlay"
+msgstr "Position de l’overlay"
 
 msgid "Overview"
 msgstr "Aperçu"
 
 msgid "Padding Between Notifications"
 msgstr "Espace entre notifications"
 
@@ -234,15 +238,15 @@
 msgid "Place & resize this window then press Save!"
 msgstr "Bougez & redimensionnez cette fenêtre puis appuyez sur Sauvegarder!"
 
 msgid "Place Window"
 msgstr "Choisir la position de la fenêtre"
 
 msgid "Please visit our discord"
-msgstr "N'hésitez pas à visiter notre discord"
+msgstr "N’hésitez pas à visiter notre discord"
 
 msgid "Popup Style"
 msgstr "Habiller le popup"
 
 msgid "Popup Timer"
 msgstr "Limite de temps du popup"
 
@@ -270,15 +274,15 @@
 msgid "Right"
 msgstr "Droite"
 
 msgid "Run Configuration on Startup"
 msgstr "Afficher la configuration au démarage"
 
 msgid "Run Overlay on Startup"
-msgstr "Afficher l'overlay au démarrage"
+msgstr "Afficher l’overlay au démarrage"
 
 msgid "Save this position"
 msgstr "Sauvegarder cette position"
 
 msgid "Send command, not start new instance."
 msgstr "Envoyer une commande, sans démarrer une nouvelle instance."
 
@@ -303,42 +307,42 @@
 msgid "Show Attachments"
 msgstr "Afficher les pièce jointes"
 
 msgid "Show Avatar"
 msgstr "Afficher les avatars"
 
 msgid "Show Connection Status"
-msgstr "Afficher l'état de la connection"
+msgstr "Afficher l’état de la connection"
 
 msgid "Show Icon"
-msgstr "Afficher l'icône"
+msgstr "Afficher l’icône"
 
 msgid "Show Names"
 msgstr "Afficher les noms"
 
 msgid "Show Test Content"
 msgstr "Afficher le contenu de test"
 
 msgid "Show Title"
 msgstr "Afficher le titre"
 
 msgid "Show Tray Icon"
-msgstr "Afficher le raccourci de la barre d'outils"
+msgstr "Afficher le raccourci de la barre d’outils"
 
 msgid "Show While Disconnected"
 msgstr "Afficher quand déconnecté"
 
 msgid "Show again after (seconds)"
 msgstr "Afficher de nouveau après (secondes)"
 
 msgid "Show an X11 or wlroots overlay with information"
 msgstr "Affiche un overlay X11 ou wlroots avec des informations"
 
 msgid "Show overlay"
-msgstr "Afficher l'overlay"
+msgstr "Afficher l’overlay"
 
 msgid "Shrink"
 msgstr "Rétrécir"
 
 msgid "Speakers Grace Period"
 msgstr "Période de grâce des parleurs"
 
@@ -365,14 +369,20 @@
 
 msgid "Text Vertical Offset"
 msgstr "Décalage vertical du texte"
 
 msgid "This screen"
 msgstr "Cet écran"
 
+msgid "Time Fading out"
+msgstr "Durée du fondu"
+
+msgid "Time before Inactive"
+msgstr "Temps avant l’inactivité"
+
 msgid "Title Font"
 msgstr "Police du titre"
 
 msgid "Top"
 msgstr "Haut"
 
 msgid "Unknown"
```

### Comparing `discover-overlay-0.7.1/discover_overlay/locales/tr/LC_MESSAGES/default.mo` & `discover-overlay-0.7.2/discover_overlay/locales/tr/LC_MESSAGES/default.mo`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover_overlay/notification_overlay.py` & `discover-overlay-0.7.2/discover_overlay/notification_overlay.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover_overlay/overlay.py` & `discover-overlay-0.7.2/discover_overlay/overlay.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,16 @@
         if "Wayland" in screen_type:
             self.is_wayland = True
             return Gtk.WindowType.TOPLEVEL
         return Gtk.WindowType.POPUP
 
     def __init__(self, discover, piggyback=None):
         Gtk.Window.__init__(self, type=self.detect_type())
+        self.is_xatom_set=False
+
         self.discover = discover
         screen = self.get_screen()
         self.text_font = None
         self.text_size = None
         self.pos_x = None
         self.pos_y = None
         self.width = None
@@ -107,23 +109,34 @@
         self.timer_after_draw = None
         if piggyback:
             self.set_piggyback(piggyback)
 
         self.get_screen().connect("composited-changed", self.check_composite)
         self.get_screen().connect("monitors-changed", self.screen_changed)
         self.get_screen().connect("size-changed", self.screen_changed)
-        self.get_window().set_events(self.get_window().get_events() | Gdk.EventMask.ENTER_NOTIFY_MASK)
+        if self.get_window():
+            self.get_window().set_events(self.get_window().get_events() | Gdk.EventMask.ENTER_NOTIFY_MASK)
         self.connect("enter-notify-event", self.mouseover)
         self.connect("leave-notify-event", self.mouseout)
         self.mouse_over_timer = None
-        
+
+        # It shouldn't be possible, but let's not leave
+        # this process hanging if it happens
+        self.connect('destroy', self.window_exited)
+
+    def window_exited(self, window=None):
+        sys.exit(1)
 
     def set_gamescope_xatom(self, enabled):
         if self.piggyback_parent:
             return
+
+        if enabled == self.is_xatom_set:
+            return
+        self.is_xatom_set = enabled
         display = Display()
         atom = display.intern_atom("GAMESCOPE_EXTERNAL_OVERLAY")
         opaq = display.intern_atom("_NET_WM_WINDOW_OPACITY")
 
         if self.get_toplevel().get_window():
             topw = display.create_resource_object(
                 "window", self.get_toplevel().get_window().get_xid())
@@ -244,32 +257,34 @@
     def set_mouseover_timer(self, time):
         self.timeout_mouse_over = time
 
     def unset_shape(self):
         """
         Remove XShape (not input shape)
         """
-        self.get_window().shape_combine_region(None, 0, 0)
+        if self.get_window():
+            self.get_window().shape_combine_region(None, 0, 0)
 
     def force_location(self):
         """
         On X11 enforce the location and sane defaults
         On Wayland just store for later
         On Gamescope enforce size of display but only if it's the primary overlay
         """
         if self.discover.steamos and not self.piggyback_parent:
             display = Gdk.Display.get_default()
             if "get_monitor" in dir(display):
                 monitor = display.get_monitor(self.monitor)
-                geometry = monitor.get_geometry()
-                scale_factor = monitor.get_scale_factor()
-                width = geometry.width
-                height = geometry.height
-                self.resize(width, height)
-                self.set_needs_redraw()
+                if monitor:
+                    geometry = monitor.get_geometry()
+                    scale_factor = monitor.get_scale_factor()
+                    width = geometry.width
+                    height = geometry.height
+                    self.resize(width, height)
+                    self.set_needs_redraw()
                 return
         if not self.is_wayland:
             self.set_decorated(False)
             self.set_keep_above(True)
             display = Gdk.Display.get_default()
             if "get_monitor" in dir(display):
                 monitor = display.get_monitor(self.monitor)
@@ -296,15 +311,15 @@
             self.width = width
             self.height = height
         self.set_needs_redraw()
 
     def set_needs_redraw(self):
         if not self.hidden and self.enabled:
             if self.piggyback_parent:
-                self.piggyback_parent.set_need_redraw()
+                self.piggyback_parent.set_needs_redraw()
 
             if self.redraw_id == None:
                 self.redraw_id = GLib.idle_add(self.redraw)
             else:
                 log.debug("Already awaiting paint")
 
             # If this overlay has data that expires after draw, plan for that here
```

### Comparing `discover-overlay-0.7.1/discover_overlay/settings_window.py` & `discover-overlay-0.7.2/discover_overlay/settings_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,14 +405,27 @@
 
         self.widget['voice_show_disconnected'].set_active(config.getboolean(
             "main", "show_disconnected", fallback=False))
 
         self.widget['voice_dummy_count'].set_value(
             config.getint("main", "dummy_count", fallback=50))
 
+        self.widget['voice_inactive_fade'].set_active(
+            config.getboolean("main", "fade_out_inactive", fallback=False)
+        )
+        self.widget['voice_inactive_opacity'].set_value(
+            config.getfloat("main", "fade_out_limit", fallback=0.3)
+        )
+        self.widget['voice_inactive_time'].set_value(
+            config.getint("main", "inactive_time", fallback=10)
+        )
+        self.widget['voice_inactive_fade_time'].set_value(
+            config.getint("main", "inactive_fade_time", fallback=30)
+        )
+
         # Read Text section
 
         self.text_floating_x = config.getint("text", "floating_x", fallback=0)
         self.text_floating_y = config.getint("text", "floating_y", fallback=0)
         self.text_floating_w = config.getint(
             "text", "floating_w", fallback=400)
         self.text_floating_h = config.getint(
@@ -1146,8 +1159,23 @@
 
     def voice_mouseover_timeout_changed(self, button):
         self.config_set("main", "autohide_timer", "%s" %
                         (int(button.get_value())))
 
     def text_mouseover_timeout_changed(self, button):
         self.config_set("text", "autohide_timer", "%s" %
-                        (int(button.get_value())))
+                        (int(button.get_value())))
+
+    def inactive_fade_changed(self, button):
+        self.config_set("main", "fade_out_inactive", "%s" % (button.get_active()))
+
+    def inactive_fade_opacity_changed(self, button):
+        self.config_set("main", "fade_out_limit", "%.2f" %
+                        (button.get_value()))
+
+    def inactive_time_changed(self, button):
+        self.config_set("main", "inactive_time", "%s" %
+                (int(button.get_value())))
+
+    def inactive_fade_time_changed(self,button):
+        self.config_set("main", "inactive_fade_time", "%s" %
+                (int(button.get_value())))
```

### Comparing `discover-overlay-0.7.1/discover_overlay/text_overlay.py` & `discover-overlay-0.7.2/discover_overlay/text_overlay.py`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover_overlay/voice_overlay.py` & `discover-overlay-0.7.2/discover_overlay/voice_overlay.py`

 * *Files 10% similar despite different names*

```diff
@@ -92,14 +92,24 @@
         self.show_connection = True
         self.show_disconnected = True
         self.channel_title = ""
         self.border_width = 2
         self.icon_transparency = 0.0
         self.fancy_border = False
 
+        self.fade_out_inactive = True
+        self.fade_out_limit = 0.1
+        self.inactive_time = 10 # Seconds
+        self.inactive_fade_time = 20 # Seconds
+        self.fade_opacity = 1.0
+        self.fade_start = 0
+
+        self.inactive_timeout = None
+        self.fadeout_timeout = None
+
         self.round_avatar = True
         self.icon_only = True
         self.talk_col = [0.0, 0.6, 0.0, 0.1]
         self.text_col = [1.0, 1.0, 1.0, 1.0]
         self.text_hili_col = [1.0, 1.0, 1.0, 1.0]
         self.norm_col = [0.0, 0.0, 0.0, 0.5]
         self.wind_col = [0.0, 0.0, 0.0, 0.0]
@@ -111,42 +121,90 @@
         self.userlist = []
         self.connection_status = "DISCONNECTED"
         self.horizontal = False
         self.guild_ids = tuple()
         self.force_location()
         get_surface(self.recv_avatar,
                     "share/icons/hicolor/256x256/apps/discover-overlay-default.png",
-                    'def', self.avatar_size, self.icon_transparency)
+                    'def', self.avatar_size)
         self.set_title("Discover Voice")
         self.redraw()
 
+    def reset_action_timer(self):
+        self.fade_opacity = 1.0
+        if self.inactive_timeout:
+            GLib.source_remove(self.inactive_timeout)
+            self.inactive_timeout = None
+        if self.fadeout_timeout:
+            GLib.source_remove(self.fadeout_timeout)
+            self.fadeout_timeout = None
+
+        if self.fade_out_inactive:
+            self.inactive_timeout = GLib.timeout_add_seconds(self.inactive_time, self.overlay_inactive)
+
+    def overlay_inactive(self):
+        self.fade_start= perf_counter()
+        self.fadeout_timeout = GLib.timeout_add(self.inactive_fade_time/200 * 1000, self.overlay_fadeout)
+        self.inactive_timeout = None
+        return False
+
+    def overlay_fadeout(self):
+        self.set_needs_redraw()
+        now = perf_counter()
+        time_percent = (now - self.fade_start) / self.inactive_fade_time
+        if time_percent>=1.0:
+            self.fade_opacity = self.fade_out_limit
+            self.fadeout_timeout = None
+            return False
+
+        self.fade_opacity = self.fade_out_limit + ((1.0 - self.fade_out_limit) * (1.0 - time_percent))
+        return True
+
+    def col(self, col, alpha=1.0):
+        """
+        Convenience function to set the cairo context next colour. Altered to account for fade-out function
+        """
+        if alpha == None:
+            self.context.set_source_rgba(col[0], col[1], col[2], col[3])
+        else:
+            self.context.set_source_rgba(col[0], col[1], col[2], col[3] * alpha * self.fade_opacity)
+
     def set_icon_transparency(self, trans):
         if self.icon_transparency == trans:
             return
         self.icon_transparency = trans
-        get_surface(self.recv_avatar,
-                    "share/icons/hicolor/256x256/apps/discover-overlay-default.png",
-                    'def', self.avatar_size, self.icon_transparency)
+        #get_surface(self.recv_avatar,
+        #            "share/icons/hicolor/256x256/apps/discover-overlay-default.png",
+        #            'def', self.avatar_size)
 
-        self.avatars = {}
-        self.avatar_masks = {}
+        #self.avatars = {}
+        #self.avatar_masks = {}
 
-        self.channel_icon = None
-        self.channel_mask = None
+        #self.channel_icon = None
+        #self.channel_mask = None
 
         self.set_needs_redraw()
 
     def set_blank(self):
         self.userlist = []
         self.channel_icon = None
         self.channel_icon_url = None
         self.channel_title = None
         self.connection_status = "DISCONNECTED"
         self.set_needs_redraw()
 
+    def set_fade_out_inactive(self, enabled, fade_time, fade_duration, fade_to):
+        if self.fade_out_inactive == enabled and self.inactive_time == fade_time and self.inactive_fade_time == fade_duration and self.fade_out_limit == fade_to:
+            return
+        self.fade_out_inactive = enabled
+        self.inactive_time = fade_time
+        self.inactive_fade_time = fade_duration
+        self.fade_out_limit = fade_to
+        self.reset_action_timer()
+
     def set_title_font(self, font):
         self.title_font = font
         self.set_needs_redraw()
 
     def set_show_connection(self, show_connection):
         self.show_connection = show_connection
         self.set_needs_redraw()
@@ -356,33 +414,33 @@
                     self.discover.connection.req_channels(_id)
         self.guild_ids = guild_ids
 
     def set_wind_col(self):
         """
         Use window colour to draw
         """
-        self.col(self.wind_col)
+        self.col(self.wind_col, None)
 
     def set_norm_col(self):
         """
         Use background colour to draw
         """
         self.col(self.norm_col)
 
     def set_talk_col(self, alpha=1.0):
         """
         Use talking colour to draw
         """
         self.col(self.talk_col, alpha)
 
-    def set_mute_col(self, alpha=1.0):
+    def set_mute_col(self):
         """
         Use mute colour to draw
         """
-        self.col(self.mute_col, alpha)
+        self.col(self.mute_col)
 
     def set_channel_title(self, channel_title):
         """
         Set title above voice list
         """
         self.channel_title = channel_title
 
@@ -391,29 +449,30 @@
         Change the icon for channel
         """
         if not url:
             self.channel_icon = None
             self.channel_icon_url = None
         else:
             get_surface(self.recv_avatar, url, "channel",
-                        self.avatar_size, self.icon_transparency)
+                        self.avatar_size)
             self.channel_icon_url = url
 
     def set_user_list(self, userlist, alt):
         """
         Set the users in list to draw
         """
         self.userlist = userlist
         for user in userlist:
             if "nick" in user:
                 user["friendlyname"] = user["nick"]
             else:
                 user["friendlyname"] = user["username"]
         self.sort_list(self.userlist)
         if alt:
+            self.reset_action_timer()
             self.set_needs_redraw()
 
     def set_connection_status(self, connection):
         """
         Set if discord has a clean connection to server
         """
         if self.connection_status != connection['state']:
@@ -443,14 +502,15 @@
         """
         Draw the Overlay
         """
         self.context = context
         context.set_antialias(cairo.ANTIALIAS_GOOD)
         # Get size of window
         (width, height) = self.get_size()
+
         # Make background transparent
         self.set_wind_col()
         # Don't layer drawing over each other, always replace
         context.set_operator(cairo.OPERATOR_SOURCE)
         context.paint()
         context.save()
         if self.piggyback:
@@ -704,18 +764,23 @@
         if self.channel_icon:
             self.draw_avatar_pix(context, self.channel_icon, self.channel_mask,
                                  pos_x, pos_y, None, avatar_size)
         else:
             self.blank_avatar(context, pos_x, pos_y, avatar_size)
             if self.channel_icon_url:
                 get_surface(self.recv_avatar, self.channel_icon_url, "channel",
-                            self.avatar_size, self.icon_transparency)
+                            self.avatar_size)
         return tw
 
     def unused_fn_needed_translations(self):
+        """
+        These are here to force them to be picked up for translations
+
+        They're fed right through from Discord client as string literals
+        """
         _("DISCONNECTED")
         _("NO_ROUTE")
         _("VOICE_DISCONNECTED")
         _("ICE_CHECKING")
         _("AWAITING_ENDPOINT")
         _("AUTHENTICATING")
         _("CONNECTING")
@@ -748,15 +813,15 @@
         Draw avatar at given Y position. Includes both text and image based on settings
         """
         # Ensure pixbuf for avatar
         if user["id"] not in self.avatars and user["avatar"] and avatar_size > 0:
             url = "https://cdn.discordapp.com/avatars/%s/%s.png" % (
                 user['id'], user['avatar'])
             get_surface(self.recv_avatar, url, user["id"],
-                        self.avatar_size, self.icon_transparency)
+                        self.avatar_size)
 
             # Set the key with no value to avoid spamming requests
             self.avatars[user["id"]] = None
             self.avatar_masks[user["id"]] = None
 
         colour = None
         mute = False
@@ -946,15 +1011,15 @@
         if self.round_avatar:
             context.new_path()
             context.arc(pos_x + (avatar_size / 2), pos_y +
                         (avatar_size / 2), avatar_size / 2, 0, 2 * math.pi)
             context.clip()
         context.set_operator(cairo.OPERATOR_OVER)
         draw_img_to_rect(pixbuf, context, pos_x, pos_y,
-                         avatar_size, avatar_size)
+                         avatar_size, avatar_size, False, False, 0,0,self.fade_opacity * self.icon_transparency)
         context.restore()
 
     def draw_mute(self, context, pos_x, pos_y, bg_col, avatar_size):
         """
         Draw Mute logo
         """
         if avatar_size <= 0:
@@ -962,15 +1027,15 @@
         context.save()
         context.translate(pos_x, pos_y)
         context.scale(avatar_size, avatar_size)
 
         # Add a dark background
         context.set_operator(cairo.OPERATOR_ATOP)
         context.rectangle(0.0, 0.0, 1.0, 1.0)
-        self.col(bg_col)
+        self.col(bg_col, None)
         context.fill()
         context.set_operator(cairo.OPERATOR_OVER)
 
         self.set_mute_col()
         context.save()
 
         # Clip Strike-through
@@ -1031,15 +1096,15 @@
         context.save()
         context.translate(pos_x, pos_y)
         context.scale(avatar_size, avatar_size)
 
         # Add a dark background
         context.set_operator(cairo.OPERATOR_ATOP)
         context.rectangle(0.0, 0.0, 1.0, 1.0)
-        self.col(bg_col)
+        self.col(bg_col,None)
         context.fill()
         context.set_operator(cairo.OPERATOR_OVER)
 
         self.set_mute_col()
         context.save()
 
         # Clip Strike-through
```

### Comparing `discover-overlay-0.7.1/discover_overlay.egg-info/PKG-INFO` & `discover-overlay-0.7.2/discover_overlay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discover-overlay
-Version: 0.7.1
+Version: 0.7.2
 Summary: Voice chat overlay
 Home-page: https://github.com/trigg/Discover
 Author: trigg
 Author-email: 
 License: GPLv3+
 Keywords: discord overlay voice linux
 Classifier: Development Status :: 4 - Beta
```

### Comparing `discover-overlay-0.7.1/discover_overlay.egg-info/SOURCES.txt` & `discover-overlay-0.7.2/discover_overlay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/discover_overlay_configure.desktop` & `discover-overlay-0.7.2/discover_overlay_configure.desktop`

 * *Files identical despite different names*

### Comparing `discover-overlay-0.7.1/setup.py` & `discover-overlay-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     return open('README.md', 'r').read()
 
 
 setup(
     name='discover-overlay',
     author='trigg',
     author_email='',
-    version='0.7.1',
+    version='0.7.2',
     description='Voice chat overlay',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/trigg/Discover',
     packages=find_namespace_packages(),
     include_package_data=True,
     data_files=[
```

