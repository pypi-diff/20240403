# Comparing `tmp/PyQtUIkit-2.0.2.tar.gz` & `tmp/PyQtUIkit-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.0.2.tar", last modified: Tue Apr  2 15:37:34 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.0.3.tar", last modified: Wed Apr  3 07:18:02 2024, max compression
```

## Comparing `PyQtUIkit-2.0.2.tar` & `PyQtUIkit-2.0.3.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.191553 PyQtUIkit-2.0.2/
--rw-rw-rw-   0        0        0     1090 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-02 15:37:34.191553 PyQtUIkit-2.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.160333 PyQtUIkit-2.0.2/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3967 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/_icons.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.160333 PyQtUIkit-2.0.2/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.160333 PyQtUIkit-2.0.2/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     4655 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.175924 PyQtUIkit-2.0.2/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.191553 PyQtUIkit-2.0.2/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     1845 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  1559111 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1207 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.191553 PyQtUIkit-2.0.2/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1469 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3515 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     4120 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2625 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0     9981 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7013 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5807 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2505 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     4180 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/hbox_layout.py
--rw-rw-rw-   0        0        0     1578 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1100 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     1311 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     2130 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1076 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     3302 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     7076 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2504 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6585 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     3881 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     7038 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    12024 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1218 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/tabs.py
--rw-rw-rw-   0        0        0     2167 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4435 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    16155 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/tree_widget.py
--rw-rw-rw-   0        0        0     4507 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/vbox_layout.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.160333 PyQtUIkit-2.0.2/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-02 15:37:34.000000 PyQtUIkit-2.0.2/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2476 2024-04-02 15:37:34.000000 PyQtUIkit-2.0.2/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 15:37:34.000000 PyQtUIkit-2.0.2/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-02 15:37:34.000000 PyQtUIkit-2.0.2/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-02 15:37:34.000000 PyQtUIkit-2.0.2/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-02 15:37:34.000000 PyQtUIkit-2.0.2/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 15:37:34.191553 PyQtUIkit-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1411 2024-04-02 15:36:53.000000 PyQtUIkit-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:18:02.145824 PyQtUIkit-2.0.3/
+-rw-rw-rw-   0        0        0     1090 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-03 07:18:02.145824 PyQtUIkit-2.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-03 07:18:02.098955 PyQtUIkit-2.0.3/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3967 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/_icons.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:18:02.114576 PyQtUIkit-2.0.3/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:18:02.114576 PyQtUIkit-2.0.3/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     4655 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:18:02.130200 PyQtUIkit-2.0.3/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-03 07:18:02.130200 PyQtUIkit-2.0.3/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     1845 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  1559097 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1207 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:18:02.145824 PyQtUIkit-2.0.3/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1469 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3515 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     4174 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2785 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0     9981 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     7013 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5807 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2505 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     4180 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/hbox_layout.py
+-rw-rw-rw-   0        0        0     1578 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1100 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     1468 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     2130 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1076 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     3302 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     7076 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2504 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6683 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     3881 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     7356 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    12024 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1218 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/tabs.py
+-rw-rw-rw-   0        0        0     2167 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4465 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    16155 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/tree_widget.py
+-rw-rw-rw-   0        0        0     4507 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/PyQtUIkit/widgets/vbox_layout.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:18:02.098955 PyQtUIkit-2.0.3/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-03 07:18:01.000000 PyQtUIkit-2.0.3/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2476 2024-04-03 07:18:02.000000 PyQtUIkit-2.0.3/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 07:18:01.000000 PyQtUIkit-2.0.3/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-03 07:18:01.000000 PyQtUIkit-2.0.3/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-03 07:18:01.000000 PyQtUIkit-2.0.3/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-03 07:18:01.000000 PyQtUIkit-2.0.3/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 07:18:02.145824 PyQtUIkit-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1411 2024-04-03 07:17:12.000000 PyQtUIkit-2.0.3/setup.py
```

### Comparing `PyQtUIkit-2.0.2/LICENSE` & `PyQtUIkit-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PKG-INFO` & `PyQtUIkit-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.0.2
+Version: 2.0.3
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/_icons.py` & `PyQtUIkit-2.0.3/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.0.3/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.0.3/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.0.3/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/core/font.py` & `PyQtUIkit-2.0.3/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.0.3/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.0.3/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.0.3/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.0.3/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.0.3/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.0.3/PyQtUIkit/themes/icons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 icons = {
-    'brands-42-group': '<svg xmlns="http://www.w3.org/2000/svg"\n     viewBox="0 0 640 512">-->\n    <path d="M320 96V416C341.011 416 361.818 411.861 381.23 403.821C400.641 395.78 418.28 383.995 433.138 369.138C447.995 354.28 459.78 336.641 467.821 317.23C475.861 297.818 480 277.011 480 256C480 234.989 475.861 214.182 467.821 194.771C459.78 175.359 447.995 157.72 433.138 142.863C418.28 128.005 400.641 116.22 381.23 108.179C361.818 100.139 341.011 96 320 96ZM0 256L160.002 416L320.003 256L160.002 96L0 256ZM480 256C480 277.011 484.138 297.818 492.179 317.23C500.219 336.643 512.005 354.28 526.862 369.138C541.72 383.995 559.357 395.781 578.77 403.821C598.182 411.862 618.989 416 640 416V96C597.565 96 556.869 112.858 526.862 142.863C496.857 172.869 480 213.565 480 256Z"/>\n</svg>',
+    'brands-42-group': '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512">--><path d="M320 96V416C341.011 416 361.818 411.861 381.23 403.821C400.641 395.78 418.28 383.995 433.138 369.138C447.995 354.28 459.78 336.641 467.821 317.23C475.861 297.818 480 277.011 480 256C480 234.989 475.861 214.182 467.821 194.771C459.78 175.359 447.995 157.72 433.138 142.863C418.28 128.005 400.641 116.22 381.23 108.179C361.818 100.139 341.011 96 320 96ZM0 256L160.002 416L320.003 256L160.002 96L0 256ZM480 256C480 277.011 484.138 297.818 492.179 317.23C500.219 336.643 512.005 354.28 526.862 369.138C541.72 383.995 559.357 395.781 578.77 403.821C598.182 411.862 618.989 416 640 416V96C597.565 96 556.869 112.858 526.862 142.863C496.857 172.869 480 213.565 480 256Z"/></svg>',
     'brands-500px': '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512">--><path d="M103.3 344.3c-6.5-14.2-6.9-18.3 7.4-23.1 25.6-8 8 9.2 43.2 49.2h.3v-93.9c1.2-50.2 44-92.2 97.7-92.2 53.9 0 97.7 43.5 97.7 96.8 0 63.4-60.8 113.2-128.5 93.3-10.5-4.2-2.1-31.7 8.5-28.6 53 0 89.4-10.1 89.4-64.4 0-61-77.1-89.6-116.9-44.6-23.5 26.4-17.6 42.1-17.6 157.6 50.7 31 118.3 22 160.4-20.1 24.8-24.8 38.5-58 38.5-93 0-35.2-13.8-68.2-38.8-93.3-24.8-24.8-57.8-38.5-93.3-38.5s-68.8 13.8-93.5 38.5c-.3.3-16 16.5-21.2 23.9l-.5.6c-3.3 4.7-6.3 9.1-20.1 6.1-6.9-1.7-14.3-5.8-14.3-11.8V20c0-5 3.9-10.5 10.5-10.5h241.3c8.3 0 8.3 11.6 8.3 15.1 0 3.9 0 15.1-8.3 15.1H130.3v132.9h.3c104.2-109.8 282.8-36 282.8 108.9 0 178.1-244.8 220.3-310.1 62.8zm63.3-260.8c-.5 4.2 4.6 24.5 14.6 20.6C306 56.6 384 144.5 390.6 144.5c4.8 0 22.8-15.3 14.3-22.8-93.2-89-234.5-57-238.3-38.2zM393 414.7C283 524.6 94 475.5 61 310.5c0-12.2-30.4-7.4-28.9 3.3 24 173.4 246 256.9 381.6 121.3 6.9-7.8-12.6-28.4-20.7-20.4zM213.6 306.6c0 4 4.3 7.3 5.5 8.5 3 3 6.1 4.4 8.5 4.4 3.8 0 2.6.2 22.3-19.5 19.6 19.3 19.1 19.5 22.3 19.5 5.4 0 18.5-10.4 10.7-18.2L265.6 284l18.2-18.2c6.3-6.8-10.1-21.8-16.2-15.7L249.7 268c-18.6-18.8-18.4-19.5-21.5-19.5-5 0-18 11.7-12.4 17.3L234 284c-18.1 17.9-20.4 19.2-20.4 22.6z"/></svg>',
     'brands-accessible-icon': '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512">--><path d="M423.9 255.8L411 413.1c-3.3 40.7-63.9 35.1-60.6-4.9l10-122.5-41.1 2.3c10.1 20.7 15.8 43.9 15.8 68.5 0 41.2-16.1 78.7-42.3 106.5l-39.3-39.3c57.9-63.7 13.1-167.2-74-167.2-25.9 0-49.5 9.9-67.2 26L73 243.2c22-20.7 50.1-35.1 81.4-40.2l75.3-85.7-42.6-24.8-51.6 46c-30 26.8-70.6-18.5-40.5-45.4l68-60.7c9.8-8.8 24.1-10.2 35.5-3.6 0 0 139.3 80.9 139.5 81.1 16.2 10.1 20.7 36 6.1 52.6L285.7 229l106.1-5.9c18.5-1.1 33.6 14.4 32.1 32.7zm-64.9-154c28.1 0 50.9-22.8 50.9-50.9C409.9 22.8 387.1 0 359 0c-28.1 0-50.9 22.8-50.9 50.9 0 28.1 22.8 50.9 50.9 50.9zM179.6 456.5c-80.6 0-127.4-90.6-82.7-156.1l-39.7-39.7C36.4 287 24 320.3 24 356.4c0 130.7 150.7 201.4 251.4 122.5l-39.7-39.7c-16 10.9-35.3 17.3-56.1 17.3z"/></svg>',
     'brands-accusoft': '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512">--><path d="M322.1 252v-1l-51.2-65.8s-12 1.6-25 15.1c-9 9.3-242.1 239.1-243.4 240.9-7 10 1.6 6.8 15.7 1.7.8 0 114.5-36.6 114.5-36.6.5-.6-.1-.1.6-.6-.4-5.1-.8-26.2-1-27.7-.6-5.2 2.2-6.9 7-8.9l92.6-33.8c.6-.8 88.5-81.7 90.2-83.3zm160.1 120.1c13.3 16.1 20.7 13.3 30.8 9.3 3.2-1.2 115.4-47.6 117.8-48.9 8-4.3-1.7-16.7-7.2-23.4-2.1-2.5-205.1-245.6-207.2-248.3-9.7-12.2-14.3-12.9-38.4-12.8-10.2 0-106.8.5-116.5.6-19.2.1-32.9-.3-19.2 16.9C250 75 476.5 365.2 482.2 372.1zm152.7 1.6c-2.3-.3-24.6-4.7-38-7.2 0 0-115 50.4-117.5 51.6-16 7.3-26.9-3.2-36.7-14.6l-57.1-74c-5.4-.9-60.4-9.6-65.3-9.3-3.1.2-9.6.8-14.4 2.9-4.9 2.1-145.2 52.8-150.2 54.7-5.1 2-11.4 3.6-11.1 7.6.2 2.5 2 2.6 4.6 3.5 2.7.8 300.9 67.6 308 69.1 15.6 3.3 38.5 10.5 53.6 1.7 2.1-1.2 123.8-76.4 125.8-77.8 5.4-4 4.3-6.8-1.7-8.2z"/></svg>',
     'brands-adn': '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 496 512">--><path d="M248 167.5l64.9 98.8H183.1l64.9-98.8zM496 256c0 136.9-111.1 248-248 248S0 392.9 0 256 111.1 8 248 8s248 111.1 248 248zm-99.8 82.7L248 115.5 99.8 338.7h30.4l33.6-51.7h168.6l33.6 51.7h30.2z"/></svg>',
     'brands-adversal': '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">--><path d="M482.1 32H28.7C5.8 32 0 37.9 0 60.9v390.2C0 474.4 5.8 480 28.7 480h453.4c24.4 0 29.9-5.2 29.9-29.7V62.2c0-24.6-5.4-30.2-29.9-30.2zM178.4 220.3c-27.5-20.2-72.1-8.7-84.2 23.4-4.3 11.1-9.3 9.5-17.5 8.3-9.7-1.5-17.2-3.2-22.5-5.5-28.8-11.4 8.6-55.3 24.9-64.3 41.1-21.4 83.4-22.2 125.3-4.8 40.9 16.8 34.5 59.2 34.5 128.5 2.7 25.8-4.3 58.3 9.3 88.8 1.9 4.4.4 7.9-2.7 10.7-8.4 6.7-39.3 2.2-46.6-7.4-1.9-2.2-1.8-3.6-3.9-6.2-3.6-3.9-7.3-2.2-11.9 1-57.4 36.4-140.3 21.4-147-43.3-3.1-29.3 12.4-57.1 39.6-71 38.2-19.5 112.2-11.8 114-30.9 1.1-10.2-1.9-20.1-11.3-27.3zm286.7 222c0 15.1-11.1 9.9-17.8 9.9H52.4c-7.4 0-18.2 4.8-17.8-10.7.4-13.9 10.5-9.1 17.1-9.1 132.3-.4 264.5-.4 396.8 0 6.8 0 16.6-4.4 16.6 9.9zm3.8-340.5v291c0 5.7-.7 13.9-8.1 13.9-12.4-.4-27.5 7.1-36.1-5.6-5.8-8.7-7.8-4-12.4-1.2-53.4 29.7-128.1 7.1-144.4-85.2-6.1-33.4-.7-67.1 15.7-100 11.8-23.9 56.9-76.1 136.1-30.5v-71c0-26.2-.1-26.2 26-26.2 3.1 0 6.6.4 9.7 0 10.1-.8 13.6 4.4 13.6 14.3-.1.2-.1.3-.1.5zm-51.5 232.3c-19.5 47.6-72.9 43.3-90 5.2-15.1-33.3-15.5-68.2.4-101.5 16.3-34.1 59.7-35.7 81.5-4.8 20.6 28.8 14.9 84.6 8.1 101.1zm-294.8 35.3c-7.5-1.3-33-3.3-33.7-27.8-.4-13.9 7.8-23 19.8-25.8 24.4-5.9 49.3-9.9 73.7-14.7 8.9-2 7.4 4.4 7.8 9.5 1.4 33-26.1 59.2-67.6 58.8z"/></svg>',
     'brands-affiliatetheme': '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">--><path d="M159.7 237.4C108.4 308.3 43.1 348.2 14 326.6-15.2 304.9 2.8 230 54.2 159.1c51.3-70.9 116.6-110.8 145.7-89.2 29.1 21.6 11.1 96.6-40.2 167.5zm351.2-57.3C437.1 303.5 319 367.8 246.4 323.7c-25-15.2-41.3-41.2-49-73.8-33.6 64.8-92.8 113.8-164.1 133.2 49.8 59.3 124.1 96.9 207 96.9 150 0 271.6-123.1 271.6-274.9.1-8.5-.3-16.8-1-25z"/></svg>',
     'brands-airbnb': '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512">--><path d="M224 373.12c-25.24-31.67-40.08-59.43-45-83.18-22.55-88 112.61-88 90.06 0-5.45 24.25-20.29 52-45 83.18zm138.15 73.23c-42.06 18.31-83.67-10.88-119.3-50.47 103.9-130.07 46.11-200-18.85-200-54.92 0-85.16 46.51-73.28 100.5 6.93 29.19 25.23 62.39 54.43 99.5-32.53 36.05-60.55 52.69-85.15 54.92-50 7.43-89.11-41.06-71.3-91.09 15.1-39.16 111.72-231.18 115.87-241.56 15.75-30.07 25.56-57.4 59.38-57.4 32.34 0 43.4 25.94 60.37 59.87 36 70.62 89.35 177.48 114.84 239.09 13.17 33.07-1.37 71.29-37.01 86.64zm47-136.12C280.27 35.93 273.13 32 224 32c-45.52 0-64.87 31.67-84.66 72.79C33.18 317.1 22.89 347.19 22 349.81-3.22 419.14 48.74 480 111.63 480c21.71 0 60.61-6.06 112.37-62.4 58.68 63.78 101.26 62.4 112.37 62.4 62.89.05 114.85-60.86 89.61-130.19.02-3.89-16.82-38.9-16.82-39.58z"/></svg>',
```

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.0.3/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.0.3/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 
     text = MethodsProperty(QPushButton.text, QPushButton.setText)
 
 
 class KitIconButton(QPushButton, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
     icon = IconProperty('icon')
+    on_click = SignalProperty('on_click', 'clicked')
 
     def __init__(self, icon=''):
         super().__init__()
         self.__widgets = []
         self._icon = icon
         self._main_palette = 'Main'
         self.setCursor(Qt.CursorShape.PointingHandCursor)
```

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/checkbox.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from PyQt6.QtCore import Qt, pyqtSignal
 from PyQt6.QtWidgets import QWidget, QHBoxLayout, QPushButton, QSizePolicy
 
-from PyQtUIkit.core import PaletteProperty, EnumProperty, KitFont, FontProperty, MethodsProperty
+from PyQtUIkit.core import *
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 from PyQtUIkit.widgets.button import KitIconButton
 
 
 class KitCheckBox(QWidget, _KitWidget):
     main_palette = PaletteProperty('main_palette', 'Main')
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     stateChanged = pyqtSignal(bool)
+    stateEdited = pyqtSignal(bool)
 
     def __init__(self, text=''):
         super().__init__()
         self.__state = False
         self.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Minimum)
 
         main_layout = QHBoxLayout()
@@ -34,14 +35,15 @@
         main_layout.addWidget(self.__label)
         if not text:
             self.__label.hide()
 
     def _on_clicked(self):
         self.__state = not self.__state
         self.__on_state_changed()
+        self.stateEdited.emit(self.__state)
 
     def __on_state_changed(self):
         self.__button.icon = 'solid-check' if self.__state else ''
         self.__button.setChecked(self.__state)
         self.stateChanged.emit(self.__state)
 
     def isChecked(self):
@@ -72,7 +74,9 @@
             color: {self.main_palette.text};
             background-color: transparent;
             text-align: left;
         }}""")
 
     state = MethodsProperty(isChecked, setChecked)
     text = MethodsProperty(getText, setText)
+    on_state_changed = SignalProperty('on_state_changed', 'stateChanged')
+    on_state_edited = SignalProperty('on_state_edited', 'stateEdited')
```

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/hbox_layout.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/hbox_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/line_edit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from PyQt6.QtWidgets import QLineEdit
 
-from PyQtUIkit.core import PaletteProperty, EnumProperty, KitFont, FontProperty, MethodsProperty
+from PyQtUIkit.core import PaletteProperty, EnumProperty, KitFont, FontProperty, MethodsProperty, SignalProperty
 from PyQtUIkit.widgets._widget import KitGroupItem as _KitGroupItem
 
 
 class KitLineEdit(QLineEdit, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
     font = FontProperty('font')
@@ -32,7 +32,9 @@
 }}
 QLineEdit:focus {{
     border: {self.border}px solid {self.border_palette.selected};
     background-color: {self.main_palette.hover};
 }}""")
 
     text = MethodsProperty(QLineEdit.text, QLineEdit.setText)
+    on_text_changed = SignalProperty('on_text_changed', 'textChanged')
+    on_text_edited = SignalProperty('on_text_edited', 'textEdited')
```

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/radio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PyQt6.QtCore import Qt, pyqtSignal
 from PyQt6.QtGui import QFontMetrics
 from PyQt6.QtWidgets import QLabel, QPushButton, QHBoxLayout, QSizePolicy
 
-from PyQtUIkit.core import IntProperty, PaletteProperty, KitFont, EnumProperty, FontProperty
+from PyQtUIkit.core import *
 from PyQtUIkit.widgets import KitVBoxLayout, KitHBoxLayout
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class KitRadioButton(QPushButton, _KitWidget):
     main_palette = PaletteProperty('Bg')
     font = FontProperty('font')
@@ -74,14 +74,15 @@
 
 class KitVRadio(KitVBoxLayout):
     button_height = IntProperty('button_size', 24)
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     currentChanged = pyqtSignal(int)
+    on_current_changed = SignalProperty('on_current_changed', 'currentChanged')
 
     def __init__(self):
         super().__init__()
         self._main_palette = 'Bg'
         self.__items = []
         self.__current = None
 
@@ -134,14 +135,15 @@
 
 class KitHRadio(KitHBoxLayout):
     button_height = IntProperty('button_size', 24)
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     currentChanged = pyqtSignal(int)
+    on_current_changed = SignalProperty('on_current_changed', 'currentChanged')
 
     def __init__(self):
         super().__init__()
         self._main_palette = 'Bg'
         self.__items = []
         self.__current = None
```

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/spin_box.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from PyQt6.QtCore import pyqtSignal, Qt
 from PyQt6.QtWidgets import QWidget, QHBoxLayout, QLineEdit, QVBoxLayout, QPushButton, QSizePolicy
 
-from PyQtUIkit.core import IntProperty, EnumProperty, KitFont, FontProperty, MethodsProperty
+from PyQtUIkit.core import IntProperty, EnumProperty, KitFont, FontProperty, MethodsProperty, SignalProperty
 from PyQtUIkit.widgets._widget import KitGroupItem as _KitGroupItem, KitGroup as _KitGroup
 
 
 class KitSpinBox(QWidget, _KitGroupItem):
     border = IntProperty('border', 1)
     radius = IntProperty('radius', 4)
     valueChanged = pyqtSignal(object)
+    valueEdited = pyqtSignal(object)
     font = FontProperty('font')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     def __init__(self, func=int):
         super().__init__()
         self._min = 0
         self._max = 100
@@ -48,72 +49,74 @@
 
         self._button_down = QPushButton()
         self._button_down.setCursor(Qt.CursorShape.PointingHandCursor)
         # self._button_down.setFixedWidth(20)
         self._button_down.clicked.connect(self._decrease)
         buttons_layout.addWidget(self._button_down)
 
-    def _on_text_edited(self):
+    def _on_text_edited(self, manually=True):
         text = self._line_edit.text()
         try:
             value = 0 if text in ['', '+', '-'] else self._func(text)
         except ValueError:
             pos = self._last_pos
             self._line_edit.setText(self._last_text)
             self._last_pos = pos
             self._line_edit.setCursorPosition(self._last_pos)
         else:
-            if value < self._min:
+            if text and value < self._min:
                 self._last_text = str(self._min)
                 self._line_edit.setText(self._last_text)
-            elif value > self._max:
+            elif text and value > self._max:
                 self._last_text = str(self._max)
                 self._line_edit.setText(self._last_text)
             else:
                 self._last_text = text
             self.valueChanged.emit(value)
+            if manually:
+                self.valueEdited.emit(value)
             self._last_pos = self._line_edit.cursorPosition()
 
     def _on_cursor_moved(self):
         self._last_pos = self._line_edit.cursorPosition()
 
     def _on_editing_finished(self):
         text = self._line_edit.text()
         if not text:
             self._line_edit.setText('0')
             self._on_text_edited()
 
     def _decrease(self):
         self.setValue(round(self.value() - self._step, 2))
         self.valueChanged.emit(self.value())
-        # self._line_edit.selectAll()
-        # self._line_edit.setFocus()
+        self._line_edit.selectAll()
+        self._line_edit.setFocus()
 
     def _increase(self):
         self.setValue(round(self.value() + self._step, 2))
         self.valueChanged.emit(self.value())
-        # self._line_edit.selectAll()
-        # self._line_edit.setFocus()
+        self._line_edit.selectAll()
+        self._line_edit.setFocus()
 
     def setRange(self, minimum, maximum):
         self._min = minimum
         self._max = maximum
-        self._on_text_edited()
+        self._on_text_edited(False)
 
     def setMinimum(self, minimum):
         self._min = minimum
-        self._on_text_edited()
+        self._on_text_edited(False)
 
     def setMaximum(self, maximum):
         self._max = maximum
-        self._on_text_edited()
+        self._on_text_edited(False)
 
     def setValue(self, value):
         self._line_edit.setText(str(value))
-        self._on_text_edited()
+        self._on_text_edited(False)
 
     def getValue(self):
         if not self._line_edit.text():
             return 0
         return self._func(self._line_edit.text())
 
     def _apply_theme(self):
@@ -162,7 +165,9 @@
                                 orientation == _KitGroup.VERTICAL and position == _KitGroup.FIRST or \
                                 orientation == _KitGroup.HORIZONTAL and position == _KitGroup.LAST else 0
         self._button_up.setStyleSheet(css.replace("top-right-radius: 0px;", f"top-right-radius: {radius}px;"))
         radius = self.radius if orientation == _KitGroup.NO_GROUP or position == _KitGroup.LAST else 0
         self._button_down.setStyleSheet(css.replace("bottom-right-radius: 0px;", f"bottom-right-radius: {radius}px;"))
 
     value = MethodsProperty(getValue, setValue)
+    on_value_changed = SignalProperty('on_value_changed', 'valueChanged')
+    on_value_edited = SignalProperty('on_value_edited', 'valueEdited')
```

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/tab_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/tabs.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/tabs.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/toggle.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum
 
 from PyQt6.QtCore import Qt, pyqtSignal, QPoint, QPropertyAnimation, QEasingCurve
 from PyQt6.QtWidgets import QWidget, QPushButton
 
-from PyQtUIkit.core import PaletteProperty, EnumProperty, MethodsProperty
+from PyQtUIkit.core import *
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 from PyQtUIkit.widgets.button import KitButton
 
 
 class KitToggle(QWidget, _KitWidget):
     class Mode(Enum):
         SMALL = 0
@@ -116,7 +116,8 @@
             color: {self.main_palette.text};
             background-color: {self.rail_palette.selected if self.__state else self.rail_palette.main};
             border: 0px solid black;
             border-radius: {sizes['rail_size'][1] // 2}px;
         }}""")
 
     state = MethodsProperty(isChecked, setChecked)
+    on_state_changed = SignalProperty('on_state_changed', 'stateChanged')
```

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/tree_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit/widgets/vbox_layout.py` & `PyQtUIkit-2.0.3/PyQtUIkit/widgets/vbox_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.0.3/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.0.2
+Version: 2.0.3
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.0.2/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.0.3/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.2/setup.py` & `PyQtUIkit-2.0.3/setup.py`

 * *Files identical despite different names*

