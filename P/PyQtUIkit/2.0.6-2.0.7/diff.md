# Comparing `tmp/PyQtUIkit-2.0.6.tar.gz` & `tmp/PyQtUIkit-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.0.6.tar", last modified: Wed Apr  3 10:22:07 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.0.7.tar", last modified: Wed Apr  3 11:10:59 2024, max compression
```

## Comparing `PyQtUIkit-2.0.6.tar` & `PyQtUIkit-2.0.7.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 10:22:07.276879 PyQtUIkit-2.0.6/
--rw-rw-rw-   0        0        0     1090 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-03 10:22:07.276879 PyQtUIkit-2.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 10:22:07.230018 PyQtUIkit-2.0.6/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3903 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/_icons.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:22:07.230018 PyQtUIkit-2.0.6/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:22:07.245631 PyQtUIkit-2.0.6/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     4655 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:22:07.261248 PyQtUIkit-2.0.6/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-03 10:22:07.261248 PyQtUIkit-2.0.6/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     2180 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  1559097 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1338 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:22:07.276879 PyQtUIkit-2.0.6/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1469 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3515 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     4174 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2785 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0     9981 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7013 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5807 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2505 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     4180 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/hbox_layout.py
--rw-rw-rw-   0        0        0     1578 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1100 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     1468 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     3448 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1076 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     3302 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     7076 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2504 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6683 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     3881 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     7356 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    12024 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1218 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/tabs.py
--rw-rw-rw-   0        0        0     2167 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4465 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    16286 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/tree_widget.py
--rw-rw-rw-   0        0        0     4507 2024-04-03 10:21:32.000000 PyQtUIkit-2.0.6/PyQtUIkit/widgets/vbox_layout.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:22:07.230018 PyQtUIkit-2.0.6/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-03 10:22:07.000000 PyQtUIkit-2.0.6/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2476 2024-04-03 10:22:07.000000 PyQtUIkit-2.0.6/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 10:22:07.000000 PyQtUIkit-2.0.6/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-03 10:22:07.000000 PyQtUIkit-2.0.6/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-03 10:22:07.000000 PyQtUIkit-2.0.6/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 10:22:07.000000 PyQtUIkit-2.0.6/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 10:22:07.276879 PyQtUIkit-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1411 2024-04-03 10:21:33.000000 PyQtUIkit-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:10:59.852574 PyQtUIkit-2.0.7/
+-rw-rw-rw-   0        0        0     1090 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-03 11:10:59.852574 PyQtUIkit-2.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-03 11:10:59.805719 PyQtUIkit-2.0.7/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3903 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/_icons.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:10:59.805719 PyQtUIkit-2.0.7/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:10:59.805719 PyQtUIkit-2.0.7/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     4655 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:10:59.821324 PyQtUIkit-2.0.7/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-03 11:10:59.836947 PyQtUIkit-2.0.7/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     2180 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  1559097 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1338 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:10:59.852574 PyQtUIkit-2.0.7/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1469 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3515 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     4174 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2785 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0     9981 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     7013 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5807 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2505 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     4180 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/hbox_layout.py
+-rw-rw-rw-   0        0        0     1578 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1100 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     1468 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     3448 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1076 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     3302 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     7076 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2504 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6683 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     3881 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     7356 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    12024 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1218 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/tabs.py
+-rw-rw-rw-   0        0        0     2167 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4465 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    16361 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/tree_widget.py
+-rw-rw-rw-   0        0        0     4507 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/PyQtUIkit/widgets/vbox_layout.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:10:59.805719 PyQtUIkit-2.0.7/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-03 11:10:59.000000 PyQtUIkit-2.0.7/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2476 2024-04-03 11:10:59.000000 PyQtUIkit-2.0.7/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 11:10:59.000000 PyQtUIkit-2.0.7/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-03 11:10:59.000000 PyQtUIkit-2.0.7/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-03 11:10:59.000000 PyQtUIkit-2.0.7/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-03 11:10:59.000000 PyQtUIkit-2.0.7/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 11:10:59.852574 PyQtUIkit-2.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1411 2024-04-03 11:10:12.000000 PyQtUIkit-2.0.7/setup.py
```

### Comparing `PyQtUIkit-2.0.6/LICENSE` & `PyQtUIkit-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PKG-INFO` & `PyQtUIkit-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.0.6
+Version: 2.0.7
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/_icons.py` & `PyQtUIkit-2.0.7/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.0.7/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.0.7/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.0.7/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/core/font.py` & `PyQtUIkit-2.0.7/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.0.7/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.0.7/PyQtUIkit/core/properties.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.0.7/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.0.7/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.0.7/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.0.7/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.0.7/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.0.7/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/button.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/combo_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/hbox_layout.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/hbox_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/label.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/line_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/spin_box.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/tab_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/tabs.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/tabs.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/tree_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         self.__children.insert(index, item)
         self.__layout.insertLayout(index, item)
 
         self.__arrow_down.setHidden(not self.__expanded)
         self.__arrow_right.setHidden(self.__expanded)
         self._update_padding()
 
-    def count(self):
+    def childrenCount(self):
         return len(self.__children)
 
     def child(self, index):
         return self.__children[index]
 
     def clear(self):
         for _ in range(self.count()):
@@ -224,14 +224,16 @@
             return self
         if self.__expanded:
             for i, el in enumerate(self.__children):
                 if res := el._find_by_pos(pos - QPoint(0, self._height * (i + (0 if self.__button.isHidden() else 1)))):
                     return res
 
     def _apply_theme(self):
+        if not self._tm or not self._tm.active:
+            return
         for el in self.__children:
             el._height = self._height
             el.main_palette = self._main_palette
             el.text_palette = self._text_palette
         if self._icon:
             self.__icon_widget._icon = self._icon
             self.__icon_widget.show()
@@ -324,15 +326,14 @@
         self.__tree = KitTreeWidgetItem()
         self.__tree._hide_button()
         self.__tree._set_root(self, None)
         self.__tree.expand()
 
         self.__widget = QWidget()
         self.__widget.setLayout(self.__tree)
-
         self.setWidget(self.__widget)
 
     def addItem(self, item: KitTreeWidgetItem):
         item._main_palette = self._main_palette
         self.__tree.addItem(item)
 
     def currentItem(self) -> KitTreeWidgetItem | None:
```

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit/widgets/vbox_layout.py` & `PyQtUIkit-2.0.7/PyQtUIkit/widgets/vbox_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.0.7/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.0.6
+Version: 2.0.7
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.0.6/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.0.7/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.6/setup.py` & `PyQtUIkit-2.0.7/setup.py`

 * *Files identical despite different names*

