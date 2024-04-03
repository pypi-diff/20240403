# Comparing `tmp/pytincture-0.4.2.tar.gz` & `tmp/pytincture-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytincture-0.4.2.tar", last modified: Wed Mar 20 20:10:30 2024, max compression
+gzip compressed data, was "pytincture-0.4.3.tar", last modified: Wed Apr  3 18:32:15 2024, max compression
```

## Comparing `pytincture-0.4.2.tar` & `pytincture-0.4.3.tar`

### file list

```diff
@@ -1,361 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.441079 pytincture-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-20 20:10:20.000000 pytincture-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-20 20:10:30.441079 pytincture-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-03-20 20:10:20.000000 pytincture-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.397079 pytincture-0.4.2/pytincture/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.397079 pytincture-0.4.2/pytincture/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/backend/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.397079 pytincture-0.4.2/pytincture/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/pytincture.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.397079 pytincture-0.4.2/pytincture/frontend/widgetsets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/accordion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.405079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.409079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    20780 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/fonts/roboto-bold-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    15804 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/fonts/roboto-bold-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    20972 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/fonts/roboto-medium-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    15908 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/fonts/roboto-medium-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    20800 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/fonts/roboto-regular-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    15668 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/fonts/roboto-regular-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/license.txt
--rw-r--r--   0 runner    (1001) docker     (127)   167425 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/suite.css
--rw-r--r--   0 runner    (1001) docker     (127)    37787 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/suite.css.map
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/suite.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)  1835207 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/suite.js
--rw-r--r--   0 runner    (1001) docker     (127)  1402615 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/suite.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   166463 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/suite.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   865826 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/suite.min.js
--rw-r--r--   0 runner    (1001) docker     (127)  1402619 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/suite.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.393079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.389078 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-all/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.409079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-all/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-all/sources/entry.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.409079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-calendar/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-calendar/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.409079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-calendar/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-calendar/sources/Calendar.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-calendar/sources/helper.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-calendar/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.409079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.409079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/AxisCreator.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/Chart.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/ComposeLayer.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/Export.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/Filters.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/Legend.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/ProChart.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/Tooltip.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.409079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/helpers/circle.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/helpers/common.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/helpers/spline.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.409079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/scales/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/scales/RadialScale.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/scales/Scale.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/scales/SvgScales.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/scales/TextScale.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/scales/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.413079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/Area.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/Bar.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/BarX.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/BaseSeria.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/CalendarHeatMap.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/Donut.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/Line.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/NoScaleSeria.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/Pie.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/Pie3D.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/Radar.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/ScaleSeria.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/Scatter.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/Spline.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/SplineArea.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/Stacker.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/TreeMap.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/series/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.413079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/shapes/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/shapes/legend.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/shapes/line.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-chart/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.413079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-colorpicker/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-colorpicker/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.413079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-colorpicker/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-colorpicker/sources/Colorpicker.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-colorpicker/sources/colors.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.413079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-colorpicker/sources/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-colorpicker/sources/helpers/calculations.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-colorpicker/sources/helpers/color.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.413079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-colorpicker/sources/locales/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-colorpicker/sources/locales/en.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-colorpicker/sources/picker.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-colorpicker/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.413079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-combobox/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-combobox/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.417079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-combobox/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-combobox/sources/Combobox.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-combobox/sources/ProCombobox.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-combobox/sources/helper.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-combobox/sources/keyListener.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.417079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-combobox/sources/locales/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-combobox/sources/locales/en.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-combobox/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.417079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/CssManager.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/FocusManager.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/KeyManager.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/ScrollView.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/core.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/date.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/dom.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/events.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/html.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/keycodes.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.417079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/polyfills/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/polyfills/array.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/polyfills/element.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/polyfills/math.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/polyfills/object.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/polyfills/string.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/types.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-common/view.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.417079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.421079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/CollectionStore.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/DragManager.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/ajax.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.421079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/datacollection/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/datacollection/loader.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/datacollection/sort.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/datacollection.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/dataproxy.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.421079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/drivers/CsvDriver.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/drivers/JsonDriver.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/drivers/XMLDriver.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/drivers/drivers.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/helpers.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/lazydataproxy.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/selection.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.421079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/serializers/xml.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/treecollection.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-data/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.421079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-dataview/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-dataview/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.421079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-dataview/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-dataview/sources/DataView.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-dataview/sources/ProDataView.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.421079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-dataview/sources/editors/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-dataview/sources/editors/InputEditor.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-dataview/sources/editors/editors.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-dataview/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.421079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.421079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/Form.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/ProForm.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.425079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/ToggleButton.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/ToggleGroup.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/avatar.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/button.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/checkbox.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/checkboxGroup.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/colorpicker.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/combo.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/container.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/dateinput.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/fieldset.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.425079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/helper/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/helper/label.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/input.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/radioGroup.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/radiobutton.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/select.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/simplevault.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/sliderform.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/spacer.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/textarea.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/textinput.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/elements/timeinput.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/helper.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.425079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/locales/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/locales/en.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-form/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.425079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.425079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/Exporter.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/Grid.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ProGrid.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/Selection.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/columnsResizer.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.429079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/helpers/cells.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/helpers/data.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/helpers/keys.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/helpers/main.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)    21100 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.429079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/Cells.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/FixedCols.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/FixedRows.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.429079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/content/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/content/ComboFilter.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/content/InputFilter.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/content/SelectFilter.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/content.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.429079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/editors/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/editors/CheckboxEditor.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/editors/ComboboxEditor.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/editors/DateEditor.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/editors/InputEditor.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/editors/SelectEditor.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/editors/TextAreaEditor.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/editors/editors.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-grid/sources/ui/render.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.429079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-layout/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-layout/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.429079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-layout/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-layout/sources/Cell.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-layout/sources/Layout.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-layout/sources/ProCell.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-layout/sources/ProLayout.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-layout/sources/helpers.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-layout/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.429079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-list/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-list/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.433079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-list/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-list/sources/List.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-list/sources/ProList.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-list/sources/Selection.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.433079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-list/sources/editors/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-list/sources/editors/InputEditor.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-list/sources/editors/editors.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-list/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.433079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-menu/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-menu/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.433079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-menu/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-menu/sources/ContextMenu.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-menu/sources/Menu.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.433079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-message/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-message/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.433079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-message/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-message/sources/alert.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-message/sources/common.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-message/sources/confirm.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.433079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-message/sources/locales/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-message/sources/locales/en.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-message/sources/message.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-message/sources/tooltip.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-message/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.433079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.433079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/Navbar.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/elements/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/elements/button.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/elements/customHTMLButton.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/elements/datePicker.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/elements/helpers.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/elements/imageButton.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/elements/input.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/elements/menuItem.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/elements/navItem.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/elements/separator.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/elements/spacer.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/elements/title.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/itemfactory.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-navbar/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-popup/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-popup/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-popup/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-popup/sources/Popup.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-popup/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-ribbon/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-ribbon/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-ribbon/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-ribbon/sources/ProRibbon.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-ribbon/sources/Ribbon.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-sidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-sidebar/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-sidebar/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-sidebar/sources/ProSidebar.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-sidebar/sources/Sidebar.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-sidebar/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-slider/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-slider/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-slider/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-slider/sources/Slider.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-slider/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-tabbar/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-tabbar/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-tabbar/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-tabbar/sources/Tabbar.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-tabbar/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-timepicker/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-timepicker/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-timepicker/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-timepicker/sources/Timepicker.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-timepicker/sources/helper.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-timepicker/sources/locales/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-timepicker/sources/locales/en.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-timepicker/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.437079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-toolbar/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-toolbar/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.441079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-toolbar/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-toolbar/sources/ProToolbar.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-toolbar/sources/Toolbar.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.441079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-tree/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-tree/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.441079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-tree/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-tree/sources/Editor.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-tree/sources/Tree.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-tree/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.441079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-vault/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-vault/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.441079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-vault/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-vault/sources/ProgressBar.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-vault/sources/ReadStackPreview.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-vault/sources/Uploader.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-vault/sources/Vault.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-vault/sources/configs.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-vault/sources/helper.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.441079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-vault/sources/locales/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-vault/sources/locales/en.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-vault/sources/types.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.441079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-window/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-window/index.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.441079 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-window/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-window/sources/ProWindow.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-window/sources/Window.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-window/sources/WindowController.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-window/sources/helpers.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/dhxsrc/types/ts-window/sources/types.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)    97035 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/form.py
--rw-r--r--   0 runner    (1001) docker     (127)    35424 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/sidebar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.441079 pytincture-0.4.2/pytincture/frontend/widgetsets/tincture/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/tincture/tincture.css
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/tincture/tincture.js
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-03-20 20:10:20.000000 pytincture-0.4.2/pytincture/frontend/widgetsets/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 20:10:30.397079 pytincture-0.4.2/pytincture.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-20 20:10:30.000000 pytincture-0.4.2/pytincture.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19895 2024-03-20 20:10:30.000000 pytincture-0.4.2/pytincture.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 20:10:30.000000 pytincture-0.4.2/pytincture.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-20 20:10:30.000000 pytincture-0.4.2/pytincture.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-20 20:10:30.000000 pytincture-0.4.2/pytincture.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 20:10:30.441079 pytincture-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-20 20:10:20.000000 pytincture-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:32:15.919792 pytincture-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-03 18:32:06.000000 pytincture-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-03 18:32:15.919792 pytincture-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-03 18:32:06.000000 pytincture-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:32:15.915792 pytincture-0.4.3/pytincture/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-03 18:32:06.000000 pytincture-0.4.3/pytincture/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:32:15.915792 pytincture-0.4.3/pytincture/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:32:06.000000 pytincture-0.4.3/pytincture/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-03 18:32:06.000000 pytincture-0.4.3/pytincture/backend/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-03 18:32:06.000000 pytincture-0.4.3/pytincture/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:32:15.915792 pytincture-0.4.3/pytincture/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-03 18:32:06.000000 pytincture-0.4.3/pytincture/frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-03 18:32:06.000000 pytincture-0.4.3/pytincture/frontend/pytincture.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:32:15.915792 pytincture-0.4.3/pytincture.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-03 18:32:15.000000 pytincture-0.4.3/pytincture.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 18:32:15.000000 pytincture-0.4.3/pytincture.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:32:15.000000 pytincture-0.4.3/pytincture.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 18:32:15.000000 pytincture-0.4.3/pytincture.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 18:32:15.000000 pytincture-0.4.3/pytincture.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:32:15.919792 pytincture-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-03 18:32:06.000000 pytincture-0.4.3/setup.py
```

### Comparing `pytincture-0.4.2/PKG-INFO` & `pytincture-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytincture
-Version: 0.4.2
+Version: 0.4.3
 Summary: UI Builder
 Home-page: https://github.com/pytincture/pytincture
 Description-Content-Type: text/markdown
 
 # pyTincture
 
 ## Overview
@@ -19,15 +19,15 @@
 ## Requirements
 - Python 3.x
 - Pyodide
 
 ## Docker Quick Start
 Run the docker image directly from Dockerhub
 ~~~
-docker run -p8070:8070 -i pytincture/pytincture:example042
+docker run -p8070:8070 -i pytincture/pytincture:example043
 ~~~
 Load url in browser
 ~~~
 http://localhost:8070/py_ui
 ~~~
 
 ## Docker build from repo
```

### Comparing `pytincture-0.4.2/README.md` & `pytincture-0.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ## Requirements
 - Python 3.x
 - Pyodide
 
 ## Docker Quick Start
 Run the docker image directly from Dockerhub
 ~~~
-docker run -p8070:8070 -i pytincture/pytincture:example042
+docker run -p8070:8070 -i pytincture/pytincture:example043
 ~~~
 Load url in browser
 ~~~
 http://localhost:8070/py_ui
 ~~~
 
 ## Docker build from repo
```

### Comparing `pytincture-0.4.2/pytincture/__init__.py` & `pytincture-0.4.3/pytincture/__init__.py`

 * *Files identical despite different names*

### Comparing `pytincture-0.4.2/pytincture/backend/app.py` & `pytincture-0.4.3/pytincture/backend/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import zipfile
 from fastapi import FastAPI, Response, Request
 from fastapi.staticfiles import StaticFiles
 from fastapi.responses import StreamingResponse
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import HTMLResponse
 from pytincture.dataclass import get_parsed_output
-import imp
+from importlib.machinery import SourceFileLoader
+from typing import Callable
 import json
 import io
 
 
 app = FastAPI()
 
 def create_appcode_pkg_in_memory(host, protocol):
@@ -103,29 +104,32 @@
     host = request.headers["host"]
     file_like = create_appcode_pkg_in_memory(host, protocol)
     return StreamingResponse(file_like, media_type="application/zip", headers={"Content-Disposition": "attachment; filename=appcode.pyt"})
 
 #Class call endpoint
 @app.get("/classcall/{file_name}/{class_name}/{function_name}")
 @app.post("/classcall/{file_name}/{class_name}/{function_name}")
-async def class_call(file_name, class_name, function_name, request: Request):
+async def class_call(file_name: str, class_name: str, function_name: str, request: Request):
     appcode_folder = os.environ["MODULES_PATH"]
     file_path = os.path.join(appcode_folder, file_name)
-    lib = imp.load_source(class_name, file_path)
-    cls = getattr(lib, class_name)
+    
+    loader = SourceFileLoader(class_name, file_path)
+    spec = loader.load_module()
+    
+    cls = getattr(spec, class_name)
     instance = cls()
     func = getattr(instance, function_name)
-    if callable(func):
+    
+    if isinstance(func, Callable):
         data = await request.json()
         data = json.loads(data)
         return func(*data["args"], **data["kwargs"])
     else:
         return func
 
-
 #Static files endpoint
 app.mount("/appcode", StaticFiles(directory=MODULE_PATH), name="static")
 
 @app.get("/appdata", response_class=HTMLResponse)
 async def main(function_name, data_module):
     pass
```

### Comparing `pytincture-0.4.2/pytincture/dataclass.py` & `pytincture-0.4.3/pytincture/dataclass.py`

 * *Files identical despite different names*

### Comparing `pytincture-0.4.2/pytincture.egg-info/PKG-INFO` & `pytincture-0.4.3/pytincture.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytincture
-Version: 0.4.2
+Version: 0.4.3
 Summary: UI Builder
 Home-page: https://github.com/pytincture/pytincture
 Description-Content-Type: text/markdown
 
 # pyTincture
 
 ## Overview
@@ -19,15 +19,15 @@
 ## Requirements
 - Python 3.x
 - Pyodide
 
 ## Docker Quick Start
 Run the docker image directly from Dockerhub
 ~~~
-docker run -p8070:8070 -i pytincture/pytincture:example042
+docker run -p8070:8070 -i pytincture/pytincture:example043
 ~~~
 Load url in browser
 ~~~
 http://localhost:8070/py_ui
 ~~~
 
 ## Docker build from repo
```

### Comparing `pytincture-0.4.2/setup.py` & `pytincture-0.4.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     install_requires = reqs.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pytincture',
-    version='0.4.2',
+    version='0.4.3',
     description=(
         'UI Builder'
     ),
     url="https://github.com/pytincture/pytincture",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages = find_packages(),
```

