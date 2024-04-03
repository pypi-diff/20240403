# Comparing `tmp/zebra_day-0.3.8.tar.gz` & `tmp/zebra_day-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zebra_day-0.3.8.tar", last modified: Mon Mar 11 17:14:55 2024, max compression
+gzip compressed data, was "zebra_day-0.3.9.tar", last modified: Wed Apr  3 18:55:06 2024, max compression
```

## Comparing `zebra_day-0.3.8.tar` & `zebra_day-0.3.9.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-03-11 17:14:55.875448 zebra_day-0.3.8/
--rw-r--r--   0 daylily    (503) staff       (20)    35149 2023-10-30 06:23:35.000000 zebra_day-0.3.8/LICENSE
--rw-r--r--   0 daylily    (503) staff       (20)      470 2024-03-11 17:14:55.875185 zebra_day-0.3.8/PKG-INFO
--rw-r--r--   0 daylily    (503) staff       (20)    26315 2024-02-28 19:17:05.000000 zebra_day-0.3.8/README.md
--rw-r--r--   0 daylily    (503) staff       (20)       38 2024-03-11 17:14:55.875501 zebra_day-0.3.8/setup.cfg
--rw-r--r--   0 daylily    (503) staff       (20)      993 2024-03-11 17:12:49.000000 zebra_day-0.3.8/setup.py
-drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-03-11 17:14:55.852074 zebra_day-0.3.8/tests/
--rw-r--r--   0 daylily    (503) staff       (20)        0 2023-10-30 06:23:35.000000 zebra_day-0.3.8/tests/__init__.py
--rw-r--r--   0 daylily    (503) staff       (20)     2284 2023-11-01 08:27:07.000000 zebra_day-0.3.8/tests/test_creating_labels.py
--rw-r--r--   0 daylily    (503) staff       (20)     2573 2023-11-01 08:14:16.000000 zebra_day-0.3.8/tests/test_setup_printers_json.py
--rw-r--r--   0 daylily    (503) staff       (20)      110 2023-10-30 06:23:35.000000 zebra_day-0.3.8/tests/test_web_server.py
-drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-03-11 17:14:55.852764 zebra_day-0.3.8/zebra_day/
--rw-r--r--   0 daylily    (503) staff       (20)        0 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/__init__.py
-drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-03-11 17:14:55.858384 zebra_day-0.3.8/zebra_day/bin/
--rw-r--r--   0 daylily    (503) staff       (20)      227 2023-10-31 07:09:53.000000 zebra_day-0.3.8/zebra_day/bin/#print_zpl_from_file.py#
--rw-r--r--   0 daylily    (503) staff       (20)      233 2023-12-13 01:46:51.000000 zebra_day-0.3.8/zebra_day/bin/#probe_zebra_printer.py#
--rw-r--r--   0 daylily    (503) staff       (20)        0 2023-12-19 20:30:38.000000 zebra_day-0.3.8/zebra_day/bin/__init__.py
--rw-r--r--   0 daylily    (503) staff       (20)     1169 2023-12-13 03:57:28.000000 zebra_day-0.3.8/zebra_day/bin/check_sgd_wml.py
--rw-r--r--   0 daylily    (503) staff       (20)      488 2023-10-31 05:42:38.000000 zebra_day-0.3.8/zebra_day/bin/fetch_zebra_config.py
--rw-r--r--   0 daylily    (503) staff       (20)     1782 2023-10-31 05:32:49.000000 zebra_day-0.3.8/zebra_day/bin/generate_coord_grid_zpl.py
--rw-r--r--   0 daylily    (503) staff       (20)      265 2023-10-31 07:11:42.000000 zebra_day-0.3.8/zebra_day/bin/print_zpl_from_file.py
--rw-r--r--   0 daylily    (503) staff       (20)     2286 2023-10-31 05:10:05.000000 zebra_day-0.3.8/zebra_day/bin/probe_new_label_dimensions.py
--rw-r--r--   0 daylily    (503) staff       (20)     1000 2023-12-13 01:47:25.000000 zebra_day-0.3.8/zebra_day/bin/probe_zebra_w_sgd.py
--rw-r--r--   0 daylily    (503) staff       (20)      848 2023-12-13 01:38:03.000000 zebra_day-0.3.8/zebra_day/bin/reset_zebra_custom_menus.py
--rw-r--r--   0 daylily    (503) staff       (20)      592 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/bin/scan_for_networed_zebra_printers.py
--rw-r--r--   0 daylily    (503) staff       (20)       25 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/bin/scan_for_networed_zebra_printers_arp_scan.sh
--rwxr-xr-x   0 daylily    (503) staff       (20)      865 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/bin/scan_for_networed_zebra_printers_curl.sh
--rw-r--r--   0 daylily    (503) staff       (20)      656 2023-12-13 03:51:46.000000 zebra_day-0.3.8/zebra_day/bin/set_no_wml.py
--rw-r--r--   0 daylily    (503) staff       (20)     1018 2023-12-13 01:51:53.000000 zebra_day-0.3.8/zebra_day/bin/set_zebra_ip_w_sgd.py
--rw-r--r--   0 daylily    (503) staff       (20)    45692 2023-12-30 00:21:34.000000 zebra_day-0.3.8/zebra_day/bin/zserve.py
--rw-r--r--   0 daylily    (503) staff       (20)     1116 2023-12-19 20:25:13.000000 zebra_day-0.3.8/zebra_day/cmd_mgr.py
-drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-03-11 17:14:55.861654 zebra_day-0.3.8/zebra_day/etc/
--rw-r--r--   0 daylily    (503) staff       (20)    79748 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/etc/Monoid-Regular-HalfTight-Dollar-0-1-l.ttf
-drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-03-11 17:14:55.867580 zebra_day-0.3.8/zebra_day/etc/label_styles/
--rw-r--r--   0 daylily    (503) staff       (20)        0 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/blank.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      552 2023-12-12 23:25:34.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/cornersStripOf4Squares_1inX1in.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      742 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/corners_1inX2in.zpl
--rw-r--r--   0 daylily    (503) staff       (20)       86 2023-11-01 09:00:12.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/corners_20cmX30cm.zpl
--rw-r--r--   0 daylily    (503) staff       (20)       99 2023-10-31 07:22:32.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/corners_smallTube.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      159 2023-10-30 23:06:51.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/corners_unspecifiedDimensions.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      261 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/generic_2inX1in.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      107 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/plate_1inX0.25in.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      107 2024-03-06 20:43:23.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/plate_1inX0.25inHD.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      181 2023-12-30 01:01:49.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/smallTubeWdotHD_prod.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      106 2023-12-12 22:04:26.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/smallTubeWdot_corners.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      176 2023-12-12 22:17:23.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/smallTubeWdot_prod.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      159 2024-02-12 03:01:15.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/smallTubeWdot_prodAlt1.zpl
--rw-r--r--   0 daylily    (503) staff       (20)       40 2024-03-11 17:13:39.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/smallTubeWdot_prodAlt1b.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      166 2024-03-11 17:13:24.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/smallTubeWdot_prodV2.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      322 2023-12-12 23:31:44.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/stripOf4Squares_1inX1in.zpl
--rw-r--r--   0 daylily    (503) staff       (20)    14582 2023-10-31 05:32:56.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/test_800dX800dCoordinateArray.zpl
-drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-03-11 17:14:55.867861 zebra_day-0.3.8/zebra_day/etc/label_styles/tmps/
--rw-r--r--   0 daylily    (503) staff       (20)        0 2023-12-30 00:02:47.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/tmps/tmp_zpl_templates.here
--rw-r--r--   0 daylily    (503) staff       (20)      320 2023-11-01 09:31:41.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/tube_20mmX30mmA.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      181 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/tube_2inX0.3in.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      181 2023-12-12 22:57:04.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/tube_2inX0.5in.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      183 2023-10-30 22:47:31.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/tube_2inX0.5inHD.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      287 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/tube_2inX1in.zpl
--rw-r--r--   0 daylily    (503) staff       (20)      273 2023-10-30 22:18:48.000000 zebra_day-0.3.8/zebra_day/etc/label_styles/tube_2inX1inHD.zpl
--rw-r--r--   0 daylily    (503) staff       (20)     2661 2023-12-19 21:15:50.000000 zebra_day-0.3.8/zebra_day/etc/printer_config.json
--rw-r--r--   0 daylily    (503) staff       (20)      372 2023-11-01 06:10:18.000000 zebra_day-0.3.8/zebra_day/etc/printer_config.template.json
-drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-03-11 17:14:55.868003 zebra_day-0.3.8/zebra_day/files/
--rw-r--r--   0 daylily    (503) staff       (20)        0 2023-12-30 00:47:36.000000 zebra_day-0.3.8/zebra_day/files/hold
-drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-03-11 17:14:55.868149 zebra_day-0.3.8/zebra_day/logs/
--rw-r--r--   0 daylily    (503) staff       (20)    64218 2023-12-19 21:20:41.000000 zebra_day-0.3.8/zebra_day/logs/print_requests.log
--rw-r--r--   0 daylily    (503) staff       (20)    17950 2023-12-30 00:09:50.000000 zebra_day-0.3.8/zebra_day/print_mgr.py
-drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-03-11 17:14:55.874848 zebra_day-0.3.8/zebra_day/static/
--rw-r--r--   0 daylily    (503) staff       (20)     3402 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/static/datschund.css
--rw-r--r--   0 daylily    (503) staff       (20)     2980 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/static/datschund.png
--rw-r--r--   0 daylily    (503) staff       (20)    18044 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/static/daylily.png
--rw-r--r--   0 daylily    (503) staff       (20)     1627 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/static/general.css
--rw-r--r--   0 daylily    (503) staff       (20)   645087 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/static/moon.jpeg
--rw-r--r--   0 daylily    (503) staff       (20)     4698 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/static/oakland.css
--rw-r--r--   0 daylily    (503) staff       (20)     3037 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/static/petrichor.css
--rw-r--r--   0 daylily    (503) staff       (20)     3382 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/static/popday_daylily.css
--rw-r--r--   0 daylily    (503) staff       (20)     3532 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/static/style.css
--rw-r--r--   0 daylily    (503) staff       (20)     2778 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/static/triangles.css
--rw-r--r--   0 daylily    (503) staff       (20)     8579 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/static/tron.css
--rw-r--r--   0 daylily    (503) staff       (20)     3600 2023-10-30 06:23:35.000000 zebra_day-0.3.8/zebra_day/static/zebras.css
-drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-03-11 17:14:55.853821 zebra_day-0.3.8/zebra_day.egg-info/
--rw-r--r--   0 daylily    (503) staff       (20)      470 2024-03-11 17:14:55.000000 zebra_day-0.3.8/zebra_day.egg-info/PKG-INFO
--rw-r--r--   0 daylily    (503) staff       (20)     2778 2024-03-11 17:14:55.000000 zebra_day-0.3.8/zebra_day.egg-info/SOURCES.txt
--rw-r--r--   0 daylily    (503) staff       (20)        1 2024-03-11 17:14:55.000000 zebra_day-0.3.8/zebra_day.egg-info/dependency_links.txt
--rw-r--r--   0 daylily    (503) staff       (20)      105 2024-03-11 17:14:55.000000 zebra_day-0.3.8/zebra_day.egg-info/entry_points.txt
--rw-r--r--   0 daylily    (503) staff       (20)       91 2024-03-11 17:14:55.000000 zebra_day-0.3.8/zebra_day.egg-info/requires.txt
--rw-r--r--   0 daylily    (503) staff       (20)       16 2024-03-11 17:14:55.000000 zebra_day-0.3.8/zebra_day.egg-info/top_level.txt
+drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-04-03 18:55:06.256081 zebra_day-0.3.9/
+-rw-r--r--   0 daylily    (503) staff       (20)    35149 2023-10-30 06:23:35.000000 zebra_day-0.3.9/LICENSE
+-rw-r--r--   0 daylily    (503) staff       (20)      470 2024-04-03 18:55:06.255838 zebra_day-0.3.9/PKG-INFO
+-rw-r--r--   0 daylily    (503) staff       (20)    26315 2024-02-28 19:17:05.000000 zebra_day-0.3.9/README.md
+-rw-r--r--   0 daylily    (503) staff       (20)       38 2024-04-03 18:55:06.256131 zebra_day-0.3.9/setup.cfg
+-rw-r--r--   0 daylily    (503) staff       (20)      993 2024-04-03 18:54:21.000000 zebra_day-0.3.9/setup.py
+drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-04-03 18:55:06.234726 zebra_day-0.3.9/tests/
+-rw-r--r--   0 daylily    (503) staff       (20)        0 2023-10-30 06:23:35.000000 zebra_day-0.3.9/tests/__init__.py
+-rw-r--r--   0 daylily    (503) staff       (20)     2284 2023-11-01 08:27:07.000000 zebra_day-0.3.9/tests/test_creating_labels.py
+-rw-r--r--   0 daylily    (503) staff       (20)     2573 2023-11-01 08:14:16.000000 zebra_day-0.3.9/tests/test_setup_printers_json.py
+-rw-r--r--   0 daylily    (503) staff       (20)      110 2023-10-30 06:23:35.000000 zebra_day-0.3.9/tests/test_web_server.py
+drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-04-03 18:55:06.235436 zebra_day-0.3.9/zebra_day/
+-rw-r--r--   0 daylily    (503) staff       (20)        0 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/__init__.py
+drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-04-03 18:55:06.240406 zebra_day-0.3.9/zebra_day/bin/
+-rw-r--r--   0 daylily    (503) staff       (20)      227 2023-10-31 07:09:53.000000 zebra_day-0.3.9/zebra_day/bin/#print_zpl_from_file.py#
+-rw-r--r--   0 daylily    (503) staff       (20)      233 2023-12-13 01:46:51.000000 zebra_day-0.3.9/zebra_day/bin/#probe_zebra_printer.py#
+-rw-r--r--   0 daylily    (503) staff       (20)        0 2023-12-19 20:30:38.000000 zebra_day-0.3.9/zebra_day/bin/__init__.py
+-rw-r--r--   0 daylily    (503) staff       (20)     1169 2023-12-13 03:57:28.000000 zebra_day-0.3.9/zebra_day/bin/check_sgd_wml.py
+-rw-r--r--   0 daylily    (503) staff       (20)      488 2023-10-31 05:42:38.000000 zebra_day-0.3.9/zebra_day/bin/fetch_zebra_config.py
+-rw-r--r--   0 daylily    (503) staff       (20)     1782 2023-10-31 05:32:49.000000 zebra_day-0.3.9/zebra_day/bin/generate_coord_grid_zpl.py
+-rw-r--r--   0 daylily    (503) staff       (20)      265 2023-10-31 07:11:42.000000 zebra_day-0.3.9/zebra_day/bin/print_zpl_from_file.py
+-rw-r--r--   0 daylily    (503) staff       (20)     2286 2023-10-31 05:10:05.000000 zebra_day-0.3.9/zebra_day/bin/probe_new_label_dimensions.py
+-rw-r--r--   0 daylily    (503) staff       (20)     1000 2023-12-13 01:47:25.000000 zebra_day-0.3.9/zebra_day/bin/probe_zebra_w_sgd.py
+-rw-r--r--   0 daylily    (503) staff       (20)      848 2023-12-13 01:38:03.000000 zebra_day-0.3.9/zebra_day/bin/reset_zebra_custom_menus.py
+-rw-r--r--   0 daylily    (503) staff       (20)      592 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/bin/scan_for_networed_zebra_printers.py
+-rw-r--r--   0 daylily    (503) staff       (20)       25 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/bin/scan_for_networed_zebra_printers_arp_scan.sh
+-rwxr-xr-x   0 daylily    (503) staff       (20)      865 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/bin/scan_for_networed_zebra_printers_curl.sh
+-rw-r--r--   0 daylily    (503) staff       (20)      656 2023-12-13 03:51:46.000000 zebra_day-0.3.9/zebra_day/bin/set_no_wml.py
+-rw-r--r--   0 daylily    (503) staff       (20)     1018 2023-12-13 01:51:53.000000 zebra_day-0.3.9/zebra_day/bin/set_zebra_ip_w_sgd.py
+-rw-r--r--   0 daylily    (503) staff       (20)    45692 2023-12-30 00:21:34.000000 zebra_day-0.3.9/zebra_day/bin/zserve.py
+-rw-r--r--   0 daylily    (503) staff       (20)     1116 2023-12-19 20:25:13.000000 zebra_day-0.3.9/zebra_day/cmd_mgr.py
+drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-04-03 18:55:06.242314 zebra_day-0.3.9/zebra_day/etc/
+-rw-r--r--   0 daylily    (503) staff       (20)    79748 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/etc/Monoid-Regular-HalfTight-Dollar-0-1-l.ttf
+drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-04-03 18:55:06.247846 zebra_day-0.3.9/zebra_day/etc/label_styles/
+-rw-r--r--   0 daylily    (503) staff       (20)        0 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/blank.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      552 2023-12-12 23:25:34.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/cornersStripOf4Squares_1inX1in.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      742 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/corners_1inX2in.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)       86 2023-11-01 09:00:12.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/corners_20cmX30cm.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)       99 2023-10-31 07:22:32.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/corners_smallTube.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      159 2023-10-30 23:06:51.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/corners_unspecifiedDimensions.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      261 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/generic_2inX1in.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      107 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/plate_1inX0.25in.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      107 2024-03-06 20:43:23.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/plate_1inX0.25inHD.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      181 2023-12-30 01:01:49.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/smallTubeWdotHD_prod.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      106 2023-12-12 22:04:26.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/smallTubeWdot_corners.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      176 2023-12-12 22:17:23.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/smallTubeWdot_prod.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      159 2024-02-12 03:01:15.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/smallTubeWdot_prodAlt1.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)       40 2024-03-11 17:13:39.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/smallTubeWdot_prodAlt1b.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      166 2024-03-11 17:13:24.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/smallTubeWdot_prodV2.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      371 2024-04-03 18:54:11.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/smallTubeWdot_reagent.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      322 2023-12-12 23:31:44.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/stripOf4Squares_1inX1in.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)    14582 2023-10-31 05:32:56.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/test_800dX800dCoordinateArray.zpl
+drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-04-03 18:55:06.248071 zebra_day-0.3.9/zebra_day/etc/label_styles/tmps/
+-rw-r--r--   0 daylily    (503) staff       (20)        0 2023-12-30 00:02:47.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/tmps/tmp_zpl_templates.here
+-rw-r--r--   0 daylily    (503) staff       (20)      320 2023-11-01 09:31:41.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/tube_20mmX30mmA.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      181 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/tube_2inX0.3in.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      181 2023-12-12 22:57:04.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/tube_2inX0.5in.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      183 2023-10-30 22:47:31.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/tube_2inX0.5inHD.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      287 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/tube_2inX1in.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)      273 2023-10-30 22:18:48.000000 zebra_day-0.3.9/zebra_day/etc/label_styles/tube_2inX1inHD.zpl
+-rw-r--r--   0 daylily    (503) staff       (20)     2661 2023-12-19 21:15:50.000000 zebra_day-0.3.9/zebra_day/etc/printer_config.json
+-rw-r--r--   0 daylily    (503) staff       (20)      372 2023-11-01 06:10:18.000000 zebra_day-0.3.9/zebra_day/etc/printer_config.template.json
+drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-04-03 18:55:06.248170 zebra_day-0.3.9/zebra_day/files/
+-rw-r--r--   0 daylily    (503) staff       (20)        0 2023-12-30 00:47:36.000000 zebra_day-0.3.9/zebra_day/files/hold
+drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-04-03 18:55:06.248264 zebra_day-0.3.9/zebra_day/logs/
+-rw-r--r--   0 daylily    (503) staff       (20)    64218 2023-12-19 21:20:41.000000 zebra_day-0.3.9/zebra_day/logs/print_requests.log
+-rw-r--r--   0 daylily    (503) staff       (20)    17950 2023-12-30 00:09:50.000000 zebra_day-0.3.9/zebra_day/print_mgr.py
+drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-04-03 18:55:06.255441 zebra_day-0.3.9/zebra_day/static/
+-rw-r--r--   0 daylily    (503) staff       (20)     3402 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/static/datschund.css
+-rw-r--r--   0 daylily    (503) staff       (20)     2980 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/static/datschund.png
+-rw-r--r--   0 daylily    (503) staff       (20)    18044 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/static/daylily.png
+-rw-r--r--   0 daylily    (503) staff       (20)     1627 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/static/general.css
+-rw-r--r--   0 daylily    (503) staff       (20)   645087 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/static/moon.jpeg
+-rw-r--r--   0 daylily    (503) staff       (20)     4698 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/static/oakland.css
+-rw-r--r--   0 daylily    (503) staff       (20)     3037 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/static/petrichor.css
+-rw-r--r--   0 daylily    (503) staff       (20)     3382 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/static/popday_daylily.css
+-rw-r--r--   0 daylily    (503) staff       (20)     3532 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/static/style.css
+-rw-r--r--   0 daylily    (503) staff       (20)     2778 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/static/triangles.css
+-rw-r--r--   0 daylily    (503) staff       (20)     8579 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/static/tron.css
+-rw-r--r--   0 daylily    (503) staff       (20)     3600 2023-10-30 06:23:35.000000 zebra_day-0.3.9/zebra_day/static/zebras.css
+drwxr-xr-x   0 daylily    (503) staff       (20)        0 2024-04-03 18:55:06.236436 zebra_day-0.3.9/zebra_day.egg-info/
+-rw-r--r--   0 daylily    (503) staff       (20)      470 2024-04-03 18:55:06.000000 zebra_day-0.3.9/zebra_day.egg-info/PKG-INFO
+-rw-r--r--   0 daylily    (503) staff       (20)     2831 2024-04-03 18:55:06.000000 zebra_day-0.3.9/zebra_day.egg-info/SOURCES.txt
+-rw-r--r--   0 daylily    (503) staff       (20)        1 2024-04-03 18:55:06.000000 zebra_day-0.3.9/zebra_day.egg-info/dependency_links.txt
+-rw-r--r--   0 daylily    (503) staff       (20)      105 2024-04-03 18:55:06.000000 zebra_day-0.3.9/zebra_day.egg-info/entry_points.txt
+-rw-r--r--   0 daylily    (503) staff       (20)       91 2024-04-03 18:55:06.000000 zebra_day-0.3.9/zebra_day.egg-info/requires.txt
+-rw-r--r--   0 daylily    (503) staff       (20)       16 2024-04-03 18:55:06.000000 zebra_day-0.3.9/zebra_day.egg-info/top_level.txt
```

### Comparing `zebra_day-0.3.8/LICENSE` & `zebra_day-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/README.md` & `zebra_day-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/setup.py` & `zebra_day-0.3.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zebra_day',
-    version='0.3.8',
+    version='0.3.9',
     description='A Python library to manage a zebra printer fleet and an api for ZPL print requests.',
     author='John Major',
     author_email='john@daylilyinformatics.com',
     url='https://github.com/Daylily-Informatics/zebra_day',
     packages=find_packages(),
     install_requires=["yaml_config_day==0.0.5", "requests", "pytz==2023.3.post1", "cherrypy==18.8.0", "ipython==8.16.1", "pytest"],
     include_package_data=True,
```

### Comparing `zebra_day-0.3.8/tests/test_creating_labels.py` & `zebra_day-0.3.9/tests/test_creating_labels.py`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/tests/test_setup_printers_json.py` & `zebra_day-0.3.9/tests/test_setup_printers_json.py`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/bin/check_sgd_wml.py` & `zebra_day-0.3.9/zebra_day/bin/check_sgd_wml.py`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/bin/generate_coord_grid_zpl.py` & `zebra_day-0.3.9/zebra_day/bin/generate_coord_grid_zpl.py`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/bin/probe_new_label_dimensions.py` & `zebra_day-0.3.9/zebra_day/bin/probe_new_label_dimensions.py`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/bin/probe_zebra_w_sgd.py` & `zebra_day-0.3.9/zebra_day/bin/probe_zebra_w_sgd.py`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/bin/reset_zebra_custom_menus.py` & `zebra_day-0.3.9/zebra_day/bin/reset_zebra_custom_menus.py`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/bin/scan_for_networed_zebra_printers.py` & `zebra_day-0.3.9/zebra_day/bin/scan_for_networed_zebra_printers.py`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/bin/scan_for_networed_zebra_printers_curl.sh` & `zebra_day-0.3.9/zebra_day/bin/scan_for_networed_zebra_printers_curl.sh`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/bin/set_no_wml.py` & `zebra_day-0.3.9/zebra_day/bin/set_no_wml.py`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/bin/set_zebra_ip_w_sgd.py` & `zebra_day-0.3.9/zebra_day/bin/set_zebra_ip_w_sgd.py`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/bin/zserve.py` & `zebra_day-0.3.9/zebra_day/bin/zserve.py`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/cmd_mgr.py` & `zebra_day-0.3.9/zebra_day/cmd_mgr.py`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/etc/Monoid-Regular-HalfTight-Dollar-0-1-l.ttf` & `zebra_day-0.3.9/zebra_day/etc/Monoid-Regular-HalfTight-Dollar-0-1-l.ttf`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/etc/label_styles/cornersStripOf4Squares_1inX1in.zpl` & `zebra_day-0.3.9/zebra_day/etc/label_styles/cornersStripOf4Squares_1inX1in.zpl`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/etc/label_styles/corners_1inX2in.zpl` & `zebra_day-0.3.9/zebra_day/etc/label_styles/corners_1inX2in.zpl`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/etc/label_styles/test_800dX800dCoordinateArray.zpl` & `zebra_day-0.3.9/zebra_day/etc/label_styles/test_800dX800dCoordinateArray.zpl`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/etc/printer_config.json` & `zebra_day-0.3.9/zebra_day/etc/printer_config.json`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/logs/print_requests.log` & `zebra_day-0.3.9/zebra_day/logs/print_requests.log`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/print_mgr.py` & `zebra_day-0.3.9/zebra_day/print_mgr.py`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/static/datschund.css` & `zebra_day-0.3.9/zebra_day/static/datschund.css`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/static/datschund.png` & `zebra_day-0.3.9/zebra_day/static/datschund.png`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/static/daylily.png` & `zebra_day-0.3.9/zebra_day/static/daylily.png`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/static/general.css` & `zebra_day-0.3.9/zebra_day/static/general.css`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/static/moon.jpeg` & `zebra_day-0.3.9/zebra_day/static/moon.jpeg`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/static/oakland.css` & `zebra_day-0.3.9/zebra_day/static/oakland.css`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/static/petrichor.css` & `zebra_day-0.3.9/zebra_day/static/petrichor.css`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/static/popday_daylily.css` & `zebra_day-0.3.9/zebra_day/static/popday_daylily.css`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/static/style.css` & `zebra_day-0.3.9/zebra_day/static/style.css`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/static/triangles.css` & `zebra_day-0.3.9/zebra_day/static/triangles.css`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/static/tron.css` & `zebra_day-0.3.9/zebra_day/static/tron.css`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day/static/zebras.css` & `zebra_day-0.3.9/zebra_day/static/zebras.css`

 * *Files identical despite different names*

### Comparing `zebra_day-0.3.8/zebra_day.egg-info/SOURCES.txt` & `zebra_day-0.3.9/zebra_day.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 zebra_day/etc/label_styles/plate_1inX0.25inHD.zpl
 zebra_day/etc/label_styles/smallTubeWdotHD_prod.zpl
 zebra_day/etc/label_styles/smallTubeWdot_corners.zpl
 zebra_day/etc/label_styles/smallTubeWdot_prod.zpl
 zebra_day/etc/label_styles/smallTubeWdot_prodAlt1.zpl
 zebra_day/etc/label_styles/smallTubeWdot_prodAlt1b.zpl
 zebra_day/etc/label_styles/smallTubeWdot_prodV2.zpl
+zebra_day/etc/label_styles/smallTubeWdot_reagent.zpl
 zebra_day/etc/label_styles/stripOf4Squares_1inX1in.zpl
 zebra_day/etc/label_styles/test_800dX800dCoordinateArray.zpl
 zebra_day/etc/label_styles/tube_20mmX30mmA.zpl
 zebra_day/etc/label_styles/tube_2inX0.3in.zpl
 zebra_day/etc/label_styles/tube_2inX0.5in.zpl
 zebra_day/etc/label_styles/tube_2inX0.5inHD.zpl
 zebra_day/etc/label_styles/tube_2inX1in.zpl
```

