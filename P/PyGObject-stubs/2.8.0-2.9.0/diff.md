# Comparing `tmp/PyGObject-stubs-2.8.0.tar.gz` & `tmp/PyGObject-stubs-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGObject-stubs-2.8.0.tar", last modified: Sun May 28 21:40:07 2023, max compression
+gzip compressed data, was "PyGObject-stubs-2.9.0.tar", last modified: Thu Sep 14 20:57:23 2023, max compression
```

## Comparing `PyGObject-stubs-2.8.0.tar` & `PyGObject-stubs-2.9.0.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:40:07.980974 PyGObject-stubs-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-28 21:40:07.976974 PyGObject-stubs-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:40:07.968974 PyGObject-stubs-2.8.0/pep517backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/pep517backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/pep517backend/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 21:40:07.980974 PyGObject-stubs-2.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:40:07.968974 PyGObject-stubs-2.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:40:07.972974 PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-28 21:40:07.000000 PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-28 21:40:07.000000 PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:40:07.000000 PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-28 21:40:07.000000 PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-28 21:40:07.000000 PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:40:07.972974 PyGObject-stubs-2.8.0/src/gi-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:40:07.976974 PyGObject-stubs-2.8.0/src/gi-stubs/repository/
--rw-r--r--   0 runner    (1001) docker     (123)   284195 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Adw.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/AppIndicator3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    47065 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Atk.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/AyatanaAppIndicator3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Farstream.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/GIRepository.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   129078 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/GLib.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/GModule.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    75309 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/GObject.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/GSound.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15989 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/GdkPixbuf.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20001 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Geoclue.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    63495 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Ggit.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   304553 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gio.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23860 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Graphene.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19621 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gsk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gspell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   165678 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gst.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/GstPbutils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Manette.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    46604 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Pango.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/PangoCairo.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Rsvg.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22165 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/Vte.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   128468 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gdk3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   112437 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gdk4.pyi
--rw-r--r--   0 runner    (1001) docker     (123)  1058819 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gtk3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)  1067152 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gtk4.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    80128 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_GtkSource4.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    89364 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_GtkSource5.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    40235 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Soup2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    49071 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Soup3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:39:57.000000 PyGObject-stubs-2.8.0/src/gi-stubs/repository/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 20:57:23.535385 PyGObject-stubs-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-09-14 20:57:23.535385 PyGObject-stubs-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 20:57:23.519385 PyGObject-stubs-2.9.0/pep517backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/pep517backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/pep517backend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-14 20:57:23.535385 PyGObject-stubs-2.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 20:57:23.515385 PyGObject-stubs-2.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 20:57:23.519385 PyGObject-stubs-2.9.0/src/PyGObject_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-09-14 20:57:23.000000 PyGObject-stubs-2.9.0/src/PyGObject_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2023-09-14 20:57:23.000000 PyGObject-stubs-2.9.0/src/PyGObject_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 20:57:23.000000 PyGObject-stubs-2.9.0/src/PyGObject_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2023-09-14 20:57:23.000000 PyGObject-stubs-2.9.0/src/PyGObject_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-14 20:57:23.000000 PyGObject-stubs-2.9.0/src/PyGObject_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 20:57:23.519385 PyGObject-stubs-2.9.0/src/gi-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 20:57:23.535385 PyGObject-stubs-2.9.0/src/gi-stubs/repository/
+-rw-r--r--   0 runner    (1001) docker     (127)   284195 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Adw.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8130 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/AppIndicator3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    71690 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/AppStream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    47065 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Atk.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/AyatanaAppIndicator3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Farstream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    38286 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Flatpak.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/GIRepository.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   129078 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/GLib.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/GModule.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    84140 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/GObject.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/GSound.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15989 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/GdkPixbuf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20001 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Geoclue.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    63495 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Ggit.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   304553 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Gio.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23860 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Graphene.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19621 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Gsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Gspell.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   165678 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Gst.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10000 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/GstPbutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Manette.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    69820 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/OSTree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    51222 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Pango.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/PangoCairo.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Rsvg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22165 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/Vte.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   128468 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/_Gdk3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   124490 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/_Gdk4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)  1059199 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/_Gtk3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)  1067152 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/_Gtk4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    80128 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/_GtkSource4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    89364 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/_GtkSource5.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    40235 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/_Soup2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    49071 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/_Soup3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 20:57:10.000000 PyGObject-stubs-2.9.0/src/gi-stubs/repository/__init__.pyi
```

### Comparing `PyGObject-stubs-2.8.0/CHANGELOG.md` & `PyGObject-stubs-2.9.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+# 2.9.0 (14 Sep 2023)
+
+## Feature
+
+* Add AyatanaAppIndicator3
+* Add AppStream and OSTree ([#152](https://github.com/pygobject/pygobject-stubs/issues/152)) (#152)
+* Add Flatpak
+
+## Improvements
+
+* generator: Strip documentation strings
+
+## Typing
+
+* Improve type hints for
+    - AppIndicator3
+    - Cairo
+    - Gdk4
+    - GObject
+    - Gtk3
+    - PangoCairo
+
+## Bug Fixes
+
+* generator: Fix documentation if empty
+
 # 2.8.0 (24 May 2023)
 
 ## Improvements
 
 * generator: Check nullability for __init__
 
 ## Typing
```

### Comparing `PyGObject-stubs-2.8.0/LICENSE` & `PyGObject-stubs-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/PKG-INFO` & `PyGObject-stubs-2.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: PyGObject-stubs
-Version: 2.8.0
+Version: 2.9.0
 Summary: Typing stubs for PyGObject
 Author: Christoph Reiter
 Author-email: reiter.christoph@gmail.com
 License: LGPL-2.1
 Project-URL: homepage, https://github.com/pygobject/pygobject-stubs
 Project-URL: repository, https://github.com/pygobject/pygobject-stubs
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: codespell; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: PyGObject; extra == "dev"
 
 # Typing Stubs for PyGObject
 
 [![image](https://travis-ci.org/pygobject/pygobject-stubs.svg?branch=master)](https://travis-ci.org/pygobject/pygobject-stubs)
 [![PyPI](https://img.shields.io/pypi/v/pygobject-stubs)](https://pypi.org/project/PyGObject-stubs)
 
 ## Installation
```

### Comparing `PyGObject-stubs-2.8.0/README.md` & `PyGObject-stubs-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/pep517backend/backend.py` & `PyGObject-stubs-2.9.0/pep517backend/backend.py`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/PKG-INFO` & `PyGObject-stubs-2.9.0/src/PyGObject_stubs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: PyGObject-stubs
-Version: 2.8.0
+Version: 2.9.0
 Summary: Typing stubs for PyGObject
 Author: Christoph Reiter
 Author-email: reiter.christoph@gmail.com
 License: LGPL-2.1
 Project-URL: homepage, https://github.com/pygobject/pygobject-stubs
 Project-URL: repository, https://github.com/pygobject/pygobject-stubs
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: codespell; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: PyGObject; extra == "dev"
 
 # Typing Stubs for PyGObject
 
 [![image](https://travis-ci.org/pygobject/pygobject-stubs.svg?branch=master)](https://travis-ci.org/pygobject/pygobject-stubs)
 [![PyPI](https://img.shields.io/pypi/v/pygobject-stubs)](https://pypi.org/project/PyGObject-stubs)
 
 ## Installation
```

### Comparing `PyGObject-stubs-2.8.0/src/PyGObject_stubs.egg-info/SOURCES.txt` & `PyGObject-stubs-2.9.0/src/PyGObject_stubs.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 src/PyGObject_stubs.egg-info/SOURCES.txt
 src/PyGObject_stubs.egg-info/dependency_links.txt
 src/PyGObject_stubs.egg-info/requires.txt
 src/PyGObject_stubs.egg-info/top_level.txt
 src/gi-stubs/__init__.pyi
 src/gi-stubs/repository/Adw.pyi
 src/gi-stubs/repository/AppIndicator3.pyi
+src/gi-stubs/repository/AppStream.pyi
 src/gi-stubs/repository/Atk.pyi
 src/gi-stubs/repository/AyatanaAppIndicator3.pyi
 src/gi-stubs/repository/Farstream.pyi
+src/gi-stubs/repository/Flatpak.pyi
 src/gi-stubs/repository/GIRepository.pyi
 src/gi-stubs/repository/GLib.pyi
 src/gi-stubs/repository/GModule.pyi
 src/gi-stubs/repository/GObject.pyi
 src/gi-stubs/repository/GSound.pyi
 src/gi-stubs/repository/GdkPixbuf.pyi
 src/gi-stubs/repository/Geoclue.pyi
@@ -27,14 +29,15 @@
 src/gi-stubs/repository/Gio.pyi
 src/gi-stubs/repository/Graphene.pyi
 src/gi-stubs/repository/Gsk.py
 src/gi-stubs/repository/Gspell.pyi
 src/gi-stubs/repository/Gst.pyi
 src/gi-stubs/repository/GstPbutils.pyi
 src/gi-stubs/repository/Manette.pyi
+src/gi-stubs/repository/OSTree.pyi
 src/gi-stubs/repository/Pango.pyi
 src/gi-stubs/repository/PangoCairo.pyi
 src/gi-stubs/repository/Rsvg.pyi
 src/gi-stubs/repository/Vte.pyi
 src/gi-stubs/repository/_Gdk3.pyi
 src/gi-stubs/repository/_Gdk4.pyi
 src/gi-stubs/repository/_Gtk3.pyi
```

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Adw.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/Adw.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Atk.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/Atk.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Farstream.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/Farstream.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/GIRepository.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/GIRepository.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/GLib.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/GLib.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/GModule.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/GModule.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/GObject.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/GObject.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -710,15 +710,15 @@
 def type_interface_instantiatable_prerequisite(interface_type: Type) -> Type: ...
 def type_interface_peek(
     instance_class: TypeClass, iface_type: Type
 ) -> TypeInterface: ...
 def type_interface_prerequisites(interface_type: Type) -> list[Type]: ...
 def type_interfaces(type: Type) -> list[Type]: ...
 def type_is_a(type: Type, is_a_type: Type) -> bool: ...
-def type_name(type: Type) -> str: ...
+def type_name(type: Type) -> Optional[str]: ...
 def type_name_from_class(g_class: TypeClass) -> str: ...
 def type_name_from_instance(instance: TypeInstance) -> str: ...
 def type_next_base(leaf_type: Type, root_type: Type) -> Type: ...
 def type_parent(type_): ...  # FIXME Function
 def type_qname(type: Type) -> int: ...
 def type_query(type: Type) -> TypeQuery: ...
 def type_register(*args, **kwargs): ...  # FIXME Function
@@ -744,14 +744,39 @@
 # override
 class _HandlerBlockManager:
     def __init__(self, obj, handler_id: int) -> None: ...
     def __enter__(self) -> None: ...
     def __exit__(self, exc_type, exc_value, traceback) -> None: ...
 
 class Binding(Object):
+    """
+    :Constructors:
+
+    ::
+
+        Binding(**properties)
+
+    Object GBinding
+
+    Properties from GBinding:
+      source -> GObject: Source
+        The source of the binding
+      target -> GObject: Target
+        The target of the binding
+      source-property -> gchararray: Source Property
+        The property on the source to bind
+      target-property -> gchararray: Target Property
+        The property on the target to bind
+      flags -> GBindingFlags: Flags
+        The binding flags
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         flags: BindingFlags
         source: Optional[Object]
         source_property: str
         target: Optional[Object]
         target_property: str
     props: Props = ...
@@ -769,18 +794,36 @@
     def get_source(self) -> Optional[Object]: ...
     def get_source_property(self) -> str: ...
     def get_target(self) -> Optional[Object]: ...
     def get_target_property(self) -> str: ...
     def unbind(self): ...  # FIXME Function
 
 class BindingGroup(Object):
+    """
+    :Constructors:
+
+    ::
+
+        BindingGroup(**properties)
+        new() -> GObject.BindingGroup
+
+    Object GBindingGroup
+
+    Properties from GBindingGroup:
+      source -> GObject: Source
+        The source GObject used for binding properties.
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         source: Optional[Object]
     props: Props = ...
-    def __init__(self, source: Object = ...): ...
+    def __init__(self, source: Optional[Object] = ...): ...
     def bind(
         self,
         source_property: str,
         target: Object,
         target_property: str,
         flags: BindingFlags,
     ) -> None: ...
@@ -795,14 +838,22 @@
     ) -> None: ...
     def dup_source(self) -> Optional[Object]: ...
     @classmethod
     def new(cls) -> BindingGroup: ...
     def set_source(self, source: Optional[Object] = None) -> None: ...
 
 class CClosure(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        CClosure()
+    """
+
     closure: Callable[..., Any] = ...
     callback: None = ...
     @staticmethod
     def marshal_BOOLEAN__BOXED_BOXED(
         closure: Callable[..., Any],
         return_value: Any,
         n_param_values: int,
@@ -1006,14 +1057,24 @@
         n_param_values: int,
         param_values: Any,
         invocation_hint: None,
         marshal_data: None,
     ) -> None: ...
 
 class Closure(GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        Closure()
+        new_object(sizeof_closure:int, object:GObject.Object) -> GObject.Closure
+        new_simple(sizeof_closure:int, data=None) -> GObject.Closure
+    """
+
     ref_count: int = ...
     meta_marshal_nouse: int = ...
     n_guards: int = ...
     n_fnotifiers: int = ...
     n_inotifiers: int = ...
     in_inotify: int = ...
     floating: int = ...
@@ -1032,44 +1093,88 @@
     @classmethod
     def new_simple(cls, sizeof_closure: int, data: None) -> Closure: ...
     def ref(self) -> Callable[..., Any]: ...
     def sink(self) -> None: ...
     def unref(self) -> None: ...
 
 class ClosureNotifyData(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        ClosureNotifyData()
+    """
+
     data: None = ...
     notify: Callable[[None, Callable[..., Any]], None] = ...
 
 class EnumClass(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        EnumClass()
+    """
+
     g_type_class: TypeClass = ...
     minimum: int = ...
     maximum: int = ...
     n_values: int = ...
     values: EnumValue = ...
 
 class EnumValue(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        EnumValue()
+    """
+
     value: int = ...
     value_name: str = ...
     value_nick: str = ...
 
 class FlagsClass(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        FlagsClass()
+    """
+
     g_type_class: TypeClass = ...
     mask: int = ...
     n_values: int = ...
     values: FlagsValue = ...
 
 class FlagsValue(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        FlagsValue()
+    """
+
     value: int = ...
     value_name: str = ...
     value_nick: str = ...
 
 class GBoxed:
+    """ """
+
     def copy(self, *args, **kwargs): ...  # FIXME Function
 
 class GError:
+    """ """
+
     def copy(self): ...  # FIXME Function
     def matches(self, domain, code): ...  # FIXME Function
     def new_literal(domain, message, code): ...  # FIXME Function
 
 # override
 class GInterface(Protocol):
     # Copy pasted from Object
@@ -1081,15 +1186,18 @@
 
     # override
     def bind_property(
         self,
         source_property: str,
         target: Object,
         target_property: str,
-        flags: BindingFlags,
+        flags: BindingFlags = BindingFlags.DEFAULT,
+        transform_to: Optional[Callable[..., Any]] = None,
+        transform_from: Optional[Callable[..., Any]] = None,
+        user_data: Optional[Any] = None,
     ) -> Binding: ...
     def bind_property_full(self, *args, **kargs): ...  # FIXME Function
     def chain(self, *args, **kwargs): ...  # FIXME Function
     def compat_control(self, *args, **kargs): ...  # FIXME Function
     # override
     def connect(
         self, detailed_signal: str, handler: Callable[..., Any], *args: Any
@@ -1164,20 +1272,26 @@
     # override
     def weak_ref(self, callback: Callable[..., Any], *args: Any) -> None: ...
 
 # override
 class GObject(Object): ...
 
 class GObjectWeakRef:
+    """
+    A GObject weak reference
+    """
+
     def unref(self, *args, **kwargs): ...  # FIXME Function
 
 class GParamSpec: ...
 class GPointer: ...
 
 class GType:
+    """ """
+
     children = ...  # FIXME Constant
     depth = ...  # FIXME Constant
     fundamental = ...  # FIXME Constant
     interfaces = ...  # FIXME Constant
     name = ...  # FIXME Constant
     parent = ...  # FIXME Constant
     pytype = ...  # FIXME Constant
@@ -1191,14 +1305,23 @@
     def is_derivable(self, *args, **kwargs): ...  # FIXME Function
     def is_instantiatable(self, *args, **kwargs): ...  # FIXME Function
     def is_interface(self, *args, **kwargs): ...  # FIXME Function
     def is_value_abstract(self, *args, **kwargs): ...  # FIXME Function
     def is_value_type(self, *args, **kwargs): ...  # FIXME Function
 
 class Idle(GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        Source()
+        new(source_funcs:GLib.SourceFuncs, struct_size:int) -> GLib.Source
+    """
+
     callback_data: None = ...
     callback_funcs: GLib.SourceCallbackFuncs = ...
     source_funcs: GLib.SourceFuncs = ...
     ref_count: int = ...
     context: GLib.MainContext = ...
     priority: int = ...
     flags: int = ...
@@ -1249,19 +1372,40 @@
     def set_name_by_id(tag: int, name: str) -> None: ...
     def set_priority(self, priority: int) -> None: ...
     def set_ready_time(self, ready_time: int) -> None: ...
     def set_static_name(self, name: str) -> None: ...
     def unref(self) -> None: ...
 
 class InitiallyUnowned(Object):
+    """
+    :Constructors:
+
+    ::
+
+        InitiallyUnowned(**properties)
+
+    Object GInitiallyUnowned
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     g_type_instance: TypeInstance = ...
     ref_count: int = ...
     qdata: GLib.Data = ...
 
 class InitiallyUnownedClass(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        InitiallyUnownedClass()
+    """
+
     g_type_class: TypeClass = ...
     construct_properties: list[None] = ...
     constructor: None = ...
     set_property: Callable[[Object, int, Any, ParamSpec], None] = ...
     get_property: Callable[[Object, int, Any, ParamSpec], None] = ...
     dispose: Callable[[Object], None] = ...
     finalize: Callable[[Object], None] = ...
@@ -1271,19 +1415,36 @@
     flags: int = ...
     n_construct_properties: int = ...
     pspecs: None = ...
     n_pspecs: int = ...
     pdummy: list[None] = ...
 
 class InterfaceInfo(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        InterfaceInfo()
+    """
+
     interface_init: Callable[[TypeInterface, None], None] = ...
     interface_finalize: Callable[[TypeInterface, None], None] = ...
     interface_data: None = ...
 
 class MainContext(GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        new() -> GLib.MainContext
+        new_with_flags(flags:GLib.MainContextFlags) -> GLib.MainContext
+    """
+
     def acquire(self) -> bool: ...
     def add_poll(self, fd: GLib.PollFD, priority: int) -> None: ...
     def check(self, max_priority: int, fds: Sequence[GLib.PollFD]) -> bool: ...
     @staticmethod
     def default() -> GLib.MainContext: ...
     def dispatch(self) -> None: ...
     def find_source_by_funcs_user_data(
@@ -1313,36 +1474,61 @@
     def release(self) -> None: ...
     def remove_poll(self, fd: GLib.PollFD) -> None: ...
     def unref(self) -> None: ...
     def wait(self, cond: GLib.Cond, mutex: GLib.Mutex) -> bool: ...
     def wakeup(self) -> None: ...
 
 class MainLoop(GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        new(context:GLib.MainContext=None, is_running:bool) -> GLib.MainLoop
+    """
+
     def get_context(self) -> GLib.MainContext: ...
     def is_running(self) -> bool: ...
     @classmethod
     def new(cls, context: Optional[GLib.MainContext], is_running: bool) -> MainLoop: ...
     def quit(self) -> None: ...
     def ref(self) -> GLib.MainLoop: ...
     def run(self): ...  # FIXME Function
     def unref(self) -> None: ...
 
 class Object:
+    """
+    :Constructors:
+
+    ::
+
+        Object(**properties)
+        newv(object_type:GType, parameters:list) -> GObject.Object
+
+    Object GObject
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     g_type_instance: TypeInstance = ...
     ref_count: int = ...
     qdata: GLib.Data = ...
     props = ...  # FIXME Constant
 
     # override
     def bind_property(
         self,
         source_property: str,
         target: Object,
         target_property: str,
-        flags: BindingFlags,
+        flags: BindingFlags = BindingFlags.DEFAULT,
+        transform_to: Optional[Callable[..., Any]] = None,
+        transform_from: Optional[Callable[..., Any]] = None,
+        user_data: Optional[Any] = None,
     ) -> Binding: ...
     def bind_property_full(self, *args, **kargs): ...  # FIXME Function
     def chain(self, *args, **kwargs): ...  # FIXME Function
     def compat_control(self, *args, **kargs): ...  # FIXME Function
     # override
     def connect(
         self, detailed_signal: str, handler: Callable[..., Any], *args: Any
@@ -1414,14 +1600,22 @@
     def thaw_notify(self) -> None: ...
     def unref(self, *args, **kargs): ...  # FIXME Function
     def watch_closure(self, *args, **kargs): ...  # FIXME Function
     # override
     def weak_ref(self, callback: Callable[..., Any], *args: Any) -> None: ...
 
 class ObjectClass(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        ObjectClass()
+    """
+
     g_type_class: TypeClass = ...
     construct_properties: list[None] = ...
     constructor: None = ...
     set_property: Callable[[Object, int, Any, ParamSpec], None] = ...
     get_property: Callable[[Object, int, Any, ParamSpec], None] = ...
     dispose: Callable[[Object], None] = ...
     finalize: Callable[[Object], None] = ...
@@ -1438,32 +1632,52 @@
         self, n_pspecs: int, pspecs: Sequence[ParamSpec]
     ) -> None: ...
     def install_property(self, property_id: int, pspec: ParamSpec) -> None: ...
     def list_properties(self) -> list[ParamSpec]: ...
     def override_property(self, property_id: int, name: str) -> None: ...
 
 class ObjectConstructParam(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        ObjectConstructParam()
+    """
+
     pspec: ParamSpec = ...
     value: Any = ...
 
 class OptionContext:
+    """ """
+
     def add_group(self, *args, **kwargs): ...  # FIXME Function
     def get_help_enabled(self, *args, **kwargs): ...  # FIXME Function
     def get_ignore_unknown_options(self, *args, **kwargs): ...  # FIXME Function
     def get_main_group(self, *args, **kwargs): ...  # FIXME Function
     def parse(self, *args, **kwargs): ...  # FIXME Function
     def set_help_enabled(self, *args, **kwargs): ...  # FIXME Function
     def set_ignore_unknown_options(self, *args, **kwargs): ...  # FIXME Function
     def set_main_group(self, *args, **kwargs): ...  # FIXME Function
 
 class OptionGroup:
+    """ """
+
     def add_entries(self, *args, **kwargs): ...  # FIXME Function
     def set_translation_domain(self, *args, **kwargs): ...  # FIXME Function
 
 class ParamSpec:
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpec(**properties)
+    """
+
     g_type_instance: TypeInstance = ...
     name: str = ...
     flags: ParamFlags = ...
     value_type: Type = ...
     owner_type: Type = ...
     _nick: str = ...
     _blurb: str = ...
@@ -1485,181 +1699,401 @@
     @staticmethod
     def is_valid_name(name: str) -> bool: ...
     def set_qdata(self, quark: int, data: None) -> None: ...
     def sink(self) -> None: ...
     def steal_qdata(self, quark: int) -> None: ...
 
 class ParamSpecBoolean(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecBoolean(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     default_value: bool = ...
 
 class ParamSpecBoxed(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecBoxed(**properties)
+    """
+
     parent_instance: ParamSpec = ...
 
 class ParamSpecChar(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecChar(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     minimum: int = ...
     maximum: int = ...
     default_value: int = ...
 
 class ParamSpecClass(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecClass()
+    """
+
     g_type_class: TypeClass = ...
     value_type: Type = ...
     finalize: Callable[[ParamSpec], None] = ...
     value_set_default: Callable[[ParamSpec, Any], None] = ...
     value_validate: Callable[[ParamSpec, Any], bool] = ...
     values_cmp: Callable[[ParamSpec, Any, Any], int] = ...
     value_is_valid: Callable[[ParamSpec, Any], bool] = ...
     dummy: list[None] = ...
 
 class ParamSpecDouble(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecDouble(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     minimum: float = ...
     maximum: float = ...
     default_value: float = ...
     epsilon: float = ...
 
 class ParamSpecEnum(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecEnum(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     enum_class: EnumClass = ...
     default_value: int = ...
 
 class ParamSpecFlags(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecFlags(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     flags_class: FlagsClass = ...
     default_value: int = ...
 
 class ParamSpecFloat(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecFloat(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     minimum: float = ...
     maximum: float = ...
     default_value: float = ...
     epsilon: float = ...
 
 class ParamSpecGType(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecGType(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     is_a_type: Type = ...
 
 class ParamSpecInt(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecInt(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     minimum: int = ...
     maximum: int = ...
     default_value: int = ...
 
 class ParamSpecInt64(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecInt64(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     minimum: int = ...
     maximum: int = ...
     default_value: int = ...
 
 class ParamSpecLong(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecLong(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     minimum: int = ...
     maximum: int = ...
     default_value: int = ...
 
 class ParamSpecObject(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecObject(**properties)
+    """
+
     parent_instance: ParamSpec = ...
 
 class ParamSpecOverride(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecOverride(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     overridden: ParamSpec = ...
 
 class ParamSpecParam(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecParam(**properties)
+    """
+
     parent_instance: ParamSpec = ...
 
 class ParamSpecPointer(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecPointer(**properties)
+    """
+
     parent_instance: ParamSpec = ...
 
 class ParamSpecPool(GPointer):
+    """ """
+
     def insert(self, pspec: ParamSpec, owner_type: Type) -> None: ...
     def list(self, owner_type: Type) -> list[ParamSpec]: ...
     def list_owned(self, owner_type: Type) -> list[ParamSpec]: ...
     def lookup(
         self, param_name: str, owner_type: Type, walk_ancestors: bool
     ) -> Optional[ParamSpec]: ...
     def remove(self, pspec: ParamSpec) -> None: ...
 
 class ParamSpecString(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecString(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     default_value: str = ...
     cset_first: str = ...
     cset_nth: str = ...
     substitutor: int = ...
     null_fold_if_empty: int = ...
     ensure_non_null: int = ...
 
 class ParamSpecTypeInfo(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecTypeInfo()
+    """
+
     instance_size: int = ...
     n_preallocs: int = ...
     instance_init: Callable[[ParamSpec], None] = ...
     value_type: Type = ...
     finalize: Callable[[ParamSpec], None] = ...
     value_set_default: Callable[[ParamSpec, Any], None] = ...
     value_validate: Callable[[ParamSpec, Any], bool] = ...
     values_cmp: Callable[[ParamSpec, Any, Any], int] = ...
 
 class ParamSpecUChar(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecUChar(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     minimum: int = ...
     maximum: int = ...
     default_value: int = ...
 
 class ParamSpecUInt(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecUInt(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     minimum: int = ...
     maximum: int = ...
     default_value: int = ...
 
 class ParamSpecUInt64(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecUInt64(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     minimum: int = ...
     maximum: int = ...
     default_value: int = ...
 
 class ParamSpecULong(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecULong(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     minimum: int = ...
     maximum: int = ...
     default_value: int = ...
 
 class ParamSpecUnichar(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecUnichar(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     default_value: str = ...
 
 class ParamSpecValueArray(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecValueArray(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     element_spec: ParamSpec = ...
     fixed_n_elements: int = ...
 
 class ParamSpecVariant(ParamSpec):
+    """
+    :Constructors:
+
+    ::
+
+        ParamSpecVariant(**properties)
+    """
+
     parent_instance: ParamSpec = ...
     type: GLib.VariantType = ...
     default_value: GLib.Variant = ...
     padding: list[None] = ...
 
 class Parameter(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        Parameter()
+    """
+
     name: str = ...
     value: Any = ...
 
 class Pid:
+    """ """
+
     denominator = ...  # FIXME Constant
     imag = ...  # FIXME Constant
     numerator = ...  # FIXME Constant
     real = ...  # FIXME Constant
 
     def as_integer_ratio(self, *args, **kwargs): ...  # FIXME Method
     def bit_count(self, *args, **kwargs): ...  # FIXME Method
     def bit_length(self, *args, **kwargs): ...  # FIXME Method
     def close(self, *args, **kwargs): ...  # FIXME Method
     def conjugate(self, *args, **kwargs): ...  # FIXME Method
     def from_bytes(self, *args, **kwargs): ...  # FIXME Method
     def to_bytes(self, *args, **kwargs): ...  # FIXME Method
 
 class PollFD(GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        PollFD()
+    """
+
     fd: int = ...
     events: int = ...
     revents: int = ...
 
 # override
 class Property:
     def __init__(
@@ -1710,58 +2144,107 @@
         def connect_detailed(
             self, callback: Callable, detail: str, *args, **kargs
         ) -> int: ...
         def disconnect(self, handler_id: int): ...
         def emit(self, *args, **kargs): ...
 
 class SignalGroup(Object):
+    """
+    :Constructors:
+
+    ::
+
+        SignalGroup(**properties)
+        new(target_type:GType) -> GObject.SignalGroup
+
+    Object GSignalGroup
+
+    Signals from GSignalGroup:
+      bind (GObject)
+      unbind ()
+
+    Properties from GSignalGroup:
+      target -> GObject: Target
+        The target instance used when connecting signals.
+      target-type -> GType: Target Type
+        The GType of the target property.
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         target: Optional[Object]
         target_type: Type
     props: Props = ...
-    def __init__(self, target: Object = ..., target_type: Type = ...): ...
+    def __init__(self, target: Optional[Object] = ..., target_type: Type = ...): ...
     def block(self) -> None: ...
     def connect_closure(
         self, detailed_signal: str, closure: Callable[..., Any], after: bool
     ) -> None: ...
     def connect_data(
         self,
         detailed_signal: str,
-        c_handler: Callable[[], None],
+        c_handler: Callable[..., None],
         flags: ConnectFlags,
         *data: Any,
     ) -> None: ...
     def connect_swapped(
-        self, detailed_signal: str, c_handler: Callable[[], None], *data: Any
+        self, detailed_signal: str, c_handler: Callable[..., None], *data: Any
     ) -> None: ...
     def dup_target(self) -> Optional[Object]: ...
     @classmethod
     def new(cls, target_type: Type) -> SignalGroup: ...
     def set_target(self, target: Optional[Object] = None) -> None: ...
     def unblock(self) -> None: ...
 
 class SignalInvocationHint(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        SignalInvocationHint()
+    """
+
     signal_id: int = ...
     detail: int = ...
     run_type: SignalFlags = ...
 
 # override
 class SignalOverride(Signal):
     def get_signal_args(self) -> Literal["override"]: ...
 
 class SignalQuery(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        SignalQuery()
+    """
+
     signal_id: int = ...
     signal_name: str = ...
     itype: Type = ...
     signal_flags: SignalFlags = ...
     return_type: Type = ...
     n_params: int = ...
     param_types: list[Type] = ...
 
 class Source(GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        Source()
+        new(source_funcs:GLib.SourceFuncs, struct_size:int) -> GLib.Source
+    """
+
     callback_data: None = ...
     callback_funcs: GLib.SourceCallbackFuncs = ...
     source_funcs: GLib.SourceFuncs = ...
     ref_count: int = ...
     context: GLib.MainContext = ...
     priority: int = ...
     flags: int = ...
@@ -1812,14 +2295,23 @@
     def set_name_by_id(tag: int, name: str) -> None: ...
     def set_priority(self, priority: int) -> None: ...
     def set_ready_time(self, ready_time: int) -> None: ...
     def set_static_name(self, name: str) -> None: ...
     def unref(self) -> None: ...
 
 class Timeout(GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        Source()
+        new(source_funcs:GLib.SourceFuncs, struct_size:int) -> GLib.Source
+    """
+
     callback_data: None = ...
     callback_funcs: GLib.SourceCallbackFuncs = ...
     source_funcs: GLib.SourceFuncs = ...
     ref_count: int = ...
     context: GLib.MainContext = ...
     priority: int = ...
     flags: int = ...
@@ -1872,14 +2364,22 @@
     def set_ready_time(self, ready_time: int) -> None: ...
     def set_static_name(self, name: str) -> None: ...
     def unref(self) -> None: ...
 
 class TypeCValue(GPointer): ...
 
 class TypeClass(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        TypeClass()
+    """
+
     g_type: Type = ...
     def add_private(self, private_size: int) -> None: ...
     @staticmethod
     def adjust_private_offset(g_class: None, private_size_or_offset: int) -> None: ...
     def get_private(self, private_type: Type) -> None: ...
     @staticmethod
     def peek(type: Type) -> TypeClass: ...
@@ -1887,33 +2387,65 @@
     @staticmethod
     def peek_static(type: Type) -> TypeClass: ...
     @staticmethod
     def ref(type: Type) -> TypeClass: ...
     def unref(self) -> None: ...
 
 class TypeFundamentalInfo(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        TypeFundamentalInfo()
+    """
+
     type_flags: TypeFundamentalFlags = ...
 
 class TypeInfo(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        TypeInfo()
+    """
+
     class_size: int = ...
     base_init: Callable[[TypeClass], None] = ...
     base_finalize: Callable[[TypeClass], None] = ...
     class_init: Callable[[TypeClass, None], None] = ...
     class_finalize: Callable[[TypeClass, None], None] = ...
     class_data: None = ...
     instance_size: int = ...
     n_preallocs: int = ...
     instance_init: Callable[[TypeInstance, TypeClass], None] = ...
     value_table: TypeValueTable = ...
 
 class TypeInstance(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        TypeInstance()
+    """
+
     g_class: TypeClass = ...
     def get_private(self, private_type: Type) -> None: ...
 
 class TypeInterface(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        TypeInterface()
+    """
+
     g_type: Type = ...
     g_instance_type: Type = ...
     @staticmethod
     def add_prerequisite(interface_type: Type, prerequisite_type: Type) -> None: ...
     @staticmethod
     def get_plugin(instance_type: Type, interface_type: Type) -> TypePlugin: ...
     @staticmethod
@@ -1943,85 +2475,129 @@
         self, parent_type: Type, type_name: str, type_info: TypeInfo, flags: TypeFlags
     ) -> Type: ...
     def set_name(self, name: str) -> None: ...
     def unuse(self) -> None: ...
     def use(self) -> bool: ...
 
 class TypeModuleClass(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        TypeModuleClass()
+    """
+
     parent_class: ObjectClass = ...
     load: Callable[[TypeModule], bool] = ...
     unload: Callable[[TypeModule], None] = ...
     reserved1: Callable[[], None] = ...
     reserved2: Callable[[], None] = ...
     reserved3: Callable[[], None] = ...
     reserved4: Callable[[], None] = ...
 
 class TypePlugin(Object):
+    """
+    Interface GTypePlugin
+    """
+
     def complete_interface_info(
         self, instance_type: Type, interface_type: Type, info: InterfaceInfo
     ) -> None: ...
     def complete_type_info(
         self, g_type: Type, info: TypeInfo, value_table: TypeValueTable
     ) -> None: ...
     def unuse(self) -> None: ...
     def use(self) -> None: ...
 
 class TypePluginClass(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        TypePluginClass()
+    """
+
     base_iface: TypeInterface = ...
     use_plugin: Callable[[TypePlugin], None] = ...
     unuse_plugin: Callable[[TypePlugin], None] = ...
     complete_type_info: Callable[
         [TypePlugin, Type, TypeInfo, TypeValueTable], None
     ] = ...
     complete_interface_info: Callable[
         [TypePlugin, Type, Type, InterfaceInfo], None
     ] = ...
 
 class TypeQuery(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        TypeQuery()
+    """
+
     type: Type = ...
     type_name: str = ...
     class_size: int = ...
     instance_size: int = ...
 
 class TypeValueTable(GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        TypeValueTable()
+    """
+
     value_init: Callable[[Any], None] = ...
     value_free: Callable[[Any], None] = ...
     value_copy: Callable[[Any, Any], None] = ...
     value_peek_pointer: Callable[[Any], None] = ...
     collect_format: str = ...
     collect_value: Callable[[Any, int, TypeCValue, int], str] = ...
     lcopy_format: str = ...
     lcopy_value: Callable[[Any, int, TypeCValue, int], str] = ...
 
 class Value(GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        Value()
+    """
+
     g_type: Type = ...
     data: list[_Value__data__union] = ...
     _Value__g_type = ...  # FIXME Constant
 
     def copy(self, dest_value: Any) -> None: ...
-    def dup_object(self) -> Object: ...
-    def dup_string(self) -> str: ...
+    def dup_object(self) -> Optional[Object]: ...
+    def dup_string(self) -> Optional[str]: ...
     def dup_variant(self) -> Optional[GLib.Variant]: ...
     def fits_pointer(self) -> bool: ...
     def get_boolean(self) -> bool: ...
     def get_boxed(self): ...  # FIXME Function
     def get_char(self) -> int: ...
     def get_double(self) -> float: ...
     def get_enum(self) -> int: ...
     def get_flags(self) -> int: ...
     def get_float(self) -> float: ...
     def get_gtype(self) -> Type: ...
     def get_int(self) -> int: ...
     def get_int64(self) -> int: ...
     def get_long(self) -> int: ...
-    def get_object(self) -> Object: ...
+    def get_object(self) -> Optional[Object]: ...
     def get_param(self) -> ParamSpec: ...
     def get_pointer(self) -> None: ...
     def get_schar(self) -> int: ...
-    def get_string(self) -> str: ...
+    def get_string(self) -> Optional[str]: ...
     def get_uchar(self) -> int: ...
     def get_uint(self) -> int: ...
     def get_uint64(self) -> int: ...
     def get_ulong(self) -> int: ...
     def get_value(self): ...  # FIXME Function
     def get_variant(self) -> Optional[GLib.Variant]: ...
     def init(self, g_type: Type) -> Any: ...
@@ -2063,47 +2639,116 @@
     @staticmethod
     def type_compatible(src_type: Type, dest_type: Type) -> bool: ...
     @staticmethod
     def type_transformable(src_type: Type, dest_type: Type) -> bool: ...
     def unset(self) -> None: ...
 
 class ValueArray(GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        ValueArray()
+        new(n_prealloced:int) -> GObject.ValueArray
+    """
+
     n_values: int = ...
     values: Any = ...
     n_prealloced: int = ...
     def append(self, value: Optional[Any] = None) -> ValueArray: ...
     def copy(self) -> ValueArray: ...
     def get_nth(self, index_: int) -> Any: ...
     def insert(self, index_: int, value: Optional[Any] = None) -> ValueArray: ...
     @classmethod
     def new(cls, n_prealloced: int) -> ValueArray: ...
     def prepend(self, value: Optional[Any] = None) -> ValueArray: ...
     def remove(self, index_: int) -> ValueArray: ...
     def sort(self, compare_func: Callable[..., int], *user_data: Any) -> ValueArray: ...
 
 class Warning:
+    """ """
+
     args = ...  # FIXME Constant
 
     def add_note(self, *args, **kwargs): ...  # FIXME Function
     def with_traceback(self, *args, **kwargs): ...  # FIXME Function
 
 class WeakRef(GPointer): ...
 
 class _Value__data__union(GPointer):
+    """ """
+
     v_double = ...  # FIXME Constant
     v_float = ...  # FIXME Constant
     v_int = ...  # FIXME Constant
     v_int64 = ...  # FIXME Constant
     v_long = ...  # FIXME Constant
     v_pointer = ...  # FIXME Constant
     v_uint = ...  # FIXME Constant
     v_uint64 = ...  # FIXME Constant
     v_ulong = ...  # FIXME Constant
 
 class property:
+    """
+    Creates a new Property which when used in conjunction with
+        GObject subclass will create a Python property accessor for the
+        GObject ParamSpec.
+
+        :param callable getter:
+            getter to get the value of the property
+        :param callable setter:
+            setter to set the value of the property
+        :param type type:
+            type of property
+        :param default:
+            default value, must match the property type.
+        :param str nick:
+            short description
+        :param str blurb:
+            long description
+        :param GObject.ParamFlags flags:
+            parameter flags
+        :keyword minimum:
+            minimum allowed value (int, float, long only)
+        :keyword maximum:
+            maximum allowed value (int, float, long only)
+
+        .. code-block:: python
+
+             class MyObject(GObject.Object):
+                 prop = GObject.Property(type=str)
+
+             obj = MyObject()
+             obj.prop = 'value'
+
+             obj.prop  # now is 'value'
+
+        The API is similar to the builtin :py:func:`property`:
+
+        .. code-block:: python
+
+            class AnotherObject(GObject.Object):
+                value = 0
+
+                @GObject.Property
+                def prop(self):
+                    'Read only property.'
+                    return 1
+
+                @GObject.Property(type=int)
+                def propInt(self):
+                    'Read-write integer property.'
+                    return self.value
+
+                @propInt.setter
+                def propInt(self, value):
+                    self.value = value
+    """
+
     _default_lookup = ...  # FIXME Constant
     _max_value_lookup = ...  # FIXME Constant
     _min_value_lookup = ...  # FIXME Constant
     _type_from_pytype_lookup = ...  # FIXME Constant
 
     def get_pspec_args(self): ...  # FIXME Function
     def getter(self, fget): ...  # FIXME Function
@@ -2176,14 +2821,15 @@
     MASK = 7
     NONE = 0
     OBJECTS = 1
     SIGNALS = 2
 
 class TypeFlags(GFlags):
     ABSTRACT = 16
+    DEPRECATED = 128
     FINAL = 64
     NONE = 0
     VALUE_ABSTRACT = 32
 
 class TypeFundamentalFlags(GFlags):
     CLASSED = 1
     DEEP_DERIVABLE = 8
```

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/GSound.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/GSound.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/GdkPixbuf.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/GdkPixbuf.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Geoclue.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/Geoclue.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Ggit.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/Ggit.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gio.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/Gio.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Graphene.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/Graphene.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gsk.py` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/Gsk.py`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gspell.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/Gspell.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Gst.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/Gst.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/GstPbutils.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/GstPbutils.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Manette.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/Manette.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Pango.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/Pango.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Any
 from typing import Callable
-from typing import Literal
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Type
 
 from gi.repository import Gio
 from gi.repository import GLib
@@ -17,18 +16,19 @@
 ATTR_INDEX_FROM_TEXT_BEGINNING: int = 0
 ATTR_INDEX_TO_TEXT_END: int = 4294967295
 GLYPH_EMPTY: int = 268435455
 GLYPH_INVALID_INPUT: int = 4294967295
 GLYPH_UNKNOWN_FLAG: int = 268435456
 SCALE: int = 1024
 VERSION_MAJOR: int = 1
-VERSION_MICRO: int = 10
+VERSION_MICRO: int = 12
 VERSION_MINOR: int = 50
-VERSION_STRING: str = "1.50.10"
+VERSION_STRING: str = "1.50.12"
 _introspection_module = ...  # FIXME Constant
+_lock = ...  # FIXME Constant
 _namespace: str = "Pango"
 _overrides_module = ...  # FIXME Constant
 _version: str = "1.0"
 
 def attr_allow_breaks_new(allow_breaks: bool) -> Attribute: ...
 def attr_background_alpha_new(alpha: int) -> Attribute: ...
 def attr_background_new(red: int, green: int, blue: int) -> Attribute: ...
@@ -120,15 +120,15 @@
     start_index: int,
     length: int,
     attrs: AttrList,
     cached_iter: Optional[AttrIterator] = None,
 ) -> list[Item]: ...
 def language_from_string(language: Optional[str] = None) -> Optional[Language]: ...
 def language_get_default() -> Language: ...
-def language_get_preferred() -> Optional[Language]: ...
+def language_get_preferred() -> Optional[list[Language]]: ...
 def layout_deserialize_error_quark() -> int: ...
 def log2vis_get_embedding_levels(
     text: str, length: int, pbase_dir: Direction
 ) -> int: ...
 def markup_parser_finish(
     context: GLib.MarkupParseContext,
 ) -> Tuple[bool, AttrList, str, str]: ...
@@ -188,70 +188,142 @@
 def version() -> int: ...
 def version_check(
     required_major: int, required_minor: int, required_micro: int
 ) -> Optional[str]: ...
 def version_string() -> str: ...
 
 class Analysis(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        Analysis()
+    """
+
     shape_engine: None = ...
     lang_engine: None = ...
     font: Font = ...
     level: int = ...
     gravity: int = ...
     flags: int = ...
     script: int = ...
     language: Language = ...
     extra_attrs: list[None] = ...
 
 class AttrClass(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        AttrClass()
+    """
+
     type: AttrType = ...
     copy: Callable[[Attribute], Attribute] = ...
     destroy: Callable[[Attribute], None] = ...
     equal: Callable[[Attribute, Attribute], bool] = ...
 
 class AttrColor(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        AttrColor()
+    """
+
     attr: Attribute = ...
     color: Color = ...
 
 class AttrFloat(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        AttrFloat()
+    """
+
     attr: Attribute = ...
     value: float = ...
 
 class AttrFontDesc(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        AttrFontDesc()
+    """
+
     attr: Attribute = ...
     desc: FontDescription = ...
     @staticmethod
     def new(desc: FontDescription) -> Attribute: ...
 
 class AttrFontFeatures(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        AttrFontFeatures()
+    """
+
     attr: Attribute = ...
     features: str = ...
     @staticmethod
     def new(features: str) -> Attribute: ...
 
 class AttrInt(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        AttrInt()
+    """
+
     attr: Attribute = ...
     value: int = ...
 
 class AttrIterator(GObject.GBoxed):
     def copy(self) -> AttrIterator: ...
     def destroy(self) -> None: ...
     def get(self, type: AttrType) -> Optional[Attribute]: ...
     def get_attrs(self) -> list[Attribute]: ...
     def get_font(self, desc: FontDescription) -> Tuple[Language, list[Attribute]]: ...
     def next(self) -> bool: ...
     def range(self) -> Tuple[int, int]: ...
 
 class AttrLanguage(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        AttrLanguage()
+    """
+
     attr: Attribute = ...
     value: Language = ...
     @staticmethod
     def new(language: Language) -> Attribute: ...
 
 class AttrList(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        new() -> Pango.AttrList
+    """
+
     def change(self, attr: Attribute) -> None: ...
     def copy(self) -> Optional[AttrList]: ...
     def equal(self, other_list: AttrList) -> bool: ...
     def filter(self, func: Callable[..., bool], *data: Any) -> Optional[AttrList]: ...
     @staticmethod
     def from_string(text: str) -> Optional[AttrList]: ...
     def get_attributes(self) -> list[Attribute]: ...
@@ -263,14 +335,22 @@
     def ref(self) -> AttrList: ...
     def splice(self, other: AttrList, pos: int, len: int) -> None: ...
     def to_string(self) -> str: ...
     def unref(self) -> None: ...
     def update(self, pos: int, remove: int, add: int) -> None: ...
 
 class AttrShape(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        AttrShape()
+    """
+
     attr: Attribute = ...
     ink_rect: Rectangle = ...
     logical_rect: Rectangle = ...
     data: None = ...
     copy_func: Callable[..., None] = ...
     destroy_func: Callable[[None], None] = ...
     @staticmethod
@@ -281,27 +361,51 @@
         logical_rect: Rectangle,
         data: None,
         copy_func: Optional[Callable[..., None]] = None,
         destroy_func: Optional[Callable[[None], None]] = None,
     ) -> Attribute: ...
 
 class AttrSize(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        AttrSize()
+    """
+
     attr: Attribute = ...
     size: int = ...
     absolute: int = ...
     @staticmethod
     def new(size: int) -> Attribute: ...
     @staticmethod
     def new_absolute(size: int) -> Attribute: ...
 
 class AttrString(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        AttrString()
+    """
+
     attr: Attribute = ...
     value: str = ...
 
 class Attribute(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        Attribute()
+    """
+
     klass: AttrClass = ...
     start_index: int = ...
     end_index: int = ...
     def as_color(self) -> Optional[AttrColor]: ...
     def as_float(self) -> Optional[AttrFloat]: ...
     def as_font_desc(self) -> Optional[AttrFontDesc]: ...
     def as_font_features(self) -> Optional[AttrFontFeatures]: ...
@@ -312,29 +416,51 @@
     def as_string(self) -> Optional[AttrString]: ...
     def copy(self) -> Attribute: ...
     def destroy(self) -> None: ...
     def equal(self, attr2: Attribute) -> bool: ...
     def init(self, klass: AttrClass) -> None: ...
 
 class Color(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        Color()
+    """
+
     red: int = ...
     green: int = ...
     blue: int = ...
     def copy(self) -> Optional[Color]: ...
     def free(self) -> None: ...
     def parse(self, spec: str) -> bool: ...
     def parse_with_alpha(self, spec: str) -> Tuple[bool, int]: ...
     def to_string(self) -> str: ...
 
 class Context(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Context(**properties)
+        new() -> Pango.Context
+
+    Object PangoContext
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     def changed(self) -> None: ...
     def get_base_dir(self) -> Direction: ...
     def get_base_gravity(self) -> Gravity: ...
-    def get_font_description(self) -> FontDescription: ...
-    def get_font_map(self) -> FontMap: ...
+    def get_font_description(self) -> Optional[FontDescription]: ...
+    def get_font_map(self) -> Optional[FontMap]: ...
     def get_gravity(self) -> Gravity: ...
     def get_gravity_hint(self) -> GravityHint: ...
     def get_language(self) -> Language: ...
     def get_matrix(self) -> Optional[Matrix]: ...
     def get_metrics(
         self,
         desc: Optional[FontDescription] = None,
@@ -347,37 +473,64 @@
     def load_fontset(
         self, desc: FontDescription, language: Language
     ) -> Optional[Fontset]: ...
     @classmethod
     def new(cls) -> Context: ...
     def set_base_dir(self, direction: Direction) -> None: ...
     def set_base_gravity(self, gravity: Gravity) -> None: ...
-    def set_font_description(self, desc: FontDescription) -> None: ...
-    def set_font_map(self, font_map: FontMap) -> None: ...
+    def set_font_description(self, desc: Optional[FontDescription] = None) -> None: ...
+    def set_font_map(self, font_map: Optional[FontMap] = None) -> None: ...
     def set_gravity_hint(self, hint: GravityHint) -> None: ...
-    def set_language(self, language: Language) -> None: ...
+    def set_language(self, language: Optional[Language] = None) -> None: ...
     def set_matrix(self, matrix: Optional[Matrix] = None) -> None: ...
     def set_round_glyph_positions(self, round_positions: bool) -> None: ...
 
 class ContextClass(GObject.GPointer): ...
 
 class Coverage(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Coverage(**properties)
+        new() -> Pango.Coverage
+
+    Object PangoCoverage
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     def copy(self) -> Coverage: ...
     @staticmethod
     def from_bytes(bytes: Sequence[int]) -> Optional[Coverage]: ...
     def get(self, index_: int) -> CoverageLevel: ...
     def max(self, other: Coverage) -> None: ...
     @classmethod
     def new(cls) -> Coverage: ...
     def ref(self) -> Coverage: ...
     def set(self, index_: int, level: CoverageLevel) -> None: ...
     def to_bytes(self) -> bytes: ...
     def unref(self) -> None: ...
 
 class Font(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Font(**properties)
+
+    Object PangoFont
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     parent_instance: GObject.Object = ...
     def describe(self) -> FontDescription: ...
     def describe_with_absolute_size(self) -> FontDescription: ...
     @staticmethod
     def descriptions_free(
         descs: Optional[Sequence[FontDescription]] = None,
     ) -> None: ...
@@ -398,27 +551,43 @@
     def get_glyph_extents(self, glyph: int) -> Tuple[Rectangle, Rectangle]: ...
     def get_languages(self) -> Optional[list[Language]]: ...
     def get_metrics(self, language: Optional[Language] = None) -> FontMetrics: ...
     def has_char(self, wc: str) -> bool: ...
     def serialize(self) -> GLib.Bytes: ...
 
 class FontClass(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        FontClass()
+    """
+
     parent_class: GObject.ObjectClass = ...
     describe: Callable[[Font], FontDescription] = ...
     get_coverage: Callable[[Font, Language], Coverage] = ...
     get_glyph_extents: Callable[
         [Optional[Font], int], Tuple[Rectangle, Rectangle]
     ] = ...
     get_metrics: Callable[[Optional[Font], Optional[Language]], FontMetrics] = ...
     get_font_map: Callable[[Optional[Font]], Optional[FontMap]] = ...
     describe_absolute: Callable[[Font], FontDescription] = ...
     get_features: Callable[[Font], Tuple[list[HarfBuzz.feature_t], int]] = ...
     create_hb_font: Callable[[Font], HarfBuzz.font_t] = ...
 
 class FontDescription(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        new() -> Pango.FontDescription
+    """
+
     def better_match(
         self, old_match: Optional[FontDescription], new_match: FontDescription
     ) -> bool: ...
     def copy(self) -> Optional[FontDescription]: ...
     def copy_static(self) -> Optional[FontDescription]: ...
     def equal(self, desc2: FontDescription) -> bool: ...
     def free(self) -> None: ...
@@ -450,42 +619,85 @@
     def set_size(self, size: int) -> None: ...
     def set_stretch(self, stretch: Stretch) -> None: ...
     def set_style(self, style: Style) -> None: ...
     def set_variant(self, variant: Variant) -> None: ...
     def set_variations(self, variations: Optional[str] = None) -> None: ...
     def set_variations_static(self, variations: str) -> None: ...
     def set_weight(self, weight: Weight) -> None: ...
-    def to_filename(self) -> str: ...
+    def to_filename(self) -> Optional[str]: ...
     def to_string(self) -> str: ...
     def unset_fields(self, to_unset: FontMask) -> None: ...
 
 class FontFace(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        FontFace(**properties)
+
+    Object PangoFontFace
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     parent_instance: GObject.Object = ...
     def describe(self) -> FontDescription: ...
     def do_describe(self) -> FontDescription: ...
     def do_get_face_name(self) -> str: ...
     def do_get_family(self) -> FontFamily: ...
     def do_is_synthesized(self) -> bool: ...
     def do_list_sizes(self) -> list[int]: ...
     def get_face_name(self) -> str: ...
     def get_family(self) -> FontFamily: ...
     def is_synthesized(self) -> bool: ...
     def list_sizes(self) -> list[int]: ...
 
 class FontFaceClass(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        FontFaceClass()
+    """
+
     parent_class: GObject.ObjectClass = ...
     get_face_name: Callable[[FontFace], str] = ...
     describe: Callable[[FontFace], FontDescription] = ...
     list_sizes: Callable[[FontFace], list[int]] = ...
     is_synthesized: Callable[[FontFace], bool] = ...
     get_family: Callable[[FontFace], FontFamily] = ...
     _pango_reserved3: None = ...
     _pango_reserved4: None = ...
 
 class FontFamily(GObject.Object, Gio.ListModel):
+    """
+    :Constructors:
+
+    ::
+
+        FontFamily(**properties)
+
+    Object PangoFontFamily
+
+    Properties from PangoFontFamily:
+      item-type -> GType:
+
+      n-items -> guint:
+
+
+    Signals from GListModel:
+      items-changed (guint, guint, guint)
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         item_type: Type
         n_items: int
     props: Props = ...
     parent_instance: GObject.Object = ...
     def do_get_face(self, name: Optional[str] = None) -> Optional[FontFace]: ...
     def do_get_name(self) -> str: ...
@@ -495,23 +707,53 @@
     def get_face(self, name: Optional[str] = None) -> Optional[FontFace]: ...
     def get_name(self) -> str: ...
     def is_monospace(self) -> bool: ...
     def is_variable(self) -> bool: ...
     def list_faces(self) -> list[FontFace]: ...
 
 class FontFamilyClass(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        FontFamilyClass()
+    """
+
     parent_class: GObject.ObjectClass = ...
     list_faces: Callable[[FontFamily], list[FontFace]] = ...
     get_name: Callable[[FontFamily], str] = ...
     is_monospace: Callable[[FontFamily], bool] = ...
     is_variable: Callable[[FontFamily], bool] = ...
     get_face: Callable[[FontFamily, Optional[str]], Optional[FontFace]] = ...
     _pango_reserved2: None = ...
 
 class FontMap(GObject.Object, Gio.ListModel):
+    """
+    :Constructors:
+
+    ::
+
+        FontMap(**properties)
+
+    Object PangoFontMap
+
+    Properties from PangoFontMap:
+      item-type -> GType:
+
+      n-items -> guint:
+
+
+    Signals from GListModel:
+      items-changed (guint, guint, guint)
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         item_type: Type
         n_items: int
     props: Props = ...
     parent_instance: GObject.Object = ...
     def changed(self) -> None: ...
     def create_context(self) -> Context: ...
@@ -530,27 +772,43 @@
     def list_families(self) -> list[FontFamily]: ...
     def load_font(self, context: Context, desc: FontDescription) -> Optional[Font]: ...
     def load_fontset(
         self, context: Context, desc: FontDescription, language: Language
     ) -> Optional[Fontset]: ...
 
 class FontMapClass(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        FontMapClass()
+    """
+
     parent_class: GObject.ObjectClass = ...
     load_font: Callable[[FontMap, Context, FontDescription], Optional[Font]] = ...
     list_families: Callable[[FontMap], list[FontFamily]] = ...
     load_fontset: Callable[
         [FontMap, Context, FontDescription, Language], Optional[Fontset]
     ] = ...
     shape_engine_type: str = ...
     get_serial: Callable[[FontMap], int] = ...
     changed: Callable[[FontMap], None] = ...
     get_family: Callable[[FontMap, str], FontFamily] = ...
     get_face: None = ...
 
 class FontMetrics(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        FontMetrics()
+    """
+
     ref_count: int = ...
     ascent: int = ...
     descent: int = ...
     height: int = ...
     approximate_char_width: int = ...
     approximate_digit_width: int = ...
     underline_position: int = ...
@@ -566,68 +824,135 @@
     def get_strikethrough_thickness(self) -> int: ...
     def get_underline_position(self) -> int: ...
     def get_underline_thickness(self) -> int: ...
     def ref(self) -> Optional[FontMetrics]: ...
     def unref(self) -> None: ...
 
 class Fontset(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Fontset(**properties)
+
+    Object PangoFontset
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     parent_instance: GObject.Object = ...
     def do_foreach(self, func: Callable[..., bool], *data: Any) -> None: ...
     def do_get_font(self, wc: int) -> Font: ...
     def do_get_language(self) -> Language: ...
     def do_get_metrics(self) -> FontMetrics: ...
     def foreach(self, func: Callable[..., bool], *data: Any) -> None: ...
     def get_font(self, wc: int) -> Font: ...
     def get_metrics(self) -> FontMetrics: ...
 
 class FontsetClass(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        FontsetClass()
+    """
+
     parent_class: GObject.ObjectClass = ...
     get_font: Callable[[Fontset, int], Font] = ...
     get_metrics: Callable[[Fontset], FontMetrics] = ...
     get_language: Callable[[Fontset], Language] = ...
     foreach: Callable[..., None] = ...
     _pango_reserved1: None = ...
     _pango_reserved2: None = ...
     _pango_reserved3: None = ...
     _pango_reserved4: None = ...
 
 class FontsetSimple(Fontset):
+    """
+    :Constructors:
+
+    ::
+
+        FontsetSimple(**properties)
+        new(language:Pango.Language) -> Pango.FontsetSimple
+
+    Object PangoFontsetSimple
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     def append(self, font: Font) -> None: ...
     @classmethod
     def new(cls, language: Language) -> FontsetSimple: ...
     def size(self) -> int: ...
 
 class FontsetSimpleClass(GObject.GPointer): ...
 
 class GlyphGeometry(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        GlyphGeometry()
+    """
+
     width: int = ...
     x_offset: int = ...
     y_offset: int = ...
 
 class GlyphInfo(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        GlyphInfo()
+    """
+
     glyph: int = ...
     geometry: GlyphGeometry = ...
     attr: GlyphVisAttr = ...
 
 class GlyphItem(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        GlyphItem()
+    """
+
     item: Item = ...
     glyphs: GlyphString = ...
     y_offset: int = ...
     start_x_offset: int = ...
     end_x_offset: int = ...
     def apply_attrs(self, text: str, list: AttrList) -> list[GlyphItem]: ...
     def copy(self) -> Optional[GlyphItem]: ...
     def free(self) -> None: ...
     def get_logical_widths(self, text: str, logical_widths: Sequence[int]) -> None: ...
     def letter_space(
         self, text: str, log_attrs: Sequence[LogAttr], letter_spacing: int
     ) -> None: ...
-    def split(self, text: str, split_index: int) -> GlyphItem: ...
+    def split(self, text: str, split_index: int) -> Optional[GlyphItem]: ...
 
 class GlyphItemIter(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        GlyphItemIter()
+    """
+
     glyph_item: GlyphItem = ...
     text: str = ...
     start_glyph: int = ...
     start_index: int = ...
     start_char: int = ...
     end_glyph: int = ...
     end_index: int = ...
@@ -636,14 +961,23 @@
     def free(self) -> None: ...
     def init_end(self, glyph_item: GlyphItem, text: str) -> bool: ...
     def init_start(self, glyph_item: GlyphItem, text: str) -> bool: ...
     def next_cluster(self) -> bool: ...
     def prev_cluster(self) -> bool: ...
 
 class GlyphString(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        GlyphString()
+        new() -> Pango.GlyphString
+    """
+
     num_glyphs: int = ...
     glyphs: list[GlyphInfo] = ...
     log_clusters: int = ...
     space: int = ...
     def copy(self) -> Optional[GlyphString]: ...
     def extents(self, font: Font) -> Tuple[Rectangle, Rectangle]: ...
     def extents_range(
@@ -674,18 +1008,35 @@
     def new(cls) -> GlyphString: ...
     def set_size(self, new_len: int) -> None: ...
     def x_to_index(
         self, text: str, length: int, analysis: Analysis, x_pos: int
     ) -> Tuple[int, int]: ...
 
 class GlyphVisAttr(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        GlyphVisAttr()
+    """
+
     is_cluster_start: int = ...
     is_color: int = ...
 
 class Item(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        Item()
+        new() -> Pango.Item
+    """
+
     offset: int = ...
     length: int = ...
     num_chars: int = ...
     analysis: Analysis = ...
     def apply_attrs(self, iter: AttrIterator) -> None: ...
     def copy(self) -> Optional[Item]: ...
     def free(self) -> None: ...
@@ -695,22 +1046,36 @@
 
 class Language(GObject.GBoxed):
     @staticmethod
     def from_string(language: Optional[str] = None) -> Optional[Language]: ...
     @staticmethod
     def get_default() -> Language: ...
     @staticmethod
-    def get_preferred() -> Optional[Language]: ...
+    def get_preferred() -> Optional[list[Language]]: ...
     def get_sample_string(self) -> str: ...
     def get_scripts(self) -> Optional[list[Script]]: ...
     def includes_script(self, script: Script) -> bool: ...
     def matches(self, range_list: str) -> bool: ...
     def to_string(self) -> str: ...
 
 class Layout(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Layout(**properties)
+        new(context:Pango.Context) -> Pango.Layout
+
+    Object PangoLayout
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     def context_changed(self) -> None: ...
     def copy(self) -> Layout: ...
     @staticmethod
     def deserialize(
         context: Context, bytes: GLib.Bytes, flags: LayoutDeserializeFlags
     ) -> Optional[Layout]: ...
     def get_alignment(self) -> Alignment: ...
@@ -773,15 +1138,15 @@
     def set_markup_with_accel(
         self, markup: str, length: int, accel_marker: str
     ) -> str: ...
     def set_single_paragraph_mode(self, setting: bool) -> None: ...
     def set_spacing(self, spacing: int) -> None: ...
     def set_tabs(self, tabs: Optional[TabArray] = None) -> None: ...
     # override
-    def set_text(self, text: str, length=-1) -> None: ...  # FIXME Function
+    def set_text(self, text: str, length=-1) -> None: ...
     def set_width(self, width: int) -> None: ...
     def set_wrap(self, wrap: WrapMode) -> None: ...
     def write_to_file(self, flags: LayoutSerializeFlags, filename: str) -> bool: ...
     def xy_to_index(self, x: int, y: int) -> Tuple[bool, int, int]: ...
 
 class LayoutClass(GObject.GPointer): ...
 
@@ -789,30 +1154,38 @@
     def at_last_line(self) -> bool: ...
     def copy(self) -> Optional[LayoutIter]: ...
     def free(self) -> None: ...
     def get_baseline(self) -> int: ...
     def get_char_extents(self) -> Rectangle: ...
     def get_cluster_extents(self) -> Tuple[Rectangle, Rectangle]: ...
     def get_index(self) -> int: ...
-    def get_layout(self) -> Layout: ...
+    def get_layout(self) -> Optional[Layout]: ...
     def get_layout_extents(self) -> Tuple[Rectangle, Rectangle]: ...
-    def get_line(self) -> LayoutLine: ...
+    def get_line(self) -> Optional[LayoutLine]: ...
     def get_line_extents(self) -> Tuple[Rectangle, Rectangle]: ...
-    def get_line_readonly(self) -> LayoutLine: ...
+    def get_line_readonly(self) -> Optional[LayoutLine]: ...
     def get_line_yrange(self) -> Tuple[int, int]: ...
     def get_run(self) -> Optional[GlyphItem]: ...
     def get_run_baseline(self) -> int: ...
     def get_run_extents(self) -> Tuple[Rectangle, Rectangle]: ...
     def get_run_readonly(self) -> Optional[GlyphItem]: ...
     def next_char(self) -> bool: ...
     def next_cluster(self) -> bool: ...
     def next_line(self) -> bool: ...
     def next_run(self) -> bool: ...
 
 class LayoutLine(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        LayoutLine()
+    """
+
     layout: Layout = ...
     start_index: int = ...
     length: int = ...
     runs: list[GlyphItem] = ...
     is_paragraph_start: int = ...
     resolved_dir: int = ...
     def get_extents(self) -> Tuple[Rectangle, Rectangle]: ...
@@ -820,19 +1193,27 @@
     def get_length(self) -> int: ...
     def get_pixel_extents(self) -> Tuple[Rectangle, Rectangle]: ...
     def get_resolved_direction(self) -> Direction: ...
     def get_start_index(self) -> int: ...
     def get_x_ranges(self, start_index: int, end_index: int) -> list[int]: ...
     def index_to_x(self, index_: int, trailing: bool) -> int: ...
     def is_paragraph_start(self) -> bool: ...
-    def ref(self) -> LayoutLine: ...
+    def ref(self) -> Optional[LayoutLine]: ...
     def unref(self) -> None: ...
     def x_to_index(self, x_pos: int) -> Tuple[bool, int, int]: ...
 
 class LogAttr(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        LogAttr()
+    """
+
     is_line_break: int = ...
     is_mandatory_break: int = ...
     is_char_break: int = ...
     is_white: int = ...
     is_cursor_position: int = ...
     is_word_start: int = ...
     is_word_end: int = ...
@@ -843,14 +1224,22 @@
     is_expandable_space: int = ...
     is_word_boundary: int = ...
     break_inserts_hyphen: int = ...
     break_removes_preceding: int = ...
     reserved: int = ...
 
 class Matrix(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        Matrix()
+    """
+
     xx: float = ...
     xy: float = ...
     yx: float = ...
     yy: float = ...
     x0: float = ...
     y0: float = ...
     def concat(self, new_matrix: Matrix) -> None: ...
@@ -864,20 +1253,41 @@
     def transform_distance(self) -> Tuple[float, float]: ...
     def transform_pixel_rectangle(self) -> Rectangle: ...
     def transform_point(self) -> Tuple[float, float]: ...
     def transform_rectangle(self) -> Rectangle: ...
     def translate(self, tx: float, ty: float) -> None: ...
 
 class Rectangle(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        Rectangle()
+    """
+
     x: int = ...
     y: int = ...
     width: int = ...
     height: int = ...
 
 class Renderer(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Renderer(**properties)
+
+    Object PangoRenderer
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     parent_instance: GObject.Object = ...
     underline: Underline = ...
     strikethrough: bool = ...
     active_count: int = ...
     matrix: Matrix = ...
     priv: RendererPrivate = ...
     def activate(self) -> None: ...
@@ -938,14 +1348,22 @@
     def get_matrix(self) -> Optional[Matrix]: ...
     def part_changed(self, part: RenderPart) -> None: ...
     def set_alpha(self, part: RenderPart, alpha: int) -> None: ...
     def set_color(self, part: RenderPart, color: Optional[Color] = None) -> None: ...
     def set_matrix(self, matrix: Optional[Matrix] = None) -> None: ...
 
 class RendererClass(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        RendererClass()
+    """
+
     parent_class: GObject.ObjectClass = ...
     draw_glyphs: Callable[[Renderer, Font, GlyphString, int, int], None] = ...
     draw_rectangle: Callable[[Renderer, RenderPart, int, int, int, int], None] = ...
     draw_error_underline: Callable[[Renderer, int, int, int, int], None] = ...
     draw_shape: Callable[[Renderer, AttrShape, int, int], None] = ...
     draw_trapezoid: Callable[
         [Renderer, RenderPart, float, float, float, float, float, float], None
@@ -961,21 +1379,37 @@
     _pango_reserved2: None = ...
     _pango_reserved3: None = ...
     _pango_reserved4: None = ...
 
 class RendererPrivate(GObject.GPointer): ...
 
 class ScriptIter(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        new(text:str, length:int) -> Pango.ScriptIter
+    """
+
     def free(self) -> None: ...
     def get_range(self) -> Tuple[str, str, Script]: ...
     @classmethod
     def new(cls, text: str, length: int) -> ScriptIter: ...
     def next(self) -> bool: ...
 
 class TabArray(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        new(initial_size:int, positions_in_pixels:bool) -> Pango.TabArray
+    """
+
     def copy(self) -> TabArray: ...
     def free(self) -> None: ...
     @staticmethod
     def from_string(text: str) -> Optional[TabArray]: ...
     def get_decimal_point(self, tab_index: int) -> str: ...
     def get_positions_in_pixels(self) -> bool: ...
     def get_size(self) -> int: ...
```

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/PangoCairo.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/PangoCairo.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,45 @@
-from __future__ import annotations
-
+from typing import Any
+from typing import Callable
 from typing import Optional
 from typing import TypeVar
 
 import cairo
 from gi.repository import GObject
 from gi.repository import Pango
 
-_namespace: str = ...
-_version: str = ...
-
 _SomeSurface = TypeVar("_SomeSurface", bound=cairo.Surface)
 
+_lock = ...  # FIXME Constant
+_namespace: str = "PangoCairo"
+_version: str = "1.0"
+
 def context_get_font_options(context: Pango.Context) -> Optional[cairo.FontOptions]: ...
 def context_get_resolution(context: Pango.Context) -> float: ...
 def context_set_font_options(
-    context: Pango.Context, options: Optional[cairo.FontOptions]
-): ...
+    context: Pango.Context, options: Optional[cairo.FontOptions] = None
+) -> None: ...
 def context_set_resolution(context: Pango.Context, dpi: float) -> None: ...
-def context_set_shape_renderer(*args, **kwargs): ...
+def context_set_shape_renderer(
+    context: Pango.Context, func: Optional[Callable[..., None]] = None, *data: Any
+) -> None: ...
 def create_context(cr: cairo.Context[_SomeSurface]) -> Pango.Context: ...
 def create_layout(cr: cairo.Context[_SomeSurface]) -> Pango.Layout: ...
 def error_underline_path(
     cr: cairo.Context[_SomeSurface], x: float, y: float, width: float, height: float
 ) -> None: ...
 def font_map_get_default() -> Pango.FontMap: ...
 def font_map_new() -> Pango.FontMap: ...
 def font_map_new_for_font_type(fonttype: cairo.FontType) -> Optional[Pango.FontMap]: ...
 def glyph_string_path(
     cr: cairo.Context[_SomeSurface], font: Pango.Font, glyphs: Pango.GlyphString
 ) -> None: ...
-def layout_line_path(cr: cairo.Context[_SomeSurface], line: Pango.LayoutLine): ...
+def layout_line_path(
+    cr: cairo.Context[_SomeSurface], line: Pango.LayoutLine
+) -> None: ...
 def layout_path(cr: cairo.Context[_SomeSurface], layout: Pango.Layout) -> None: ...
 def show_error_underline(
     cr: cairo.Context[_SomeSurface], x: float, y: float, width: float, height: float
 ) -> None: ...
 def show_glyph_item(
     cr: cairo.Context[_SomeSurface], text: str, glyph_item: Pango.GlyphItem
 ) -> None: ...
@@ -45,17 +50,37 @@
 def show_layout_line(
     cr: cairo.Context[_SomeSurface], line: Pango.LayoutLine
 ) -> None: ...
 def update_context(cr: cairo.Context[_SomeSurface], context: Pango.Context) -> None: ...
 def update_layout(cr: cairo.Context[_SomeSurface], layout: Pango.Layout) -> None: ...
 
 class Font(GObject.GInterface):
+    """
+    Interface PangoCairoFont
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     def get_scaled_font(self) -> Optional[cairo.ScaledFont]: ...
 
 class FontMap(GObject.GInterface):
+    """
+    Interface PangoCairoFontMap
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
+    # override
+    @classmethod
     def get_default(cls) -> Pango.FontMap: ...
     def get_font_type(self) -> cairo.FontType: ...
     def get_resolution(self) -> float: ...
+    # override
+    @classmethod
     def new(cls) -> Pango.FontMap: ...
+    # override
+    @classmethod
     def new_for_font_type(cls, fonttype: cairo.FontType) -> Optional[Pango.FontMap]: ...
     def set_default(self) -> None: ...
     def set_resolution(self, dpi: float) -> None: ...
```

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Rsvg.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/Rsvg.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/Vte.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/Vte.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gdk3.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/_Gdk3.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gdk4.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/_Gdk4.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2332,42 +2332,32 @@
 def cairo_set_source_rgba(cr: cairo.Context[_SomeSurface], rgba: RGBA) -> None: ...
 def content_deserialize_async(
     stream: Gio.InputStream,
     mime_type: str,
     type: Type,
     io_priority: int,
     cancellable: Optional[Gio.Cancellable] = None,
-    callback: Optional[
-        Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
-    ] = None,
+    callback: Optional[Callable[..., None]] = None,
     *user_data: Any,
 ) -> None: ...
 def content_deserialize_finish(result: Gio.AsyncResult) -> Tuple[bool, Any]: ...
 def content_formats_parse(string: str) -> Optional[ContentFormats]: ...
 def content_register_deserializer(
-    mime_type: str,
-    type: Type,
-    deserialize: Callable[[ContentDeserializer], None],
-    *data: Any,
+    mime_type: str, type: Type, deserialize: Callable[..., None], *data: Any
 ) -> None: ...
 def content_register_serializer(
-    type: Type,
-    mime_type: str,
-    serialize: Callable[[ContentSerializer], None],
-    *data: Any,
+    type: Type, mime_type: str, serialize: Callable[..., None], *data: Any
 ) -> None: ...
 def content_serialize_async(
     stream: Gio.OutputStream,
     mime_type: str,
     value: Any,
     io_priority: int,
     cancellable: Optional[Gio.Cancellable] = None,
-    callback: Optional[
-        Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
-    ] = None,
+    callback: Optional[Callable[..., None]] = None,
     *user_data: Any,
 ) -> None: ...
 def content_serialize_finish(result: Gio.AsyncResult) -> bool: ...
 def drag_action_is_unique(action: DragAction) -> bool: ...
 def events_get_angle(event1: Event, event2: Event) -> Tuple[bool, float]: ...
 def events_get_center(event1: Event, event2: Event) -> Tuple[bool, float, float]: ...
 def events_get_distance(event1: Event, event2: Event) -> Tuple[bool, float]: ...
@@ -2389,36 +2379,104 @@
 def set_allowed_backends(backends: str) -> None: ...
 def texture_error_quark() -> int: ...
 def toplevel_size_get_type() -> Type: ...
 def unicode_to_keyval(wc: int) -> int: ...
 def vulkan_error_quark() -> int: ...
 
 class AppLaunchContext(Gio.AppLaunchContext):
+    """
+    :Constructors:
+
+    ::
+
+        AppLaunchContext(**properties)
+
+    Object GdkAppLaunchContext
+
+    Properties from GdkAppLaunchContext:
+      display -> GdkDisplay: display
+
+    Signals from GAppLaunchContext:
+      launch-failed (gchararray)
+      launch-started (GAppInfo, GVariant)
+      launched (GAppInfo, GVariant)
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         display: Display
     props: Props = ...
     def __init__(self, display: Display = ...): ...
     def get_display(self) -> Display: ...
     def set_desktop(self, desktop: int) -> None: ...
     def set_icon(self, icon: Optional[Gio.Icon] = None) -> None: ...
     def set_icon_name(self, icon_name: Optional[str] = None) -> None: ...
     def set_timestamp(self, timestamp: int) -> None: ...
 
 class ButtonEvent(Event):
+    """
+    :Constructors:
+
+    ::
+
+        ButtonEvent(**properties)
+    """
+
     def get_button(self) -> int: ...
 
 class CairoContext(DrawContext):
+    """
+    :Constructors:
+
+    ::
+
+        CairoContext(**properties)
+
+    Object GdkCairoContext
+
+    Properties from GdkDrawContext:
+      display -> GdkDisplay: display
+      surface -> GdkSurface: surface
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         display: Optional[Display]
         surface: Optional[Surface]
     props: Props = ...
     def __init__(self, display: Display = ..., surface: Surface = ...): ...
     def cairo_create(self) -> Optional[cairo.Context]: ...
 
 class Clipboard(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Clipboard(**properties)
+
+    Object GdkClipboard
+
+    Signals from GdkClipboard:
+      changed ()
+
+    Properties from GdkClipboard:
+      display -> GdkDisplay: display
+      formats -> GdkContentFormats: formats
+      local -> gboolean: local
+      content -> GdkContentProvider: content
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         content: Optional[ContentProvider]
         display: Display
         formats: ContentFormats
         local: bool
     props: Props = ...
     def __init__(self, display: Display = ...): ...
@@ -2427,78 +2485,90 @@
     def get_formats(self) -> ContentFormats: ...
     def is_local(self) -> bool: ...
     def read_async(
         self,
         mime_types: Sequence[str],
         io_priority: int,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[
-            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
-        ] = None,
+        callback: Optional[Callable[..., None]] = None,
         *user_data: Any,
     ) -> None: ...
     def read_finish(
         self, result: Gio.AsyncResult
     ) -> Tuple[Optional[Gio.InputStream], str]: ...
     def read_text_async(
         self,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[
-            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
-        ] = None,
+        callback: Optional[Callable[..., None]] = None,
         *user_data: Any,
     ) -> None: ...
     def read_text_finish(self, result: Gio.AsyncResult) -> Optional[str]: ...
     def read_texture_async(
         self,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[
-            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
-        ] = None,
+        callback: Optional[Callable[..., None]] = None,
         *user_data: Any,
     ) -> None: ...
     def read_texture_finish(self, result: Gio.AsyncResult) -> Optional[Texture]: ...
     def read_value_async(
         self,
         type: Type,
         io_priority: int,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[
-            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
-        ] = None,
+        callback: Optional[Callable[..., None]] = None,
         *user_data: Any,
     ) -> None: ...
     def read_value_finish(self, result: Gio.AsyncResult) -> Any: ...
     def set(self, value: Any) -> None: ...
     def set_content(self, provider: Optional[ContentProvider] = None) -> bool: ...
     def store_async(
         self,
         io_priority: int,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[
-            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
-        ] = None,
+        callback: Optional[Callable[..., None]] = None,
         *user_data: Any,
     ) -> None: ...
     def store_finish(self, result: Gio.AsyncResult) -> bool: ...
 
 class ContentDeserializer(GObject.Object, Gio.AsyncResult):
+    """
+    :Constructors:
+
+    ::
+
+        ContentDeserializer(**properties)
+
+    Object GdkContentDeserializer
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     def get_cancellable(self) -> Optional[Gio.Cancellable]: ...
     def get_gtype(self) -> Type: ...
     def get_input_stream(self) -> Gio.InputStream: ...
     def get_mime_type(self) -> str: ...
     def get_priority(self) -> int: ...
     def get_task_data(self) -> None: ...
     def get_user_data(self) -> None: ...
     def get_value(self) -> Any: ...
     def return_error(self, error: GLib.Error) -> None: ...
     def return_success(self) -> None: ...
     def set_task_data(self, data: None, notify: Callable[[None], None]) -> None: ...
 
 class ContentFormats(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        new(mime_types:list=None) -> Gdk.ContentFormats
+        new_for_gtype(type:GType) -> Gdk.ContentFormats
+    """
+
     def contain_gtype(self, type: Type) -> bool: ...
     def contain_mime_type(self, mime_type: str) -> bool: ...
     def get_gtypes(self) -> Optional[list[Type]]: ...
     def get_mime_types(self) -> Optional[list[str]]: ...
     def match(self, second: ContentFormats) -> bool: ...
     def match_gtype(self, second: ContentFormats) -> Type: ...
     def match_mime_type(self, second: ContentFormats) -> Optional[str]: ...
@@ -2515,24 +2585,55 @@
     def union_deserialize_gtypes(self) -> ContentFormats: ...
     def union_deserialize_mime_types(self) -> ContentFormats: ...
     def union_serialize_gtypes(self) -> ContentFormats: ...
     def union_serialize_mime_types(self) -> ContentFormats: ...
     def unref(self) -> None: ...
 
 class ContentFormatsBuilder(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        new() -> Gdk.ContentFormatsBuilder
+    """
+
     def add_formats(self, formats: ContentFormats) -> None: ...
     def add_gtype(self, type: Type) -> None: ...
     def add_mime_type(self, mime_type: str) -> None: ...
     @classmethod
     def new(cls) -> ContentFormatsBuilder: ...
     def ref(self) -> ContentFormatsBuilder: ...
     def to_formats(self) -> ContentFormats: ...
     def unref(self) -> None: ...
 
 class ContentProvider(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        ContentProvider(**properties)
+        new_for_bytes(mime_type:str, bytes:GLib.Bytes) -> Gdk.ContentProvider
+        new_for_value(value:GObject.Value) -> Gdk.ContentProvider
+        new_union(providers:list=None) -> Gdk.ContentProvider
+
+    Object GdkContentProvider
+
+    Signals from GdkContentProvider:
+      content-changed ()
+
+    Properties from GdkContentProvider:
+      formats -> GdkContentFormats: formats
+      storable-formats -> GdkContentFormats: storable-formats
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         formats: ContentFormats
         storable_formats: ContentFormats
     props: Props = ...
     parent: GObject.Object = ...
     def content_changed(self) -> None: ...
     def do_attach_clipboard(self, clipboard: Clipboard) -> None: ...
@@ -2543,17 +2644,15 @@
     def do_ref_storable_formats(self) -> ContentFormats: ...
     def do_write_mime_type_async(
         self,
         mime_type: str,
         stream: Gio.OutputStream,
         io_priority: int,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[
-            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
-        ] = None,
+        callback: Optional[Callable[..., None]] = None,
         *user_data: Any,
     ) -> None: ...
     def do_write_mime_type_finish(self, result: Gio.AsyncResult) -> bool: ...
     def get_value(self) -> Tuple[bool, Any]: ...
     @classmethod
     def new_for_bytes(cls, mime_type: str, bytes: GLib.Bytes) -> ContentProvider: ...
     @classmethod
@@ -2566,52 +2665,101 @@
     def ref_storable_formats(self) -> ContentFormats: ...
     def write_mime_type_async(
         self,
         mime_type: str,
         stream: Gio.OutputStream,
         io_priority: int,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[
-            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
-        ] = None,
+        callback: Optional[Callable[..., None]] = None,
         *user_data: Any,
     ) -> None: ...
     def write_mime_type_finish(self, result: Gio.AsyncResult) -> bool: ...
 
 class ContentProviderClass(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        ContentProviderClass()
+    """
+
     parent_class: GObject.ObjectClass = ...
     content_changed: Callable[[ContentProvider], None] = ...
     attach_clipboard: Callable[[ContentProvider, Clipboard], None] = ...
     detach_clipboard: Callable[[ContentProvider, Clipboard], None] = ...
     ref_formats: Callable[[ContentProvider], ContentFormats] = ...
     ref_storable_formats: Callable[[ContentProvider], ContentFormats] = ...
     write_mime_type_async: Callable[..., None] = ...
     write_mime_type_finish: Callable[[ContentProvider, Gio.AsyncResult], bool] = ...
     get_value: Callable[[ContentProvider], Tuple[bool, Any]] = ...
     padding: list[None] = ...
 
 class ContentSerializer(GObject.Object, Gio.AsyncResult):
+    """
+    :Constructors:
+
+    ::
+
+        ContentSerializer(**properties)
+
+    Object GdkContentSerializer
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     def get_cancellable(self) -> Optional[Gio.Cancellable]: ...
     def get_gtype(self) -> Type: ...
     def get_mime_type(self) -> str: ...
     def get_output_stream(self) -> Gio.OutputStream: ...
     def get_priority(self) -> int: ...
     def get_task_data(self) -> None: ...
     def get_user_data(self) -> None: ...
     def get_value(self) -> Any: ...
     def return_error(self, error: GLib.Error) -> None: ...
     def return_success(self) -> None: ...
     def set_task_data(self, data: None, notify: Callable[[None], None]) -> None: ...
 
 class CrossingEvent(Event):
+    """
+    :Constructors:
+
+    ::
+
+        CrossingEvent(**properties)
+    """
+
     def get_detail(self) -> NotifyType: ...
     def get_focus(self) -> bool: ...
     def get_mode(self) -> CrossingMode: ...
 
 class Cursor(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Cursor(**properties)
+        new_from_name(name:str, fallback:Gdk.Cursor=None) -> Gdk.Cursor or None
+        new_from_texture(texture:Gdk.Texture, hotspot_x:int, hotspot_y:int, fallback:Gdk.Cursor=None) -> Gdk.Cursor
+
+    Object GdkCursor
+
+    Properties from GdkCursor:
+      fallback -> GdkCursor: fallback
+      hotspot-x -> gint: hotspot-x
+      hotspot-y -> gint: hotspot-y
+      name -> gchararray: name
+      texture -> GdkTexture: texture
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         fallback: Optional[Cursor]
         hotspot_x: int
         hotspot_y: int
         name: Optional[str]
         texture: Optional[Texture]
     props: Props = ...
@@ -2638,19 +2786,62 @@
         texture: Texture,
         hotspot_x: int,
         hotspot_y: int,
         fallback: Optional[Cursor] = None,
     ) -> Cursor: ...
 
 class DNDEvent(Event):
+    """
+    :Constructors:
+
+    ::
+
+        DNDEvent(**properties)
+    """
+
     def get_drop(self) -> Optional[Drop]: ...
 
 class DeleteEvent(Event): ...
 
 class Device(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Device(**properties)
+
+    Object GdkDevice
+
+    Signals from GdkDevice:
+      changed ()
+      tool-changed (GdkDeviceTool)
+
+    Properties from GdkDevice:
+      display -> GdkDisplay: display
+      name -> gchararray: name
+      source -> GdkInputSource: source
+      has-cursor -> gboolean: has-cursor
+      n-axes -> guint: n-axes
+      vendor-id -> gchararray: vendor-id
+      product-id -> gchararray: product-id
+      seat -> GdkSeat: seat
+      num-touches -> guint: num-touches
+      tool -> GdkDeviceTool: tool
+      direction -> PangoDirection: direction
+      has-bidi-layouts -> gboolean: has-bidi-layouts
+      caps-lock-state -> gboolean: caps-lock-state
+      num-lock-state -> gboolean: num-lock-state
+      scroll-lock-state -> gboolean: scroll-lock-state
+      modifier-state -> GdkModifierType: modifier-state
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         caps_lock_state: bool
         direction: Pango.Direction
         display: Display
         has_bidi_layouts: bool
         has_cursor: bool
         modifier_state: ModifierType
@@ -2691,22 +2882,48 @@
     def get_source(self) -> InputSource: ...
     def get_surface_at_position(self) -> Tuple[Optional[Surface], float, float]: ...
     def get_timestamp(self) -> int: ...
     def get_vendor_id(self) -> Optional[str]: ...
     def has_bidi_layouts(self) -> bool: ...
 
 class DevicePad(GObject.GInterface):
+    """
+    Interface GdkDevicePad
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     def get_feature_group(self, feature: DevicePadFeature, feature_idx: int) -> int: ...
     def get_group_n_modes(self, group_idx: int) -> int: ...
     def get_n_features(self, feature: DevicePadFeature) -> int: ...
     def get_n_groups(self) -> int: ...
 
 class DevicePadInterface(GObject.GPointer): ...
 
 class DeviceTool(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        DeviceTool(**properties)
+
+    Object GdkDeviceTool
+
+    Properties from GdkDeviceTool:
+      serial -> guint64: serial
+      tool-type -> GdkDeviceToolType: tool-type
+      axes -> GdkAxisFlags: axes
+      hardware-id -> guint64: hardware-id
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         axes: AxisFlags
         hardware_id: int
         serial: int
         tool_type: DeviceToolType
     props: Props = ...
     def __init__(
@@ -2718,14 +2935,39 @@
     ): ...
     def get_axes(self) -> AxisFlags: ...
     def get_hardware_id(self) -> int: ...
     def get_serial(self) -> int: ...
     def get_tool_type(self) -> DeviceToolType: ...
 
 class Display(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Display(**properties)
+
+    Object GdkDisplay
+
+    Signals from GdkDisplay:
+      opened ()
+      closed (gboolean)
+      seat-added (GdkSeat)
+      seat-removed (GdkSeat)
+      setting-changed (gchararray)
+
+    Properties from GdkDisplay:
+      composited -> gboolean: composited
+      rgba -> gboolean: rgba
+      input-shapes -> gboolean: input-shapes
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         composited: bool
         input_shapes: bool
         rgba: bool
     props: Props = ...
     def beep(self) -> None: ...
     def close(self) -> None: ...
@@ -2757,26 +2999,72 @@
     def supports_input_shapes(self) -> bool: ...
     def sync(self) -> None: ...
     def translate_key(
         self, keycode: int, state: ModifierType, group: int
     ) -> Tuple[bool, int, int, int, ModifierType]: ...
 
 class DisplayManager(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        DisplayManager(**properties)
+
+    Object GdkDisplayManager
+
+    Signals from GdkDisplayManager:
+      display-opened (GdkDisplay)
+
+    Properties from GdkDisplayManager:
+      default-display -> GdkDisplay: default-display
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         default_display: Optional[Display]
     props: Props = ...
     def __init__(self, default_display: Display = ...): ...
     @staticmethod
     def get() -> DisplayManager: ...
     def get_default_display(self) -> Optional[Display]: ...
     def list_displays(self) -> list[Display]: ...
     def open_display(self, name: str) -> Optional[Display]: ...
     def set_default_display(self, display: Display) -> None: ...
 
 class Drag(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Drag(**properties)
+
+    Object GdkDrag
+
+    Signals from GdkDrag:
+      cancel (GdkDragCancelReason)
+      drop-performed ()
+      dnd-finished ()
+
+    Properties from GdkDrag:
+      content -> GdkContentProvider: content
+      device -> GdkDevice: device
+      display -> GdkDisplay: display
+      formats -> GdkContentFormats: formats
+      selected-action -> GdkDragAction: selected-action
+      actions -> GdkDragAction: actions
+      surface -> GdkSurface: surface
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         actions: DragAction
         content: ContentProvider
         device: Device
         display: Display
         formats: ContentFormats
         selected_action: DragAction
@@ -2808,32 +3096,77 @@
     def get_drag_surface(self) -> Optional[Surface]: ...
     def get_formats(self) -> ContentFormats: ...
     def get_selected_action(self) -> DragAction: ...
     def get_surface(self) -> Surface: ...
     def set_hotspot(self, hot_x: int, hot_y: int) -> None: ...
 
 class DragSurface(GObject.GInterface):
+    """
+    Interface GdkDragSurface
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     def present(self, width: int, height: int) -> bool: ...
 
 class DragSurfaceInterface(GObject.GPointer): ...
 
 class DrawContext(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        DrawContext(**properties)
+
+    Object GdkDrawContext
+
+    Properties from GdkDrawContext:
+      display -> GdkDisplay: display
+      surface -> GdkSurface: surface
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         display: Optional[Display]
         surface: Optional[Surface]
     props: Props = ...
     def __init__(self, display: Display = ..., surface: Surface = ...): ...
     def begin_frame(self, region: cairo.Region) -> None: ...
     def end_frame(self) -> None: ...
     def get_display(self) -> Optional[Display]: ...
     def get_frame_region(self) -> Optional[cairo.Region]: ...
     def get_surface(self) -> Optional[Surface]: ...
     def is_in_frame(self) -> bool: ...
 
 class Drop(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Drop(**properties)
+
+    Object GdkDrop
+
+    Properties from GdkDrop:
+      actions -> GdkDragAction: actions
+      device -> GdkDevice: device
+      display -> GdkDisplay: display
+      drag -> GdkDrag: drag
+      formats -> GdkContentFormats: formats
+      surface -> GdkSurface: surface
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         actions: DragAction
         device: Device
         display: Display
         drag: Optional[Drag]
         formats: ContentFormats
         surface: Surface
@@ -2854,36 +3187,40 @@
     def get_formats(self) -> ContentFormats: ...
     def get_surface(self) -> Surface: ...
     def read_async(
         self,
         mime_types: Sequence[str],
         io_priority: int,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[
-            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
-        ] = None,
+        callback: Optional[Callable[..., None]] = None,
         *user_data: Any,
     ) -> None: ...
     def read_finish(
         self, result: Gio.AsyncResult
     ) -> Tuple[Optional[Gio.InputStream], str]: ...
     def read_value_async(
         self,
         type: Type,
         io_priority: int,
         cancellable: Optional[Gio.Cancellable] = None,
-        callback: Optional[
-            Callable[[Optional[GObject.Object], Gio.AsyncResult, None], None]
-        ] = None,
+        callback: Optional[Callable[..., None]] = None,
         *user_data: Any,
     ) -> None: ...
     def read_value_finish(self, result: Gio.AsyncResult) -> Any: ...
     def status(self, actions: DragAction, preferred: DragAction) -> None: ...
 
 class Event:
+    """
+    :Constructors:
+
+    ::
+
+        Event(**properties)
+    """
+
     def get_axes(self) -> Tuple[bool, list[float]]: ...
     def get_axis(self, axis_use: AxisUse) -> Tuple[bool, float]: ...
     def get_device(self) -> Optional[Device]: ...
     def get_device_tool(self) -> Optional[DeviceTool]: ...
     def get_display(self) -> Optional[Display]: ...
     def get_event_sequence(self) -> EventSequence: ...
     def get_event_type(self) -> EventType: ...
@@ -2897,24 +3234,63 @@
     def ref(self) -> Event: ...
     def triggers_context_menu(self) -> bool: ...
     def unref(self) -> None: ...
 
 class EventSequence(GObject.GBoxed): ...
 
 class FileList(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        new_from_array(files:list) -> Gdk.FileList
+        new_from_list(files:list) -> Gdk.FileList
+    """
+
     def get_files(self) -> list[Gio.File]: ...
     @classmethod
     def new_from_array(cls, files: Sequence[Gio.File]) -> FileList: ...
     @classmethod
     def new_from_list(cls, files: list[Gio.File]) -> FileList: ...
 
 class FocusEvent(Event):
+    """
+    :Constructors:
+
+    ::
+
+        FocusEvent(**properties)
+    """
+
     def get_in(self) -> bool: ...
 
 class FrameClock(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        FrameClock(**properties)
+
+    Object GdkFrameClock
+
+    Signals from GdkFrameClock:
+      flush-events ()
+      before-paint ()
+      update ()
+      layout ()
+      paint ()
+      after-paint ()
+      resume-events ()
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     def begin_updating(self) -> None: ...
     def end_updating(self) -> None: ...
     def get_current_timings(self) -> Optional[FrameTimings]: ...
     def get_fps(self) -> float: ...
     def get_frame_counter(self) -> int: ...
     def get_frame_time(self) -> int: ...
     def get_history_start(self) -> int: ...
@@ -2932,14 +3308,36 @@
     def get_predicted_presentation_time(self) -> int: ...
     def get_presentation_time(self) -> int: ...
     def get_refresh_interval(self) -> int: ...
     def ref(self) -> FrameTimings: ...
     def unref(self) -> None: ...
 
 class GLContext(DrawContext):
+    """
+    :Constructors:
+
+    ::
+
+        GLContext(**properties)
+
+    Object GdkGLContext
+
+    Properties from GdkGLContext:
+      allowed-apis -> GdkGLAPI: allowed-apis
+      api -> GdkGLAPI: api
+      shared-context -> GdkGLContext: shared-context
+
+    Properties from GdkDrawContext:
+      display -> GdkDisplay: display
+      surface -> GdkSurface: surface
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         allowed_apis: GLAPI
         api: GLAPI
         shared_context: Optional[GLContext]
         display: Optional[Display]
         surface: Optional[Surface]
     props: Props = ...
@@ -2971,14 +3369,40 @@
     def set_allowed_apis(self, apis: GLAPI) -> None: ...
     def set_debug_enabled(self, enabled: bool) -> None: ...
     def set_forward_compatible(self, compatible: bool) -> None: ...
     def set_required_version(self, major: int, minor: int) -> None: ...
     def set_use_es(self, use_es: int) -> None: ...
 
 class GLTexture(Texture, Paintable, Gio.Icon, Gio.LoadableIcon):
+    """
+    :Constructors:
+
+    ::
+
+        GLTexture(**properties)
+        new(context:Gdk.GLContext, id:int, width:int, height:int, destroy:GLib.DestroyNotify, data=None) -> Gdk.GLTexture
+
+    Object GdkGLTexture
+
+    Signals from GdkPaintable:
+      invalidate-contents ()
+      invalidate-size ()
+
+    Properties from GdkTexture:
+      width -> gint: width
+      height -> gint: height
+
+    Signals from GdkPaintable:
+      invalidate-contents ()
+      invalidate-size ()
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         height: int
         width: int
     props: Props = ...
     def __init__(self, height: int = ..., width: int = ...): ...
     @classmethod
     def new(
@@ -2991,33 +3415,83 @@
         data: None,
     ) -> GLTexture: ...
     def release(self) -> None: ...
 
 class GLTextureClass(GObject.GPointer): ...
 
 class GrabBrokenEvent(Event):
+    """
+    :Constructors:
+
+    ::
+
+        GrabBrokenEvent(**properties)
+    """
+
     def get_grab_surface(self) -> Surface: ...
     def get_implicit(self) -> bool: ...
 
 class KeyEvent(Event):
+    """
+    :Constructors:
+
+    ::
+
+        KeyEvent(**properties)
+    """
+
     def get_consumed_modifiers(self) -> ModifierType: ...
     def get_keycode(self) -> int: ...
     def get_keyval(self) -> int: ...
     def get_layout(self) -> int: ...
     def get_level(self) -> int: ...
     def get_match(self) -> Tuple[bool, int, ModifierType]: ...
     def is_modifier(self) -> bool: ...
     def matches(self, keyval: int, modifiers: ModifierType) -> KeyMatch: ...
 
 class KeymapKey(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        KeymapKey()
+    """
+
     keycode: int = ...
     group: int = ...
     level: int = ...
 
 class MemoryTexture(Texture, Paintable, Gio.Icon, Gio.LoadableIcon):
+    """
+    :Constructors:
+
+    ::
+
+        MemoryTexture(**properties)
+        new(width:int, height:int, format:Gdk.MemoryFormat, bytes:GLib.Bytes, stride:int) -> Gdk.MemoryTexture
+
+    Object GdkMemoryTexture
+
+    Signals from GdkPaintable:
+      invalidate-contents ()
+      invalidate-size ()
+
+    Properties from GdkTexture:
+      width -> gint: width
+      height -> gint: height
+
+    Signals from GdkPaintable:
+      invalidate-contents ()
+      invalidate-size ()
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         height: int
         width: int
     props: Props = ...
     def __init__(self, height: int = ..., width: int = ...): ...
     @classmethod
     def new(
@@ -3028,14 +3502,44 @@
         bytes: GLib.Bytes,
         stride: int,
     ) -> MemoryTexture: ...
 
 class MemoryTextureClass(GObject.GPointer): ...
 
 class Monitor(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Monitor(**properties)
+
+    Object GdkMonitor
+
+    Signals from GdkMonitor:
+      invalidate ()
+
+    Properties from GdkMonitor:
+      description -> gchararray: description
+      display -> GdkDisplay: display
+      manufacturer -> gchararray: manufacturer
+      model -> gchararray: model
+      connector -> gchararray: connector
+      scale-factor -> gint: scale-factor
+      geometry -> GdkRectangle: geometry
+      width-mm -> gint: width-mm
+      height-mm -> gint: height-mm
+      refresh-rate -> gint: refresh-rate
+      subpixel-layout -> GdkSubpixelLayout: subpixel-layout
+      valid -> gboolean: valid
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         connector: Optional[str]
         description: Optional[str]
         display: Display
         geometry: Rectangle
         height_mm: int
         manufacturer: Optional[str]
@@ -3060,19 +3564,34 @@
     def get_width_mm(self) -> int: ...
     def is_valid(self) -> bool: ...
 
 class MonitorClass(GObject.GPointer): ...
 class MotionEvent(Event): ...
 
 class PadEvent(Event):
+    """
+    :Constructors:
+
+    ::
+
+        PadEvent(**properties)
+    """
+
     def get_axis_value(self) -> Tuple[int, float]: ...
     def get_button(self) -> int: ...
     def get_group_mode(self) -> Tuple[int, int]: ...
 
 class Paintable(GObject.GInterface):
+    """
+    Interface GdkPaintable
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     def compute_concrete_size(
         self,
         specified_width: float,
         specified_height: float,
         default_width: float,
         default_height: float,
     ) -> Tuple[float, float]: ...
@@ -3084,34 +3603,57 @@
     def invalidate_contents(self) -> None: ...
     def invalidate_size(self) -> None: ...
     @staticmethod
     def new_empty(intrinsic_width: int, intrinsic_height: int) -> Paintable: ...
     def snapshot(self, snapshot: Snapshot, width: float, height: float) -> None: ...
 
 class PaintableInterface(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        PaintableInterface()
+    """
+
     g_iface: GObject.TypeInterface = ...
     snapshot: Callable[[Paintable, Snapshot, float, float], None] = ...
     get_current_image: Callable[[Paintable], Paintable] = ...
     get_flags: Callable[[Paintable], PaintableFlags] = ...
     get_intrinsic_width: Callable[[Paintable], int] = ...
     get_intrinsic_height: Callable[[Paintable], int] = ...
     get_intrinsic_aspect_ratio: Callable[[Paintable], float] = ...
 
 class Popup(GObject.GInterface):
+    """
+    Interface GdkPopup
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     def get_autohide(self) -> bool: ...
     def get_parent(self) -> Optional[Surface]: ...
     def get_position_x(self) -> int: ...
     def get_position_y(self) -> int: ...
     def get_rect_anchor(self) -> Gravity: ...
     def get_surface_anchor(self) -> Gravity: ...
     def present(self, width: int, height: int, layout: PopupLayout) -> bool: ...
 
 class PopupInterface(GObject.GPointer): ...
 
 class PopupLayout(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        new(anchor_rect:Gdk.Rectangle, rect_anchor:Gdk.Gravity, surface_anchor:Gdk.Gravity) -> Gdk.PopupLayout
+    """
+
     def copy(self) -> PopupLayout: ...
     def equal(self, other: PopupLayout) -> bool: ...
     def get_anchor_hints(self) -> AnchorHints: ...
     def get_anchor_rect(self) -> Rectangle: ...
     def get_offset(self) -> Tuple[int, int]: ...
     def get_rect_anchor(self) -> Gravity: ...
     def get_shadow_width(self) -> Tuple[int, int, int, int]: ...
@@ -3130,44 +3672,90 @@
     ) -> None: ...
     def set_surface_anchor(self, anchor: Gravity) -> None: ...
     def unref(self) -> None: ...
 
 class ProximityEvent(Event): ...
 
 class RGBA(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        RGBA()
+    """
+
     red: float = ...
     green: float = ...
     blue: float = ...
     alpha: float = ...
     def copy(self) -> RGBA: ...
     def equal(self, p2: RGBA) -> bool: ...
     def free(self) -> None: ...
     def hash(self) -> int: ...
     def is_clear(self) -> bool: ...
     def is_opaque(self) -> bool: ...
     def parse(self, spec: str) -> bool: ...
     def to_string(self) -> str: ...
 
 class Rectangle(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        Rectangle()
+    """
+
     x: int = ...
     y: int = ...
     width: int = ...
     height: int = ...
     def contains_point(self, x: int, y: int) -> bool: ...
     def equal(self, rect2: Rectangle) -> bool: ...
     def intersect(self, src2: Rectangle) -> Tuple[bool, Rectangle]: ...
     def union(self, src2: Rectangle) -> Rectangle: ...
 
 class ScrollEvent(Event):
+    """
+    :Constructors:
+
+    ::
+
+        ScrollEvent(**properties)
+    """
+
     def get_deltas(self) -> Tuple[float, float]: ...
     def get_direction(self) -> ScrollDirection: ...
     def get_unit(self) -> ScrollUnit: ...
     def is_stop(self) -> bool: ...
 
 class Seat(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Seat(**properties)
+
+    Object GdkSeat
+
+    Signals from GdkSeat:
+      device-added (GdkDevice)
+      device-removed (GdkDevice)
+      tool-added (GdkDeviceTool)
+      tool-removed (GdkDeviceTool)
+
+    Properties from GdkSeat:
+      display -> GdkDisplay: display
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         display: Display
     props: Props = ...
     parent_instance: GObject.Object = ...
     def __init__(self, display: Display = ...): ...
     def get_capabilities(self) -> SeatCapabilities: ...
     def get_devices(self, capabilities: SeatCapabilities) -> list[Device]: ...
@@ -3176,26 +3764,57 @@
     def get_pointer(self) -> Optional[Device]: ...
     def get_tools(self) -> list[DeviceTool]: ...
 
 class Snapshot(GObject.Object): ...
 class SnapshotClass(GObject.GPointer): ...
 
 class Surface(GObject.Object):
+    """
+    :Constructors:
+
+    ::
+
+        Surface(**properties)
+        new_popup(parent:Gdk.Surface, autohide:bool) -> Gdk.Surface
+        new_toplevel(display:Gdk.Display) -> Gdk.Surface
+
+    Object GdkSurface
+
+    Signals from GdkSurface:
+      layout (gint, gint)
+      render (CairoRegion) -> gboolean
+      event (gpointer) -> gboolean
+      enter-monitor (GdkMonitor)
+      leave-monitor (GdkMonitor)
+
+    Properties from GdkSurface:
+      cursor -> GdkCursor: cursor
+      display -> GdkDisplay: display
+      frame-clock -> GdkFrameClock: frame-clock
+      mapped -> gboolean: mapped
+      width -> gint: width
+      height -> gint: height
+      scale-factor -> gint: scale-factor
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         cursor: Optional[Cursor]
         display: Display
         frame_clock: FrameClock
         height: int
         mapped: bool
         scale_factor: int
         width: int
     props: Props = ...
     def __init__(
         self,
-        cursor: Cursor = ...,
+        cursor: Optional[Cursor] = ...,
         display: Display = ...,
         frame_clock: FrameClock = ...,
     ): ...
     def beep(self) -> None: ...
     def create_cairo_context(self) -> CairoContext: ...
     def create_gl_context(self) -> GLContext: ...
     def create_similar_surface(
@@ -3227,14 +3846,40 @@
     def set_input_region(self, region: cairo.Region) -> None: ...
     def set_opaque_region(self, region: Optional[cairo.Region] = None) -> None: ...
     def translate_coordinates(self, to: Surface) -> Tuple[bool, float, float]: ...
 
 class SurfaceClass(GObject.GPointer): ...
 
 class Texture(GObject.Object, Paintable, Gio.Icon, Gio.LoadableIcon):
+    """
+    :Constructors:
+
+    ::
+
+        Texture(**properties)
+        new_for_pixbuf(pixbuf:GdkPixbuf.Pixbuf) -> Gdk.Texture
+        new_from_bytes(bytes:GLib.Bytes) -> Gdk.Texture
+        new_from_file(file:Gio.File) -> Gdk.Texture
+        new_from_filename(path:str) -> Gdk.Texture
+        new_from_resource(resource_path:str) -> Gdk.Texture
+
+    Object GdkTexture
+
+    Properties from GdkTexture:
+      width -> gint: width
+      height -> gint: height
+
+    Signals from GdkPaintable:
+      invalidate-contents ()
+      invalidate-size ()
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         height: int
         width: int
     props: Props = ...
     def __init__(self, height: int = ..., width: int = ...): ...
     def download(self, data: Sequence[int], stride: int) -> None: ...
     def get_format(self) -> MemoryFormat: ...
@@ -3254,31 +3899,54 @@
     def save_to_png_bytes(self) -> GLib.Bytes: ...
     def save_to_tiff(self, filename: str) -> bool: ...
     def save_to_tiff_bytes(self) -> GLib.Bytes: ...
 
 class TextureClass(GObject.GPointer): ...
 
 class TextureDownloader(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        new(texture:Gdk.Texture) -> Gdk.TextureDownloader
+    """
+
     def copy(self) -> TextureDownloader: ...
     def download_bytes(self) -> Tuple[GLib.Bytes, int]: ...
     def download_into(self, data: Sequence[int], stride: int) -> None: ...
     def free(self) -> None: ...
     def get_format(self) -> MemoryFormat: ...
     def get_texture(self) -> Texture: ...
     @classmethod
     def new(cls, texture: Texture) -> TextureDownloader: ...
     def set_format(self, format: MemoryFormat) -> None: ...
     def set_texture(self, texture: Texture) -> None: ...
 
 class TimeCoord(GObject.GPointer):
+    """
+    :Constructors:
+
+    ::
+
+        TimeCoord()
+    """
+
     time: int = ...
     flags: AxisFlags = ...
     axes: list[float] = ...
 
 class Toplevel(GObject.GInterface):
+    """
+    Interface GdkToplevel
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     def begin_move(
         self, device: Device, button: int, x: float, y: float, timestamp: int
     ) -> None: ...
     def begin_resize(
         self,
         edge: SurfaceEdge,
         device: Optional[Device],
@@ -3304,14 +3972,22 @@
     def show_window_menu(self, event: Event) -> bool: ...
     def supports_edge_constraints(self) -> bool: ...
     def titlebar_gesture(self, gesture: TitlebarGesture) -> bool: ...
 
 class ToplevelInterface(GObject.GPointer): ...
 
 class ToplevelLayout(GObject.GBoxed):
+    """
+    :Constructors:
+
+    ::
+
+        new() -> Gdk.ToplevelLayout
+    """
+
     def copy(self) -> ToplevelLayout: ...
     def equal(self, other: ToplevelLayout) -> bool: ...
     def get_fullscreen(self) -> Tuple[bool, bool]: ...
     def get_fullscreen_monitor(self) -> Optional[Monitor]: ...
     def get_maximized(self) -> Tuple[bool, bool]: ...
     def get_resizable(self) -> bool: ...
     @classmethod
@@ -3329,24 +4005,60 @@
     def set_min_size(self, min_width: int, min_height: int) -> None: ...
     def set_shadow_width(
         self, left: int, right: int, top: int, bottom: int
     ) -> None: ...
     def set_size(self, width: int, height: int) -> None: ...
 
 class TouchEvent(Event):
+    """
+    :Constructors:
+
+    ::
+
+        TouchEvent(**properties)
+    """
+
     def get_emulating_pointer(self) -> bool: ...
 
 class TouchpadEvent(Event):
+    """
+    :Constructors:
+
+    ::
+
+        TouchpadEvent(**properties)
+    """
+
     def get_deltas(self) -> Tuple[float, float]: ...
     def get_gesture_phase(self) -> TouchpadGesturePhase: ...
     def get_n_fingers(self) -> int: ...
     def get_pinch_angle_delta(self) -> float: ...
     def get_pinch_scale(self) -> float: ...
 
 class VulkanContext(DrawContext, Gio.Initable):
+    """
+    :Constructors:
+
+    ::
+
+        VulkanContext(**properties)
+
+    Object GdkVulkanContext
+
+    Signals from GdkVulkanContext:
+      images-updated ()
+
+    Properties from GdkDrawContext:
+      display -> GdkDisplay: display
+      surface -> GdkSurface: surface
+
+    Signals from GObject:
+      notify (GParam)
+    """
+
     class Props:
         display: Optional[Display]
         surface: Optional[Surface]
     props: Props = ...
     def __init__(self, display: Display = ..., surface: Surface = ...): ...
 
 class AnchorHints(GObject.GFlags):
```

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gtk3.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/_Gtk3.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -25324,20 +25324,31 @@
     _gtk_reserved1: None = ...
     _gtk_reserved2: None = ...
     _gtk_reserved3: None = ...
     _gtk_reserved4: None = ...
 
 class TearoffMenuItemPrivate(GObject.GPointer): ...
 
+# override
 class Template:
-    def from_file(filename): ...  # FIXME Function
-    def from_resource(resource_path): ...  # FIXME Function
-    def from_string(string): ...  # FIXME Function
+    def __init__(
+        self, filename: str = ..., resource_path: str = ..., string: str = ...
+    ) -> None: ...
+    @classmethod
+    def from_file(cls, filename: str): ...
+    @classmethod
+    def from_resource(cls, resource_path: str): ...
+    @classmethod
+    def from_string(cls, string: str): ...
+    def __call__(self, cls): ...
+
+    class Callback:
+        def __init__(self, name: str = ...) -> None: ...
+        def __call__(self, func: Callable[..., Any]) -> Any: ...
 
-    class Callback: ...
     class Child: ...
 
 class TextAppearance(GObject.GPointer):
     bg_color: Gdk.Color = ...
     fg_color: Gdk.Color = ...
     rise: int = ...
     underline: int = ...
@@ -28271,15 +28282,17 @@
     def expand_row(self, path: TreePath, open_all: bool) -> bool: ...
     def expand_to_path(self, path: TreePath) -> None: ...
     def get_activate_on_single_click(self) -> bool: ...
     def get_background_area(
         self, path: Optional[TreePath] = None, column: Optional[TreeViewColumn] = None
     ) -> Gdk.Rectangle: ...
     def get_bin_window(self) -> Optional[Gdk.Window]: ...
-    def get_cell_area(self, *args, **kwargs): ...
+    def get_cell_area(
+        self, path: Optional[TreePath], column: Optional[TreeViewColumn]
+    ) -> Gdk.Rectangle: ...
     def get_column(self, n: int) -> Optional[TreeViewColumn]: ...
     def get_columns(self) -> list[TreeViewColumn]: ...
     def get_cursor(self) -> Tuple[TreePath, TreeViewColumn]: ...
     def get_dest_row_at_pos(
         self, drag_x: int, drag_y: int
     ) -> Optional[tuple[TreePath, TreeViewDropPosition]]: ...
     def get_drag_dest_row(self) -> Tuple[TreePath, TreeViewDropPosition]: ...
```

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Gtk4.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/_Gtk4.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_GtkSource4.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/_GtkSource4.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_GtkSource5.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/_GtkSource5.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Soup2.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/_Soup2.pyi`

 * *Files identical despite different names*

### Comparing `PyGObject-stubs-2.8.0/src/gi-stubs/repository/_Soup3.pyi` & `PyGObject-stubs-2.9.0/src/gi-stubs/repository/_Soup3.pyi`

 * *Files identical despite different names*

