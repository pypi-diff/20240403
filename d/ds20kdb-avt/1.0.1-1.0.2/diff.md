# Comparing `tmp/ds20kdb-avt-1.0.1.tar.gz` & `tmp/ds20kdb-avt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds20kdb-avt-1.0.1.tar", last modified: Thu Mar 28 13:28:47 2024, max compression
+gzip compressed data, was "ds20kdb-avt-1.0.2.tar", last modified: Wed Apr  3 17:30:49 2024, max compression
```

## Comparing `ds20kdb-avt-1.0.1.tar` & `ds20kdb-avt-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-03-28 13:28:47.454387 ds20kdb-avt-1.0.1/
--rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.1/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     6889 2024-03-28 13:28:47.453450 ds20kdb-avt-1.0.1/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     5281 2023-10-13 14:30:24.000000 ds20kdb-avt-1.0.1/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.1/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2024-03-28 13:28:47.454595 ds20kdb-avt-1.0.1/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     3208 2024-03-27 16:51:59.000000 ds20kdb-avt-1.0.1/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-03-28 13:28:47.412500 ds20kdb-avt-1.0.1/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-03-28 13:28:47.445024 ds20kdb-avt-1.0.1/src/ds20kdb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.1/src/ds20kdb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)     9414 2023-09-17 11:41:52.000000 ds20kdb-avt-1.0.1/src/ds20kdb/auth.py
--rw-r--r--   0 avt        (501) staff       (20)    38424 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.1/src/ds20kdb/common.py
--rw-r--r--   0 avt        (501) staff       (20)      182 2023-04-01 13:34:13.000000 ds20kdb-avt-1.0.1/src/ds20kdb/constants.py
--rwxr-xr-x   0 avt        (501) staff       (20)     2123 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.1/src/ds20kdb/create_credentials_file.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33522 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.1/src/ds20kdb/gen_tray_files_gui.py
--rw-r--r--   0 avt        (501) staff       (20)    93422 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.1/src/ds20kdb/interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)     6936 2023-09-06 15:42:42.000000 ds20kdb-avt-1.0.1/src/ds20kdb/qr.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7876 2023-09-09 12:18:43.000000 ds20kdb-avt-1.0.1/src/ds20kdb/qrgen.py
--rwxr-xr-x   0 avt        (501) staff       (20)    32509 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.1/src/ds20kdb/scanner_auto.py
--rwxr-xr-x   0 avt        (501) staff       (20)   117866 2024-03-28 13:27:09.000000 ds20kdb-avt-1.0.1/src/ds20kdb/submit_vtile.py
--rwxr-xr-x   0 avt        (501) staff       (20)    22398 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.1/src/ds20kdb/submit_vtile_json.py
--rwxr-xr-x   0 avt        (501) staff       (20)    11674 2024-02-29 13:53:11.000000 ds20kdb-avt-1.0.1/src/ds20kdb/veto_location.py
--rwxr-xr-x   0 avt        (501) staff       (20)    19987 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.1/src/ds20kdb/veto_location_gui.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14551 2024-01-10 17:21:38.000000 ds20kdb-avt-1.0.1/src/ds20kdb/visual.py
--rwxr-xr-x   0 avt        (501) staff       (20)     8909 2023-09-17 11:55:13.000000 ds20kdb-avt-1.0.1/src/ds20kdb/vtile_test_submit_cr.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7679 2024-01-10 17:21:38.000000 ds20kdb-avt-1.0.1/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py
--rwx------   0 avt        (501) staff       (20)    10441 2023-12-09 19:41:04.000000 ds20kdb-avt-1.0.1/src/ds20kdb/wafer_location_gui.py
--rwxr-xr-x   0 avt        (501) staff       (20)    24651 2024-02-29 13:53:11.000000 ds20kdb-avt-1.0.1/src/ds20kdb/wafer_map_from_db.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-03-28 13:28:47.452340 ds20kdb-avt-1.0.1/src/ds20kdb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     6889 2024-03-28 13:28:47.000000 ds20kdb-avt-1.0.1/src/ds20kdb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      830 2024-03-28 13:28:47.000000 ds20kdb-avt-1.0.1/src/ds20kdb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2024-03-28 13:28:47.000000 ds20kdb-avt-1.0.1/src/ds20kdb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      868 2024-03-28 13:28:47.000000 ds20kdb-avt-1.0.1/src/ds20kdb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      111 2024-03-28 13:28:47.000000 ds20kdb-avt-1.0.1/src/ds20kdb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        8 2024-03-28 13:28:47.000000 ds20kdb-avt-1.0.1/src/ds20kdb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-03 17:30:49.346766 ds20kdb-avt-1.0.2/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.2/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-03 17:30:49.345959 ds20kdb-avt-1.0.2/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     5281 2023-10-13 14:30:24.000000 ds20kdb-avt-1.0.2/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.2/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2024-04-03 17:30:49.346975 ds20kdb-avt-1.0.2/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     3208 2024-04-03 17:30:23.000000 ds20kdb-avt-1.0.2/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-03 17:30:49.309522 ds20kdb-avt-1.0.2/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-03 17:30:49.338715 ds20kdb-avt-1.0.2/src/ds20kdb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.2/src/ds20kdb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)     9414 2023-09-17 11:41:52.000000 ds20kdb-avt-1.0.2/src/ds20kdb/auth.py
+-rw-r--r--   0 avt        (501) staff       (20)    38424 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.2/src/ds20kdb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)      182 2023-04-01 13:34:13.000000 ds20kdb-avt-1.0.2/src/ds20kdb/constants.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     2123 2023-02-09 15:44:46.000000 ds20kdb-avt-1.0.2/src/ds20kdb/create_credentials_file.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33510 2024-04-03 17:21:01.000000 ds20kdb-avt-1.0.2/src/ds20kdb/gen_tray_files_gui.py
+-rw-r--r--   0 avt        (501) staff       (20)    93422 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.2/src/ds20kdb/interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     6936 2023-09-06 15:42:42.000000 ds20kdb-avt-1.0.2/src/ds20kdb/qr.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7876 2023-09-09 12:18:43.000000 ds20kdb-avt-1.0.2/src/ds20kdb/qrgen.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    32509 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.2/src/ds20kdb/scanner_auto.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   117866 2024-03-28 13:27:09.000000 ds20kdb-avt-1.0.2/src/ds20kdb/submit_vtile.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    22398 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.2/src/ds20kdb/submit_vtile_json.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    11674 2024-02-29 13:53:11.000000 ds20kdb-avt-1.0.2/src/ds20kdb/veto_location.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    19987 2024-03-21 17:12:00.000000 ds20kdb-avt-1.0.2/src/ds20kdb/veto_location_gui.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14551 2024-01-10 17:21:38.000000 ds20kdb-avt-1.0.2/src/ds20kdb/visual.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     8909 2023-09-17 11:55:13.000000 ds20kdb-avt-1.0.2/src/ds20kdb/vtile_test_submit_cr.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     8222 2024-03-31 13:35:23.000000 ds20kdb-avt-1.0.2/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py
+-rwx------   0 avt        (501) staff       (20)    10441 2023-12-09 19:41:04.000000 ds20kdb-avt-1.0.2/src/ds20kdb/wafer_location_gui.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    24651 2024-02-29 13:53:11.000000 ds20kdb-avt-1.0.2/src/ds20kdb/wafer_map_from_db.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-03 17:30:49.345085 ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-03 17:30:49.000000 ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      830 2024-04-03 17:30:49.000000 ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2024-04-03 17:30:49.000000 ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      868 2024-04-03 17:30:49.000000 ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      111 2024-04-03 17:30:49.000000 ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        8 2024-04-03 17:30:49.000000 ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/top_level.txt
```

### Comparing `ds20kdb-avt-1.0.1/PKG-INFO` & `ds20kdb-avt-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds20kdb-avt
-Version: 1.0.1
+Version: 1.0.2
 Summary: A cross-platform Python interface to the DarkSide-20k production database
 Home-page: https://gitlab.in2p3.fr/darkside/productiondb_software/
 Author: Alan Taylor, Paolo Franchini, Seraphim Koulosousas
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ds20kdb-avt-1.0.1/README.md` & `ds20kdb-avt-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/setup.py` & `ds20kdb-avt-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ds20kdb-avt",
-    version="1.0.1",
+    version="1.0.2",
     author="Alan Taylor, Paolo Franchini, Seraphim Koulosousas",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="A cross-platform Python interface to the DarkSide-20k production database",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/auth.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/auth.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/common.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/common.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/create_credentials_file.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/create_credentials_file.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/gen_tray_files_gui.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/gen_tray_files_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -739,16 +739,16 @@
         existing_yellow = common.evaluate_tray_files(self.filenames[Tab.YELLOW])
 
         ##########################################################################
         # fill existing tray files with SiPMs
         ##########################################################################
 
         tasks = [
-            ('GREEN', existing_green, list(wafer_map_green)),
-            ('YELLOW', existing_yellow, list(wafer_map_yellow)),
+            ('GREEN', existing_green, wafer_map_green),
+            ('YELLOW', existing_yellow, wafer_map_yellow),
         ]
 
         if any([existing_green, existing_yellow]):
             self.print_to_console(
                 f'\n{"#" * 58}\n# Filling existing files\n{"#" * 58}'
             )
         else:
```

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/interface.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/interface.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/qr.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/qr.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/qrgen.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/qrgen.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/scanner_auto.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/scanner_auto.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/submit_vtile.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/submit_vtile.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/submit_vtile_json.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/submit_vtile_json.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/veto_location.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/veto_location.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/veto_location_gui.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/veto_location_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/visual.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/visual.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/vtile_test_submit_cr.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/vtile_test_submit_cr.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,18 +55,34 @@
 
     args = parser.parse_args()
 
     return args
 
 
 ##############################################################################
-# main
+# utilities
 ##############################################################################
 
 
+def col(group_num, num_groups, invert=False):
+    """
+    Set single-byte grey between 63 and 255 (so we can always see the
+    black frequency value text)
+    """
+    try:
+        grey = group_num * (256 // (num_groups - 1)) - 1
+    except ZeroDivisionError:
+        grey = 255
+
+    if invert:
+        grey = 255 - grey
+
+    return grey, grey, grey
+
+
 def value_to_vtile_id(value, qr_to_id):
     """
     Obtain the vTile ID for the supplied QR code or serial number. For the
     latter case we are assuming the serial numbers are for the VETO on behalf
     of the user.
 
     --------------------------------------------------------------------------
@@ -193,35 +209,37 @@
 
     dbi = interface.Database()
     vtile_ids = get_vtile_ids_from_values(dbi, args.qrcodes)
     sipm_ids = get_sipm_ids_from_vtile_ids(dbi, vtile_ids)
 
     count_grp = get_locations_from_sipm_ids(dbi, sipm_ids)
 
+    # remove SiPMs we don't care about
+    valid_locations = set(interface.wafer_map_valid_locations())
+    count_grp = {k: v for k, v in count_grp.items() if k in valid_locations}
+
     fgrp = collections.defaultdict(set)
     for loc, freq in count_grp.items():
         fgrp[freq].add(loc)
 
-    def col(group_num, num_groups):
-        grey = 64 + group_num * (192 // num_groups)
-        return grey, grey, grey
-
     num_groups = len(fgrp)
+    frequencies = sorted(fgrp)
 
+    # greyscale lookup table for frequency values
     clut = {
-        f: col(f, num_groups)
-        for f in range(1, len(fgrp) + 1)
+        f: col(i, num_groups)
+        for i, f in enumerate(frequencies)
     }
 
     sipm_groups = [
         {
             'name': str(frq),
             'locations': sipm_locations,
             'sipm_colour': clut[frq],
-            'text_colour': frq,
+            'text_colour': 'black' if clut[frq][0] > 96 else 'lightgray',
         }
         for frq, sipm_locations in fgrp.items()
     ]
 
     status = types.SimpleNamespace(success=0, unreserved_error_code=3)
 
     visual.DrawWafer(
```

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/wafer_location_gui.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/wafer_location_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb/wafer_map_from_db.py` & `ds20kdb-avt-1.0.2/src/ds20kdb/wafer_map_from_db.py`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb_avt.egg-info/PKG-INFO` & `ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds20kdb-avt
-Version: 1.0.1
+Version: 1.0.2
 Summary: A cross-platform Python interface to the DarkSide-20k production database
 Home-page: https://gitlab.in2p3.fr/darkside/productiondb_software/
 Author: Alan Taylor, Paolo Franchini, Seraphim Koulosousas
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb_avt.egg-info/SOURCES.txt` & `ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ds20kdb-avt-1.0.1/src/ds20kdb_avt.egg-info/entry_points.txt` & `ds20kdb-avt-1.0.2/src/ds20kdb_avt.egg-info/entry_points.txt`

 * *Files identical despite different names*

