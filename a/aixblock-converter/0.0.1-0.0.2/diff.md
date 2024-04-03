# Comparing `tmp/aixblock_converter-0.0.1.tar.gz` & `tmp/aixblock_converter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixblock_converter-0.0.1.tar", max compression
+gzip compressed data, was "aixblock_converter-0.0.2.tar", max compression
```

## Comparing `aixblock_converter-0.0.1.tar` & `aixblock_converter-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       17 2024-04-03 06:21:01.079312 aixblock_converter-0.0.1/README.md
--rw-r--r--   0        0        0      198 2023-11-30 02:34:31.438792 aixblock_converter-0.0.1/aixblock_converter/__init__.py
--rw-r--r--   0        0        0     1907 2023-11-30 02:34:31.439468 aixblock_converter-0.0.1/aixblock_converter/audio.py
--rw-r--r--   0        0        0    13291 2023-11-30 02:34:31.440209 aixblock_converter-0.0.1/aixblock_converter/brush.py
--rw-r--r--   0        0        0     3847 2024-04-03 06:07:37.220486 aixblock_converter-0.0.1/aixblock_converter/cli.py
--rw-r--r--   0        0        0    57486 2024-04-03 06:07:40.400484 aixblock_converter-0.0.1/aixblock_converter/converter.py
--rw-r--r--   0        0        0        0 2023-11-30 02:34:31.442573 aixblock_converter-0.0.1/aixblock_converter/exports/__init__.py
--rw-r--r--   0        0        0     2865 2023-11-30 02:34:31.442951 aixblock_converter-0.0.1/aixblock_converter/exports/csv.py
--rw-r--r--   0        0        0     2548 2023-11-30 02:34:31.443278 aixblock_converter-0.0.1/aixblock_converter/funsd.py
--rw-r--r--   0        0        0        0 2023-11-30 02:34:31.443459 aixblock_converter-0.0.1/aixblock_converter/imports/__init__.py
--rw-r--r--   0        0        0    10191 2024-04-03 06:07:37.261216 aixblock_converter-0.0.1/aixblock_converter/imports/coco.py
--rw-r--r--   0        0        0     3827 2023-11-30 02:34:31.444747 aixblock_converter-0.0.1/aixblock_converter/imports/colors.py
--rw-r--r--   0        0        0     1210 2024-04-03 06:07:37.220106 aixblock_converter-0.0.1/aixblock_converter/imports/label_config.py
--rw-r--r--   0        0        0     8096 2023-11-30 02:34:31.445632 aixblock_converter-0.0.1/aixblock_converter/imports/pathtrack.py
--rw-r--r--   0        0        0     7985 2024-04-03 06:07:37.220435 aixblock_converter-0.0.1/aixblock_converter/imports/yolo.py
--rw-r--r--   0        0        0     5806 2024-04-03 06:07:37.220073 aixblock_converter-0.0.1/aixblock_converter/main.py
--rw-r--r--   0        0        0    11773 2023-11-30 02:34:31.446922 aixblock_converter-0.0.1/aixblock_converter/utils.py
--rw-r--r--   0        0        0      270 2024-04-03 06:25:13.442171 aixblock_converter-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 aixblock_converter-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-03 06:21:01.079312 aixblock_converter-0.0.2/README.md
+-rw-r--r--   0        0        0      197 2024-04-03 07:16:04.496166 aixblock_converter-0.0.2/aixblock_converter/__init__.py
+-rw-r--r--   0        0        0     1907 2023-11-30 02:34:31.439468 aixblock_converter-0.0.2/aixblock_converter/audio.py
+-rw-r--r--   0        0        0    13291 2023-11-30 02:34:31.440209 aixblock_converter-0.0.2/aixblock_converter/brush.py
+-rw-r--r--   0        0        0     3847 2024-04-03 06:07:37.220486 aixblock_converter-0.0.2/aixblock_converter/cli.py
+-rw-r--r--   0        0        0    57486 2024-04-03 06:07:40.400484 aixblock_converter-0.0.2/aixblock_converter/converter.py
+-rw-r--r--   0        0        0        0 2023-11-30 02:34:31.442573 aixblock_converter-0.0.2/aixblock_converter/exports/__init__.py
+-rw-r--r--   0        0        0     2865 2023-11-30 02:34:31.442951 aixblock_converter-0.0.2/aixblock_converter/exports/csv.py
+-rw-r--r--   0        0        0     2548 2023-11-30 02:34:31.443278 aixblock_converter-0.0.2/aixblock_converter/funsd.py
+-rw-r--r--   0        0        0        0 2023-11-30 02:34:31.443459 aixblock_converter-0.0.2/aixblock_converter/imports/__init__.py
+-rw-r--r--   0        0        0    10191 2024-04-03 06:07:37.261216 aixblock_converter-0.0.2/aixblock_converter/imports/coco.py
+-rw-r--r--   0        0        0     3827 2023-11-30 02:34:31.444747 aixblock_converter-0.0.2/aixblock_converter/imports/colors.py
+-rw-r--r--   0        0        0     1210 2024-04-03 06:07:37.220106 aixblock_converter-0.0.2/aixblock_converter/imports/label_config.py
+-rw-r--r--   0        0        0     8096 2023-11-30 02:34:31.445632 aixblock_converter-0.0.2/aixblock_converter/imports/pathtrack.py
+-rw-r--r--   0        0        0     7985 2024-04-03 06:07:37.220435 aixblock_converter-0.0.2/aixblock_converter/imports/yolo.py
+-rw-r--r--   0        0        0     5806 2024-04-03 06:07:37.220073 aixblock_converter-0.0.2/aixblock_converter/main.py
+-rw-r--r--   0        0        0    11769 2024-04-03 07:24:29.986007 aixblock_converter-0.0.2/aixblock_converter/utils.py
+-rw-r--r--   0        0        0      270 2024-04-03 07:24:48.289359 aixblock_converter-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 aixblock_converter-0.0.2/PKG-INFO
```

### Comparing `aixblock_converter-0.0.1/aixblock_converter/audio.py` & `aixblock_converter-0.0.2/aixblock_converter/audio.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.1/aixblock_converter/brush.py` & `aixblock_converter-0.0.2/aixblock_converter/brush.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.1/aixblock_converter/cli.py` & `aixblock_converter-0.0.2/aixblock_converter/cli.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.1/aixblock_converter/converter.py` & `aixblock_converter-0.0.2/aixblock_converter/converter.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.1/aixblock_converter/exports/csv.py` & `aixblock_converter-0.0.2/aixblock_converter/exports/csv.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.1/aixblock_converter/funsd.py` & `aixblock_converter-0.0.2/aixblock_converter/funsd.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.1/aixblock_converter/imports/coco.py` & `aixblock_converter-0.0.2/aixblock_converter/imports/coco.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.1/aixblock_converter/imports/colors.py` & `aixblock_converter-0.0.2/aixblock_converter/imports/colors.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.1/aixblock_converter/imports/label_config.py` & `aixblock_converter-0.0.2/aixblock_converter/imports/label_config.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.1/aixblock_converter/imports/pathtrack.py` & `aixblock_converter-0.0.2/aixblock_converter/imports/pathtrack.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.1/aixblock_converter/imports/yolo.py` & `aixblock_converter-0.0.2/aixblock_converter/imports/yolo.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.1/aixblock_converter/main.py` & `aixblock_converter-0.0.2/aixblock_converter/main.py`

 * *Files identical despite different names*

### Comparing `aixblock_converter-0.0.1/aixblock_converter/utils.py` & `aixblock_converter-0.0.2/aixblock_converter/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from operator import itemgetter
 from PIL import Image
 from urllib.parse import urlparse
 from nltk.tokenize.treebank import TreebankWordTokenizer
 from lxml import etree
 from collections import defaultdict
-from label_studio_tools.core.utils.params import get_env
+from aixblock_tools.core.utils.params import get_env
 
 logger = logging.getLogger(__name__)
 
 _LABEL_TAGS = {'Label', 'Choice'}
 _NOT_CONTROL_TAGS = {
     'Filter',
 }
```

