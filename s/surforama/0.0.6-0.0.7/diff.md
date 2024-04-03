# Comparing `tmp/surforama-0.0.6.tar.gz` & `tmp/surforama-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surforama-0.0.6.tar", last modified: Sun Mar 31 15:27:23 2024, max compression
+gzip compressed data, was "surforama-0.0.7.tar", last modified: Wed Apr  3 05:57:14 2024, max compression
```

## Comparing `surforama-0.0.6.tar` & `surforama-0.0.7.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:23.647340 surforama-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:23.635340 surforama-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:23.643340 surforama-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-03-31 15:27:12.000000 surforama-0.0.6/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-31 15:27:12.000000 surforama-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-31 15:27:12.000000 surforama-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-31 15:27:12.000000 surforama-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-31 15:27:12.000000 surforama-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-03-31 15:27:23.647340 surforama-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-31 15:27:12.000000 surforama-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:23.643340 surforama-0.0.6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   112422 2024-03-31 15:27:12.000000 surforama-0.0.6/examples/example_usecase_stats.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-31 15:27:12.000000 surforama-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-31 15:27:23.647340 surforama-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:23.635340 surforama-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:23.643340 surforama-0.0.6/src/surforama/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:23.643340 surforama-0.0.6/src/surforama/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/_tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-31 15:27:23.000000 surforama-0.0.6/src/surforama/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    17585 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:23.643340 surforama-0.0.6/src/surforama/data/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/data/_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:23.647340 surforama-0.0.6/src/surforama/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/gui/qt_mesh_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/gui/qt_point_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:23.647340 surforama-0.0.6/src/surforama/io/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/io/_reader_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:23.647340 surforama-0.0.6/src/surforama/io/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/io/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/io/_tests/test_star.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/io/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/io/star.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:23.647340 surforama-0.0.6/src/surforama/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/utils/napari.py
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-03-31 15:27:12.000000 surforama-0.0.6/src/surforama/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 15:27:23.647340 surforama-0.0.6/src/surforama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-03-31 15:27:23.000000 surforama-0.0.6/src/surforama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-31 15:27:23.000000 surforama-0.0.6/src/surforama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 15:27:23.000000 surforama-0.0.6/src/surforama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-31 15:27:23.000000 surforama-0.0.6/src/surforama.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-31 15:27:23.000000 surforama-0.0.6/src/surforama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-31 15:27:23.000000 surforama-0.0.6/src/surforama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)  2606156 2024-03-31 15:27:12.000000 surforama-0.0.6/surforama_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-31 15:27:12.000000 surforama-0.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.406288 surforama-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.394288 surforama-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.398288 surforama-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-03 05:57:03.000000 surforama-0.0.7/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-03 05:57:03.000000 surforama-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-03 05:57:03.000000 surforama-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 05:57:03.000000 surforama-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 05:57:03.000000 surforama-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-03 05:57:14.406288 surforama-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-03 05:57:03.000000 surforama-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.398288 surforama-0.0.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   112422 2024-04-03 05:57:03.000000 surforama-0.0.7/examples/example_usecase_stats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-03 05:57:03.000000 surforama-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-03 05:57:14.406288 surforama-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.394288 surforama-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.398288 surforama-0.0.7/src/surforama/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.402288 surforama-0.0.7/src/surforama/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/_tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 05:57:14.000000 surforama-0.0.7/src/surforama/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.402288 surforama-0.0.7/src/surforama/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/data/_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.402288 surforama-0.0.7/src/surforama/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/gui/qt_mesh_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/gui/qt_point_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/gui/qt_surface_picker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.402288 surforama-0.0.7/src/surforama/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/io/_reader_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.402288 surforama-0.0.7/src/surforama/io/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/io/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/io/_tests/test_star.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/io/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/io/star.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.402288 surforama-0.0.7/src/surforama/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/utils/napari.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-04-03 05:57:03.000000 surforama-0.0.7/src/surforama/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:57:14.402288 surforama-0.0.7/src/surforama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-03 05:57:14.000000 surforama-0.0.7/src/surforama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-03 05:57:14.000000 surforama-0.0.7/src/surforama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:57:14.000000 surforama-0.0.7/src/surforama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 05:57:14.000000 surforama-0.0.7/src/surforama.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 05:57:14.000000 surforama-0.0.7/src/surforama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 05:57:14.000000 surforama-0.0.7/src/surforama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  2606156 2024-04-03 05:57:03.000000 surforama-0.0.7/surforama_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-03 05:57:03.000000 surforama-0.0.7/tox.ini
```

### Comparing `surforama-0.0.6/.github/workflows/test_and_deploy.yml` & `surforama-0.0.7/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/.gitignore` & `surforama-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/.pre-commit-config.yaml` & `surforama-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/LICENSE` & `surforama-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/PKG-INFO` & `surforama-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surforama
-Version: 0.0.6
+Version: 0.0.7
 Summary: a tool for using surfaces to explore volumetric data in napari
 Home-page: https://github.com/cellcanvas/surforama
 Author: Kyle Harrington
 Author-email: surforama@kyleharrington.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cellcanvas/surforama/issues
 Project-URL: Documentation, https://github.com/cellcanvas/surforama#README.md
```

### Comparing `surforama-0.0.6/README.md` & `surforama-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/examples/example_usecase_stats.ipynb` & `surforama-0.0.7/examples/example_usecase_stats.ipynb`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/pyproject.toml` & `surforama-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/setup.cfg` & `surforama-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/src/surforama/_cli.py` & `surforama-0.0.7/src/surforama/_cli.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/src/surforama/_tests/test_geometry.py` & `surforama-0.0.7/src/surforama/_tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/src/surforama/_tests/test_widget.py` & `surforama-0.0.7/src/surforama/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/src/surforama/data/_datasets.py` & `surforama-0.0.7/src/surforama/data/_datasets.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/src/surforama/gui/qt_mesh_generator.py` & `surforama-0.0.7/src/surforama/gui/qt_mesh_generator.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/src/surforama/gui/qt_point_io.py` & `surforama-0.0.7/src/surforama/gui/qt_point_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import TYPE_CHECKING, Optional
 
 from magicgui import magicgui
 from napari.utils.notifications import show_warning
 from qtpy.QtWidgets import QGroupBox, QTabWidget, QVBoxLayout, QWidget
 
 if TYPE_CHECKING:
-    from surforama.app import QtSurfacePicker
+    from surforama.gui.qt_surface_picker import QtSurfacePicker
 from surforama.io.star import (
     load_points_layer_data_from_star_file,
     oriented_points_to_star_file,
 )
 from surforama.utils.napari import vectors_data_from_points_data
```

### Comparing `surforama-0.0.6/src/surforama/io/_reader_plugin.py` & `surforama-0.0.7/src/surforama/io/_reader_plugin.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/src/surforama/io/_tests/test_star.py` & `surforama-0.0.7/src/surforama/io/_tests/test_star.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/src/surforama/io/mesh.py` & `surforama-0.0.7/src/surforama/io/mesh.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/src/surforama/io/star.py` & `surforama-0.0.7/src/surforama/io/star.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/src/surforama/napari.yaml` & `surforama-0.0.7/src/surforama/napari.yaml`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/src/surforama/utils/geometry.py` & `surforama-0.0.7/src/surforama/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/src/surforama/utils/napari.py` & `surforama-0.0.7/src/surforama/utils/napari.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/src/surforama/utils/stats.py` & `surforama-0.0.7/src/surforama/utils/stats.py`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/src/surforama.egg-info/PKG-INFO` & `surforama-0.0.7/src/surforama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surforama
-Version: 0.0.6
+Version: 0.0.7
 Summary: a tool for using surfaces to explore volumetric data in napari
 Home-page: https://github.com/cellcanvas/surforama
 Author: Kyle Harrington
 Author-email: surforama@kyleharrington.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cellcanvas/surforama/issues
 Project-URL: Documentation, https://github.com/cellcanvas/surforama#README.md
```

### Comparing `surforama-0.0.6/src/surforama.egg-info/SOURCES.txt` & `surforama-0.0.7/src/surforama.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 src/surforama/_tests/test_geometry.py
 src/surforama/_tests/test_widget.py
 src/surforama/data/__init__.py
 src/surforama/data/_datasets.py
 src/surforama/gui/__init__.py
 src/surforama/gui/qt_mesh_generator.py
 src/surforama/gui/qt_point_io.py
+src/surforama/gui/qt_surface_picker.py
 src/surforama/io/__init__.py
 src/surforama/io/_reader_plugin.py
 src/surforama/io/mesh.py
 src/surforama/io/star.py
 src/surforama/io/_tests/__init__.py
 src/surforama/io/_tests/test_star.py
 src/surforama/utils/__init__.py
```

### Comparing `surforama-0.0.6/surforama_screenshot.png` & `surforama-0.0.7/surforama_screenshot.png`

 * *Files identical despite different names*

### Comparing `surforama-0.0.6/tox.ini` & `surforama-0.0.7/tox.ini`

 * *Files identical despite different names*

