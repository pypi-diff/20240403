# Comparing `tmp/schedula-1.5.5.tar.gz` & `tmp/schedula-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schedula-1.5.5.tar", last modified: Tue Mar 19 12:03:14 2024, max compression
+gzip compressed data, was "schedula-1.5.6.tar", last modified: Wed Apr  3 14:54:33 2024, max compression
```

## Comparing `schedula-1.5.5.tar` & `schedula-1.5.6.tar`

### file list

```diff
@@ -1,283 +1,288 @@
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.071883 schedula-1.5.5/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       67 2020-04-22 23:09:02.000000 schedula-1.5.5/AUTHORS.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13141 2020-04-22 23:09:02.000000 schedula-1.5.5/LICENSE.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14353 2024-03-19 12:03:14.071721 schedula-1.5.5/PKG-INFO
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    21979 2024-03-19 11:33:18.000000 schedula-1.5.5/README.rst
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:13.989919 schedula-1.5.5/schedula/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4300 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      777 2024-03-19 11:33:18.000000 schedula-1.5.5/schedula/_version.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    68652 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/dispatcher.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:13.991929 schedula-1.5.5/schedula/ext/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      450 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/ext/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10745 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/ext/autosummary.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:13.992819 schedula-1.5.5/schedula/ext/dispatcher/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      715 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/ext/dispatcher/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12020 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/ext/dispatcher/documenter.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3162 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/ext/dispatcher/graphviz.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:13.996600 schedula-1.5.5/schedula/utils/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1446 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/__init__.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    13251 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/alg.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:13.997295 schedula-1.5.5/schedula/utils/asy/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11064 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/asy/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8126 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/asy/executors.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3284 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/asy/factory.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    17292 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/base.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    24001 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/blue.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2009 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/cst.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:13.997438 schedula-1.5.5/schedula/utils/des/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     6766 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/des/__init__.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:13.998252 schedula-1.5.5/schedula/utils/drw/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    64721 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/drw/__init__.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:13.986983 schedula-1.5.5/schedula/utils/drw/index/
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:13.999688 schedula-1.5.5/schedula/utils/drw/index/css/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   155758 2020-04-22 23:09:02.000000 schedula-1.5.5/schedula/utils/drw/index/css/bootstrap.min.css
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   625953 2020-04-22 23:09:02.000000 schedula-1.5.5/schedula/utils/drw/index/css/bootstrap.min.css.map
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    18280 2023-11-19 15:42:01.000000 schedula-1.5.5/schedula/utils/drw/index/css/icon.css
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3340 2020-04-22 23:09:02.000000 schedula-1.5.5/schedula/utils/drw/index/css/index.css
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.001088 schedula-1.5.5/schedula/utils/drw/index/js/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    15950 2020-04-22 23:09:02.000000 schedula-1.5.5/schedula/utils/drw/index/js/bootstrap-treeview.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    58072 2020-04-22 23:09:02.000000 schedula-1.5.5/schedula/utils/drw/index/js/bootstrap.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   190253 2020-04-22 23:09:02.000000 schedula-1.5.5/schedula/utils/drw/index/js/bootstrap.min.js.map
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16226 2020-04-22 23:09:02.000000 schedula-1.5.5/schedula/utils/drw/index/js/d3-scale.v3.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88144 2020-04-22 23:09:02.000000 schedula-1.5.5/schedula/utils/drw/index/js/jquery-3.4.1.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6341 2020-04-22 23:09:02.000000 schedula-1.5.5/schedula/utils/drw/index/js/jquery.fullscreen.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    67320 2020-04-22 23:09:02.000000 schedula-1.5.5/schedula/utils/drw/index/js/sunburst-chart.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1839 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/drw/nodes.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.001409 schedula-1.5.5/schedula/utils/drw/templates/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    18102 2023-11-19 15:42:01.000000 schedula-1.5.5/schedula/utils/drw/templates/index.html
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11626 2023-11-19 15:42:01.000000 schedula-1.5.5/schedula/utils/drw/templates/render.html
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.001568 schedula-1.5.5/schedula/utils/drw/viz/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)  2396719 2023-11-19 09:38:55.000000 schedula-1.5.5/schedula/utils/drw/viz/viz.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    56461 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/dsp.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1392 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/exc.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.008597 schedula-1.5.5/schedula/utils/form/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11801 2024-03-18 19:03:02.000000 schedula-1.5.5/schedula/utils/form/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5433 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/form/config.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1928 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/form/mail.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12868 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/form/server.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:13.987311 schedula-1.5.5/schedula/utils/form/static/
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:13.987588 schedula-1.5.5/schedula/utils/form/static/schedula/
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.013752 schedula-1.5.5/schedula/utils/form/static/schedula/css/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      234 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/1357.496fcbc7.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2151 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      280 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/1724.5fbb5eb3.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2164 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      137 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/2706.83c2b1be.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      147 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/3667.3d691932.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      139 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/414.4a9f9388.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      172 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/4337.95ac7f8b.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      346 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/4459.a24c0b46.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      135 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/5255.de163d1c.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      314 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/5836.0a2c9e70.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      135 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/6753.de163d1c.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      499 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/7101.8501d8d8.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      494 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/8428.03ea8396.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      685 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/9003.d2d6266b.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      249 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/9106.8d761a00.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      147 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/9665.80050c43.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      426 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/9835.6b615d8b.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      272 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/css/main.539ebc22.css.gz
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.014167 schedula-1.5.5/schedula/utils/form/static/schedula/forms/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1326 2023-11-19 15:42:01.000000 schedula-1.5.5/schedula/utils/form/static/schedula/forms/index-schema.json
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3421 2023-11-15 13:00:39.000000 schedula-1.5.5/schedula/utils/form/static/schedula/forms/index-ui.json
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.055823 schedula-1.5.5/schedula/utils/form/static/schedula/js/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7191 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1064.85be30e8.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      546 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1165.ff804d16.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1226 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1177.950ebcc8.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      364 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/132.a4de6573.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4268 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1320.8d42e1b4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2339 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1357.d39a01da.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      832 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1362.0594020f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5084 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1431.780747e9.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13937 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1432.f3b34f42.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      578 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1465.edd9ba38.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      269 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1476.d0e9ba73.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      298 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1511.d20fbe21.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3958 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1583.fbdd1527.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      291 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/159.42f57d98.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      601 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1641.cc9646e9.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      779 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1642.5186d671.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16150 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4504 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3777 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1724.8474ed1b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1443 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1748.33ff7ac6.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3521 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/183.76a6294f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      311 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1831.7a4c7750.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7431 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/1973.bcd66253.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      649 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      415 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2085.3afcba83.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12859 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2120.8ea1a31a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1281 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    36347 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3772 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2256.c3de48fa.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4864 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2286.a0b82906.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   432061 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      324 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2452.288238f6.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6016 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6928 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      388 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2604.46d4f061.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      281 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2638.b7999325.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4571 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/268.deedefec.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2749 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      744 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3769 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2723.e492696d.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4170 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2742.edfc3acf.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   468024 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2768.93ab5524.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      718 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8687 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    20917 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10229 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3070.25639b4f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      498 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3099.e186daed.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7065 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/31.3bee8367.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3101.c13d903f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4704 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3281.a4f1ba69.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1622 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3327.f5840c2f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      655 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3333.3da6381e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      465 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3368.b732d88e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      279 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3509.62544ca4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      268 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3565.b1e72cb6.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1781 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3642.27ee29bf.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      272 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3667.19631032.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3636 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3676.1ee61f29.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11274 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/368.9a0bfb9a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1405 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3850.689e0ff9.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      496 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/3963.54debd2a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10537 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4048.6f416a19.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11847 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4093.fa03dad5.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4818 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4095.87cc9b62.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5841 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/414.56817ff7.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      282 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4164.9cdf0caa.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6643 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4279.d5144a2b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      953 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4337.b839f823.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4390.3c3f840c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5056 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4438.acbb2994.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1785 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4459.7c486c55.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      463 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4569.9990e2a1.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5746 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4587.5ff7f02e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3347 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4596.53d31027.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1499 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4672.f1f003ed.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1777 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4786.f0dbe7a4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      297 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4842.17363063.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1422 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4906.d6a6dad2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4218 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/4925.6cb145d6.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5029.09813ba3.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      283 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5051.955a4b55.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3733 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5097.04da753b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4011 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5255.baba9ad1.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28348 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5349.d6abdf80.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2750 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5415.96511657.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2155 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5459.ab6195a8.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5522.772b12da.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1727 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5652.0a2d25f3.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3731 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5672.d78485cb.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2752 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5784.aa6dfd10.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      278 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5827.1e26cd85.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1962 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5836.722242c0.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      702 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5880.208b3048.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      284 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5954.df1a43db.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     9308 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5959.d5ebe3fe.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28956 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/5973.9de918f7.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4893 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/6043.6bea23a4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11589 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/608.60f30d1f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14429 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/6085.d41a2240.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      306 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/6302.996dbe65.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4647 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/6474.6af0dc33.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      608 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/654.98d33eb8.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7291 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/6753.2b6e62d5.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      426 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/6801.62068c84.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1430 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/6855.c4d51fc1.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      334 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/6907.0fe74465.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1421 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/6925.228697fa.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4333 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/6938.c8986bc2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2161 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2949 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4366 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6023 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16317 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/7381.62ff7f32.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8089 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/7435.8ac4b848.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      275 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/744.c1913bc4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    27276 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3735 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/7565.867674bc.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16144 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/7605.9c355065.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2984 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5252 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    37416 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/796.a463ad0d.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   266663 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/7974.f57f09fe.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4005 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1367 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8861 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/8148.e27d34a2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1015 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/8191.a6547494.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3730 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/8259.439eef4a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/8384.733495df.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3298 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/8428.6d9c78b7.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      336 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/853.c4b3a572.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11595 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/8531.1c721013.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12186 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/8583.baa4f5a0.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7429 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/8698.5bb1b696.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8133 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3512 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      269 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/8797.9e3c01c2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      273 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/8916.4a5d5d2c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      425 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9003.b108ee29.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4065 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9009.78b5479a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9079.476a64c2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2482 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9106.262dfeb4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3721 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9196.312a3d80.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6097 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9235.b2714593.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2955 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9238.8ae8b0d0.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4148 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9367.127331a0.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2613 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6409 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      264 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9559.52882117.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13323 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9628.5b2d7fe9.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      602 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9665.894f2277.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3122 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9835.0870cf0f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    25595 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      486 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/9925.cc714497.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   432295 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/js/main.85117e28.js.gz
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.063924 schedula-1.5.5/schedula/utils/form/static/schedula/media/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    89335 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    97121 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88989 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    95155 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    94641 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88308 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    95760 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-LightItalic.c590382422f2742d788b.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    89222 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-Medium.7c8d04cd831df3033c8a.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    96312 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-MediumItalic.82736aaa11c64709055f.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88471 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-Regular.fc2b5060f7accec5cf74.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    86875 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-Thin.a732a12eb07742232407.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    93771 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      229 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/media/getFetch.40f37ddea2378391108f.cjs.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      515 2024-03-19 11:30:05.000000 schedula-1.5.5/schedula/utils/form/static/schedula/media/index.42119833dddefe38a9fa.cjs.gz
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:13.987707 schedula-1.5.5/schedula/utils/form/templates/
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.064434 schedula-1.5.5/schedula/utils/form/templates/schedula/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4460 2024-03-14 10:09:53.000000 schedula-1.5.5/schedula/utils/form/templates/schedula/base.html
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.065149 schedula-1.5.5/schedula/utils/form/templates/schedula/email/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      238 2023-11-15 13:00:39.000000 schedula-1.5.5/schedula/utils/form/templates/schedula/email/contact-body-en.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      250 2023-11-15 13:00:39.000000 schedula-1.5.5/schedula/utils/form/templates/schedula/email/contact-body-it.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       57 2023-11-15 13:00:39.000000 schedula-1.5.5/schedula/utils/form/templates/schedula/email/contact-subject.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       34 2022-10-19 15:46:09.000000 schedula-1.5.5/schedula/utils/form/templates/schedula/index.html
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2194 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/gen.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4332 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/graph.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      692 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/imp.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.065316 schedula-1.5.5/schedula/utils/io/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     6380 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/io/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    40509 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/sol.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1630 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/utl.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.065621 schedula-1.5.5/schedula/utils/web/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7053 2024-03-14 10:25:40.000000 schedula-1.5.5/schedula/utils/web/__init__.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.068041 schedula-1.5.5/schedula.egg-info/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14353 2024-03-19 12:03:13.000000 schedula-1.5.5/schedula.egg-info/PKG-INFO
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14664 2024-03-19 12:03:13.000000 schedula-1.5.5/schedula.egg-info/SOURCES.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        1 2024-03-19 12:03:13.000000 schedula-1.5.5/schedula.egg-info/dependency_links.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      990 2024-03-19 12:03:13.000000 schedula-1.5.5/schedula.egg-info/requires.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        9 2024-03-19 12:03:13.000000 schedula-1.5.5/schedula.egg-info/top_level.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      162 2024-03-19 12:03:14.072200 schedula-1.5.5/setup.cfg
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7084 2024-03-14 10:25:40.000000 schedula-1.5.5/setup.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-03-19 12:03:14.067802 schedula-1.5.5/tests/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    89504 2024-03-14 10:25:40.000000 schedula-1.5.5/tests/test_dispatcher.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1020 2024-03-14 10:25:40.000000 schedula-1.5.5/tests/test_import.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1164 2024-03-14 10:25:40.000000 schedula-1.5.5/tests/test_micropython.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)      872 2024-03-14 10:25:40.000000 schedula-1.5.5/tests/test_readme.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1028 2024-03-14 10:25:40.000000 schedula-1.5.5/tests/test_setup.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.521578 schedula-1.5.6/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       67 2020-04-22 23:09:02.000000 schedula-1.5.6/AUTHORS.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13141 2020-04-22 23:09:02.000000 schedula-1.5.6/LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14353 2024-04-03 14:54:33.521445 schedula-1.5.6/PKG-INFO
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    21979 2024-04-03 14:51:38.000000 schedula-1.5.6/README.rst
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.423327 schedula-1.5.6/schedula/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4300 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      777 2024-04-03 14:51:38.000000 schedula-1.5.6/schedula/_version.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    68892 2024-04-03 12:07:12.000000 schedula-1.5.6/schedula/dispatcher.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.425384 schedula-1.5.6/schedula/ext/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      450 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/ext/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10745 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/ext/autosummary.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.426362 schedula-1.5.6/schedula/ext/dispatcher/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      715 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/ext/dispatcher/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12020 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/ext/dispatcher/documenter.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3162 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/ext/dispatcher/graphviz.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.431119 schedula-1.5.6/schedula/utils/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1446 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/__init__.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    13251 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/alg.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.432188 schedula-1.5.6/schedula/utils/asy/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11064 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/asy/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8126 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/asy/executors.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3284 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/asy/factory.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    17367 2024-03-30 08:05:12.000000 schedula-1.5.6/schedula/utils/base.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    24001 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/blue.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2009 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/cst.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.432508 schedula-1.5.6/schedula/utils/des/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     6766 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/des/__init__.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.433756 schedula-1.5.6/schedula/utils/drw/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    64721 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/drw/__init__.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.420059 schedula-1.5.6/schedula/utils/drw/index/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.435173 schedula-1.5.6/schedula/utils/drw/index/css/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   155758 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/css/bootstrap.min.css
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   625953 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/css/bootstrap.min.css.map
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    18280 2023-11-19 15:42:01.000000 schedula-1.5.6/schedula/utils/drw/index/css/icon.css
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3340 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/css/index.css
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.436843 schedula-1.5.6/schedula/utils/drw/index/js/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    15950 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/js/bootstrap-treeview.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    58072 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/js/bootstrap.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   190253 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/js/bootstrap.min.js.map
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16226 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/js/d3-scale.v3.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88144 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/js/jquery-3.4.1.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6341 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/js/jquery.fullscreen.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    67320 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/js/sunburst-chart.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1839 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/drw/nodes.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.437245 schedula-1.5.6/schedula/utils/drw/templates/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    18102 2023-11-19 15:42:01.000000 schedula-1.5.6/schedula/utils/drw/templates/index.html
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11626 2023-11-19 15:42:01.000000 schedula-1.5.6/schedula/utils/drw/templates/render.html
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.437456 schedula-1.5.6/schedula/utils/drw/viz/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)  2396719 2023-11-19 09:38:55.000000 schedula-1.5.6/schedula/utils/drw/viz/viz.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    56461 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/dsp.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1392 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/exc.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.442708 schedula-1.5.6/schedula/utils/form/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12042 2024-03-22 15:04:12.000000 schedula-1.5.6/schedula/utils/form/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5433 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/form/config.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1171 2024-03-22 15:04:12.000000 schedula-1.5.6/schedula/utils/form/json_secrets.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1928 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/form/mail.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13359 2024-03-22 16:24:55.000000 schedula-1.5.6/schedula/utils/form/server.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.420478 schedula-1.5.6/schedula/utils/form/static/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.420814 schedula-1.5.6/schedula/utils/form/static/schedula/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.448004 schedula-1.5.6/schedula/utils/form/static/schedula/css/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2151 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      280 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/1724.5fbb5eb3.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      837 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/1737.87abdd03.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2164 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      137 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/2706.83c2b1be.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      147 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/3667.3d691932.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      139 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/414.4a9f9388.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      185 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/4337.588bea5b.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      234 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/4452.70b7e4bb.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      346 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/4459.a24c0b46.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      135 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/5255.de163d1c.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      314 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/5836.0a2c9e70.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      135 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/6753.de163d1c.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      251 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/6836.4de17ac7.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      499 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/7101.8501d8d8.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      425 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/7450.1773328b.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      494 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/8428.03ea8396.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      685 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/9003.d2d6266b.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      147 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/9665.80050c43.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      272 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/main.539ebc22.css.gz
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.448466 schedula-1.5.6/schedula/utils/form/static/schedula/forms/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1326 2023-11-19 15:42:01.000000 schedula-1.5.6/schedula/utils/form/static/schedula/forms/index-schema.json
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3421 2023-11-15 13:00:39.000000 schedula-1.5.6/schedula/utils/form/static/schedula/forms/index-ui.json
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.506291 schedula-1.5.6/schedula/utils/form/static/schedula/js/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      546 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1165.ff804d16.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1226 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1177.950ebcc8.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      364 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/132.a4de6573.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4268 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1320.8d42e1b4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      832 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1362.0594020f.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5084 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1431.780747e9.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13937 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1432.f3b34f42.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      578 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1465.edd9ba38.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      269 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1476.d0e9ba73.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      298 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1511.d20fbe21.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3958 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1583.fbdd1527.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      291 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/159.42f57d98.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      601 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1641.cc9646e9.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      779 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1642.5186d671.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16150 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4504 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3768 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1724.d97efc34.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      936 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1737.13089dbe.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1444 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1748.0df73428.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3521 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/183.76a6294f.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      311 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1831.7a4c7750.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7431 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1973.bcd66253.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      649 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      415 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2085.3afcba83.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12859 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2120.8ea1a31a.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1281 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    36347 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3772 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2256.c3de48fa.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4864 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2286.850702e1.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   432061 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      324 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2452.288238f6.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6016 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6928 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      388 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2604.46d4f061.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      281 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2638.b7999325.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4571 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/268.deedefec.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2749 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      744 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3769 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2723.e492696d.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4365 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2742.cef81b1c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   468024 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2768.93ab5524.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      718 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8687 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    20917 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10229 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3070.25639b4f.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      498 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3099.e186daed.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3101.c13d903f.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4704 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3281.a4f1ba69.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1622 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3327.f5840c2f.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      655 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3333.3da6381e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      465 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3368.b732d88e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    19245 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3457.a6f7a355.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      279 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3509.62544ca4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      268 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3565.b1e72cb6.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1781 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3642.27ee29bf.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      272 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3667.19631032.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3636 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3676.1ee61f29.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11274 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/368.9a0bfb9a.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1405 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3850.689e0ff9.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      496 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3963.54debd2a.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10537 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4048.6f416a19.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11849 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4093.1b358dc3.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4818 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4095.87cc9b62.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7251 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4129.3e3e6e91.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5841 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/414.56817ff7.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      282 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4164.9cdf0caa.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6643 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4279.d5144a2b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      976 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4337.8da858ce.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4390.3c3f840c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5056 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4438.acbb2994.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3472 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4452.45bca48d.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1781 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4459.6704ca6e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      463 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4569.9990e2a1.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5746 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4587.5ff7f02e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3347 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4596.53d31027.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1499 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4672.f1f003ed.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7078 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4673.aa83f5e0.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1777 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4786.f0dbe7a4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      297 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4842.17363063.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1422 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4906.d6a6dad2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4218 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4925.6cb145d6.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16182 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5025.2850b7b4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5029.09813ba3.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      283 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5051.955a4b55.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3733 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5097.04da753b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4011 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5255.baba9ad1.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28348 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5349.d6abdf80.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2750 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5415.96511657.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2155 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5459.ab6195a8.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5522.772b12da.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1668 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5652.dde5ef02.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3731 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5672.d78485cb.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2752 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5784.aa6dfd10.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      278 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5827.1e26cd85.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1962 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5836.722242c0.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      734 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5880.5ad7e40e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      284 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5954.df1a43db.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     9308 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5959.d5ebe3fe.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4893 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6043.6bea23a4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11589 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/608.60f30d1f.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14429 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6085.d41a2240.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      306 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6302.996dbe65.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4647 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6474.6af0dc33.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      608 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/654.98d33eb8.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7293 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6753.e37ed964.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      426 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6801.62068c84.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3702 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6836.43947ef9.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1430 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6855.c4d51fc1.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      334 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6907.0fe74465.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1421 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6925.228697fa.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4333 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6938.c8986bc2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2161 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2949 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4366 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6023 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   261511 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7193.528d18c4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8089 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7435.8ac4b848.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      275 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/744.c1913bc4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3130 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7450.d618087b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    27276 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3735 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7565.867674bc.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2984 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5252 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    37416 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/796.a7fc5105.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   266679 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7974.7e7de702.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4005 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      669 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8115.11a85e47.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1367 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8861 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8148.e27d34a2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1015 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8191.a6547494.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3730 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8259.439eef4a.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8384.733495df.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3291 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8428.7d81c7b5.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28905 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8497.f11bc0ea.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13322 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8516.30c79314.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      336 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/853.c4b3a572.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11595 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8531.1c721013.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12186 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8583.baa4f5a0.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7429 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8698.5bb1b696.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8133 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3512 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      269 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8797.9e3c01c2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      273 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8916.4a5d5d2c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      425 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9003.b108ee29.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4065 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9009.78b5479a.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9079.476a64c2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3721 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9196.312a3d80.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6097 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9235.b2714593.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2955 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9238.8ae8b0d0.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4148 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9367.127331a0.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2613 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6409 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      264 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9559.52882117.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      604 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9665.8425fb6b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    25595 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      486 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9925.cc714497.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   432329 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/main.d401041d.js.gz
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.512147 schedula-1.5.6/schedula/utils/form/static/schedula/media/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    89335 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    97121 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88989 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    95155 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    94641 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88308 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    95760 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-LightItalic.c590382422f2742d788b.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    89222 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Medium.7c8d04cd831df3033c8a.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    96312 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-MediumItalic.82736aaa11c64709055f.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88471 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Regular.fc2b5060f7accec5cf74.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    86875 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Thin.a732a12eb07742232407.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    93771 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      229 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/getFetch.40f37ddea2378391108f.cjs.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      515 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/index.42119833dddefe38a9fa.cjs.gz
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.420971 schedula-1.5.6/schedula/utils/form/templates/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.512622 schedula-1.5.6/schedula/utils/form/templates/schedula/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4460 2024-03-14 10:09:53.000000 schedula-1.5.6/schedula/utils/form/templates/schedula/base.html
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.513526 schedula-1.5.6/schedula/utils/form/templates/schedula/email/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      238 2023-11-15 13:00:39.000000 schedula-1.5.6/schedula/utils/form/templates/schedula/email/contact-body-en.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      250 2023-11-15 13:00:39.000000 schedula-1.5.6/schedula/utils/form/templates/schedula/email/contact-body-it.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       57 2023-11-15 13:00:39.000000 schedula-1.5.6/schedula/utils/form/templates/schedula/email/contact-subject.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       34 2022-10-19 15:46:09.000000 schedula-1.5.6/schedula/utils/form/templates/schedula/index.html
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2194 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/gen.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4332 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/graph.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      692 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/imp.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.513721 schedula-1.5.6/schedula/utils/io/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     6380 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/io/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    40509 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/sol.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1630 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/utl.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.514036 schedula-1.5.6/schedula/utils/web/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7053 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/web/__init__.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.517130 schedula-1.5.6/schedula.egg-info/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14353 2024-04-03 14:54:33.000000 schedula-1.5.6/schedula.egg-info/PKG-INFO
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14964 2024-04-03 14:54:33.000000 schedula-1.5.6/schedula.egg-info/SOURCES.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        1 2024-04-03 14:54:33.000000 schedula-1.5.6/schedula.egg-info/dependency_links.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      990 2024-04-03 14:54:33.000000 schedula-1.5.6/schedula.egg-info/requires.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        9 2024-04-03 14:54:33.000000 schedula-1.5.6/schedula.egg-info/top_level.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      162 2024-04-03 14:54:33.521906 schedula-1.5.6/setup.cfg
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7084 2024-03-14 10:25:40.000000 schedula-1.5.6/setup.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.516773 schedula-1.5.6/tests/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    89504 2024-03-14 10:25:40.000000 schedula-1.5.6/tests/test_dispatcher.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1020 2024-03-14 10:25:40.000000 schedula-1.5.6/tests/test_import.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1164 2024-03-14 10:25:40.000000 schedula-1.5.6/tests/test_micropython.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)      872 2024-03-14 10:25:40.000000 schedula-1.5.6/tests/test_readme.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1028 2024-03-14 10:25:40.000000 schedula-1.5.6/tests/test_setup.py
```

### Comparing `schedula-1.5.5/LICENSE.txt` & `schedula-1.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/PKG-INFO` & `schedula-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: schedula
-Version: 1.5.5
+Version: 1.5.6
 Summary: Produce a plan that dispatches calls based on a graph of functions, satisfying data dependencies.
 Home-page: https://github.com/vinci1it2000/schedula
-Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.5
+Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.6
 Author: Vincenzo Arcidiacono
 Author-email: vinci1it2000@gmail.com
 License: EUPL 1.1+
 Project-URL: Documentation, https://schedula.readthedocs.io
 Project-URL: Issue tracker, https://github.com/vinci1it2000/schedula/issues
 Keywords: flow-based programming,dataflow,parallel,asynchronous,async,scheduling,dispatch,functional programming,dataflow programming
 Classifier: Programming Language :: Python
```

### Comparing `schedula-1.5.5/README.rst` & `schedula-1.5.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 #######################################################################
 schedula: A smart function scheduler for dynamic flow-based programming
 #######################################################################
 |pypi_ver| |test_status| |cover_status| |docs_status| |downloads|
 |month_downloads| |github_issues| |python_ver| |proj_license| |binder|
 
-:release:       1.5.5
-:date:          2024-03-19 12:30:00
+:release:       1.5.6
+:date:          2024-04-03 15:00:00
 :repository:    https://github.com/vinci1it2000/schedula
 :pypi-repo:     https://pypi.org/project/schedula/
 :docs:          https://schedula.readthedocs.io/
 :wiki:          https://github.com/vinci1it2000/schedula/wiki/
 :download:      https://github.com/vinci1it2000/schedula/releases/
 :keywords:      flow-based programming, dataflow, parallel, async, scheduling,
                 dispatch, functional programming, dataflow programming
```

### Comparing `schedula-1.5.5/schedula/__init__.py` & `schedula-1.5.6/schedula/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/_version.py` & `schedula-1.5.6/schedula/_version.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 # You may not use this work except in compliance with the Licence.
 # You may obtain a copy of the Licence at: http://ec.europa.eu/idabc/eupl
 
 __all__ = ['__version__', '__updated__', '__title__', '__author__',
            '__license__', '__copyright__']
 
 #: Authoritative project's PEP 440 version.
-__version__ = version = "1.5.5"  # Also update README.rst
+__version__ = version = "1.5.6"  # Also update README.rst
 
 # Please UPDATE TIMESTAMP WHEN BUMPING VERSIONS AND BEFORE RELEASE.
 #: Release date.
-__updated__ = "2024-03-19 12:30:00"
+__updated__ = "2024-04-03 15:00:00"
 
 __title__ = 'schedula'
 
 __author__ = 'Vincenzo Arcidiacono <vinci1it2000@gmail.com>'
 
 __license__ = 'EUPL, see LICENSE.txt'
```

### Comparing `schedula-1.5.5/schedula/dispatcher.py` & `schedula-1.5.6/schedula/dispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1190,15 +1190,15 @@
         sub_dsp.default_values = {k: dmap_dv[k] for k in dmap_dv if k in nodes}
 
         return sub_dsp  # Return the sub-dispatcher.
 
     def get_sub_dsp_from_workflow(
             self, sources, graph=None, reverse=False, add_missing=False,
             check_inputs=True, blockers=None, wildcard=False,
-            _update_links=True):
+            _update_links=True, avoid_cycles=False):
         """
         Returns the sub-dispatcher induced by the workflow from sources.
 
         The induced sub-dispatcher of the dsp contains the reachable nodes and
         edges evaluated with breadth-first-search on the workflow graph from
         source nodes.
 
@@ -1357,14 +1357,18 @@
             def _check_node_inputs(c, p):
                 if c == START:
                     try:
                         node_attr = dmap_nodes[p]
                         return node_attr['type'] == 'data'
                     except KeyError:
                         return True
+                if avoid_cycles:
+                    node_attr = dmap_nodes[c]
+                    if node_attr['type'] == 'function':
+                        return any(k in family for k in node_attr['inputs'])
                 return False
 
         from collections import deque
         queue = deque([])
 
         blockers = set(blockers or ())
 
@@ -1382,15 +1386,15 @@
             if add2family:
                 # Append a new parent to the family.
                 family[n] = () if block and n in blockers else neighbors[n]
 
                 queue.append(n)
 
         # Set initial node attributes.
-        for s in sources:
+        for s in sorted(sources):
             if s in dmap_nodes and s in graph.nodes:
                 _set_node_attr(s, block=not (wildcard and s in blockers))
 
         # Start breadth-first-search.
         while queue:
             parent = queue.popleft()
```

### Comparing `schedula-1.5.5/schedula/ext/autosummary.py` & `schedula-1.5.6/schedula/ext/autosummary.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/ext/dispatcher/__init__.py` & `schedula-1.5.6/schedula/ext/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/ext/dispatcher/documenter.py` & `schedula-1.5.6/schedula/ext/dispatcher/documenter.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/ext/dispatcher/graphviz.py` & `schedula-1.5.6/schedula/ext/dispatcher/graphviz.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/__init__.py` & `schedula-1.5.6/schedula/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/alg.py` & `schedula-1.5.6/schedula/utils/alg.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/asy/__init__.py` & `schedula-1.5.6/schedula/utils/asy/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/asy/executors.py` & `schedula-1.5.6/schedula/utils/asy/executors.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/asy/factory.py` & `schedula-1.5.6/schedula/utils/asy/factory.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/base.py` & `schedula-1.5.6/schedula/utils/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,17 +113,17 @@
             sites.add(webmap.site(view=run))
         elif run:
             return webmap.site(view=run)
         return webmap
 
     def form(self, depth=1, node_data=NONE, node_function=NONE, directory=None,
              sites=None, run=True, view=True, get_context=NONE, get_data=NONE,
-             edit_on_change='./static/schedula/onChange/*.js',
-             pre_submit='./static/schedula/preSubmit/*.js',
-             post_submit='./static/schedula/postSubmit/*.js',
+             edit_on_change='static/schedula/onChange/*.js',
+             pre_submit='static/schedula/preSubmit/*.js',
+             post_submit='static/schedula/postSubmit/*.js',
              subsite_idle_timeout=600, basic_app_config=None,
              stripe_event_handler=lambda event: None):
         """
         Creates a dispatcher Form Flask app.
 
         :param depth:
             Depth of sub-dispatch API. If negative all levels are configured.
@@ -208,14 +208,15 @@
             'get_edit_on_change_func': edit_on_change,
             'get_pre_submit_func': pre_submit,
             'get_post_submit_func': post_submit
         }
         for k, v in methods.items():
             if isinstance(v, str):
                 methods[k] = d = {}
+                v = osp.join(directory or '.', *v.replace('\\', '/').split('/'))
                 for fpath in glob.glob(v):
                     with open(fpath) as f:
                         d[f'/{osp.splitext(osp.basename(fpath))[0]}'] = f.read()
                 if '/' not in d and '/index' in d:
                     d['/'] = d['/index']
                 elif not d:
                     methods[k] = NONE
```

### Comparing `schedula-1.5.5/schedula/utils/blue.py` & `schedula-1.5.6/schedula/utils/blue.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/cst.py` & `schedula-1.5.6/schedula/utils/cst.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/des/__init__.py` & `schedula-1.5.6/schedula/utils/des/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/__init__.py` & `schedula-1.5.6/schedula/utils/drw/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/index/css/bootstrap.min.css` & `schedula-1.5.6/schedula/utils/drw/index/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/index/css/bootstrap.min.css.map` & `schedula-1.5.6/schedula/utils/drw/index/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/index/css/icon.css` & `schedula-1.5.6/schedula/utils/drw/index/css/icon.css`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/index/css/index.css` & `schedula-1.5.6/schedula/utils/drw/index/css/index.css`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/index/js/bootstrap-treeview.min.js` & `schedula-1.5.6/schedula/utils/drw/index/js/bootstrap-treeview.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/index/js/bootstrap.min.js` & `schedula-1.5.6/schedula/utils/drw/index/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/index/js/bootstrap.min.js.map` & `schedula-1.5.6/schedula/utils/drw/index/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/index/js/d3-scale.v3.min.js` & `schedula-1.5.6/schedula/utils/drw/index/js/d3-scale.v3.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/index/js/jquery-3.4.1.min.js` & `schedula-1.5.6/schedula/utils/drw/index/js/jquery-3.4.1.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/index/js/jquery.fullscreen.min.js` & `schedula-1.5.6/schedula/utils/drw/index/js/jquery.fullscreen.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/index/js/sunburst-chart.min.js` & `schedula-1.5.6/schedula/utils/drw/index/js/sunburst-chart.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/nodes.py` & `schedula-1.5.6/schedula/utils/drw/nodes.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/templates/index.html` & `schedula-1.5.6/schedula/utils/drw/templates/index.html`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/templates/render.html` & `schedula-1.5.6/schedula/utils/drw/templates/render.html`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/drw/viz/viz.js` & `schedula-1.5.6/schedula/utils/drw/viz/viz.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/dsp.py` & `schedula-1.5.6/schedula/utils/dsp.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/exc.py` & `schedula-1.5.6/schedula/utils/exc.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/form/__init__.py` & `schedula-1.5.6/schedula/utils/form/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,23 @@
     server
 """
 import io
 import os
 import gzip
 import glob
 import hmac
+import json
 import secrets
 import hashlib
 import datetime
 import mimetypes
 import webbrowser
 import os.path as osp
 from ..web import WebMap
+from . import json_secrets
 from urllib.parse import urlparse
 from jinja2 import TemplateNotFound
 from werkzeug.exceptions import NotFound
 from itsdangerous import URLSafeTimedSerializer, BadData
 from .server import Config, basic_app, default_get_form_context
 from flask import (
     render_template, Blueprint, current_app, session, g, request, send_file,
@@ -273,14 +275,15 @@
             now = datetime.datetime.now(tz=datetime.timezone.utc)
             if not (0 <= (now - timestamp).total_seconds() <= time_limit):
                 g.csrf_refresh = True
         g.csrf_valid = True  # mark this request as CSRF valid
 
     @staticmethod
     def send_static_file(filename):
+        is_form = filename.startswith('forms')
         filename = f'schedula/{filename}'.split('/')
         download_name = filename[-1]
         kw = {
             'conditional': True,
             'download_name': download_name,
             'max_age': current_app.get_send_file_max_age(download_name)
         }
@@ -288,20 +291,24 @@
         for i, sdir in enumerate((current_app.static_folder, static_dir)):
             sdir = osp.join(sdir, *filename[:-1])
             for ext in ('.gz', '')[::gzipped and 1 or -1]:
                 fn = f'{download_name}{ext}'
                 fp = osp.join(sdir, fn)
                 if osp.exists(fp):
                     with open(fp, "rb") as f:
-                        if gzipped != bool(ext):
-                            func = gzipped and gzip.compress or gzip.decompress
-                            f = io.BytesIO(func(f.read()))
-                            fn = gzipped and f'{fn}.gz' or download_name
+                        if is_form:
+                            data = json_secrets.dumps(json.load(f)).encode()
                         else:
-                            f = io.BytesIO(f.read())
+                            data = f.read()
+                    if gzipped != bool(ext):
+                        func = gzipped and gzip.compress or gzip.decompress
+                        f = io.BytesIO(func(data))
+                        fn = gzipped and f'{fn}.gz' or download_name
+                    else:
+                        f = io.BytesIO(data)
                     kw['last_modified'] = os.stat(fp).st_mtime
                     mimetype, encoding = mimetypes.guess_type(fn)
 
                     response = send_file(f, **kw)
                     if i:
                         response.cache_control.immutable = True
                         response.cache_control.public = True
```

### Comparing `schedula-1.5.5/schedula/utils/form/config.py` & `schedula-1.5.6/schedula/utils/form/config.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/form/mail.py` & `schedula-1.5.6/schedula/utils/form/mail.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/form/server.py` & `schedula-1.5.6/schedula/utils/form/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 # You may not use this work except in compliance with the Licence.
 # You may obtain a copy of the Licence at: http://ec.europa.eu/idabc/eupl
 
 """
 It provides functions to build the base form flask app.
 """
 import logging
-import secrets
 import datetime
 import collections
 import os.path as osp
 import schedula as sh
 from .mail import Mail
+from . import json_secrets
 from .config import Config
 from flask_sqlalchemy import SQLAlchemy
 from flask_babel import Babel, lazy_gettext
 from werkzeug.datastructures import MultiDict
 from flask_wtf.recaptcha import RecaptchaField
 from flask_principal import Permission, RoleNeed
 from flask_security.models import fsqla_v3 as fsqla
@@ -266,43 +266,52 @@
     mail = Mail(app)
 
     @app.route('/stripe/create-checkout-session', methods=['POST'])
     def create_payment():
         import stripe
         try:
             data = request.get_json() if request.is_json else dict(request.form)
-            if not isinstance(data, list):
-                data = data,
-            lookup_keys = collections.OrderedDict()
+            data = json_secrets.secrets(data, False)
             api_key = current_app.config.get('STRIPE_SECRET_KEY')
-            for i, d in enumerate(data):
-                if 'lookup_key' in d:
-                    sh.get_nested_dicts(
-                        lookup_keys, d['lookup_key'], default=list
-                    ).append(i)
-            if lookup_keys:
-                for price, it in zip(stripe.Price.list(
-                        api_key=api_key,
-                        lookup_keys=list(lookup_keys.keys()),
-                        expand=['data.product']
-                ).data, lookup_keys.values()):
-                    for i in it:
-                        data[i].update({'price': price.id})
+            if 'line_items' in data:
+                line_items = data['line_items']
+                if not isinstance(line_items, list):
+                    line_items = line_items,
+                lookup_keys = collections.OrderedDict()
+
+                for i, d in enumerate(line_items):
+                    lookup_key = d.pop('lookup_key')
+                    if lookup_key:
+                        sh.get_nested_dicts(
+                            lookup_keys, lookup_key, default=list
+                        ).append(i)
+                if lookup_keys:
+                    for price, it in zip(stripe.Price.list(
+                            api_key=api_key,
+                            lookup_keys=list(lookup_keys.keys()),
+                            expand=['data.product']
+                    ).data, lookup_keys.values()):
+                        for i in it:
+                            line_items[i].update({'price': price.id})
+                data['line_items'] = line_items
+
             session = stripe.checkout.Session.create(
-                api_key=api_key,
-                ui_mode='embedded',
-                line_items=data,
-                mode='payment',
-                automatic_tax={'enabled': True},
-                redirect_on_completion='never',
-                metadata={
-                    f'customer_{k}': getattr(cu, k)
-                    for k in ('id', 'firstname', 'lastname')
-                    if hasattr(cu, k)
-                }
+                api_key=current_app.config.get('STRIPE_SECRET_KEY'),
+                **sh.combine_nested_dicts(json_secrets.secrets(
+                    data, False
+                ), base={
+                    'ui_mode': 'embedded',
+                    'automatic_tax': {'enabled': True},
+                    'redirect_on_completion': 'never',
+                    'metadata': {
+                        f'customer_{k}': getattr(cu, k)
+                        for k in ('id', 'firstname', 'lastname')
+                        if hasattr(cu, k)
+                    }
+                })
             )
         except Exception as e:
             return jsonify(error=str(e))
 
         return jsonify(
             clientSecret=session.client_secret, sessionId=session.id
         )
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz`

 * *Files 9% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1362.038687f8.chunk.css", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "1362.038687f8.chunk.css", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2286.6e5fc492.chunk.css", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "2286.6e5fc492.chunk.css", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/css/9003.d2d6266b.chunk.css.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/css/9003.d2d6266b.chunk.css.gz`

 * *Files 4% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9003.d2d6266b.chunk.css", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "9003.d2d6266b.chunk.css", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/forms/index-schema.json` & `schedula-1.5.6/schedula/utils/form/static/schedula/forms/index-schema.json`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/forms/index-ui.json` & `schedula-1.5.6/schedula/utils/form/static/schedula/forms/index-ui.json`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/1165.ff804d16.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/1165.ff804d16.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1165.ff804d16.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "1165.ff804d16.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/1177.950ebcc8.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/1177.950ebcc8.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1177.950ebcc8.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "1177.950ebcc8.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/1320.8d42e1b4.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/1320.8d42e1b4.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1320.8d42e1b4.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "1320.8d42e1b4.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/1362.0594020f.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/1362.0594020f.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1362.0594020f.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "1362.0594020f.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/1431.780747e9.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/1431.780747e9.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1431.780747e9.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "1431.780747e9.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/1432.f3b34f42.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/1432.f3b34f42.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1432.f3b34f42.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "1432.f3b34f42.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/1465.edd9ba38.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/1465.edd9ba38.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1465.edd9ba38.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "1465.edd9ba38.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/1583.fbdd1527.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/1583.fbdd1527.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1583.fbdd1527.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "1583.fbdd1527.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/1641.cc9646e9.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/1641.cc9646e9.chunk.js.gz`

 * *Files 4% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1641.cc9646e9.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "1641.cc9646e9.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/1642.5186d671.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/1642.5186d671.chunk.js.gz`

 * *Files 20% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1642.5186d671.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "1642.5186d671.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1656.c5fbd8dc.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "1656.c5fbd8dc.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1678.b278cefb.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "1678.b278cefb.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/183.76a6294f.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/183.76a6294f.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "183.76a6294f.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "183.76a6294f.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/1973.bcd66253.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/1973.bcd66253.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1973.bcd66253.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "1973.bcd66253.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2055.204f9b8c.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "2055.204f9b8c.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/2120.8ea1a31a.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/2120.8ea1a31a.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2120.8ea1a31a.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "2120.8ea1a31a.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz`

 * *Files 11% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2128.9a07d096.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "2128.9a07d096.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "218.37c2a3e8.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "218.37c2a3e8.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/2256.c3de48fa.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/2256.c3de48fa.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2256.c3de48fa.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "2256.c3de48fa.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "24.5f2a5395.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "24.5f2a5395.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2506.47c8c058.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "2506.47c8c058.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2556.ab2f7391.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "2556.ab2f7391.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/268.deedefec.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/268.deedefec.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "268.deedefec.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "268.deedefec.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2698.09529134.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "2698.09529134.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz`

 * *Files 19% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2706.a995f39e.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "2706.a995f39e.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/2723.e492696d.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/2723.e492696d.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2723.e492696d.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "2723.e492696d.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/2768.93ab5524.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/2768.93ab5524.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2768.93ab5524.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "2768.93ab5524.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz`

 * *Files 17% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "287.053696ba.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "287.053696ba.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2894.d8c25e8b.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "2894.d8c25e8b.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3052.40fbeb2c.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "3052.40fbeb2c.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/3070.25639b4f.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/3070.25639b4f.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3070.25639b4f.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "3070.25639b4f.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/3281.a4f1ba69.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/3281.a4f1ba69.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3281.a4f1ba69.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "3281.a4f1ba69.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/3327.f5840c2f.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/3327.f5840c2f.chunk.js.gz`

 * *Files 16% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3327.f5840c2f.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "3327.f5840c2f.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/3333.3da6381e.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/3333.3da6381e.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3333.3da6381e.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "3333.3da6381e.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/3642.27ee29bf.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/3642.27ee29bf.chunk.js.gz`

 * *Files 9% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3642.27ee29bf.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "3642.27ee29bf.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/3676.1ee61f29.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/3676.1ee61f29.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3676.1ee61f29.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "3676.1ee61f29.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/368.9a0bfb9a.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/368.9a0bfb9a.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "368.9a0bfb9a.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "368.9a0bfb9a.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/3850.689e0ff9.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/3850.689e0ff9.chunk.js.gz`

 * *Files 12% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3850.689e0ff9.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "3850.689e0ff9.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/4048.6f416a19.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/4048.6f416a19.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4048.6f416a19.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "4048.6f416a19.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/4095.87cc9b62.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/4095.87cc9b62.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4095.87cc9b62.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "4095.87cc9b62.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/414.56817ff7.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/414.56817ff7.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "414.56817ff7.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "414.56817ff7.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/4279.d5144a2b.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/4279.d5144a2b.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4279.d5144a2b.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "4279.d5144a2b.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/4438.acbb2994.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/4438.acbb2994.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4438.acbb2994.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "4438.acbb2994.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/4587.5ff7f02e.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/4587.5ff7f02e.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4587.5ff7f02e.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "4587.5ff7f02e.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/4596.53d31027.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/4596.53d31027.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4596.53d31027.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "4596.53d31027.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/4672.f1f003ed.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/4672.f1f003ed.chunk.js.gz`

 * *Files 10% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4672.f1f003ed.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "4672.f1f003ed.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/4786.f0dbe7a4.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/4786.f0dbe7a4.chunk.js.gz`

 * *Files 5% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4786.f0dbe7a4.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "4786.f0dbe7a4.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/4906.d6a6dad2.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/4906.d6a6dad2.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4906.d6a6dad2.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "4906.d6a6dad2.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/4925.6cb145d6.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/4925.6cb145d6.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4925.6cb145d6.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "4925.6cb145d6.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/5097.04da753b.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/5097.04da753b.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5097.04da753b.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "5097.04da753b.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/5255.baba9ad1.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/5255.baba9ad1.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5255.baba9ad1.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "5255.baba9ad1.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/5349.d6abdf80.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/5349.d6abdf80.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5349.d6abdf80.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "5349.d6abdf80.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/5415.96511657.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/5415.96511657.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5415.96511657.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "5415.96511657.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/5459.ab6195a8.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/5459.ab6195a8.chunk.js.gz`

 * *Files 8% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5459.ab6195a8.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "5459.ab6195a8.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/5672.d78485cb.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/5672.d78485cb.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5672.d78485cb.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "5672.d78485cb.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/5784.aa6dfd10.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/5784.aa6dfd10.chunk.js.gz`

 * *Files 4% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5784.aa6dfd10.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "5784.aa6dfd10.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/5836.722242c0.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/5836.722242c0.chunk.js.gz`

 * *Files 6% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5836.722242c0.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "5836.722242c0.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/5959.d5ebe3fe.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/5959.d5ebe3fe.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5959.d5ebe3fe.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "5959.d5ebe3fe.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/6043.6bea23a4.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/6043.6bea23a4.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "6043.6bea23a4.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "6043.6bea23a4.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/608.60f30d1f.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/608.60f30d1f.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "608.60f30d1f.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "608.60f30d1f.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/6085.d41a2240.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/6085.d41a2240.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "6085.d41a2240.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "6085.d41a2240.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/6474.6af0dc33.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/6474.6af0dc33.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "6474.6af0dc33.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "6474.6af0dc33.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/654.98d33eb8.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/654.98d33eb8.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "654.98d33eb8.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "654.98d33eb8.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/6753.2b6e62d5.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/6753.e37ed964.chunk.js.gz`

 * *Files 4% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "6753.2b6e62d5.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "6753.e37ed964.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

#### Comparing `6753.2b6e62d5.chunk.js` & `6753.e37ed964.chunk.js`

##### js-beautify {}

```diff
@@ -877,15 +877,15 @@
                 r = o(61431),
                 i = o(2556),
                 a = o(72506),
                 l = o(66106),
                 c = o(30914),
                 d = o(14692),
                 s = o(77128),
-                h = o(87605),
+                h = o(65025),
                 m = o(65560),
                 f = o(39475),
                 g = o(87462);
             const p = {
                 icon: {
                     tag: "svg",
                     attrs: {
@@ -1292,8 +1292,8 @@
                     }
                 }
             })
         },
         42480: () => {}
     }
 ]);
-//# sourceMappingURL=6753.2b6e62d5.chunk.js.map
+//# sourceMappingURL=6753.e37ed964.chunk.js.map
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/6855.c4d51fc1.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/6855.c4d51fc1.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "6855.c4d51fc1.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "6855.c4d51fc1.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/6925.228697fa.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/6925.228697fa.chunk.js.gz`

 * *Files 12% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "6925.228697fa.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "6925.228697fa.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/6938.c8986bc2.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/6938.c8986bc2.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "6938.c8986bc2.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "6938.c8986bc2.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz`

 * *Files 5% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "6984.ab1ec70c.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "6984.ab1ec70c.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "7035.5a8c5d98.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "7035.5a8c5d98.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "7101.48b6eb7a.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "7101.48b6eb7a.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz`

 * *Files 5% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "7106.0babb553.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "7106.0babb553.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/7435.8ac4b848.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/7435.8ac4b848.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "7435.8ac4b848.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "7435.8ac4b848.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "7522.bc15dd2d.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "7522.bc15dd2d.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/7565.867674bc.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/7565.867674bc.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "7565.867674bc.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "7565.867674bc.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "78.d0c28d0b.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "78.d0c28d0b.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "7828.8fdd74db.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "7828.8fdd74db.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/796.a463ad0d.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/796.a7fc5105.chunk.js.gz`

 * *Files 22% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "796.a463ad0d.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "796.a7fc5105.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

#### Comparing `796.a463ad0d.chunk.js` & `796.a7fc5105.chunk.js`

##### js-beautify {}

```diff
@@ -3718,15 +3718,15 @@
                 };
             const mn = o.forwardRef(pn);
             var gn = n(19581);
             var hn = n(2556),
                 bn = n(34664),
                 vn = n(83388),
                 xn = n(31678),
-                yn = n(87605),
+                yn = n(65025),
                 Cn = n(11730),
                 wn = n(49389);
             const Sn = function(e) {
                 let {
                     value: t,
                     onChange: n,
                     filterSearch: r,
@@ -6129,8 +6129,8 @@
                     left: t.left + (window.pageXOffset || n.scrollLeft) - (n.clientLeft || document.body.clientLeft || 0),
                     top: t.top + (window.pageYOffset || n.scrollTop) - (n.clientTop || document.body.clientTop || 0)
                 }
             }
         }
     }
 ]);
-//# sourceMappingURL=796.a463ad0d.chunk.js.map
+//# sourceMappingURL=796.a7fc5105.chunk.js.map
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "8007.cbee9608.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "8007.cbee9608.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "8119.038d4e91.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "8119.038d4e91.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/8148.e27d34a2.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/8148.e27d34a2.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "8148.e27d34a2.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "8148.e27d34a2.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/8191.a6547494.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/8191.a6547494.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "8191.a6547494.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "8191.a6547494.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/8259.439eef4a.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/8259.439eef4a.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "8259.439eef4a.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "8259.439eef4a.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/8531.1c721013.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/8531.1c721013.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "8531.1c721013.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "8531.1c721013.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/8583.baa4f5a0.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/8583.baa4f5a0.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "8583.baa4f5a0.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "8583.baa4f5a0.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/8698.5bb1b696.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/8698.5bb1b696.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "8698.5bb1b696.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "8698.5bb1b696.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "8703.743baf71.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "8703.743baf71.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "875.2593b9db.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "875.2593b9db.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/9009.78b5479a.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/9009.78b5479a.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9009.78b5479a.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "9009.78b5479a.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/9196.312a3d80.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/9196.312a3d80.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9196.312a3d80.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "9196.312a3d80.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/9235.b2714593.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/9235.b2714593.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9235.b2714593.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "9235.b2714593.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/9238.8ae8b0d0.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/9238.8ae8b0d0.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9238.8ae8b0d0.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "9238.8ae8b0d0.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/9367.127331a0.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/9367.127331a0.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9367.127331a0.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "9367.127331a0.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9419.1497cff3.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "9419.1497cff3.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9517.d6983e61.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "9517.d6983e61.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9919.f339f893.chunk.js", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "9919.f339f893.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-Black.cf56c1b149d0a5e8d7c6.ttf", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "Roboto-Black.cf56c1b149d0a5e8d7c6.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-Bold.f80816a5455d171f948d.ttf", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "Roboto-Bold.f80816a5455d171f948d.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-Italic.87f3afe16a8c3c370634.ttf", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "Roboto-Italic.87f3afe16a8c3c370634.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-Light.333da16a3f3cc391d087.ttf", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "Roboto-Light.333da16a3f3cc391d087.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-LightItalic.c590382422f2742d788b.ttf.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-LightItalic.c590382422f2742d788b.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-LightItalic.c590382422f2742d788b.ttf", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "Roboto-LightItalic.c590382422f2742d788b.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-Medium.7c8d04cd831df3033c8a.ttf.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Medium.7c8d04cd831df3033c8a.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-Medium.7c8d04cd831df3033c8a.ttf", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "Roboto-Medium.7c8d04cd831df3033c8a.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-MediumItalic.82736aaa11c64709055f.ttf.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-MediumItalic.82736aaa11c64709055f.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-MediumItalic.82736aaa11c64709055f.ttf", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "Roboto-MediumItalic.82736aaa11c64709055f.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-Regular.fc2b5060f7accec5cf74.ttf.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Regular.fc2b5060f7accec5cf74.ttf.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-Regular.fc2b5060f7accec5cf74.ttf", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "Roboto-Regular.fc2b5060f7accec5cf74.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-Thin.a732a12eb07742232407.ttf.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Thin.a732a12eb07742232407.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-Thin.a732a12eb07742232407.ttf", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "Roboto-Thin.a732a12eb07742232407.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/media/Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/static/schedula/media/index.42119833dddefe38a9fa.cjs.gz` & `schedula-1.5.6/schedula/utils/form/static/schedula/media/index.42119833dddefe38a9fa.cjs.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index.42119833dddefe38a9fa.cjs", last modified: Tue Mar 19 11:30:05 2024, from Unix
+gzip compressed data, was "index.42119833dddefe38a9fa.cjs", last modified: Wed Apr  3 12:52:57 2024, from Unix
```

### Comparing `schedula-1.5.5/schedula/utils/form/templates/schedula/base.html` & `schedula-1.5.6/schedula/utils/form/templates/schedula/base.html`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/gen.py` & `schedula-1.5.6/schedula/utils/gen.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/graph.py` & `schedula-1.5.6/schedula/utils/graph.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/imp.py` & `schedula-1.5.6/schedula/utils/imp.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/io/__init__.py` & `schedula-1.5.6/schedula/utils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/sol.py` & `schedula-1.5.6/schedula/utils/sol.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/utl.py` & `schedula-1.5.6/schedula/utils/utl.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula/utils/web/__init__.py` & `schedula-1.5.6/schedula/utils/web/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/schedula.egg-info/PKG-INFO` & `schedula-1.5.6/schedula.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: schedula
-Version: 1.5.5
+Version: 1.5.6
 Summary: Produce a plan that dispatches calls based on a graph of functions, satisfying data dependencies.
 Home-page: https://github.com/vinci1it2000/schedula
-Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.5
+Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.6
 Author: Vincenzo Arcidiacono
 Author-email: vinci1it2000@gmail.com
 License: EUPL 1.1+
 Project-URL: Documentation, https://schedula.readthedocs.io
 Project-URL: Issue tracker, https://github.com/vinci1it2000/schedula/issues
 Keywords: flow-based programming,dataflow,parallel,asynchronous,async,scheduling,dispatch,functional programming,dataflow programming
 Classifier: Programming Language :: Python
```

### Comparing `schedula-1.5.5/schedula.egg-info/SOURCES.txt` & `schedula-1.5.6/schedula.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,191 +46,196 @@
 schedula/utils/drw/index/js/jquery.fullscreen.min.js
 schedula/utils/drw/index/js/sunburst-chart.min.js
 schedula/utils/drw/templates/index.html
 schedula/utils/drw/templates/render.html
 schedula/utils/drw/viz/viz.js
 schedula/utils/form/__init__.py
 schedula/utils/form/config.py
+schedula/utils/form/json_secrets.py
 schedula/utils/form/mail.py
 schedula/utils/form/server.py
-schedula/utils/form/static/schedula/css/1357.496fcbc7.chunk.css.gz
 schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz
 schedula/utils/form/static/schedula/css/1724.5fbb5eb3.chunk.css.gz
+schedula/utils/form/static/schedula/css/1737.87abdd03.chunk.css.gz
 schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz
 schedula/utils/form/static/schedula/css/2706.83c2b1be.chunk.css.gz
 schedula/utils/form/static/schedula/css/3667.3d691932.chunk.css.gz
 schedula/utils/form/static/schedula/css/414.4a9f9388.chunk.css.gz
-schedula/utils/form/static/schedula/css/4337.95ac7f8b.chunk.css.gz
+schedula/utils/form/static/schedula/css/4337.588bea5b.chunk.css.gz
+schedula/utils/form/static/schedula/css/4452.70b7e4bb.chunk.css.gz
 schedula/utils/form/static/schedula/css/4459.a24c0b46.chunk.css.gz
 schedula/utils/form/static/schedula/css/5255.de163d1c.chunk.css.gz
 schedula/utils/form/static/schedula/css/5836.0a2c9e70.chunk.css.gz
 schedula/utils/form/static/schedula/css/6753.de163d1c.chunk.css.gz
+schedula/utils/form/static/schedula/css/6836.4de17ac7.chunk.css.gz
 schedula/utils/form/static/schedula/css/7101.8501d8d8.chunk.css.gz
+schedula/utils/form/static/schedula/css/7450.1773328b.chunk.css.gz
 schedula/utils/form/static/schedula/css/8428.03ea8396.chunk.css.gz
 schedula/utils/form/static/schedula/css/9003.d2d6266b.chunk.css.gz
-schedula/utils/form/static/schedula/css/9106.8d761a00.chunk.css.gz
 schedula/utils/form/static/schedula/css/9665.80050c43.chunk.css.gz
-schedula/utils/form/static/schedula/css/9835.6b615d8b.chunk.css.gz
 schedula/utils/form/static/schedula/css/main.539ebc22.css.gz
 schedula/utils/form/static/schedula/forms/index-schema.json
 schedula/utils/form/static/schedula/forms/index-ui.json
-schedula/utils/form/static/schedula/js/1064.85be30e8.chunk.js.gz
 schedula/utils/form/static/schedula/js/1165.ff804d16.chunk.js.gz
 schedula/utils/form/static/schedula/js/1177.950ebcc8.chunk.js.gz
 schedula/utils/form/static/schedula/js/132.a4de6573.chunk.js.gz
 schedula/utils/form/static/schedula/js/1320.8d42e1b4.chunk.js.gz
-schedula/utils/form/static/schedula/js/1357.d39a01da.chunk.js.gz
 schedula/utils/form/static/schedula/js/1362.0594020f.chunk.js.gz
 schedula/utils/form/static/schedula/js/1431.780747e9.chunk.js.gz
 schedula/utils/form/static/schedula/js/1432.f3b34f42.chunk.js.gz
 schedula/utils/form/static/schedula/js/1465.edd9ba38.chunk.js.gz
 schedula/utils/form/static/schedula/js/1476.d0e9ba73.chunk.js.gz
 schedula/utils/form/static/schedula/js/1511.d20fbe21.chunk.js.gz
 schedula/utils/form/static/schedula/js/1583.fbdd1527.chunk.js.gz
 schedula/utils/form/static/schedula/js/159.42f57d98.chunk.js.gz
 schedula/utils/form/static/schedula/js/1641.cc9646e9.chunk.js.gz
 schedula/utils/form/static/schedula/js/1642.5186d671.chunk.js.gz
 schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz
 schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz
-schedula/utils/form/static/schedula/js/1724.8474ed1b.chunk.js.gz
-schedula/utils/form/static/schedula/js/1748.33ff7ac6.chunk.js.gz
+schedula/utils/form/static/schedula/js/1724.d97efc34.chunk.js.gz
+schedula/utils/form/static/schedula/js/1737.13089dbe.chunk.js.gz
+schedula/utils/form/static/schedula/js/1748.0df73428.chunk.js.gz
 schedula/utils/form/static/schedula/js/183.76a6294f.chunk.js.gz
 schedula/utils/form/static/schedula/js/1831.7a4c7750.chunk.js.gz
 schedula/utils/form/static/schedula/js/1973.bcd66253.chunk.js.gz
 schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz
 schedula/utils/form/static/schedula/js/2085.3afcba83.chunk.js.gz
 schedula/utils/form/static/schedula/js/2120.8ea1a31a.chunk.js.gz
 schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz
 schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz
 schedula/utils/form/static/schedula/js/2256.c3de48fa.chunk.js.gz
-schedula/utils/form/static/schedula/js/2286.a0b82906.chunk.js.gz
+schedula/utils/form/static/schedula/js/2286.850702e1.chunk.js.gz
 schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz
 schedula/utils/form/static/schedula/js/2452.288238f6.chunk.js.gz
 schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz
 schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz
 schedula/utils/form/static/schedula/js/2604.46d4f061.chunk.js.gz
 schedula/utils/form/static/schedula/js/2638.b7999325.chunk.js.gz
 schedula/utils/form/static/schedula/js/268.deedefec.chunk.js.gz
 schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz
 schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz
 schedula/utils/form/static/schedula/js/2723.e492696d.chunk.js.gz
-schedula/utils/form/static/schedula/js/2742.edfc3acf.chunk.js.gz
+schedula/utils/form/static/schedula/js/2742.cef81b1c.chunk.js.gz
 schedula/utils/form/static/schedula/js/2768.93ab5524.chunk.js.gz
 schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz
 schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz
 schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz
 schedula/utils/form/static/schedula/js/3070.25639b4f.chunk.js.gz
 schedula/utils/form/static/schedula/js/3099.e186daed.chunk.js.gz
-schedula/utils/form/static/schedula/js/31.3bee8367.chunk.js.gz
 schedula/utils/form/static/schedula/js/3101.c13d903f.chunk.js.gz
 schedula/utils/form/static/schedula/js/3281.a4f1ba69.chunk.js.gz
 schedula/utils/form/static/schedula/js/3327.f5840c2f.chunk.js.gz
 schedula/utils/form/static/schedula/js/3333.3da6381e.chunk.js.gz
 schedula/utils/form/static/schedula/js/3368.b732d88e.chunk.js.gz
+schedula/utils/form/static/schedula/js/3457.a6f7a355.chunk.js.gz
 schedula/utils/form/static/schedula/js/3509.62544ca4.chunk.js.gz
 schedula/utils/form/static/schedula/js/3565.b1e72cb6.chunk.js.gz
 schedula/utils/form/static/schedula/js/3642.27ee29bf.chunk.js.gz
 schedula/utils/form/static/schedula/js/3667.19631032.chunk.js.gz
 schedula/utils/form/static/schedula/js/3676.1ee61f29.chunk.js.gz
 schedula/utils/form/static/schedula/js/368.9a0bfb9a.chunk.js.gz
 schedula/utils/form/static/schedula/js/3850.689e0ff9.chunk.js.gz
 schedula/utils/form/static/schedula/js/3963.54debd2a.chunk.js.gz
 schedula/utils/form/static/schedula/js/4048.6f416a19.chunk.js.gz
-schedula/utils/form/static/schedula/js/4093.fa03dad5.chunk.js.gz
+schedula/utils/form/static/schedula/js/4093.1b358dc3.chunk.js.gz
 schedula/utils/form/static/schedula/js/4095.87cc9b62.chunk.js.gz
+schedula/utils/form/static/schedula/js/4129.3e3e6e91.chunk.js.gz
 schedula/utils/form/static/schedula/js/414.56817ff7.chunk.js.gz
 schedula/utils/form/static/schedula/js/4164.9cdf0caa.chunk.js.gz
 schedula/utils/form/static/schedula/js/4279.d5144a2b.chunk.js.gz
-schedula/utils/form/static/schedula/js/4337.b839f823.chunk.js.gz
+schedula/utils/form/static/schedula/js/4337.8da858ce.chunk.js.gz
 schedula/utils/form/static/schedula/js/4390.3c3f840c.chunk.js.gz
 schedula/utils/form/static/schedula/js/4438.acbb2994.chunk.js.gz
-schedula/utils/form/static/schedula/js/4459.7c486c55.chunk.js.gz
+schedula/utils/form/static/schedula/js/4452.45bca48d.chunk.js.gz
+schedula/utils/form/static/schedula/js/4459.6704ca6e.chunk.js.gz
 schedula/utils/form/static/schedula/js/4569.9990e2a1.chunk.js.gz
 schedula/utils/form/static/schedula/js/4587.5ff7f02e.chunk.js.gz
 schedula/utils/form/static/schedula/js/4596.53d31027.chunk.js.gz
 schedula/utils/form/static/schedula/js/4672.f1f003ed.chunk.js.gz
+schedula/utils/form/static/schedula/js/4673.aa83f5e0.chunk.js.gz
 schedula/utils/form/static/schedula/js/4786.f0dbe7a4.chunk.js.gz
 schedula/utils/form/static/schedula/js/4842.17363063.chunk.js.gz
 schedula/utils/form/static/schedula/js/4906.d6a6dad2.chunk.js.gz
 schedula/utils/form/static/schedula/js/4925.6cb145d6.chunk.js.gz
+schedula/utils/form/static/schedula/js/5025.2850b7b4.chunk.js.gz
 schedula/utils/form/static/schedula/js/5029.09813ba3.chunk.js.gz
 schedula/utils/form/static/schedula/js/5051.955a4b55.chunk.js.gz
 schedula/utils/form/static/schedula/js/5097.04da753b.chunk.js.gz
 schedula/utils/form/static/schedula/js/5255.baba9ad1.chunk.js.gz
 schedula/utils/form/static/schedula/js/5349.d6abdf80.chunk.js.gz
 schedula/utils/form/static/schedula/js/5415.96511657.chunk.js.gz
 schedula/utils/form/static/schedula/js/5459.ab6195a8.chunk.js.gz
 schedula/utils/form/static/schedula/js/5522.772b12da.chunk.js.gz
-schedula/utils/form/static/schedula/js/5652.0a2d25f3.chunk.js.gz
+schedula/utils/form/static/schedula/js/5652.dde5ef02.chunk.js.gz
 schedula/utils/form/static/schedula/js/5672.d78485cb.chunk.js.gz
 schedula/utils/form/static/schedula/js/5784.aa6dfd10.chunk.js.gz
 schedula/utils/form/static/schedula/js/5827.1e26cd85.chunk.js.gz
 schedula/utils/form/static/schedula/js/5836.722242c0.chunk.js.gz
-schedula/utils/form/static/schedula/js/5880.208b3048.chunk.js.gz
+schedula/utils/form/static/schedula/js/5880.5ad7e40e.chunk.js.gz
 schedula/utils/form/static/schedula/js/5954.df1a43db.chunk.js.gz
 schedula/utils/form/static/schedula/js/5959.d5ebe3fe.chunk.js.gz
-schedula/utils/form/static/schedula/js/5973.9de918f7.chunk.js.gz
 schedula/utils/form/static/schedula/js/6043.6bea23a4.chunk.js.gz
 schedula/utils/form/static/schedula/js/608.60f30d1f.chunk.js.gz
 schedula/utils/form/static/schedula/js/6085.d41a2240.chunk.js.gz
 schedula/utils/form/static/schedula/js/6302.996dbe65.chunk.js.gz
 schedula/utils/form/static/schedula/js/6474.6af0dc33.chunk.js.gz
 schedula/utils/form/static/schedula/js/654.98d33eb8.chunk.js.gz
-schedula/utils/form/static/schedula/js/6753.2b6e62d5.chunk.js.gz
+schedula/utils/form/static/schedula/js/6753.e37ed964.chunk.js.gz
 schedula/utils/form/static/schedula/js/6801.62068c84.chunk.js.gz
+schedula/utils/form/static/schedula/js/6836.43947ef9.chunk.js.gz
 schedula/utils/form/static/schedula/js/6855.c4d51fc1.chunk.js.gz
 schedula/utils/form/static/schedula/js/6907.0fe74465.chunk.js.gz
 schedula/utils/form/static/schedula/js/6925.228697fa.chunk.js.gz
 schedula/utils/form/static/schedula/js/6938.c8986bc2.chunk.js.gz
 schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz
 schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz
 schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz
 schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz
-schedula/utils/form/static/schedula/js/7381.62ff7f32.chunk.js.gz
+schedula/utils/form/static/schedula/js/7193.528d18c4.chunk.js.gz
 schedula/utils/form/static/schedula/js/7435.8ac4b848.chunk.js.gz
 schedula/utils/form/static/schedula/js/744.c1913bc4.chunk.js.gz
+schedula/utils/form/static/schedula/js/7450.d618087b.chunk.js.gz
 schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz
 schedula/utils/form/static/schedula/js/7565.867674bc.chunk.js.gz
-schedula/utils/form/static/schedula/js/7605.9c355065.chunk.js.gz
 schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz
 schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz
-schedula/utils/form/static/schedula/js/796.a463ad0d.chunk.js.gz
-schedula/utils/form/static/schedula/js/7974.f57f09fe.chunk.js.gz
+schedula/utils/form/static/schedula/js/796.a7fc5105.chunk.js.gz
+schedula/utils/form/static/schedula/js/7974.7e7de702.chunk.js.gz
 schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz
+schedula/utils/form/static/schedula/js/8115.11a85e47.chunk.js.gz
 schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz
 schedula/utils/form/static/schedula/js/8148.e27d34a2.chunk.js.gz
 schedula/utils/form/static/schedula/js/8191.a6547494.chunk.js.gz
 schedula/utils/form/static/schedula/js/8259.439eef4a.chunk.js.gz
 schedula/utils/form/static/schedula/js/8384.733495df.chunk.js.gz
-schedula/utils/form/static/schedula/js/8428.6d9c78b7.chunk.js.gz
+schedula/utils/form/static/schedula/js/8428.7d81c7b5.chunk.js.gz
+schedula/utils/form/static/schedula/js/8497.f11bc0ea.chunk.js.gz
+schedula/utils/form/static/schedula/js/8516.30c79314.chunk.js.gz
 schedula/utils/form/static/schedula/js/853.c4b3a572.chunk.js.gz
 schedula/utils/form/static/schedula/js/8531.1c721013.chunk.js.gz
 schedula/utils/form/static/schedula/js/8583.baa4f5a0.chunk.js.gz
 schedula/utils/form/static/schedula/js/8698.5bb1b696.chunk.js.gz
 schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz
 schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz
 schedula/utils/form/static/schedula/js/8797.9e3c01c2.chunk.js.gz
 schedula/utils/form/static/schedula/js/8916.4a5d5d2c.chunk.js.gz
 schedula/utils/form/static/schedula/js/9003.b108ee29.chunk.js.gz
 schedula/utils/form/static/schedula/js/9009.78b5479a.chunk.js.gz
 schedula/utils/form/static/schedula/js/9079.476a64c2.chunk.js.gz
-schedula/utils/form/static/schedula/js/9106.262dfeb4.chunk.js.gz
 schedula/utils/form/static/schedula/js/9196.312a3d80.chunk.js.gz
 schedula/utils/form/static/schedula/js/9235.b2714593.chunk.js.gz
 schedula/utils/form/static/schedula/js/9238.8ae8b0d0.chunk.js.gz
 schedula/utils/form/static/schedula/js/9367.127331a0.chunk.js.gz
 schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz
 schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz
 schedula/utils/form/static/schedula/js/9559.52882117.chunk.js.gz
-schedula/utils/form/static/schedula/js/9628.5b2d7fe9.chunk.js.gz
-schedula/utils/form/static/schedula/js/9665.894f2277.chunk.js.gz
-schedula/utils/form/static/schedula/js/9835.0870cf0f.chunk.js.gz
+schedula/utils/form/static/schedula/js/9665.8425fb6b.chunk.js.gz
 schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz
 schedula/utils/form/static/schedula/js/9925.cc714497.chunk.js.gz
-schedula/utils/form/static/schedula/js/main.85117e28.js.gz
+schedula/utils/form/static/schedula/js/main.d401041d.js.gz
 schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-LightItalic.c590382422f2742d788b.ttf.gz
```

### Comparing `schedula-1.5.5/schedula.egg-info/requires.txt` & `schedula-1.5.6/schedula.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/setup.py` & `schedula-1.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/tests/test_dispatcher.py` & `schedula-1.5.6/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/tests/test_import.py` & `schedula-1.5.6/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/tests/test_micropython.py` & `schedula-1.5.6/tests/test_micropython.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/tests/test_readme.py` & `schedula-1.5.6/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.5/tests/test_setup.py` & `schedula-1.5.6/tests/test_setup.py`

 * *Files identical despite different names*

