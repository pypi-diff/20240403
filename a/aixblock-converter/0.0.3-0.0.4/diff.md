# Comparing `tmp/aixblock_converter-0.0.3.tar.gz` & `tmp/aixblock_converter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixblock_converter-0.0.3.tar", max compression
+gzip compressed data, was "aixblock_converter-0.0.4.tar", max compression
```

## Comparing `aixblock_converter-0.0.3.tar` & `aixblock_converter-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       17 2024-04-03 06:21:01.079312 aixblock_converter-0.0.3/README.md
--rw-r--r--   0        0        0      197 2024-04-03 07:16:04.496166 aixblock_converter-0.0.3/aixblock_converter/__init__.py
--rw-r--r--   0        0        0     1907 2023-11-30 02:34:31.439468 aixblock_converter-0.0.3/aixblock_converter/audio.py
--rw-r--r--   0        0        0    13291 2023-11-30 02:34:31.440209 aixblock_converter-0.0.3/aixblock_converter/brush.py
--rw-r--r--   0        0        0     3829 2024-04-03 07:46:25.567052 aixblock_converter-0.0.3/aixblock_converter/cli.py
--rw-r--r--   0        0        0    57486 2024-04-03 06:07:40.400484 aixblock_converter-0.0.3/aixblock_converter/converter.py
--rw-r--r--   0        0        0        0 2023-11-30 02:34:31.442573 aixblock_converter-0.0.3/aixblock_converter/exports/__init__.py
--rw-r--r--   0        0        0     2865 2023-11-30 02:34:31.442951 aixblock_converter-0.0.3/aixblock_converter/exports/csv.py
--rw-r--r--   0        0        0     2548 2023-11-30 02:34:31.443278 aixblock_converter-0.0.3/aixblock_converter/funsd.py
--rw-r--r--   0        0        0        0 2023-11-30 02:34:31.443459 aixblock_converter-0.0.3/aixblock_converter/imports/__init__.py
--rw-r--r--   0        0        0    10191 2024-04-03 06:07:37.261216 aixblock_converter-0.0.3/aixblock_converter/imports/coco.py
--rw-r--r--   0        0        0     3827 2023-11-30 02:34:31.444747 aixblock_converter-0.0.3/aixblock_converter/imports/colors.py
--rw-r--r--   0        0        0     1210 2024-04-03 06:07:37.220106 aixblock_converter-0.0.3/aixblock_converter/imports/label_config.py
--rw-r--r--   0        0        0     8096 2023-11-30 02:34:31.445632 aixblock_converter-0.0.3/aixblock_converter/imports/pathtrack.py
--rw-r--r--   0        0        0     7985 2024-04-03 06:07:37.220435 aixblock_converter-0.0.3/aixblock_converter/imports/yolo.py
--rw-r--r--   0        0        0     5734 2024-04-03 07:46:53.775888 aixblock_converter-0.0.3/aixblock_converter/main.py
--rw-r--r--   0        0        0    11769 2024-04-03 07:47:01.646870 aixblock_converter-0.0.3/aixblock_converter/utils.py
--rw-r--r--   0        0        0      270 2024-04-03 07:47:53.302377 aixblock_converter-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 aixblock_converter-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-03 06:21:01.079312 aixblock_converter-0.0.4/README.md
+-rw-r--r--   0        0        0      232 2024-04-03 08:01:32.692474 aixblock_converter-0.0.4/aixblock_converter/__init__.py
+-rw-r--r--   0        0        0     1907 2023-11-30 02:34:31.439468 aixblock_converter-0.0.4/aixblock_converter/audio.py
+-rw-r--r--   0        0        0    13291 2023-11-30 02:34:31.440209 aixblock_converter-0.0.4/aixblock_converter/brush.py
+-rw-r--r--   0        0        0     3829 2024-04-03 07:46:25.567052 aixblock_converter-0.0.4/aixblock_converter/cli.py
+-rw-r--r--   0        0        0    57486 2024-04-03 06:07:40.400484 aixblock_converter-0.0.4/aixblock_converter/converter.py
+-rw-r--r--   0        0        0        0 2023-11-30 02:34:31.442573 aixblock_converter-0.0.4/aixblock_converter/exports/__init__.py
+-rw-r--r--   0        0        0     2865 2023-11-30 02:34:31.442951 aixblock_converter-0.0.4/aixblock_converter/exports/csv.py
+-rw-r--r--   0        0        0     2548 2023-11-30 02:34:31.443278 aixblock_converter-0.0.4/aixblock_converter/funsd.py
+-rw-r--r--   0        0        0        0 2023-11-30 02:34:31.443459 aixblock_converter-0.0.4/aixblock_converter/imports/__init__.py
+-rw-r--r--   0        0        0    10191 2024-04-03 06:07:37.261216 aixblock_converter-0.0.4/aixblock_converter/imports/coco.py
+-rw-r--r--   0        0        0     3827 2023-11-30 02:34:31.444747 aixblock_converter-0.0.4/aixblock_converter/imports/colors.py
+-rw-r--r--   0        0        0     1210 2024-04-03 06:07:37.220106 aixblock_converter-0.0.4/aixblock_converter/imports/label_config.py
+-rw-r--r--   0        0        0     8096 2023-11-30 02:34:31.445632 aixblock_converter-0.0.4/aixblock_converter/imports/pathtrack.py
+-rw-r--r--   0        0        0     7985 2024-04-03 06:07:37.220435 aixblock_converter-0.0.4/aixblock_converter/imports/yolo.py
+-rw-r--r--   0        0        0     5734 2024-04-03 07:46:53.775888 aixblock_converter-0.0.4/aixblock_converter/main.py
+-rw-r--r--   0        0        0    11769 2024-04-03 07:47:01.646870 aixblock_converter-0.0.4/aixblock_converter/utils.py
+-rw-r--r--   0        0        0      270 2024-04-03 08:01:48.101795 aixblock_converter-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 aixblock_converter-0.0.4/PKG-INFO
```

### Comparing `aixblock_converter-0.0.3/aixblock_converter/audio.py` & `aixblock_converter-0.0.4/aixblock_converter/audio.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.3/aixblock_converter/brush.py` & `aixblock_converter-0.0.4/aixblock_converter/brush.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.3/aixblock_converter/cli.py` & `aixblock_converter-0.0.4/aixblock_converter/cli.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.3/aixblock_converter/converter.py` & `aixblock_converter-0.0.4/aixblock_converter/converter.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.3/aixblock_converter/exports/csv.py` & `aixblock_converter-0.0.4/aixblock_converter/exports/csv.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.3/aixblock_converter/funsd.py` & `aixblock_converter-0.0.4/aixblock_converter/funsd.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.3/aixblock_converter/imports/coco.py` & `aixblock_converter-0.0.4/aixblock_converter/imports/coco.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.3/aixblock_converter/imports/colors.py` & `aixblock_converter-0.0.4/aixblock_converter/imports/colors.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.3/aixblock_converter/imports/label_config.py` & `aixblock_converter-0.0.4/aixblock_converter/imports/label_config.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.3/aixblock_converter/imports/pathtrack.py` & `aixblock_converter-0.0.4/aixblock_converter/imports/pathtrack.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.3/aixblock_converter/imports/yolo.py` & `aixblock_converter-0.0.4/aixblock_converter/imports/yolo.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.3/aixblock_converter/main.py` & `aixblock_converter-0.0.4/aixblock_converter/main.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.3/aixblock_converter/utils.py` & `aixblock_converter-0.0.4/aixblock_converter/utils.py`

 * *Files identical despite different names*

