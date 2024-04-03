# Comparing `tmp/neuronsmemorytestpipeline-0.0.8.tar.gz` & `tmp/neuronsmemorytestpipeline-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuronsmemorytestpipeline-0.0.8.tar", max compression
+gzip compressed data, was "neuronsmemorytestpipeline-0.0.9.tar", max compression
```

## Comparing `neuronsmemorytestpipeline-0.0.8.tar` & `neuronsmemorytestpipeline-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2024-03-18 10:43:12.257440 neuronsmemorytestpipeline-0.0.8/LICENSE
--rw-r--r--   0        0        0     1115 2024-03-19 13:13:11.252224 neuronsmemorytestpipeline-0.0.8/README.md
--rw-r--r--   0        0        0     1079 2024-03-21 10:02:07.723742 neuronsmemorytestpipeline-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    15955 2024-03-18 12:58:02.824909 neuronsmemorytestpipeline-0.0.8/src/neuronsmemorytestpipeline/FRT_metric.py
--rw-r--r--   0        0        0     5058 2024-03-21 10:02:05.037136 neuronsmemorytestpipeline-0.0.8/src/neuronsmemorytestpipeline/MRT_free_recall_metric.py
--rw-r--r--   0        0        0    15564 2024-03-20 10:29:23.298502 neuronsmemorytestpipeline-0.0.8/src/neuronsmemorytestpipeline/MRT_recognition_metric.py
--rw-r--r--   0        0        0     5713 2024-03-18 12:58:02.829954 neuronsmemorytestpipeline-0.0.8/src/neuronsmemorytestpipeline/MRT_text_processing.py
--rw-r--r--   0        0        0     3496 2024-03-18 12:58:02.833281 neuronsmemorytestpipeline-0.0.8/src/neuronsmemorytestpipeline/QA_modules.py
--rw-r--r--   0        0        0        0 2024-03-19 13:56:49.945585 neuronsmemorytestpipeline-0.0.8/src/neuronsmemorytestpipeline/__init__.py
--rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 neuronsmemorytestpipeline-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-03-18 10:43:12.257440 neuronsmemorytestpipeline-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1115 2024-03-19 13:13:11.252224 neuronsmemorytestpipeline-0.0.9/README.md
+-rw-r--r--   0        0        0      908 2024-03-22 12:35:51.567866 neuronsmemorytestpipeline-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    15955 2024-03-18 12:58:02.824909 neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/FRT_metric.py
+-rw-r--r--   0        0        0     5058 2024-03-21 10:02:05.037136 neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/MRT_free_recall_metric.py
+-rw-r--r--   0        0        0    15564 2024-03-20 10:29:23.298502 neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/MRT_recognition_metric.py
+-rw-r--r--   0        0        0     5713 2024-03-18 12:58:02.829954 neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/MRT_text_processing.py
+-rw-r--r--   0        0        0     3496 2024-03-18 12:58:02.833281 neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/QA_modules.py
+-rw-r--r--   0        0        0        0 2024-03-19 13:56:49.945585 neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/__init__.py
+-rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 neuronsmemorytestpipeline-0.0.9/PKG-INFO
```

### Comparing `neuronsmemorytestpipeline-0.0.8/LICENSE` & `neuronsmemorytestpipeline-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `neuronsmemorytestpipeline-0.0.8/README.md` & `neuronsmemorytestpipeline-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `neuronsmemorytestpipeline-0.0.8/pyproject.toml` & `neuronsmemorytestpipeline-0.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "NeuronsMemoryTestPipeline"
-version = "0.0.8"
+version = "0.0.9"
 description = "Package provides QA, MRT and FRT metrics calculation for frt and mrt scores."
 authors = [
     "Irina White <i.white@neuronsinc.com>",
     "Theo Sell <t.sell@neuronsinc.com>"
 ]
 license = "MIT"
 homepage = "https://gitlab.com/neurons-inc1/data-analyst/neurons_metrics_package"
@@ -20,23 +20,13 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fuzzywuzzy = "*"
-google_cloud_aiplatform = "*"
-matplotlib = "*"
 numpy = "*"
 pandas = "*"
-protobuf = "*"
-scikit_learn = "*"
-scipy = "*"
-seaborn = "*"
-setuptools = "*"
-torch = "*"
 tqdm = "*"
-transformers = "*"
-vertexai = "*"
 openpyxl = "*"
 python-Levenshtein = "*"
-ipywidgets = "*"
+ipywidgets = "*"
```

### Comparing `neuronsmemorytestpipeline-0.0.8/src/neuronsmemorytestpipeline/FRT_metric.py` & `neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/FRT_metric.py`

 * *Files identical despite different names*

### Comparing `neuronsmemorytestpipeline-0.0.8/src/neuronsmemorytestpipeline/MRT_free_recall_metric.py` & `neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/MRT_free_recall_metric.py`

 * *Files identical despite different names*

### Comparing `neuronsmemorytestpipeline-0.0.8/src/neuronsmemorytestpipeline/MRT_recognition_metric.py` & `neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/MRT_recognition_metric.py`

 * *Files identical despite different names*

### Comparing `neuronsmemorytestpipeline-0.0.8/src/neuronsmemorytestpipeline/MRT_text_processing.py` & `neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/MRT_text_processing.py`

 * *Files identical despite different names*

### Comparing `neuronsmemorytestpipeline-0.0.8/src/neuronsmemorytestpipeline/QA_modules.py` & `neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/QA_modules.py`

 * *Files identical despite different names*

