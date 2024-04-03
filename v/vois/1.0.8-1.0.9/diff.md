# Comparing `tmp/vois-1.0.8.tar.gz` & `tmp/vois-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vois-1.0.8.tar", last modified: Tue Jun 20 05:42:06 2023, max compression
+gzip compressed data, was "vois-1.0.9.tar", last modified: Mon Aug 21 12:46:47 2023, max compression
```

## Comparing `vois-1.0.8.tar` & `vois-1.0.9.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 05:42:06.153756 vois-1.0.8/
--rw-rw-rw-   0        0        0    14155 2023-06-09 08:06:09.000000 vois-1.0.8/LICENCE
--rw-rw-rw-   0        0        0      631 2023-06-09 16:48:21.000000 vois-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0    73887 2023-06-09 08:06:09.000000 vois-1.0.8/Notice.txt
--rw-rw-rw-   0        0        0    21433 2023-06-20 05:42:06.152756 vois-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3628 2023-06-16 10:57:43.000000 vois-1.0.8/README.md
--rw-rw-rw-   0        0        0     6091 2023-06-20 05:40:20.000000 vois-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 05:42:06.154755 vois-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 05:42:03.117012 vois-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 05:42:04.605162 vois-1.0.8/src/vois/
--rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/__init__.py
--rw-rw-rw-   0        0        0    11918 2023-06-09 16:34:04.000000 vois-1.0.8/src/vois/colors.py
--rw-rw-rw-   0        0        0     4168 2023-06-09 16:34:04.000000 vois-1.0.8/src/vois/download.py
--rw-rw-rw-   0        0        0    17916 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/eucountries.py
--rw-rw-rw-   0        0        0    10493 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/geojsonUtils.py
--rw-rw-rw-   0        0        0    66667 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/interMap.py
--rw-rw-rw-   0        0        0     9302 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/ipytrees.py
--rw-rw-rw-   0        0        0    35732 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/leafletMap.py
--rw-rw-rw-   0        0        0    29755 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/svgBubblesChart.py
--rw-rw-rw-   0        0        0    11325 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/svgGraph.py
--rw-rw-rw-   0        0        0    18669 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/svgHeatmap.py
--rw-rw-rw-   0        0        0  1033396 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/svgMap.py
--rw-rw-rw-   0        0        0    21956 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/svgPackedCirclesChart.py
--rw-rw-rw-   0        0        0    18049 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/svgRankChart.py
--rw-rw-rw-   0        0        0    48423 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/svgUtils.py
--rw-rw-rw-   0        0        0     7363 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/treemapPlotly.py
--rw-rw-rw-   0        0        0     2290 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/urlOpen.py
--rw-rw-rw-   0        0        0     2017 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/urlUpdate.py
-drwxrwxrwx   0        0        0        0 2023-06-20 05:42:06.096788 vois-1.0.8/src/vois/vuetify/
--rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/__init__.py
--rw-rw-rw-   0        0        0    52950 2023-06-13 09:22:47.000000 vois-1.0.8/src/vois/vuetify/app.py
--rw-rw-rw-   0        0        0    43073 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/basemaps.py
--rw-rw-rw-   0        0        0    13241 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/button.py
--rw-rw-rw-   0        0        0    12779 2023-06-16 10:48:12.000000 vois-1.0.8/src/vois/vuetify/card.py
--rw-rw-rw-   0        0        0    10734 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/cardsGrid.py
--rw-rw-rw-   0        0        0     8770 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/colorPicker.py
--rw-rw-rw-   0        0        0    10437 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/datatable.py
--rw-rw-rw-   0        0        0     7269 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/datePicker.py
--rw-rw-rw-   0        0        0     9804 2023-06-20 05:40:20.000000 vois-1.0.8/src/vois/vuetify/dialogGeneric.py
--rw-rw-rw-   0        0        0     4304 2023-06-20 05:40:20.000000 vois-1.0.8/src/vois/vuetify/dialogMessage.py
--rw-rw-rw-   0        0        0     5785 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/dialogWait.py
--rw-rw-rw-   0        0        0     5423 2023-06-20 05:40:20.000000 vois-1.0.8/src/vois/vuetify/dialogYesNo.py
-drwxrwxrwx   0        0        0        0 2023-06-20 05:42:06.148757 vois-1.0.8/src/vois/vuetify/extra/
--rw-rw-rw-   0        0        0       47 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/extra/__init__.py
--rw-rw-rw-   0        0        0     6838 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/extra/file_input.py
--rw-rw-rw-   0        0        0     2251 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/extra/file_input.vue
--rw-rw-rw-   0        0        0    12885 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/fab.py
--rw-rw-rw-   0        0        0      996 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/fontsettings.py
--rw-rw-rw-   0        0        0    13881 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/footer.py
--rw-rw-rw-   0        0        0     5865 2023-06-20 05:40:20.000000 vois-1.0.8/src/vois/vuetify/iconButton.py
--rw-rw-rw-   0        0        0     8029 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/label.py
--rw-rw-rw-   0        0        0    48546 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/layers.py
--rw-rw-rw-   0        0        0    23017 2023-06-16 10:48:12.000000 vois-1.0.8/src/vois/vuetify/mainPage.py
--rw-rw-rw-   0        0        0     6454 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/menu.py
--rw-rw-rw-   0        0        0     7649 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/multiSwitch.py
--rw-rw-rw-   0        0        0    56576 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/page.py
--rw-rw-rw-   0        0        0    24701 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/paletteEditor.py
--rw-rw-rw-   0        0        0    15331 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/palettePicker.py
--rw-rw-rw-   0        0        0     8048 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/palettePickerEx.py
--rw-rw-rw-   0        0        0     6284 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/popup.py
--rw-rw-rw-   0        0        0     6181 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/progress.py
--rw-rw-rw-   0        0        0     1821 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/queryStrings.py
--rw-rw-rw-   0        0        0     4708 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/radio.py
--rw-rw-rw-   0        0        0     4390 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/rangeSlider.py
--rw-rw-rw-   0        0        0    17054 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/rangeSliderFloat.py
--rw-rw-rw-   0        0        0     9365 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/selectImage.py
--rw-rw-rw-   0        0        0     6052 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/selectMultiple.py
--rw-rw-rw-   0        0        0     8721 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/selectSingle.py
--rw-rw-rw-   0        0        0     4816 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/settings.py
--rw-rw-rw-   0        0        0     6679 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/sidePanel.py
--rw-rw-rw-   0        0        0     5546 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/slider.py
--rw-rw-rw-   0        0        0    12119 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/sliderFloat.py
--rw-rw-rw-   0        0        0     4590 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/snackbar.py
--rw-rw-rw-   0        0        0    24635 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/sortableList.py
--rw-rw-rw-   0        0        0     6575 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/svgsGrid.py
--rw-rw-rw-   0        0        0     4695 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/switch.py
--rw-rw-rw-   0        0        0     6967 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/tabs.py
--rw-rw-rw-   0        0        0     6369 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/textlist.py
--rw-rw-rw-   0        0        0     7009 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/title.py
--rw-rw-rw-   0        0        0     7465 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/toggle.py
--rw-rw-rw-   0        0        0     3179 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/tooltip.py
--rw-rw-rw-   0        0        0    68877 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/treeview.py
--rw-rw-rw-   0        0        0     5036 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/upload.py
-drwxrwxrwx   0        0        0        0 2023-06-20 05:42:04.790057 vois-1.0.8/src/vois.egg-info/
--rw-rw-rw-   0        0        0    21433 2023-06-20 05:42:02.000000 vois-1.0.8/src/vois.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2219 2023-06-20 05:42:03.000000 vois-1.0.8/src/vois.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 05:42:02.000000 vois-1.0.8/src/vois.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-06-20 05:42:02.000000 vois-1.0.8/src/vois.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-20 05:42:02.000000 vois-1.0.8/src/vois.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-21 12:46:47.578068 vois-1.0.9/
+-rw-rw-rw-   0        0        0    14155 2023-06-09 08:06:09.000000 vois-1.0.9/LICENCE
+-rw-rw-rw-   0        0        0      631 2023-06-09 16:48:21.000000 vois-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    73887 2023-06-09 08:06:09.000000 vois-1.0.9/Notice.txt
+-rw-rw-rw-   0        0        0    21433 2023-08-21 12:46:47.576068 vois-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3628 2023-06-16 10:57:43.000000 vois-1.0.9/README.md
+-rw-rw-rw-   0        0        0     6091 2023-08-21 12:44:10.000000 vois-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-21 12:46:47.579066 vois-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-21 12:46:45.695147 vois-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-08-21 12:46:46.324783 vois-1.0.9/src/vois/
+-rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/__init__.py
+-rw-rw-rw-   0        0        0    11918 2023-06-09 16:34:04.000000 vois-1.0.9/src/vois/colors.py
+-rw-rw-rw-   0        0        0     4168 2023-06-09 16:34:04.000000 vois-1.0.9/src/vois/download.py
+-rw-rw-rw-   0        0        0    17916 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/eucountries.py
+-rw-rw-rw-   0        0        0    10493 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/geojsonUtils.py
+-rw-rw-rw-   0        0        0    66667 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/interMap.py
+-rw-rw-rw-   0        0        0     9302 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/ipytrees.py
+-rw-rw-rw-   0        0        0    35732 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/leafletMap.py
+-rw-rw-rw-   0        0        0    29755 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/svgBubblesChart.py
+-rw-rw-rw-   0        0        0    11325 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/svgGraph.py
+-rw-rw-rw-   0        0        0    18669 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/svgHeatmap.py
+-rw-rw-rw-   0        0        0  1033396 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/svgMap.py
+-rw-rw-rw-   0        0        0    21956 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/svgPackedCirclesChart.py
+-rw-rw-rw-   0        0        0    18049 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/svgRankChart.py
+-rw-rw-rw-   0        0        0    48817 2023-08-21 12:42:55.000000 vois-1.0.9/src/vois/svgUtils.py
+-rw-rw-rw-   0        0        0     7363 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/treemapPlotly.py
+-rw-rw-rw-   0        0        0     2290 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/urlOpen.py
+-rw-rw-rw-   0        0        0     2017 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/urlUpdate.py
+drwxrwxrwx   0        0        0        0 2023-08-21 12:46:47.508110 vois-1.0.9/src/vois/vuetify/
+-rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/__init__.py
+-rw-rw-rw-   0        0        0    52950 2023-06-13 09:22:47.000000 vois-1.0.9/src/vois/vuetify/app.py
+-rw-rw-rw-   0        0        0    43073 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/basemaps.py
+-rw-rw-rw-   0        0        0    13359 2023-08-21 12:42:55.000000 vois-1.0.9/src/vois/vuetify/button.py
+-rw-rw-rw-   0        0        0    12798 2023-08-21 12:42:55.000000 vois-1.0.9/src/vois/vuetify/card.py
+-rw-rw-rw-   0        0        0    10734 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/cardsGrid.py
+-rw-rw-rw-   0        0        0     8770 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/colorPicker.py
+-rw-rw-rw-   0        0        0    10435 2023-08-21 12:42:55.000000 vois-1.0.9/src/vois/vuetify/datatable.py
+-rw-rw-rw-   0        0        0     7269 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/datePicker.py
+-rw-rw-rw-   0        0        0     9804 2023-06-20 05:40:20.000000 vois-1.0.9/src/vois/vuetify/dialogGeneric.py
+-rw-rw-rw-   0        0        0     4304 2023-06-20 05:40:20.000000 vois-1.0.9/src/vois/vuetify/dialogMessage.py
+-rw-rw-rw-   0        0        0     5785 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/dialogWait.py
+-rw-rw-rw-   0        0        0     5423 2023-06-20 05:40:20.000000 vois-1.0.9/src/vois/vuetify/dialogYesNo.py
+drwxrwxrwx   0        0        0        0 2023-08-21 12:46:47.572083 vois-1.0.9/src/vois/vuetify/extra/
+-rw-rw-rw-   0        0        0       47 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/extra/__init__.py
+-rw-rw-rw-   0        0        0     6838 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/extra/file_input.py
+-rw-rw-rw-   0        0        0     2251 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/extra/file_input.vue
+-rw-rw-rw-   0        0        0    12885 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/fab.py
+-rw-rw-rw-   0        0        0      996 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/fontsettings.py
+-rw-rw-rw-   0        0        0    13881 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/footer.py
+-rw-rw-rw-   0        0        0     5865 2023-06-20 05:40:20.000000 vois-1.0.9/src/vois/vuetify/iconButton.py
+-rw-rw-rw-   0        0        0     8029 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/label.py
+-rw-rw-rw-   0        0        0    48546 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/layers.py
+-rw-rw-rw-   0        0        0    23017 2023-06-16 10:48:12.000000 vois-1.0.9/src/vois/vuetify/mainPage.py
+-rw-rw-rw-   0        0        0     6454 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/menu.py
+-rw-rw-rw-   0        0        0     7653 2023-08-21 12:42:55.000000 vois-1.0.9/src/vois/vuetify/multiSwitch.py
+-rw-rw-rw-   0        0        0    57418 2023-08-21 12:42:55.000000 vois-1.0.9/src/vois/vuetify/page.py
+-rw-rw-rw-   0        0        0    24701 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/paletteEditor.py
+-rw-rw-rw-   0        0        0    15331 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/palettePicker.py
+-rw-rw-rw-   0        0        0     8048 2023-06-09 16:34:03.000000 vois-1.0.9/src/vois/vuetify/palettePickerEx.py
+-rw-rw-rw-   0        0        0     6284 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/popup.py
+-rw-rw-rw-   0        0        0     6181 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/progress.py
+-rw-rw-rw-   0        0        0     1821 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/queryStrings.py
+-rw-rw-rw-   0        0        0     4708 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/radio.py
+-rw-rw-rw-   0        0        0     4390 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/rangeSlider.py
+-rw-rw-rw-   0        0        0    17054 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/rangeSliderFloat.py
+-rw-rw-rw-   0        0        0     9365 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/selectImage.py
+-rw-rw-rw-   0        0        0     6052 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/selectMultiple.py
+-rw-rw-rw-   0        0        0     8721 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/selectSingle.py
+-rw-rw-rw-   0        0        0     4816 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/settings.py
+-rw-rw-rw-   0        0        0     6679 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/sidePanel.py
+-rw-rw-rw-   0        0        0     5546 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/slider.py
+-rw-rw-rw-   0        0        0    12119 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/sliderFloat.py
+-rw-rw-rw-   0        0        0     4590 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/snackbar.py
+-rw-rw-rw-   0        0        0    24635 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/sortableList.py
+-rw-rw-rw-   0        0        0     6575 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/svgsGrid.py
+-rw-rw-rw-   0        0        0     4695 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/switch.py
+-rw-rw-rw-   0        0        0     6967 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/tabs.py
+-rw-rw-rw-   0        0        0     6369 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/textlist.py
+-rw-rw-rw-   0        0        0     7009 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/title.py
+-rw-rw-rw-   0        0        0     7903 2023-08-21 12:42:55.000000 vois-1.0.9/src/vois/vuetify/toggle.py
+-rw-rw-rw-   0        0        0     3179 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/tooltip.py
+-rw-rw-rw-   0        0        0    68877 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/treeview.py
+-rw-rw-rw-   0        0        0     5036 2023-06-09 16:34:02.000000 vois-1.0.9/src/vois/vuetify/upload.py
+drwxrwxrwx   0        0        0        0 2023-08-21 12:46:46.414731 vois-1.0.9/src/vois.egg-info/
+-rw-rw-rw-   0        0        0    21433 2023-08-21 12:46:45.000000 vois-1.0.9/src/vois.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2219 2023-08-21 12:46:45.000000 vois-1.0.9/src/vois.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-21 12:46:45.000000 vois-1.0.9/src/vois.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-08-21 12:46:45.000000 vois-1.0.9/src/vois.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-21 12:46:45.000000 vois-1.0.9/src/vois.egg-info/top_level.txt
```

### Comparing `vois-1.0.8/LICENCE` & `vois-1.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/MANIFEST.in` & `vois-1.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/Notice.txt` & `vois-1.0.9/Notice.txt`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/PKG-INFO` & `vois-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vois
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python Voilà simplification library
 Author-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 Maintainer-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 License: Copyright © European Union 2022-2023
         
         
                               EUROPEAN UNION PUBLIC LICENCE v. 1.2
```

### Comparing `vois-1.0.8/README.md` & `vois-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/pyproject.toml` & `vois-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 name = "vois"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.8"  # Required
+version = "1.0.9"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A Python Voilà simplification library"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `vois-1.0.8/src/vois/colors.py` & `vois-1.0.9/src/vois/colors.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/download.py` & `vois-1.0.9/src/vois/download.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/eucountries.py` & `vois-1.0.9/src/vois/eucountries.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/geojsonUtils.py` & `vois-1.0.9/src/vois/geojsonUtils.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/interMap.py` & `vois-1.0.9/src/vois/interMap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/ipytrees.py` & `vois-1.0.9/src/vois/ipytrees.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/leafletMap.py` & `vois-1.0.9/src/vois/leafletMap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/svgBubblesChart.py` & `vois-1.0.9/src/vois/svgBubblesChart.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/svgGraph.py` & `vois-1.0.9/src/vois/svgGraph.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/svgHeatmap.py` & `vois-1.0.9/src/vois/svgHeatmap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/svgMap.py` & `vois-1.0.9/src/vois/svgMap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/svgPackedCirclesChart.py` & `vois-1.0.9/src/vois/svgPackedCirclesChart.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/svgRankChart.py` & `vois-1.0.9/src/vois/svgRankChart.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/svgUtils.py` & `vois-1.0.9/src/vois/svgUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -563,15 +563,15 @@
     fill50  = 3
     fill40  = 4
 
 def AnimatedPieChart(values=[10.0, 25.0, 34.0, 24.0, 23.0], colors=['#2d82c2', '#95cb92', '#e7ee99', '#ffde88', '#ff945a', '#e34e4f'], labels=None, duration=0.75, # Seconds
                      fillpercentage=FillPercentage.fill60, backcolor="#f1f1f1", dimension=400,
                      textcolor=settings.select_textcolor, fontsize=15, textweight=400, decimals=1,
                      centertext='', centercolor=settings.select_textcolor, centerfontsize=18, centertextweight=500,
-                     onclick=None, additional_argument=None, is_selected=False):
+                     onclick=None, additional_argument=None, is_selected=False, displayvalues=True):
     """
     Creation of an animated pie chart in SVG format. Given an array of float values, and optional labels, the function draws a pie chart that fills its slices with a short animation. An ipywidgets.Output instance is returned, which has the SVG chart displayed in it. By passing a value to the onclick parameter, it is possible to manage the click event on the slices of the pie, providing interactivity to the drawing. The capture of the click event is done using the `ipyevents library <https://github.com/mwcraig/ipyevents>`_ .
     
     Parameters
     ----------
     values : list of float values, optional
         List of float values that represent the relative dimension of each of the slices (default is [10.0, 25.0, 34.0, 24.0, 23.0])
@@ -605,14 +605,16 @@
         Weight of central text (default is 500, >= 500 is Bold)
     onclick : function, optional
         Python function to call when the user clicks on one of the slices of the pie. The function will receive as first parameter the index of the clicked slice, and the additional_argument as second parameter
     additional_argument : any, optional
         Additional parameter passed to the onclick function when the user clicks on one of the slices of the pie (default is None)
     is_selected : bool, optional
         Flag to select the pie chart (default is False)
+    displayvalues: bool, optional
+        If True each slide of the pie will display, inside parenthesis, the corresponding value (default is True)
    
     
     Return
     ------
         a tuple containing an instance of ipywidgets.Output() widget, and a string containing the SVG code of the drawing
     
     Example
@@ -733,20 +735,27 @@
                 
         color = colors[i % len(colors)]
         color_no_answer = '#757575'
 
         strvalue = '{:.{prec}f}'.format(perc[i], prec=decimals)
 
         if not labels is None and i < len(labels):
-            text = '%s<br>%s%%<br>(%s)' % (labels[i],strvalue,values[i])
+            if displayvalues:
+                text = '%s<br>%s%%<br>(%s)' % (labels[i],strvalue,values[i])
+            else:
+                text = '%s<br>%s%%' % (labels[i],strvalue)
+                     
             
             if text[:9] == 'no answer' or text[:12] == 'no<br>answer': color = color_no_answer    # Request for same color for all the "no answer" slices
             #print(text)
         else:
-            text = strvalue + '<br>(' + str(values[i])+ ')'
+            if displayvalues:
+                text = strvalue + '<br>(' + str(values[i])+ ')'
+            else:
+                text = strvalue
         
         fulltext = centertext + ': ' + text.replace('<br>',' ')
         tooltip = '<title>%s</title>' % (fulltext)
             
         x,y = textPosition(startangle+angle/2.0, textdistance)
 
         svgtext = ''
```

### Comparing `vois-1.0.8/src/vois/treemapPlotly.py` & `vois-1.0.9/src/vois/treemapPlotly.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/urlOpen.py` & `vois-1.0.9/src/vois/urlOpen.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/urlUpdate.py` & `vois-1.0.9/src/vois/urlUpdate.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/app.py` & `vois-1.0.9/src/vois/vuetify/app.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/basemaps.py` & `vois-1.0.9/src/vois/vuetify/basemaps.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/button.py` & `vois-1.0.9/src/vois/vuetify/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,16 @@
         Color of the icon (default is 'black')
     autoselect : bool, optional
         If True, the button becomes selected when clicked (default is False)
     dark : bool, optional
         Flag to invert the text and backcolor (default is the value of settings.dark_mode)
     rounded : bool, optional
         Flag to display the button with rounded corners (default is the value of settings.button_rounded)
+    tile : bool, optional
+        Flag to remove the button small border (default is False)
     colorselected : str, optional
         Color used for the button when it is selected (default is settings.color_first)
     colorunselected : str, optional
         Color used for the button when it is not selected (default is settings.color_second)
             
     Note
     ----
@@ -144,15 +146,15 @@
    """
 
    
     # Initialization
     def __init__(self, text, onclick=None, argument=None, width=100, height=36, selected=False, disabled=False, tooltip='', large=False, small=False, xsmall=False, outlined=False, textweight=500,
                  href=None, target=None, onlytext=False, textcolor=None,  class_="pa-0 ma-0",
                  icon=None, iconlarge=False, iconsmall=False, iconleft=False, iconcolor='black',
-                 autoselect=False, dark=settings.dark_mode, rounded=settings.button_rounded,
+                 autoselect=False, dark=settings.dark_mode, rounded=settings.button_rounded, tile=False,
                  colorselected=settings.color_first, colorunselected=settings.color_second
                 ):
         self.onclick    = onclick
         self.argument   = argument
         self._selected  = selected
         self._disabled  = disabled
         self.autoselect = autoselect
@@ -181,15 +183,15 @@
                 if len(self.text) == 0: childs = [icn]
                 else:                   childs = [icn, self.text]
             else:
                 if len(self.text) == 0: childs = [icn]
                 else:                   childs = [self.text, icn]
             
         self.b = v.Btn(color=color, dark=dark, icon=onlytext, depressed=True, outlined=outlined, large=large, small=small, x_small=xsmall, 
-                       disabled=disabled, width=width, min_width=width, height=height, min_height=height, href=href, target=target,
+                       disabled=disabled, width=width, min_width=width, height=height, min_height=height, href=href, target=target, tile=tile, 
                        children=childs, style_='font-family: %s; font-size: 17; font-weight: %d; text-transform: none' % (fontsettings.font_name, textweight), rounded=rounded)
                 
         self.b.on_event('click', self.__internal_onclick)
         
         if len(tooltip) > 0: self.b.v_on = 'tooltip.on'
         self.container = v.Container(class_=class_, children=[ v.Tooltip(color=settings.tooltip_backcolor, transition="scale-transition", bottom=True, 
                                                                          v_slots=[{'name': 'activator', 'variable': 'tooltip', 'children': self.b }],
```

### Comparing `vois-1.0.8/src/vois/vuetify/card.py` & `vois-1.0.9/src/vois/vuetify/card.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,14 +156,15 @@
   <v-card
     class="pa-1 ma-1"
     :width="width"
     :height="height"
     :color="color"
     :dark="dark"
     raised
+    hover
     :elevation="elevation"
     :ripple="ripple"
     :disabled="disabled"
     @click="clicked"
     style="overflow: hidden;"
     :img="backgroundimageurl"
   >
@@ -178,15 +179,15 @@
                 %s
                 <v-card-title %s class="mt-n2 mb-1" :style="fontSizeTitle" v-text="title"></v-card-title>
                 %s
             </v-row>
           <div :class="subtitlemargins" :style="fontSizeSubTitle" v-html="subtitle"/>
       </div>
       <v-avatar class="ma-n1" :size="imagesize" tile >
-         <v-img :src="image"></v-img>
+         <v-img :src="image" contain></v-img>
       </v-avatar>
     </div>
   </v-card>
 %s
 
 <script>
   export default {
```

### Comparing `vois-1.0.8/src/vois/vuetify/cardsGrid.py` & `vois-1.0.9/src/vois/vuetify/cardsGrid.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/colorPicker.py` & `vois-1.0.9/src/vois/vuetify/colorPicker.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/datatable.py` & `vois-1.0.9/src/vois/vuetify/datatable.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                 :height="height"
                 :headers="headers"
                 :items="items"
                 :item-key="index_col"
                 :footer-props="{'items-per-page-options': [10000000]}">
                 <template v-slot:no-data> 
                   <v-alert :value="true" :color="color" :dark="dark" icon="mdi-alert">
-                    No use-cases to display
+                    No records to display
                   </v-alert>
                 </template>
                 <template v-slot:no-results>
                     <v-alert :value="true" :color="color" :dark="dark" icon="mdi-alert" width="80vw">
                       Your search for "{{ search }}" found no results
                     </v-alert>
                 </template>
```

### Comparing `vois-1.0.8/src/vois/vuetify/datePicker.py` & `vois-1.0.9/src/vois/vuetify/datePicker.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/dialogGeneric.py` & `vois-1.0.9/src/vois/vuetify/dialogGeneric.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/dialogMessage.py` & `vois-1.0.9/src/vois/vuetify/dialogMessage.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/dialogWait.py` & `vois-1.0.9/src/vois/vuetify/dialogWait.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/dialogYesNo.py` & `vois-1.0.9/src/vois/vuetify/dialogYesNo.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/extra/file_input.py` & `vois-1.0.9/src/vois/vuetify/extra/file_input.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/extra/file_input.vue` & `vois-1.0.9/src/vois/vuetify/extra/file_input.vue`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/fab.py` & `vois-1.0.9/src/vois/vuetify/fab.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/fontsettings.py` & `vois-1.0.9/src/vois/vuetify/fontsettings.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/footer.py` & `vois-1.0.9/src/vois/vuetify/footer.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/iconButton.py` & `vois-1.0.9/src/vois/vuetify/iconButton.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/label.py` & `vois-1.0.9/src/vois/vuetify/label.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/layers.py` & `vois-1.0.9/src/vois/vuetify/layers.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/mainPage.py` & `vois-1.0.9/src/vois/vuetify/mainPage.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/menu.py` & `vois-1.0.9/src/vois/vuetify/menu.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/multiSwitch.py` & `vois-1.0.9/src/vois/vuetify/multiSwitch.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,21 +72,21 @@
         
         from vois.vuetify import multiSwitch
         from ipywidgets import widgets
         from IPython.display import display
         
         output = widgets.Output()
 
-        def onchange(index):
+        def onchange(values):
             with output:
-                print(index)
+                print(values)
 
         m = multiSwitch.multiSwitch([False, True, False], ['Option 1', 'Option 2', 'Option 3'],
                                     tooltips=['Tooltip for option 1'], 
-                                    onchange=onchange, row=False, width=150, rounded=Falseoutlined=True,
+                                    onchange=onchange, row=False, width=150, rounded=False, outlined=True,
                                     colorselected='#FFA300', colorunselected='#aaaaaa')
 
         display(m.draw())
         display(output)
 
 
     .. figure:: figures/multiSwitch.png
```

### Comparing `vois-1.0.8/src/vois/vuetify/page.py` & `vois-1.0.9/src/vois/vuetify/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,20 @@
             
         if len(self.title) > 0:
             subtitle = v.ToolbarTitle(children=[self.title], class_='pa-0 ma-0 mt-1 ml-2', style_='height: 30px; color: %s; font-size: 26;'%textcolor)
             children.append(subtitle)
         
         children.append(v.Spacer())
         
+        for cb in self.custom_buttons:
+            iconname,tooltiptext,callback = cb
+            btn = v.Btn(icon=True, class_="pa-0 ma-0 mt-1", dark=self.titledark, children=[v.Icon(children=[iconname])])
+            btn.on_event('click', callback)
+            children.append(tooltip.tooltip(tooltiptext, btn))
+        
         if self.show_back:
             btn_back = v.Btn(icon=True, class_="pa-0 ma-0 mt-1", dark=self.titledark, children=[v.Icon(children=['mdi-arrow-left'])])
             btn_back.on_event('click', self.click_on_back)
             children.append(tooltip.tooltip("Close current page", btn_back))
             
         if self.show_help:
             btn_help = v.Btn(icon=True, class_="pa-0 ma-0 mt-1 mr-3", dark=self.titledark, children=[v.Icon(children=['mdi-help'])])
@@ -211,15 +217,23 @@
     # Close the dialog
     def close(self):
         if not self.dlg is None:
             self.dlg.close()
             if not self.onclose is None:
                 self.onclose()
         
+        
+    # Add a custom buttom to the page (before the call to create!)
+    def customButtonAdd(self, iconname, tooltiptext, callback):
+        self.custom_buttons.append((iconname,tooltiptext,callback))   # Each item has an icon name, a tooltip string and a callback function
     
+    # Remove all custom buttons
+    def customButtonClear(self):
+        self.custom_buttons = []
+        
     
     # Initialization
     def __init__(self,
                  appname,
                  title,
                  output,
                  onclose=None,
@@ -259,14 +273,16 @@
         self.on_help       = on_help
         self.show_credits  = show_credits
         self.on_credits    = on_credits
         self.on_logoapp    = on_logoapp
         
         self.transition    = transition
         
+        self.custom_buttons = []   # Each item has an icon name, a tooltip string and a callback function
+        
         if len(logoappurl) > 0:
             self.logoapp = v.Img(class_='pa-0 ma-0 mr-2', max_width=self.logowidth, src=logoappurl)
         else:
             self.logoapp = None
         
         if len(logocreditsurl) > 0:
             self.logoCredits = v.Img(class_='pa-0 ma-0 mr-2', max_width=120, src=logocreditsurl)
```

### Comparing `vois-1.0.8/src/vois/vuetify/paletteEditor.py` & `vois-1.0.9/src/vois/vuetify/paletteEditor.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/palettePicker.py` & `vois-1.0.9/src/vois/vuetify/palettePicker.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/palettePickerEx.py` & `vois-1.0.9/src/vois/vuetify/palettePickerEx.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/popup.py` & `vois-1.0.9/src/vois/vuetify/popup.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/progress.py` & `vois-1.0.9/src/vois/vuetify/progress.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/queryStrings.py` & `vois-1.0.9/src/vois/vuetify/queryStrings.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/radio.py` & `vois-1.0.9/src/vois/vuetify/radio.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/rangeSlider.py` & `vois-1.0.9/src/vois/vuetify/rangeSlider.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/rangeSliderFloat.py` & `vois-1.0.9/src/vois/vuetify/rangeSliderFloat.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/selectImage.py` & `vois-1.0.9/src/vois/vuetify/selectImage.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/selectMultiple.py` & `vois-1.0.9/src/vois/vuetify/selectMultiple.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/selectSingle.py` & `vois-1.0.9/src/vois/vuetify/selectSingle.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/settings.py` & `vois-1.0.9/src/vois/vuetify/settings.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/sidePanel.py` & `vois-1.0.9/src/vois/vuetify/sidePanel.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/slider.py` & `vois-1.0.9/src/vois/vuetify/slider.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/sliderFloat.py` & `vois-1.0.9/src/vois/vuetify/sliderFloat.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/snackbar.py` & `vois-1.0.9/src/vois/vuetify/snackbar.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/sortableList.py` & `vois-1.0.9/src/vois/vuetify/sortableList.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/svgsGrid.py` & `vois-1.0.9/src/vois/vuetify/svgsGrid.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/switch.py` & `vois-1.0.9/src/vois/vuetify/switch.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/tabs.py` & `vois-1.0.9/src/vois/vuetify/tabs.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/textlist.py` & `vois-1.0.9/src/vois/vuetify/textlist.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/title.py` & `vois-1.0.9/src/vois/vuetify/title.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/toggle.py` & `vois-1.0.9/src/vois/vuetify/toggle.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,20 @@
         Flag to display the buttons as outlined (default is False)
     colorselected : str, optional
         Color used for the buttons when they are selected (default is settings.color_first)
     colorunselected : str, optional
         Color used for the buttons when they are not selected (default is settings.color_second)
     dark : bool, optional
         Flag that controls the color of the text in foreground (if True, the text will be displayed in white, elsewhere in black)
+    paddingrow : int, optional
+        Horizontal padding among toggle buttons (1 unit means 4 pixels). Default is 1
+    paddingcol : int, optional
+        Vertical padding among toggle buttons (1 unit means 4 pixels). Default is 2
+    tile : bool, optional
+        Flag to remove the buttons small border (default is False)
 
     Example
     -------
     Creation and display of a widget for the selection among 3 options::
         
         from vois.vuetify import toggle
         from ipywidgets import widgets
@@ -93,52 +99,52 @@
 
        Toogle widget for selecting alternative options using buttons.
    """
 
     # Initialization
     def __init__(self, index, labels, tooltips=None, color=settings.color_first, onchange=None,
                  row=True, width=150, justify='space-between', rounded=settings.button_rounded, outlined=False,
-                 colorselected=settings.color_first, colorunselected=settings.color_second, dark=settings.dark_mode):
+                 colorselected=settings.color_first, colorunselected=settings.color_second, dark=settings.dark_mode,
+                 paddingrow=1, paddingcol=2, tile=False):
         
         self.index    = index    # Index of the selected button
         self.labels   = labels
         self.tooltips = tooltips
         self.color    = color
         self.onchange = onchange
         self.row      = row
         self.width    = width
         self.justify  = justify
         self.rounded  = rounded
         self.outlined = outlined
         self.colorselected   = colorselected
         self.colorunselected = colorunselected
         self.dark            = dark
+        self.paddingrow      = paddingrow
+        self.paddingcol      = paddingcol
+        self.tile            = tile
         
         self.__createButtons()
         
         
     # Create the toggle buttons
     def __createButtons(self):
 
         self.buttons = []
         i = 0
         for label in self.labels:
             tooltip = ''
             if i < len(self.tooltips):
                 tooltip = self.tooltips[i]
             
-            if self.row: c = "pa-0 ma-0 mr-1"
-            else:
-                if i == len(self.labels)-1:
-                    c = "pa-0 ma-0 mb-7"
-                else:
-                    c = "pa-0 ma-0 mb-2"
+            if self.row: c = "pa-0 ma-0 mr-%d"%self.paddingrow
+            else:        c = "pa-0 ma-0 mb-%d"%self.paddingcol
                     
             b = button.button(label, dark=self.dark, class_=c, onclick=self.__internal_onchange, argument=i, width=self.width, tooltip=tooltip, selected=(i==self.index),
-                              rounded=self.rounded, outlined=self.outlined, colorselected=self.colorselected, colorunselected=self.colorunselected)
+                              rounded=self.rounded, tile=self.tile, outlined=self.outlined, colorselected=self.colorselected, colorunselected=self.colorunselected)
             self.buttons.append(b)
             i += 1
 
         if self.row: self.group = v.Row(class_="pa-0 ma-0", justify=self.justify, children=[x.draw() for x in self.buttons], style_="overflow: hidden;")
         else:        self.group = v.Col(cols=12, class_="pa-0 ma-0", children=[x.draw() for x in self.buttons], style_="overflow: hidden;")
```

### Comparing `vois-1.0.8/src/vois/vuetify/tooltip.py` & `vois-1.0.9/src/vois/vuetify/tooltip.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/treeview.py` & `vois-1.0.9/src/vois/vuetify/treeview.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois/vuetify/upload.py` & `vois-1.0.9/src/vois/vuetify/upload.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.8/src/vois.egg-info/PKG-INFO` & `vois-1.0.9/src/vois.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vois
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python Voilà simplification library
 Author-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 Maintainer-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 License: Copyright © European Union 2022-2023
         
         
                               EUROPEAN UNION PUBLIC LICENCE v. 1.2
```

### Comparing `vois-1.0.8/src/vois.egg-info/SOURCES.txt` & `vois-1.0.9/src/vois.egg-info/SOURCES.txt`

 * *Files identical despite different names*

