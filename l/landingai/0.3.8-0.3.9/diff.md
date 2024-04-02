# Comparing `tmp/landingai-0.3.8.tar.gz` & `tmp/landingai-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingai-0.3.8.tar", max compression
+gzip compressed data, was "landingai-0.3.9.tar", max compression
```

## Comparing `landingai-0.3.8.tar` & `landingai-0.3.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1063 2023-10-13 18:01:18.424689 landingai-0.3.8/LICENSE.md
--rw-r--r--   0        0        0     7604 2023-10-13 18:01:18.424689 landingai-0.3.8/README.md
--rw-r--r--   0        0        0      360 2023-10-13 18:01:18.456689 landingai-0.3.8/landingai/__init__.py
--rw-r--r--   0        0        0     7691 2023-10-13 18:01:18.456689 landingai-0.3.8/landingai/common.py
--rw-r--r--   0        0        0       72 2023-10-13 18:01:18.456689 landingai-0.3.8/landingai/data_management/__init__.py
--rw-r--r--   0        0        0     9255 2023-10-13 18:01:18.456689 landingai-0.3.8/landingai/data_management/client.py
--rw-r--r--   0        0        0     1707 2023-10-13 18:01:18.456689 landingai-0.3.8/landingai/data_management/label.py
--rw-r--r--   0        0        0    24122 2023-10-13 18:01:18.456689 landingai-0.3.8/landingai/data_management/media.py
--rw-r--r--   0        0        0     4192 2023-10-13 18:01:18.456689 landingai-0.3.8/landingai/data_management/metadata.py
--rw-r--r--   0        0        0     2745 2023-10-13 18:01:18.456689 landingai-0.3.8/landingai/data_management/utils.py
--rw-r--r--   0        0        0     9730 2023-10-13 18:01:18.456689 landingai-0.3.8/landingai/exceptions.py
--rw-r--r--   0        0        0  1594400 2023-10-13 18:01:18.464689 landingai-0.3.8/landingai/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     6035 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/image_source_ops.py
--rw-r--r--   0        0        0     2154 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/notebook_utils.py
--rw-r--r--   0        0        0      420 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/pipeline/__init__.py
--rw-r--r--   0        0        0    23757 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/pipeline/frameset.py
--rw-r--r--   0        0        0    16405 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/pipeline/image_source.py
--rw-r--r--   0        0        0     1339 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/pipeline/postprocessing.py
--rw-r--r--   0        0        0     8389 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/postprocess.py
--rw-r--r--   0        0        0    30300 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/predict.py
--rw-r--r--   0        0        0     6462 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/st_utils.py
--rw-r--r--   0        0        0       40 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/storage/__init__.py
--rw-r--r--   0        0        0     4439 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/storage/data_access.py
--rw-r--r--   0        0        0     4361 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/storage/snowflake.py
--rw-r--r--   0        0        0     1503 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/telemetry.py
--rw-r--r--   0        0        0     6129 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/timer.py
--rw-r--r--   0        0        0     1685 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/transform.py
--rw-r--r--   0        0        0     2985 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/utils.py
--rw-r--r--   0        0        0    13403 2023-10-13 18:01:18.468689 landingai-0.3.8/landingai/visualize.py
--rw-r--r--   0        0        0     2730 2023-10-13 18:01:19.200694 landingai-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 landingai-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-10-13 20:53:45.195024 landingai-0.3.9/LICENSE.md
+-rw-r--r--   0        0        0     7604 2023-10-13 20:53:45.195024 landingai-0.3.9/README.md
+-rw-r--r--   0        0        0      360 2023-10-13 20:53:45.231025 landingai-0.3.9/landingai/__init__.py
+-rw-r--r--   0        0        0     7691 2023-10-13 20:53:45.231025 landingai-0.3.9/landingai/common.py
+-rw-r--r--   0        0        0       72 2023-10-13 20:53:45.231025 landingai-0.3.9/landingai/data_management/__init__.py
+-rw-r--r--   0        0        0     9255 2023-10-13 20:53:45.231025 landingai-0.3.9/landingai/data_management/client.py
+-rw-r--r--   0        0        0     1707 2023-10-13 20:53:45.231025 landingai-0.3.9/landingai/data_management/label.py
+-rw-r--r--   0        0        0    24122 2023-10-13 20:53:45.231025 landingai-0.3.9/landingai/data_management/media.py
+-rw-r--r--   0        0        0     4192 2023-10-13 20:53:45.231025 landingai-0.3.9/landingai/data_management/metadata.py
+-rw-r--r--   0        0        0     2745 2023-10-13 20:53:45.231025 landingai-0.3.9/landingai/data_management/utils.py
+-rw-r--r--   0        0        0     9730 2023-10-13 20:53:45.231025 landingai-0.3.9/landingai/exceptions.py
+-rw-r--r--   0        0        0  1594400 2023-10-13 20:53:45.239025 landingai-0.3.9/landingai/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     6035 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/image_source_ops.py
+-rw-r--r--   0        0        0     2154 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/notebook_utils.py
+-rw-r--r--   0        0        0      420 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/pipeline/__init__.py
+-rw-r--r--   0        0        0    23757 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/pipeline/frameset.py
+-rw-r--r--   0        0        0    16405 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/pipeline/image_source.py
+-rw-r--r--   0        0        0     1339 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/pipeline/postprocessing.py
+-rw-r--r--   0        0        0     8389 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/postprocess.py
+-rw-r--r--   0        0        0    30300 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/predict.py
+-rw-r--r--   0        0        0     6462 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/st_utils.py
+-rw-r--r--   0        0        0       40 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/storage/__init__.py
+-rw-r--r--   0        0        0     4439 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/storage/data_access.py
+-rw-r--r--   0        0        0     4361 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/storage/snowflake.py
+-rw-r--r--   0        0        0     1503 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/telemetry.py
+-rw-r--r--   0        0        0     6129 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/timer.py
+-rw-r--r--   0        0        0     1685 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/transform.py
+-rw-r--r--   0        0        0     2985 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/utils.py
+-rw-r--r--   0        0        0    13403 2023-10-13 20:53:45.243025 landingai-0.3.9/landingai/visualize.py
+-rw-r--r--   0        0        0     2730 2023-10-13 20:53:45.963043 landingai-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 landingai-0.3.9/PKG-INFO
```

### Comparing `landingai-0.3.8/LICENSE.md` & `landingai-0.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/README.md` & `landingai-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/common.py` & `landingai-0.3.9/landingai/common.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/data_management/client.py` & `landingai-0.3.9/landingai/data_management/client.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/data_management/label.py` & `landingai-0.3.9/landingai/data_management/label.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/data_management/media.py` & `landingai-0.3.9/landingai/data_management/media.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/data_management/metadata.py` & `landingai-0.3.9/landingai/data_management/metadata.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/data_management/utils.py` & `landingai-0.3.9/landingai/data_management/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/exceptions.py` & `landingai-0.3.9/landingai/exceptions.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/fonts/default_font_ch_en.ttf` & `landingai-0.3.9/landingai/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/image_source_ops.py` & `landingai-0.3.9/landingai/image_source_ops.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/notebook_utils.py` & `landingai-0.3.9/landingai/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/pipeline/frameset.py` & `landingai-0.3.9/landingai/pipeline/frameset.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/pipeline/image_source.py` & `landingai-0.3.9/landingai/pipeline/image_source.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/pipeline/postprocessing.py` & `landingai-0.3.9/landingai/pipeline/postprocessing.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/postprocess.py` & `landingai-0.3.9/landingai/postprocess.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/predict.py` & `landingai-0.3.9/landingai/predict.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/st_utils.py` & `landingai-0.3.9/landingai/st_utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/storage/data_access.py` & `landingai-0.3.9/landingai/storage/data_access.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/storage/snowflake.py` & `landingai-0.3.9/landingai/storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/telemetry.py` & `landingai-0.3.9/landingai/telemetry.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/timer.py` & `landingai-0.3.9/landingai/timer.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/transform.py` & `landingai-0.3.9/landingai/transform.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/utils.py` & `landingai-0.3.9/landingai/utils.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/landingai/visualize.py` & `landingai-0.3.9/landingai/visualize.py`

 * *Files identical despite different names*

### Comparing `landingai-0.3.8/pyproject.toml` & `landingai-0.3.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "landingai"
-version = "0.3.8"
+version = "0.3.9"
 description = "Helper library for interacting with Landing AI LandingLens"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "landingai"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `landingai-0.3.8/PKG-INFO` & `landingai-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingai
-Version: 0.3.8
+Version: 0.3.9
 Summary: Helper library for interacting with Landing AI LandingLens
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

