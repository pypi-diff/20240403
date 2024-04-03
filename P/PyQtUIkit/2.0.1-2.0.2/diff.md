# Comparing `tmp/PyQtUIkit-2.0.1.tar.gz` & `tmp/PyQtUIkit-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQtUIkit-2.0.1.tar", last modified: Tue Apr  2 13:34:06 2024, max compression
+gzip compressed data, was "PyQtUIkit-2.0.2.tar", last modified: Tue Apr  2 15:37:34 2024, max compression
```

## Comparing `PyQtUIkit-2.0.1.tar` & `PyQtUIkit-2.0.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.469556 PyQtUIkit-2.0.1/
--rw-rw-rw-   0        0        0     1090 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     2938 2024-04-02 13:34:06.469556 PyQtUIkit-2.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.438339 PyQtUIkit-2.0.1/PyQtUIkit/
--rw-rw-rw-   0        0        0       49 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/__init__.py
--rw-rw-rw-   0        0        0     3967 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/_icons.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.438339 PyQtUIkit-2.0.1/PyQtUIkit/builder/
--rw-rw-rw-   0        0        0     1116 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/builder/__init__.py
--rw-rw-rw-   0        0        0     1825 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/builder/builder_class.py
--rw-rw-rw-   0        0        0     1383 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/builder/builder_module.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.438339 PyQtUIkit-2.0.1/PyQtUIkit/core/
--rw-rw-rw-   0        0        0       84 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/core/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/core/_version.py
--rw-rw-rw-   0        0        0     1503 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/core/font.py
--rw-rw-rw-   0        0        0     1019 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/core/icon.py
--rw-rw-rw-   0        0        0     4478 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/core/properties.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.453929 PyQtUIkit-2.0.1/PyQtUIkit/fonts/
--rw-rw-rw-   0        0        0   168060 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Black.ttf
--rw-rw-rw-   0        0        0   174108 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
--rw-rw-rw-   0        0        0   167336 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Bold.ttf
--rw-rw-rw-   0        0        0   171508 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
--rw-rw-rw-   0        0        0   170504 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Italic.ttf
--rw-rw-rw-   0        0        0   167000 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Light.ttf
--rw-rw-rw-   0        0        0   173172 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf
--rw-rw-rw-   0        0        0   168644 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Medium.ttf
--rw-rw-rw-   0        0        0   173416 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
--rw-rw-rw-   0        0        0   168260 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Regular.ttf
--rw-rw-rw-   0        0        0   168488 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Thin.ttf
--rw-rw-rw-   0        0        0   172860 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
--rw-rw-rw-   0        0        0    87392 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    94636 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
--rw-rw-rw-   0        0        0    88248 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    94016 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
--rw-rw-rw-   0        0        0    94372 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf
--rw-rw-rw-   0        0        0    87980 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    94256 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
--rw-rw-rw-   0        0        0    87172 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    94412 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
--rw-rw-rw-   0        0        0    87236 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87496 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    94508 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
--rw-rw-rw-   0        0        0    88288 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0    93588 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
-drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.453929 PyQtUIkit-2.0.1/PyQtUIkit/themes/
--rw-rw-rw-   0        0        0     1845 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/themes/__init__.py
--rw-rw-rw-   0        0        0     5879 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/themes/builtin_themes.py
--rw-rw-rw-   0        0        0  1559111 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/themes/icons.py
--rw-rw-rw-   0        0        0     1207 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/themes/svg.py
--rw-rw-rw-   0        0        0     1402 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/themes/theme.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.469556 PyQtUIkit-2.0.1/PyQtUIkit/widgets/
--rw-rw-rw-   0        0        0     1469 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/__init__.py
--rw-rw-rw-   0        0        0     3515 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/_widget.py
--rw-rw-rw-   0        0        0     1359 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/application.py
--rw-rw-rw-   0        0        0     3857 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/button.py
--rw-rw-rw-   0        0        0     2594 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/checkbox.py
--rw-rw-rw-   0        0        0     9950 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/combo_box.py
--rw-rw-rw-   0        0        0     7013 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/dialog.py
--rw-rw-rw-   0        0        0     5807 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/flow_layout.py
--rw-rw-rw-   0        0        0     2505 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/group.py
--rw-rw-rw-   0        0        0     4142 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/hbox_layout.py
--rw-rw-rw-   0        0        0     1578 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/icon_widget.py
--rw-rw-rw-   0        0        0     1076 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/label.py
--rw-rw-rw-   0        0        0     1287 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/line_edit.py
--rw-rw-rw-   0        0        0     2130 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/list_widget.py
--rw-rw-rw-   0        0        0     1076 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/main_window.py
--rw-rw-rw-   0        0        0     3302 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/menu.py
--rw-rw-rw-   0        0        0     7076 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/navigation.py
--rw-rw-rw-   0        0        0     2504 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/progress_bar.py
--rw-rw-rw-   0        0        0     6585 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/radio.py
--rw-rw-rw-   0        0        0     3881 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     7014 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/spin_box.py
--rw-rw-rw-   0        0        0     3580 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/spinner.py
--rw-rw-rw-   0        0        0    11841 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/tab_bar.py
--rw-rw-rw-   0        0        0     1218 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/tabs.py
--rw-rw-rw-   0        0        0     2167 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/text_edit.py
--rw-rw-rw-   0        0        0     4411 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/toggle.py
--rw-rw-rw-   0        0        0    15985 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/tree_widget.py
--rw-rw-rw-   0        0        0     4441 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/PyQtUIkit/widgets/vbox_layout.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:34:06.438339 PyQtUIkit-2.0.1/PyQtUIkit.egg-info/
--rw-rw-rw-   0        0        0     2938 2024-04-02 13:34:06.000000 PyQtUIkit-2.0.1/PyQtUIkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2476 2024-04-02 13:34:06.000000 PyQtUIkit-2.0.1/PyQtUIkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 13:34:06.000000 PyQtUIkit-2.0.1/PyQtUIkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-02 13:34:06.000000 PyQtUIkit-2.0.1/PyQtUIkit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2024-04-02 13:34:06.000000 PyQtUIkit-2.0.1/PyQtUIkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-02 13:34:06.000000 PyQtUIkit-2.0.1/PyQtUIkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 13:34:06.469556 PyQtUIkit-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1411 2024-04-02 13:33:14.000000 PyQtUIkit-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.191553 PyQtUIkit-2.0.2/
+-rw-rw-rw-   0        0        0     1090 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2938 2024-04-02 15:37:34.191553 PyQtUIkit-2.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.160333 PyQtUIkit-2.0.2/PyQtUIkit/
+-rw-rw-rw-   0        0        0       49 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/__init__.py
+-rw-rw-rw-   0        0        0     3967 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/_icons.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.160333 PyQtUIkit-2.0.2/PyQtUIkit/builder/
+-rw-rw-rw-   0        0        0     1116 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/builder/__init__.py
+-rw-rw-rw-   0        0        0     1825 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/builder/builder_class.py
+-rw-rw-rw-   0        0        0     1383 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/builder/builder_module.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.160333 PyQtUIkit-2.0.2/PyQtUIkit/core/
+-rw-rw-rw-   0        0        0       84 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/core/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/core/_version.py
+-rw-rw-rw-   0        0        0     1503 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/core/font.py
+-rw-rw-rw-   0        0        0     1019 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/core/icon.py
+-rw-rw-rw-   0        0        0     4655 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/core/properties.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.175924 PyQtUIkit-2.0.2/PyQtUIkit/fonts/
+-rw-rw-rw-   0        0        0   168060 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Black.ttf
+-rw-rw-rw-   0        0        0   174108 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-BlackItalic.ttf
+-rw-rw-rw-   0        0        0   167336 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Bold.ttf
+-rw-rw-rw-   0        0        0   171508 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-BoldItalic.ttf
+-rw-rw-rw-   0        0        0   170504 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Italic.ttf
+-rw-rw-rw-   0        0        0   167000 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Light.ttf
+-rw-rw-rw-   0        0        0   173172 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-LightItalic.ttf
+-rw-rw-rw-   0        0        0   168644 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Medium.ttf
+-rw-rw-rw-   0        0        0   173416 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-MediumItalic.ttf
+-rw-rw-rw-   0        0        0   168260 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Regular.ttf
+-rw-rw-rw-   0        0        0   168488 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Thin.ttf
+-rw-rw-rw-   0        0        0   172860 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-ThinItalic.ttf
+-rw-rw-rw-   0        0        0    87392 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    94636 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf
+-rw-rw-rw-   0        0        0    88248 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    94016 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf
+-rw-rw-rw-   0        0        0    94372 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Italic.ttf
+-rw-rw-rw-   0        0        0    87980 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    94256 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf
+-rw-rw-rw-   0        0        0    87172 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    94412 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf
+-rw-rw-rw-   0        0        0    87236 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87496 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    94508 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf
+-rw-rw-rw-   0        0        0    88288 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0    93588 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf
+drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.191553 PyQtUIkit-2.0.2/PyQtUIkit/themes/
+-rw-rw-rw-   0        0        0     1845 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/themes/__init__.py
+-rw-rw-rw-   0        0        0     5879 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/themes/builtin_themes.py
+-rw-rw-rw-   0        0        0  1559111 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/themes/icons.py
+-rw-rw-rw-   0        0        0     1207 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/themes/svg.py
+-rw-rw-rw-   0        0        0     1402 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/themes/theme.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.191553 PyQtUIkit-2.0.2/PyQtUIkit/widgets/
+-rw-rw-rw-   0        0        0     1469 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3515 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/_widget.py
+-rw-rw-rw-   0        0        0     1359 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/application.py
+-rw-rw-rw-   0        0        0     4120 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/button.py
+-rw-rw-rw-   0        0        0     2625 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/checkbox.py
+-rw-rw-rw-   0        0        0     9981 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/combo_box.py
+-rw-rw-rw-   0        0        0     7013 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/dialog.py
+-rw-rw-rw-   0        0        0     5807 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/flow_layout.py
+-rw-rw-rw-   0        0        0     2505 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/group.py
+-rw-rw-rw-   0        0        0     4180 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/hbox_layout.py
+-rw-rw-rw-   0        0        0     1578 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/icon_widget.py
+-rw-rw-rw-   0        0        0     1100 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/label.py
+-rw-rw-rw-   0        0        0     1311 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/line_edit.py
+-rw-rw-rw-   0        0        0     2130 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/list_widget.py
+-rw-rw-rw-   0        0        0     1076 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/main_window.py
+-rw-rw-rw-   0        0        0     3302 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/menu.py
+-rw-rw-rw-   0        0        0     7076 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/navigation.py
+-rw-rw-rw-   0        0        0     2504 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/progress_bar.py
+-rw-rw-rw-   0        0        0     6585 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/radio.py
+-rw-rw-rw-   0        0        0     3881 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     7038 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/spin_box.py
+-rw-rw-rw-   0        0        0     3580 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/spinner.py
+-rw-rw-rw-   0        0        0    12024 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/tab_bar.py
+-rw-rw-rw-   0        0        0     1218 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/tabs.py
+-rw-rw-rw-   0        0        0     2167 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/text_edit.py
+-rw-rw-rw-   0        0        0     4435 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/toggle.py
+-rw-rw-rw-   0        0        0    16155 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/tree_widget.py
+-rw-rw-rw-   0        0        0     4507 2024-04-02 15:36:52.000000 PyQtUIkit-2.0.2/PyQtUIkit/widgets/vbox_layout.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:37:34.160333 PyQtUIkit-2.0.2/PyQtUIkit.egg-info/
+-rw-rw-rw-   0        0        0     2938 2024-04-02 15:37:34.000000 PyQtUIkit-2.0.2/PyQtUIkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2476 2024-04-02 15:37:34.000000 PyQtUIkit-2.0.2/PyQtUIkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 15:37:34.000000 PyQtUIkit-2.0.2/PyQtUIkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-02 15:37:34.000000 PyQtUIkit-2.0.2/PyQtUIkit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2024-04-02 15:37:34.000000 PyQtUIkit-2.0.2/PyQtUIkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-02 15:37:34.000000 PyQtUIkit-2.0.2/PyQtUIkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 15:37:34.191553 PyQtUIkit-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1411 2024-04-02 15:36:53.000000 PyQtUIkit-2.0.2/setup.py
```

### Comparing `PyQtUIkit-2.0.1/LICENSE` & `PyQtUIkit-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PKG-INFO` & `PyQtUIkit-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.0.1
+Version: 2.0.2
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/_icons.py` & `PyQtUIkit-2.0.2/PyQtUIkit/_icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/builder/__init__.py` & `PyQtUIkit-2.0.2/PyQtUIkit/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/builder/builder_class.py` & `PyQtUIkit-2.0.2/PyQtUIkit/builder/builder_class.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/builder/builder_module.py` & `PyQtUIkit-2.0.2/PyQtUIkit/builder/builder_module.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/core/font.py` & `PyQtUIkit-2.0.2/PyQtUIkit/core/font.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/core/icon.py` & `PyQtUIkit-2.0.2/PyQtUIkit/core/icon.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/core/properties.py` & `PyQtUIkit-2.0.2/PyQtUIkit/core/properties.py`

 * *Files 8% similar despite different names*

```diff
@@ -145,7 +145,12 @@
         def getter(obj):
             return None
 
         def setter(obj, value: str):
             getattr(obj, self._signal).connect(value)
 
         super().__init__(getter, setter)
+        
+        
+class MethodsProperty(property):
+    def __init__(self, getter, setter):
+        super().__init__(lambda obj: getter(obj), lambda obj, x: setter(obj, x))
```

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Black.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-BlackItalic.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Bold.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-BoldItalic.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Italic.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Light.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-LightItalic.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Medium.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-MediumItalic.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Regular.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-Thin.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/Roboto-ThinItalic.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Bold.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Italic.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Light.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Medium.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Regular.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-Thin.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf` & `PyQtUIkit-2.0.2/PyQtUIkit/fonts/RobotoMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/themes/__init__.py` & `PyQtUIkit-2.0.2/PyQtUIkit/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/themes/builtin_themes.py` & `PyQtUIkit-2.0.2/PyQtUIkit/themes/builtin_themes.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/themes/icons.py` & `PyQtUIkit-2.0.2/PyQtUIkit/themes/icons.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/themes/svg.py` & `PyQtUIkit-2.0.2/PyQtUIkit/themes/svg.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/themes/theme.py` & `PyQtUIkit-2.0.2/PyQtUIkit/themes/theme.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/__init__.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/_widget.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/application.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/application.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/button.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/button.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PyQt6.QtCore import Qt
 from PyQt6.QtWidgets import QPushButton, QVBoxLayout
 
 from PyQtUIkit.core import IconProperty, EnumProperty, IntProperty, PaletteProperty, KitFont, FontProperty, \
-    SignalProperty
+    SignalProperty, MethodsProperty
 from PyQtUIkit.themes import ThemeManager
 from PyQtUIkit.widgets import KitIconWidget
 from PyQtUIkit.widgets._widget import KitGroupItem as _KitGroupItem
 
 
 class KitButton(QPushButton, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
@@ -54,20 +54,19 @@
     subcontrol-origin: padding;
     padding-right: 5px;
     subcontrol-position: right;
 }}""")
         if self.icon is not None:
             self.setIcon(self.icon.icon(self.main_palette.text))
 
-    text = property(QPushButton.text, QPushButton.setText)
+    text = MethodsProperty(QPushButton.text, QPushButton.setText)
 
 
 class KitIconButton(QPushButton, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
-    size = IntProperty('size', 24)
     icon = IconProperty('icon')
 
     def __init__(self, icon=''):
         super().__init__()
         self.__widgets = []
         self._icon = icon
         self._main_palette = 'Main'
@@ -80,21 +79,28 @@
         self._icon_label._use_text_only = False
         self.__layout.addWidget(self._icon_label)
 
     def _set_tm(self, tm: ThemeManager):
         super()._set_tm(tm)
         self._icon_label._set_tm(tm)
 
+    def _set_size(self, x, y=None):
+        if isinstance(x, int) and isinstance(y, int):
+            self.setFixedSize(x, y)
+        elif y is None:
+            self.setFixedSize(x, x)
+        else:
+            self.setFixedSize(x)
+
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
         self._icon_label.icon = self.icon
         self._icon_label._main_palette = self._main_palette
-        self.setFixedSize(self.size, self.size)
-        self.__layout.setContentsMargins(*[self.size // 5] * 4)
+        self.__layout.setContentsMargins(*[min(self.width(), self.height()) // 5] * 4)
         self.setStyleSheet(f"""
 QPushButton {{
     background-color: {self.main_palette.main};
     border: {self.border}px solid {self.border_palette.main};
     {self._border_radius_css()}
     padding: 3px 8px 3px 8px;
 }}
@@ -110,7 +116,9 @@
     background-color: {self.main_palette.selected};
     border: {self.border}px solid {self.border_palette.selected};
 }}
 QPushButton::menu-indicator {{
     image: none;
     subcontrol-position: right;
 }}""")
+
+    size = MethodsProperty(QPushButton.size, _set_size)
```

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/checkbox.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/checkbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PyQt6.QtCore import Qt, pyqtSignal
 from PyQt6.QtWidgets import QWidget, QHBoxLayout, QPushButton, QSizePolicy
 
-from PyQtUIkit.core import PaletteProperty, EnumProperty, KitFont, FontProperty
+from PyQtUIkit.core import PaletteProperty, EnumProperty, KitFont, FontProperty, MethodsProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 from PyQtUIkit.widgets.button import KitIconButton
 
 
 class KitCheckBox(QWidget, _KitWidget):
     main_palette = PaletteProperty('main_palette', 'Main')
     font = FontProperty('font')
@@ -70,9 +70,9 @@
         self.__label.setStyleSheet(f"""
         QPushButton {{
             color: {self.main_palette.text};
             background-color: transparent;
             text-align: left;
         }}""")
 
-    state = property(isChecked, setChecked)
-    text = property(getText, setText)
+    state = MethodsProperty(isChecked, setChecked)
+    text = MethodsProperty(getText, setText)
```

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/combo_box.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/combo_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from PyQt6.QtCore import pyqtSignal, Qt, QPoint, QPropertyAnimation, QEasingCurve, QSize, QParallelAnimationGroup
 from PyQt6.QtGui import QIcon
 from PyQt6.QtWidgets import QPushButton, QVBoxLayout, QMenu, QHBoxLayout, QApplication
 
-from PyQtUIkit.core import IntProperty, PaletteProperty, IconProperty, EnumProperty, KitFont, FontProperty
+from PyQtUIkit.core import IntProperty, PaletteProperty, IconProperty, EnumProperty, KitFont, FontProperty, \
+    MethodsProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget, KitGroupItem as _KitGroupItem
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
 from PyQtUIkit.widgets.scroll_area import KitScrollArea
 from PyQtUIkit.widgets.vbox_layout import KitVBoxLayout
 
 
 class KitComboBoxItem(QPushButton, _KitWidget):
@@ -53,15 +54,15 @@
 }}
 QPushButton::checked {{
     background-color: {self.main_palette.selected};
 }}""")
         if self.icon is not None:
             self.setIcon(self.icon.icon(self.main_palette.text))
 
-    name = property(QPushButton.text, QPushButton.setText)
+    name = MethodsProperty(QPushButton.text, QPushButton.setText)
 
 
 class KitComboBox(QPushButton, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
     type = IntProperty('type', 1)
     icon = IconProperty('icon')
     font = FontProperty('font')
```

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/dialog.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/flow_layout.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/flow_layout.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/group.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/group.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/hbox_layout.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/hbox_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PyQt6.QtCore import QMargins
 from PyQt6.QtWidgets import QWidget, QHBoxLayout
 
-from PyQtUIkit.core.properties import IntProperty
+from PyQtUIkit.core.properties import IntProperty, MethodsProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class KitHBoxLayout(QWidget, _KitWidget):
     border = IntProperty('border', 0)
     radius = IntProperty('radius', 4)
 
@@ -112,10 +112,10 @@
         QWidget {{
             background-color: {self.main_palette.main};
             border: {self.border}px solid {self.border_palette.main};
             border-radius: {self.radius}px;
         }}
         """)
 
-    padding = property(getContentsMargins, _set_margins)
-    spacing = property(getSpacing, setSpacing)
-    alignment = property(getAlignment, setAlignment)
+    padding = MethodsProperty(getContentsMargins, _set_margins)
+    spacing = MethodsProperty(getSpacing, setSpacing)
+    alignment = MethodsProperty(getAlignment, setAlignment)
```

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/icon_widget.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/icon_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/label.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/label.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from PyQt6.QtWidgets import QLabel
 
-from PyQtUIkit.core import IntProperty, PaletteProperty, EnumProperty, KitFont, FontProperty
+from PyQtUIkit.core import IntProperty, PaletteProperty, EnumProperty, KitFont, FontProperty, MethodsProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class KitLabel(QLabel, _KitWidget):
     main_palette = PaletteProperty('main_palette', 'Transparent')
     border = IntProperty('border', 0)
     radius = IntProperty('radius', 4)
@@ -23,8 +23,8 @@
         self.setStyleSheet(f"""
         QWidget {{
             color: {self.main_palette.text_only if self._use_text_only else self.main_palette.text};
             background-color: transparent;
             border: none;
         }}""")
 
-    text = property(QLabel.text, QLabel.setText)
+    text = MethodsProperty(QLabel.text, QLabel.setText)
```

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/line_edit.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/line_edit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from PyQt6.QtWidgets import QLineEdit
 
-from PyQtUIkit.core import PaletteProperty, EnumProperty, KitFont, FontProperty
+from PyQtUIkit.core import PaletteProperty, EnumProperty, KitFont, FontProperty, MethodsProperty
 from PyQtUIkit.widgets._widget import KitGroupItem as _KitGroupItem
 
 
 class KitLineEdit(QLineEdit, _KitGroupItem):
     main_palette = PaletteProperty('main_palette', 'Main')
     font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
     font = FontProperty('font')
@@ -31,8 +31,8 @@
     background-color: {self.main_palette.hover};
 }}
 QLineEdit:focus {{
     border: {self.border}px solid {self.border_palette.selected};
     background-color: {self.main_palette.hover};
 }}""")
 
-    text = property(QLineEdit.text, QLineEdit.setText)
+    text = MethodsProperty(QLineEdit.text, QLineEdit.setText)
```

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/list_widget.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/main_window.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/main_window.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/menu.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/navigation.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/progress_bar.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/progress_bar.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/radio.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/scroll_area.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/scroll_area.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/spin_box.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/spin_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PyQt6.QtCore import pyqtSignal, Qt
 from PyQt6.QtWidgets import QWidget, QHBoxLayout, QLineEdit, QVBoxLayout, QPushButton, QSizePolicy
 
-from PyQtUIkit.core import IntProperty, EnumProperty, KitFont, FontProperty
+from PyQtUIkit.core import IntProperty, EnumProperty, KitFont, FontProperty, MethodsProperty
 from PyQtUIkit.widgets._widget import KitGroupItem as _KitGroupItem, KitGroup as _KitGroup
 
 
 class KitSpinBox(QWidget, _KitGroupItem):
     border = IntProperty('border', 1)
     radius = IntProperty('radius', 4)
     valueChanged = pyqtSignal(object)
@@ -161,8 +161,8 @@
         radius = self.radius if orientation == _KitGroup.NO_GROUP or \
                                 orientation == _KitGroup.VERTICAL and position == _KitGroup.FIRST or \
                                 orientation == _KitGroup.HORIZONTAL and position == _KitGroup.LAST else 0
         self._button_up.setStyleSheet(css.replace("top-right-radius: 0px;", f"top-right-radius: {radius}px;"))
         radius = self.radius if orientation == _KitGroup.NO_GROUP or position == _KitGroup.LAST else 0
         self._button_down.setStyleSheet(css.replace("bottom-right-radius: 0px;", f"bottom-right-radius: {radius}px;"))
 
-    value = property(getValue, setValue)
+    value = MethodsProperty(getValue, setValue)
```

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/spinner.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/tab_bar.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/tab_bar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from time import time
 
 from PyQt6.QtCore import pyqtSignal, Qt, QPoint, QPropertyAnimation, QEasingCurve
 from PyQt6.QtWidgets import QPushButton, QHBoxLayout, QSizePolicy, QWidget
 from PyQt6.QtGui import QFontMetrics
 
-from PyQtUIkit.core.properties import IntProperty, PaletteProperty, IconProperty
+from PyQtUIkit.core import KitFont
+from PyQtUIkit.core.properties import IntProperty, PaletteProperty, IconProperty, EnumProperty, FontProperty
 from PyQtUIkit.themes import KitPalette
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
 from PyQtUIkit.widgets.button import KitIconButton, KitButton
 from PyQtUIkit.widgets.scroll_area import KitScrollArea
 from PyQtUIkit.widgets.hbox_layout import KitHBoxLayout
 from PyQtUIkit.widgets.label import KitLabel
 
 
 class KitTab(QPushButton, _KitWidget):
     radius_top = IntProperty('radius_top', 5)
     radius_bottom = IntProperty('radius_bottom', 0)
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     selected = pyqtSignal(object)
     _mousePress = pyqtSignal(object)
     _mouseRelease = pyqtSignal()
     icon = IconProperty('icon')
 
     def __init__(self, name, value=None, icon=''):
@@ -93,15 +96,15 @@
         return self._value
 
     def _apply_theme(self):
         if not self._tm or not self._tm.active:
             return
         self.__button_close.main_palette = KitPalette('#00000000', self.main_palette.main,
                                                       text=self.main_palette.text)
-        self.__label.setFont(self._tm.font_medium)
+        self.__label.setFont(font := self.font.get(self.font_size))
         self.setStyleSheet(f"""
 QPushButton {{
     color: {self.main_palette.text};
     background-color: {self.main_palette.main if not self.__checked else self.main_palette.selected};
     border: 0px solid {self.border_palette.main};
     border-top-left-radius: {self.radius_top}px;
     border-top-right-radius: {self.radius_top}px;
@@ -109,16 +112,16 @@
     border-bottom-right-radius: {self.radius_bottom}px;
     padding: 3px 5px 3px 5px;
     text-align: left;
 }}
 QPushButton::hover {{
     background-color: {self.main_palette.hover if not self.__checked else self.main_palette.selected};
 }}""")
-        font_metrics = QFontMetrics(self.font())
-        width = font_metrics.size(0, self.__label.text()).width() + 10
+        font_metrics = QFontMetrics(font)
+        width = font_metrics.size(0, self.__label.text).width() + 10
         if self.icon:
             width += 20
         if self.__closable:
             width += 20
         self.setFixedWidth(width)
 
         self.__label._apply_theme()
```

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/tabs.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/tabs.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/text_edit.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/text_edit.py`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/toggle.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/toggle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum
 
 from PyQt6.QtCore import Qt, pyqtSignal, QPoint, QPropertyAnimation, QEasingCurve
 from PyQt6.QtWidgets import QWidget, QPushButton
 
-from PyQtUIkit.core import PaletteProperty, EnumProperty
+from PyQtUIkit.core import PaletteProperty, EnumProperty, MethodsProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 from PyQtUIkit.widgets.button import KitButton
 
 
 class KitToggle(QWidget, _KitWidget):
     class Mode(Enum):
         SMALL = 0
@@ -115,8 +115,8 @@
         QWidget {{
             color: {self.main_palette.text};
             background-color: {self.rail_palette.selected if self.__state else self.rail_palette.main};
             border: 0px solid black;
             border-radius: {sizes['rail_size'][1] // 2}px;
         }}""")
 
-    state = property(isChecked, setChecked)
+    state = MethodsProperty(isChecked, setChecked)
```

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/tree_widget.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/tree_widget.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from enum import Enum
 
 from PyQt6.QtCore import Qt, pyqtSignal, QPoint
 from PyQt6.QtWidgets import QPushButton, QHBoxLayout, QLabel, QVBoxLayout, QWidget
 
+from PyQtUIkit.core import KitFont
 from PyQtUIkit.core.properties import IntProperty, StringProperty, IconProperty, BoolProperty, EnumProperty, \
-    PaletteProperty
+    PaletteProperty, FontProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 from PyQtUIkit.widgets.dialog import KitDialog
 from PyQtUIkit.widgets.hbox_layout import KitHBoxLayout
 from PyQtUIkit.widgets.icon_widget import KitIconWidget
 from PyQtUIkit.widgets.label import KitLabel
 from PyQtUIkit.widgets.scroll_area import KitScrollArea
 
 
 class KitTreeWidgetItem(QVBoxLayout, _KitWidget):
     name = StringProperty('name', '')
     radius = IntProperty('radius', 4)
     icon = IconProperty('icon')
     text_palette = PaletteProperty('text_palette', 'Main')
+    font = FontProperty('font')
+    font_size = EnumProperty('font_size', KitFont.Size, KitFont.Size.MEDIUM)
 
     def __init__(self, name='', icon=''):
         super().__init__()
         self._name = name
         self._icon = icon
         self._main_palette = 'Main'
         self._text_palette = 'Main'
@@ -231,15 +234,15 @@
             self.__icon_widget._apply_theme()
         else:
             self.__icon_widget.hide()
         self.__button.setFixedHeight(self._height)
         self.__arrow_right.setIcon(self.__root._icon1)
         self.__arrow_down.setIcon(self.__root._icon2)
         self._apply_selected_theme()
-        self.__label.setFont(self._tm.font_medium)
+        self.__label.setFont(self.font.get(self.font_size))
         for el in [self.__arrow_right, self.__arrow_down]:
             el.setStyleSheet(f"""
             QPushButton {{
                 background-color: transparent;
                 border: 0px solid black;
                 border-radius: {self.radius}px;
             }}
```

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit/widgets/vbox_layout.py` & `PyQtUIkit-2.0.2/PyQtUIkit/widgets/vbox_layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PyQt6.QtCore import QMargins
 from PyQt6.QtWidgets import QWidget, QVBoxLayout
 
-from PyQtUIkit.core.properties import IntProperty
+from PyQtUIkit.core.properties import IntProperty, MethodsProperty
 from PyQtUIkit.widgets._widget import _KitWidget as _KitWidget
 
 
 class KitVBoxLayout(QWidget, _KitWidget):
     border = IntProperty('border', 0)
     radius = IntProperty('radius', 4)
 
@@ -112,14 +112,14 @@
         QWidget {{
             background-color: {self.main_palette.main};
             border: {self.border}px solid {self.border_palette.main};
             border-radius: {self.radius}px;
         }}
         """)
 
-    padding = property(getContentsMargins, _set_margins)
-    spacing = property(getSpacing, setSpacing)
-    alignment = property(getAlignment, setAlignment)
-    max_width = property(QWidget.maximumWidth, QWidget.setMaximumWidth)
-    min_width = property(QWidget.minimumWidth, QWidget.setMinimumWidth)
-    max_height = property(QWidget.maximumHeight, QWidget.setMaximumHeight)
-    min_height = property(QWidget.minimumHeight, QWidget.setMinimumHeight)
+    padding = MethodsProperty(getContentsMargins, _set_margins)
+    spacing = MethodsProperty(getSpacing, setSpacing)
+    alignment = MethodsProperty(getAlignment, setAlignment)
+    max_width = MethodsProperty(QWidget.maximumWidth, QWidget.setMaximumWidth)
+    min_width = MethodsProperty(QWidget.minimumWidth, QWidget.setMinimumWidth)
+    max_height = MethodsProperty(QWidget.maximumHeight, QWidget.setMaximumHeight)
+    min_height = MethodsProperty(QWidget.minimumHeight, QWidget.setMinimumHeight)
```

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit.egg-info/PKG-INFO` & `PyQtUIkit-2.0.2/PyQtUIkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQtUIkit
-Version: 2.0.1
+Version: 2.0.2
 Summary: A PyQtUIkit package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `PyQtUIkit-2.0.1/PyQtUIkit.egg-info/SOURCES.txt` & `PyQtUIkit-2.0.2/PyQtUIkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQtUIkit-2.0.1/setup.py` & `PyQtUIkit-2.0.2/setup.py`

 * *Files identical despite different names*

