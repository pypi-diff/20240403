# Comparing `tmp/napari-ehooke-0.0.5.tar.gz` & `tmp/napari-ehooke-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-ehooke-0.0.5.tar", last modified: Tue Mar 14 13:04:53 2023, max compression
+gzip compressed data, was "napari-ehooke-0.0.6.tar", last modified: Wed Apr  3 09:58:28 2024, max compression
```

## Comparing `napari-ehooke-0.0.5.tar` & `napari-ehooke-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 13:04:53.299376 napari-ehooke-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-03-14 13:04:53.299376 napari-ehooke-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-03-14 13:04:53.299376 napari-ehooke-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 13:04:53.295376 napari-ehooke-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 13:04:53.299376 napari-ehooke-0.0.5/src/napari_ehooke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/_computecells.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/_computefeatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/_computemask.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 13:04:53.299376 napari-ehooke-0.0.5/src/napari_ehooke/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/_tests/test_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 13:04:53.299376 napari-ehooke-0.0.5/src/napari_ehooke/ehooke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/ehooke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/ehooke/cellaverager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/ehooke/cellcycleclassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/ehooke/cellprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    27588 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/ehooke/cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/ehooke/colocmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/ehooke/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/ehooke/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-14 13:04:37.000000 napari-ehooke-0.0.5/src/napari_ehooke/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 13:04:53.299376 napari-ehooke-0.0.5/src/napari_ehooke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-03-14 13:04:53.000000 napari-ehooke-0.0.5/src/napari_ehooke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-14 13:04:53.000000 napari-ehooke-0.0.5/src/napari_ehooke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 13:04:53.000000 napari-ehooke-0.0.5/src/napari_ehooke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-14 13:04:53.000000 napari-ehooke-0.0.5/src/napari_ehooke.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-14 13:04:53.000000 napari-ehooke-0.0.5/src/napari_ehooke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-14 13:04:53.000000 napari-ehooke-0.0.5/src/napari_ehooke.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:58:28.252734 napari-ehooke-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-03 09:58:28.252734 napari-ehooke-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-03 09:58:28.252734 napari-ehooke-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:58:28.248734 napari-ehooke-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:58:28.248734 napari-ehooke-0.0.6/src/napari_ehooke/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/_computecells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/_computefeatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/_computemask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/_filtercells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:58:28.248734 napari-ehooke-0.0.6/src/napari_ehooke/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/_tests/test_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:58:28.252734 napari-ehooke-0.0.6/src/napari_ehooke/ehooke/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/ehooke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/ehooke/cellaverager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/ehooke/cellcycleclassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/ehooke/cellprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29768 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/ehooke/cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/ehooke/colocmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/ehooke/mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/ehooke/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/ehooke/segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-03 09:58:16.000000 napari-ehooke-0.0.6/src/napari_ehooke/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:58:28.252734 napari-ehooke-0.0.6/src/napari_ehooke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-03 09:58:28.000000 napari-ehooke-0.0.6/src/napari_ehooke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-03 09:58:28.000000 napari-ehooke-0.0.6/src/napari_ehooke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:58:28.000000 napari-ehooke-0.0.6/src/napari_ehooke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 09:58:28.000000 napari-ehooke-0.0.6/src/napari_ehooke.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 09:58:28.000000 napari-ehooke-0.0.6/src/napari_ehooke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 09:58:28.000000 napari-ehooke-0.0.6/src/napari_ehooke.egg-info/top_level.txt
```

### Comparing `napari-ehooke-0.0.5/LICENSE` & `napari-ehooke-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-ehooke-0.0.5/PKG-INFO` & `napari-ehooke-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-ehooke
-Version: 0.0.5
+Version: 0.0.6
 Summary: eHooke implementation within napari
 Home-page: https://github.com/antmsbrito/napari-ehooke
 Author: António Brito
 Author-email: antmsbrito95@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/antmsbrito/napari-ehooke/issues
 Project-URL: Documentation, https://github.com/antmsbrito/napari-ehooke#README.md
@@ -20,16 +20,31 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: magicgui
+Requires-Dist: qtpy
+Requires-Dist: napari[all]
+Requires-Dist: tensorflow
+Requires-Dist: napari-skimage-regionprops
+Requires-Dist: stardist-napari
+Requires-Dist: scikit-learn
+Requires-Dist: pandas
+Provides-Extra: testing
+Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-qt; extra == "testing"
+Requires-Dist: napari; extra == "testing"
+Requires-Dist: pyqt5; extra == "testing"
 
 # napari-ehooke
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-ehooke.svg?color=green)](https://github.com/antmsbrito/napari-ehooke/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-ehooke.svg?color=green)](https://pypi.org/project/napari-ehooke)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-ehooke.svg?color=green)](https://python.org)
 [![tests](https://github.com/antmsbrito/napari-ehooke/workflows/tests/badge.svg)](https://github.com/antmsbrito/napari-ehooke/actions)
```

### Comparing `napari-ehooke-0.0.5/README.md` & `napari-ehooke-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `napari-ehooke-0.0.5/setup.cfg` & `napari-ehooke-0.0.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-ehooke
-version = 0.0.5
+version = 0.0.6
 description = eHooke implementation within napari
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/antmsbrito/napari-ehooke
 author = António Brito
 author_email = antmsbrito95@gmail.com
 license = BSD-3-Clause
```

### Comparing `napari-ehooke-0.0.5/src/napari_ehooke/_computecells.py` & `napari-ehooke-0.0.6/src/napari_ehooke/_computecells.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-TODO
+Module responsible for computing per cell statistics
 """
 import os
 import typing
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     import napari
```

### Comparing `napari-ehooke-0.0.5/src/napari_ehooke/_computemask.py` & `napari-ehooke-0.0.6/src/napari_ehooke/ehooke/mask.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,55 @@
 """
-TODO
+Module that contains the logic for mask computation
 """
 
-import typing
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    import napari
-
-from magicgui import magic_factory
-
 import numpy as np
 from scipy import ndimage, signal
 from skimage.filters import threshold_isodata, threshold_local
 from skimage.morphology import binary_closing, binary_dilation
 from skimage.transform import EuclideanTransform, warp
 
-@magic_factory(algorithm={"choices":["Isodata","Local Average"]})
-def compute_mask(Viewer:"napari.Viewer",Base:"napari.types.ImageData",Fluor:"napari.types.ImageData",algorithm="Isodata",blocksize:int=151,offset:float=0.02,closing:int=1,dilation:int=0,fillholes:bool=False,autoalign:bool=False)->typing.List["napari.types.LayerDataTuple"]:
-    """
-    TODO    
-    """
-    # TODO MOVE ALL LOGIC TO EHOOKE SUBFOLDER
+def mask_computation(base_image:np.ndarray, algorithm:str="Isodata",
+                     blocksize:int=151,offset:float=0.02,closing:int=1,
+                     dilation:int=0,fillholes:bool=False):
+    
+    # Binarization
     if algorithm == "Isodata":
-
-        mask = Base > threshold_isodata(Base)
+        mask = base_image > threshold_isodata(base_image)
         mask = mask.astype(int)
         mask = 1 - mask
-
     elif algorithm == "Local Average":
         if blocksize%2==0:
             blocksize += 1
-        mask = Base > threshold_local(Base, block_size=blocksize, method="gaussian", offset=offset)
+        mask = base_image > threshold_local(base_image, block_size=blocksize, method="gaussian", offset=offset)
         mask = mask.astype(int)
         mask = 1 - mask
     
+    # remove spots (both white and dark)
     if closing > 0:
         # removes small white spots and then small dark spots
         closing_matrix = np.ones((int(closing), int(closing)))
         mask = binary_closing(mask, closing_matrix)
         mask = 1 - binary_closing(1 - mask, closing_matrix)
 
+    # dilation
     for f in range(dilation):
         mask = binary_dilation(mask, np.ones((3, 3)))
 
+    # binary fill holes
     if fillholes:
         mask = ndimage.binary_fill_holes(mask)
 
+    return mask 
 
-    if autoalign:
-        corr = signal.fftconvolve(mask,Fluor[::-1,::-1])
-        deviation = np.unravel_index(np.argmax(corr),corr.shape)
-        cm = ndimage.center_of_mass(np.ones(corr.shape))
+def mask_alignment(mask:np.ndarray, fluor_image:np.ndarray):
+        
+    corr = signal.fftconvolve(mask,fluor_image[::-1,::-1])
+    deviation = np.unravel_index(np.argmax(corr),corr.shape)
+    cm = ndimage.center_of_mass(np.ones(corr.shape))
         
-        dy,dx = np.subtract(deviation,cm)
-        matrix = EuclideanTransform(rotation=0, translation=(dx,dy))
+    dy,dx = np.subtract(deviation,cm)
+    matrix = EuclideanTransform(rotation=0, translation=(dx,dy))
 
-        aligned_fluor = warp(Fluor, matrix.inverse, preserve_range=True) # TODO check if fluor intensity values stay the same
+    aligned_fluor = warp(fluor_image, matrix.inverse, preserve_range=True) # TODO check if fluor intensity values stay the same
 
-        return [(aligned_fluor,{'name':'Aligned fluor'}, 'Image'),(mask, {'name': 'Mask'}, 'Labels')]
-    else:
-        return [(mask, {'name': 'Mask'}, 'Labels'),]
+    return aligned_fluor
```

### Comparing `napari-ehooke-0.0.5/src/napari_ehooke/ehooke/cellaverager.py` & `napari-ehooke-0.0.6/src/napari_ehooke/ehooke/cellaverager.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 from sklearn.decomposition import PCA
 
 class CellAverager:
     """
     Class in charge of building an average heatmap 
     """
 
-    def __init__(self):
+    def __init__(self, fluor):
         
+        self.fluor = fluor
         self.model = None
         self.aligned_fluor_masks = []
 
     def align(self, cell):
 
         angle = self.calculate_rotation_angle(cell)
-        self.aligned_fluor_masks.append(rotate(cell.image_box(cell.fluor) * cell.cell_mask, angle))
+        self.aligned_fluor_masks.append(rotate(cell.image_box(self.fluor) * cell.cell_mask, angle))
 
     def average(self):
 
         mean_x = int(np.median([s.shape[0] for s in self.aligned_fluor_masks]))
         mean_y = int(np.median([s.shape[1] for s in self.aligned_fluor_masks]))
 
         fluor_crops_array = [resize(s, (mean_x, mean_y)) for s in self.aligned_fluor_masks]
@@ -31,15 +32,15 @@
         for cell in fluor_crops_array:
             model_cell += cell
         model_cell /= float(len(fluor_crops_array))
 
         self.model = model_cell
 
     def calculate_rotation_angle(self, cell):
-        binary = cell.image_box(cell.fluor) * cell.cell_mask
+        binary = cell.image_box(self.fluor) * cell.cell_mask
         outline = self.calculate_cell_outline(binary)
         major_axis = self.calculate_major_axis(outline)
         return self.calculate_axis_angle(major_axis)
 
     @staticmethod
     def calculate_cell_outline(binary):
         outline = binary * (1 - binary_erosion(binary))
```

### Comparing `napari-ehooke-0.0.5/src/napari_ehooke/ehooke/cellcycleclassifier.py` & `napari-ehooke-0.0.6/src/napari_ehooke/ehooke/cellcycleclassifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
 
 
 class CellCycleClassifier:
 
     def __init__(self, fluor_fov, optional_fov, microscope):
 
-        # todo
         cnnmodel = get_file("model","https://github.com/antmsbrito/napari-ehooke/blob/main/docs/cellcycle_cnn_model?raw=true")
         self.model = load_model(cnnmodel)
 
         self.fluor_fov = fluor_fov
         self.optional_fov = optional_fov
 
         self.microscope = microscope
```

### Comparing `napari-ehooke-0.0.5/src/napari_ehooke/ehooke/cellprocessing.py` & `napari-ehooke-0.0.6/src/napari_ehooke/ehooke/cellprocessing.py`

 * *Files identical despite different names*

### Comparing `napari-ehooke-0.0.5/src/napari_ehooke/ehooke/cells.py` & `napari-ehooke-0.0.6/src/napari_ehooke/ehooke/cells.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,29 +18,33 @@
 from .cellaverager import CellAverager
 from .colocmanager import ColocManager
 from .reports import ReportManager
 
 class Cell:
     """Template for each cell object."""
 
-    def __init__(self, label, regionmask, intensity, params):
+    def __init__(self, label, regionmask, intensity, params, optional=None):
         
-        self.label = label
-        self.mask = regionmask.astype(int)
-        self.fluor = intensity
+        self.label = label 
+
+        # THESE 3 PARAMETERS HAVE TO GO
+        #self.mask = regionmask.astype(int)
+        #self.fluor = intensity
+        #self.optional = optional
 
         self.params = params
 
         self.box_margin = 5
 
         properties = regionprops(regionmask.astype(int), intensity)[0]
 
         self.box = properties.bbox # (min_row, min_col, max_row, max_col)
        
-        w,h = self.fluor.shape
+        w,h = intensity.shape
+        self.img_shape = intensity.shape
         self.box = (max(self.box[0] - self.box_margin, 0),
                     max(self.box[1] - self.box_margin, 0),
                     min(self.box[2] + self.box_margin, w - 1),
                     min(self.box[3] + self.box_margin, h - 1))
         
         y0, x0 = properties.centroid
         x1 = x0 + math.cos(properties.orientation) * 0.5 * properties.axis_minor_length
@@ -57,15 +61,18 @@
         y2 = y0 + math.cos(properties.orientation) * 0.5 * properties.axis_major_length
         
         # NOTE THE SWAP ON X AND Y 
         self.short_axis = np.rint(np.array([[y1,x1],[y2,x2]])).astype(int)
 
         # CHECK IF SHORT AXIS AND LONG AXIS ARE OUTSIDE OF BOX TODO
 
-        self.cell_mask = self.image_box(self.mask)
+        self.cell_mask = self.image_box(regionmask.astype(int))
+        self.fluor_mask = self.image_box(intensity)
+        self.optional_mask = self.image_box(optional)
+
         self.perim_mask = None
         self.sept_mask = None
         self.cyto_mask = None
         self.membsept_mask = None
 
         self.stats = dict([("Baseline", 0),
                            ("Cell Median", 0),
@@ -80,74 +87,79 @@
                            ("Area",properties.area),
                            ("Perimeter",properties.perimeter),
                            ("Eccentricity",properties.eccentricity),
                            ])
         
         self.selection_state = 1
         self.compute_regions(self.params)
-        self.compute_fluor_stats(self.params)
+        self.compute_fluor_stats(self.params, regionmask.astype(int), intensity)
 
         self.image = None
-        self.set_image()
+        self.set_image(intensity,optional)
 
 
     def image_box(self, image):
         """ returns box """
 
         x0, y0, x1, y1 = self.box
         try:
             return image[x0:x1+1, y0:y1+1]
         except TypeError:
             return None
 
-    def compute_perim_mask(self, mask, thick):
+    def compute_perim_mask(self, thick):
         """returns mask for perimeter
             needs cell mask
         """
+        mask = self.cell_mask
 
         eroded = morphology.binary_erosion(mask, np.ones(
             (thick * 2 - 1, thick - 1))).astype(float)
         perim = mask - eroded
 
         return perim
 
-    def compute_sept_mask(self, mask, thick, algorithm):
+    def compute_sept_mask(self, thick, algorithm):
         """ returns mask for axis.
         needs cell mask
         """
 
+        mask = self.cell_mask
+
         if algorithm == "Isodata":
             return self.compute_sept_isodata(mask, thick)
 
         elif algorithm == "Box":
             return self.compute_sept_box(mask, thick)
 
         else:
             print("Not a a valid algorithm")
 
-    def compute_opensept_mask(self, mask, thick, algorithm):
+    def compute_opensept_mask(self, thick, algorithm):
         """ 
         returns mask for axis.
         needs cell mask
         """
 
+        mask = self.cell_mask
+
         if algorithm == "Isodata":
             return self.compute_opensept_isodata(mask, thick)
         elif algorithm == "Box":
             return self.compute_sept_box(mask, thick)
 
         else:
             print("Not a a valid algorithm")
 
-    def compute_sept_isodata(self, mask, thick):
+    def compute_sept_isodata(self, thick):
         """Method used to create the cell sept_mask using the threshold_isodata
         to separate the cytoplasm from the septum"""
-        cell_mask = mask
-        fluor_box = self.image_box(self.fluor)
-        perim_mask = self.compute_perim_mask(cell_mask, thick)
+        cell_mask = self.cell_mask
+        fluor_box = self.fluor_mask
+        perim_mask = self.compute_perim_mask(thick)
         inner_mask = cell_mask - perim_mask
         inner_fluor = (inner_mask > 0) * fluor_box
 
         threshold = threshold_isodata(inner_fluor[inner_fluor > 0])
         interest_matrix = inner_mask * (inner_fluor > threshold)
 
         label_matrix = label(interest_matrix, connectivity=2)
@@ -158,20 +170,20 @@
             if np.sum(img_as_float(label_matrix == l + 1)) > interest_label_sum:
                 interest_label = l + 1
                 interest_label_sum = np.sum(
                     img_as_float(label_matrix == l + 1))
 
         return img_as_float(label_matrix == interest_label)
 
-    def compute_opensept_isodata(self, mask, thick):
+    def compute_opensept_isodata(self, thick):
         """Method used to create the cell sept_mask using the threshold_isodata
         to separate the cytoplasm from the septum"""
-        cell_mask = mask
-        fluor_box = self.image_box(self.fluor)
-        perim_mask = self.compute_perim_mask(cell_mask, thick)
+        cell_mask = self.cell_mask
+        fluor_box = self.fluor_mask
+        perim_mask = self.compute_perim_mask(thick)
         inner_mask = cell_mask - perim_mask
         inner_fluor = (inner_mask > 0) * fluor_box
 
         threshold = threshold_isodata(inner_fluor[inner_fluor > 0])
         interest_matrix = inner_mask * (inner_fluor > threshold)
 
         label_matrix = label(interest_matrix, connectivity=2)
@@ -200,18 +212,21 @@
                 break
 
         if second_label != 0:
             return img_as_float((label_matrix == first_label) + (label_matrix == second_label))
         else:
             return img_as_float((label_matrix == first_label))
 
-    def compute_sept_box(self, mask, thick):
+    def compute_sept_box(self, thick):
         """Method used to create a mask of the septum based on creating a box
         around the cell and then defining the septum as being the dilated short
         axis of the box."""
+
+        mask = self.cell_mask
+
         x0, y0, x1, y1 = self.box
         lx0, ly0 = self.short_axis[0]
         lx1, ly1 = self.short_axis[1]
         x, y = line(lx0 - x0, ly0 - y0, lx1 - x0, ly1 - y0)
 
         linmask = np.zeros((x1 - x0 + 1, y1 - y0 + 1))
         linmask[x, y] = 1
@@ -420,70 +435,70 @@
                     linmask, np.ones((bin_factor, bin_factor))).astype(float)
             except RuntimeError:
                 bin_factor = 4
                 linmask = morphology.binary_dilation(
                     linmask, np.ones((bin_factor, bin_factor))).astype(float)
         return img_as_float(linmask)
 
-    def recursive_compute_sept(self, cell_mask, inner_mask_thickness,algorithm):
+    def recursive_compute_sept(self, inner_mask_thickness,algorithm):
         try:
-            self.sept_mask = self.compute_sept_mask(cell_mask,inner_mask_thickness,algorithm)
+            self.sept_mask = self.compute_sept_mask(inner_mask_thickness,algorithm)
         except IndexError:
             try:
-                self.recursive_compute_sept(cell_mask, inner_mask_thickness - 1, algorithm)
+                self.recursive_compute_sept(inner_mask_thickness - 1, algorithm)
             except RuntimeError:
-                self.recursive_compute_sept(cell_mask, inner_mask_thickness - 1, "Box")
+                self.recursive_compute_sept(inner_mask_thickness - 1, "Box")
 
-    def recursive_compute_opensept(self, cell_mask, inner_mask_thickness,algorithm):
+    def recursive_compute_opensept(self, inner_mask_thickness,algorithm):
         try:
-            self.sept_mask = self.compute_opensept_mask(cell_mask,inner_mask_thickness,algorithm)
+            self.sept_mask = self.compute_opensept_mask(inner_mask_thickness,algorithm)
         except IndexError:
             try:
-                self.recursive_compute_opensept(cell_mask, inner_mask_thickness - 1,algorithm)
+                self.recursive_compute_opensept(inner_mask_thickness - 1,algorithm)
             except RuntimeError:
-                self.recursive_compute_opensept(cell_mask, inner_mask_thickness - 1, "Box")
+                self.recursive_compute_opensept(inner_mask_thickness - 1, "Box")
 
     def compute_regions(self, params):
         """Computes each different region of the cell (whole cell, membrane,
         septum, cytoplasm) and creates their respectives masks."""
 
         if params["find_septum"]:
-            self.recursive_compute_sept(self.cell_mask,params["inner_mask_thickness"],params["septum_algorithm"])
+            self.recursive_compute_sept(params["inner_mask_thickness"],params["septum_algorithm"])
 
             if params["septum_algorithm"] == "Isodata":
-                self.perim_mask = self.compute_perim_mask(self.cell_mask, params["inner_mask_thickness"])
+                self.perim_mask = self.compute_perim_mask(params["inner_mask_thickness"])
                 self.membsept_mask = (self.perim_mask + self.sept_mask) > 0
-                linmask = self.remove_sept_from_membrane(self.fluor.shape)
+                linmask = self.remove_sept_from_membrane(self.img_shape)
                 self.cyto_mask = (self.cell_mask - self.perim_mask - self.sept_mask) > 0
                 if linmask is not None:
                     old_membrane = self.perim_mask
                     self.perim_mask = (old_membrane - linmask) > 0
             else:
-                self.perim_mask = (self.compute_perim_mask(self.cell_mask, params["inner_mask_thickness"]) - self.sept_mask) > 0
+                self.perim_mask = (self.compute_perim_mask(params["inner_mask_thickness"]) - self.sept_mask) > 0
                 self.membsept_mask = (self.perim_mask + self.sept_mask) > 0
                 self.cyto_mask = (self.cell_mask - self.perim_mask - self.sept_mask) > 0
         elif params["find_openseptum"]:
-            self.recursive_compute_opensept(self.cell_mask,params["inner_mask_thickness"],params["septum_algorithm"])
+            self.recursive_compute_opensept(params["inner_mask_thickness"],params["septum_algorithm"])
 
             if params["septum_algorithm"] == "Isodata":
-                self.perim_mask = self.compute_perim_mask(self.cell_mask,params["inner_mask_thickness"])
+                self.perim_mask = self.compute_perim_mask(params["inner_mask_thickness"])
 
                 self.membsept_mask = (self.perim_mask + self.sept_mask) > 0
-                linmask = self.remove_sept_from_membrane(self.fluor.shape)
+                linmask = self.remove_sept_from_membrane(self.img_shape)
                 self.cyto_mask = (self.cell_mask - self.perim_mask - self.sept_mask) > 0
                 if linmask is not None:
                     old_membrane = self.perim_mask
                     self.perim_mask = (old_membrane - linmask) > 0
             else:
-                self.perim_mask = (self.compute_perim_mask(self.cell_mask, params["inner_mask_thickness"]) - self.sept_mask) > 0
+                self.perim_mask = (self.compute_perim_mask(params["inner_mask_thickness"]) - self.sept_mask) > 0
                 self.membsept_mask = (self.perim_mask + self.sept_mask) > 0
                 self.cyto_mask = (self.cell_mask - self.perim_mask - self.sept_mask) > 0
         else:
             self.sept_mask = None
-            self.perim_mask = self.compute_perim_mask(self.cell_mask, params["inner_mask_thickness"])
+            self.perim_mask = self.compute_perim_mask(params["inner_mask_thickness"])
             self.cyto_mask = (self.cell_mask - self.perim_mask) > 0
 
     def compute_fluor_baseline(self, mask, fluor, margin):
         """mask and fluor are the global images
            NOTE: mask is 0 (black) at cells and 1 (white) outside
         """
         # compatibility
@@ -531,21 +546,21 @@
                 return np.median(sortvals)
 
             else:
                 return np.median(bright)
         else:
             return 0
 
-    def compute_fluor_stats(self, params):
+    def compute_fluor_stats(self, params, mask, fluor):
         """Computes the cell stats related to the fluorescence"""
-        self.compute_fluor_baseline(self.mask,
-                                    self.fluor,
+        self.compute_fluor_baseline(mask,
+                                    fluor,
                                     params["baseline_margin"])
 
-        fluorbox = self.image_box(self.fluor)
+        fluorbox = self.fluor_mask
 
         self.stats["Cell Median"] = \
             self.measure_fluor(fluorbox, self.cell_mask) - \
             self.stats["Baseline"]
 
         self.stats["Membrane Median"] = \
             self.measure_fluor(fluorbox, self.perim_mask) - \
@@ -581,38 +596,56 @@
 
             self.stats["Fluor Ratio 25%"] = 0
 
             self.stats["Fluor Ratio 10%"] = 0
 
             self.stats["Memb+Sept Median"] = 0
 
-    def set_image(self):
+    def set_image(self, fluor, optional):
 
-        fluor = img_as_float(self.fluor)
+        fluor = img_as_float(fluor)
         fluor = exposure.rescale_intensity(fluor)
 
+        optional = img_as_float(optional)
+        optional = exposure.rescale_intensity(optional)
+
+        perim = self.perim_mask
+        axial = self.sept_mask
+        cyto = self.cyto_mask
+
         x0, y0, x1, y1 = self.box
-        img = color.gray2rgb(np.zeros((x1 - x0 + 1, 5 * (y1 - y0 + 1))))
+        img = color.gray2rgb(np.zeros((x1 - x0 + 1, 7 * (y1 - y0 + 1))))
         bx0 = 0
         bx1 = x1 - x0 + 1
         by0 = 0
         by1 = y1 - y0 + 1
 
+        # 7 images
+
+        # #1 is the fluorescence 
         img[bx0:bx1, by0:by1] = color.gray2rgb(fluor[x0:x1 + 1, y0:y1 + 1])
         by0 = by0 + y1 - y0 + 1
         by1 = by1 + y1 - y0 + 1
+        
+        # #2 is the fluorescence segmented
+        img[bx0:bx1, by0:by1] = color.gray2rgb(fluor[x0:x1 + 1, y0:y1 + 1] * self.cell_mask)
+        by0 = by0 + y1 - y0 + 1
+        by1 = by1 + y1 - y0 + 1
 
-        perim = self.perim_mask
-        axial = self.sept_mask
-        cyto = self.cyto_mask
+        # #3 is the dna
+        img[bx0:bx1, by0:by1] = color.gray2rgb(optional[x0:x1 + 1, y0:y1 + 1])
+        by0 = by0 + y1 - y0 + 1
+        by1 = by1 + y1 - y0 + 1
 
-        img[bx0:bx1, by0:by1] = color.gray2rgb(fluor[x0:x1 + 1, y0:y1 + 1] * self.cell_mask)
+        # #4 is the dna segmented
+        img[bx0:bx1, by0:by1] = color.gray2rgb(optional[x0:x1 + 1, y0:y1 + 1] * self.cell_mask)
         by0 = by0 + y1 - y0 + 1
         by1 = by1 + y1 - y0 + 1
 
+        # 5,6,7 is perimeter, cytoplasm and septa
         img[bx0:bx1, by0:by1] = color.gray2rgb(fluor[x0:x1 + 1, y0:y1 + 1] * perim)
         by0 = by0 + y1 - y0 + 1
         by1 = by1 + y1 - y0 + 1
 
         img[bx0:bx1, by0:by1] = color.gray2rgb(fluor[x0:x1 + 1, y0:y1 + 1] * cyto)
 
         if self.params['find_septum'] or self.params['find_openseptum']:
@@ -633,14 +666,16 @@
         self.optional_img = optional
 
         self.params = params
 
         self.properties = None
         self.heatmap_model = None
 
+        #self.random_sample = []
+
 
     def compute_cell_properties(self):
 
         Label = []
         Area = []
         Perimeter = []
         Eccentricity = []
@@ -649,33 +684,45 @@
         Septum_Median = []
         Cytoplasm_Median = [] 
         Fluor_Ratio = []
         Fluor_Ratio_75 = []
         Fluor_Ratio_25 = []
         Fluor_Ratio_10 = []
         CellCyclePhase = []
+        DNARatio = []
         All_Cells = [] # TODO consider always saving
 
         if self.params['classify_cell_cycle']:
+            print("Cell cycle...")
             ccc = CellCycleClassifier(self.fluor_img, self.optional_img, self.params['microscope'])
         if self.params['cell_averager']:
-            ca = CellAverager()
+            print("Cell averager...")
+            ca = CellAverager(self.fluor_img)
 
-        for l in np.unique(self.label_img):
+        print("Per cell stats...")
+        label_list = np.unique(self.label_img)
+        for i,l in enumerate(label_list):
 
             if l == 0: # BG
                 continue
 
             mask = self.label_img==l
-            c = Cell(label=l, regionmask=mask, intensity=self.fluor_img, params=self.params)
+            c = Cell(label=l, regionmask=mask, intensity=self.fluor_img, params=self.params, optional=self.optional_img) 
             
             if self.params['generate_report']:
                 All_Cells.append(c)
             if self.params['cell_averager']:
                 ca.align(c)
+            # if self.params['random_sample']:
+            #     if len(self.random_sample)>int(0.25*len(label_list)):
+            #         j = np.random.randint(0,i)
+            #         if j <= int(0.25*len(label_list))-1:
+            #             self.random_sample[j] = c
+            #     else:
+            #         self.random_sample.append(c)
 
             Label.append(c.label)
             Area.append(c.stats['Area'])
             Perimeter.append(c.stats['Perimeter'])
             Eccentricity.append(c.stats['Eccentricity'])
             Baseline.append(c.stats['Baseline'])
             Membrane_Median.append(c.stats['Membrane Median'])
@@ -686,14 +733,15 @@
             Fluor_Ratio_25.append(c.stats['Fluor Ratio 25%'])
             Fluor_Ratio_10.append(c.stats['Fluor Ratio 10%'])
             if self.params['classify_cell_cycle']:
                 c.stats['Cell Cycle Phase'] = ccc.classify_cell(c)
             else:
                 c.stats['Cell Cycle Phase'] = 0
             CellCyclePhase.append(c.stats['Cell Cycle Phase'])
+            DNARatio.append(self.calculate_DNARatio(c,self.optional_img))
 
         properties = {}
         properties['label'] = np.array(Label)
         properties['Area'] = np.array(Area)
         properties['Perimeter'] = np.array(Perimeter)
         properties['Eccentricity'] = np.array(Eccentricity)
         properties['Baseline'] = np.array(Baseline)
@@ -701,20 +749,37 @@
         properties['Septum Median'] = np.array(Septum_Median)
         properties['Cytoplasm Median'] = np.array(Cytoplasm_Median)
         properties['Fluor Ratio'] = np.array(Fluor_Ratio)
         properties['Fluor Ratio 75%'] = np.array(Fluor_Ratio_75)
         properties['Fluor Ratio 25%'] = np.array(Fluor_Ratio_25)
         properties['Fluor Ratio 10%'] = np.array(Fluor_Ratio_10)
         properties['Cell Cycle Phase'] = np.array(CellCyclePhase)
+        properties['DNA Ratio'] = np.array(DNARatio)
 
         self.properties = properties
 
         if self.params['cell_averager']:
             ca.average()
             self.heatmap_model = ca.model
 
         if self.params['generate_report']:
             rm = ReportManager(parameters=self.params,cells=All_Cells)
-            rm.generate_report(self.params['report_path'])
+            rm.generate_report(self.params['report_path'], report_id=self.params.get('report_id',None))
             if self.params['coloc']:
                 coloc = ColocManager()
                 coloc.compute_pcc(self.fluor_img, self.optional_img,All_Cells,self.params,rm.cell_data_filename)
+
+        # if self.params['random_sample']:
+        #     rm = ReportManager(parameters=self.params,cells=self.random_sample)
+        #     rm.generate_report(self.params['report_path'],"RANDOM_SAMPLE")
+
+    @staticmethod
+    def calculate_DNARatio(cell_object, dna_fov):
+
+        thresh = threshold_isodata(dna_fov[np.nonzero(dna_fov)])
+        x0, y0, x1, y1 = cell_object.box
+        cell_mask = cell_object.cell_mask
+        optional_cell = dna_fov[x0:x1 + 1, y0:y1 + 1]
+        optional_signal = (optional_cell * cell_mask) > thresh
+
+        return np.sum(optional_signal) / np.sum(cell_mask)
+
```

### Comparing `napari-ehooke-0.0.5/src/napari_ehooke/ehooke/colocmanager.py` & `napari-ehooke-0.0.6/src/napari_ehooke/ehooke/colocmanager.py`

 * *Files identical despite different names*

### Comparing `napari-ehooke-0.0.5/src/napari_ehooke/ehooke/reports.py` & `napari-ehooke-0.0.6/src/napari_ehooke/ehooke/reports.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from skimage.io import imsave
 from skimage.util import img_as_float, img_as_uint
 from skimage.filters import threshold_isodata
 from skimage.color import gray2rgb
 from decimal import Decimal
 import numpy as np
 import os
+from tifffile import imwrite
 
 from .cellprocessing import stats_format
 
 class ReportManager:
 
     def __init__(self, parameters, cells):
         self.cells = cells
@@ -52,14 +53,24 @@
 
             print("Total Cells: " + str(len(cells)))
 
             for cell in cells:
                 if cell.selection_state == 1:
                     cellid = str(int(cell.label))
                     img = img_as_float(cell.image)
+
+                    """
+                    x0, y0, x1, y1 = cell.box
+                    memb_img = cell.fluor[x0:x1 + 1, y0:y1 + 1]
+                    dna_img = cell.optional[x0:x1 + 1, y0:y1 + 1]
+                    imwrite(filename + "/_images/membrane" + os.sep + cellid + '.tif', memb_img)
+                    imwrite(filename + "/_images/dna" + os.sep + cellid + '.tif', dna_img)
+                    imsave(filename + "/_images/crops" + os.sep + cellid + '.png', img)
+                    """
+                    
                     imsave(filename + "/_images" +
                            os.sep + cellid + '.png', img)
                     lin = '<tr><td>' + cellid + '</td><td><img src="./' + '_images/' + \
                           cellid + '.png" alt="pic" width="200"/></td>'
 
                     count += 1
 
@@ -157,23 +168,29 @@
         if report_id is None:
             filename = path + "/Report_1"
             filename = self.check_filename(filename)
             self.cell_data_filename = filename
 
             if not os.path.exists(filename + "/_images"):
                 os.makedirs(filename + "/_images")
+                os.makedirs(filename + "/_images/membrane")
+                os.makedirs(filename + "/_images/dna")
+                os.makedirs(filename + "/_images/crops")
             if not os.path.exists(filename + "/_rejected_images"):
                 os.makedirs(filename + "/_rejected_images")
         else:
             filename = path + "/Report_" + report_id + "_1"
             filename = self.check_filename(filename)
             self.cell_data_filename = filename
 
             if not os.path.exists(filename + "/_images"):
                 os.makedirs(filename + "/_images")
+                os.makedirs(filename + "/_images/membrane")
+                os.makedirs(filename + "/_images/dna")
+                os.makedirs(filename + "/_images/crops")
             if not os.path.exists(filename + "/_rejected_images"):
                 os.makedirs(filename + "/_rejected_images")
 
         self.html_report(filename)
 
         # TODO add view of selected cells
         # TODO SAVE PARS
```

### Comparing `napari-ehooke-0.0.5/src/napari_ehooke/ehooke/segments.py` & `napari-ehooke-0.0.6/src/napari_ehooke/ehooke/segments.py`

 * *Files identical despite different names*

### Comparing `napari-ehooke-0.0.5/src/napari_ehooke/napari.yaml` & `napari-ehooke-0.0.6/src/napari_ehooke/napari.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       title: Compute base mask
     - id: napari-ehooke.compute_features
       python_name: napari_ehooke._computefeatures:compute_features
       title: Compute features
     - id: napari-ehooke.compute_cells
       python_name: napari_ehooke._computecells:compute_cells
       title: Compute cells
+    - id: napari-ehooke.filter_cells
+      python_name: napari_ehooke._filtercells:filter_cells
+      title: Filter cells
   sample_data:
     - command: napari-ehooke.phase_example
       display_name: Phase contrast S. aureus
       key: unique_id.1
     - command: napari-ehooke.membrane_example
       display_name: Membrane dye S.aureus
       key: unique_id.2
@@ -32,8 +35,10 @@
       key: unique_id.3
   widgets:
     - command: napari-ehooke.compute_mask
       display_name: Compute base mask
     - command: napari-ehooke.compute_features
       display_name: Compute features
     - command: napari-ehooke.compute_cells
-      display_name: Compute cells
+      display_name: Compute cells
+    - command: napari-ehooke.filter_cells
+      display_name: Filter cells
```

### Comparing `napari-ehooke-0.0.5/src/napari_ehooke.egg-info/PKG-INFO` & `napari-ehooke-0.0.6/src/napari_ehooke.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-ehooke
-Version: 0.0.5
+Version: 0.0.6
 Summary: eHooke implementation within napari
 Home-page: https://github.com/antmsbrito/napari-ehooke
 Author: António Brito
 Author-email: antmsbrito95@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/antmsbrito/napari-ehooke/issues
 Project-URL: Documentation, https://github.com/antmsbrito/napari-ehooke#README.md
@@ -20,16 +20,31 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: magicgui
+Requires-Dist: qtpy
+Requires-Dist: napari[all]
+Requires-Dist: tensorflow
+Requires-Dist: napari-skimage-regionprops
+Requires-Dist: stardist-napari
+Requires-Dist: scikit-learn
+Requires-Dist: pandas
+Provides-Extra: testing
+Requires-Dist: tox; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: pytest-qt; extra == "testing"
+Requires-Dist: napari; extra == "testing"
+Requires-Dist: pyqt5; extra == "testing"
 
 # napari-ehooke
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-ehooke.svg?color=green)](https://github.com/antmsbrito/napari-ehooke/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-ehooke.svg?color=green)](https://pypi.org/project/napari-ehooke)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-ehooke.svg?color=green)](https://python.org)
 [![tests](https://github.com/antmsbrito/napari-ehooke/workflows/tests/badge.svg)](https://github.com/antmsbrito/napari-ehooke/actions)
```

### Comparing `napari-ehooke-0.0.5/src/napari_ehooke.egg-info/SOURCES.txt` & `napari-ehooke-0.0.6/src/napari_ehooke.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.cfg
 src/napari_ehooke/__init__.py
 src/napari_ehooke/_computecells.py
 src/napari_ehooke/_computefeatures.py
 src/napari_ehooke/_computemask.py
+src/napari_ehooke/_filtercells.py
 src/napari_ehooke/_sample_data.py
 src/napari_ehooke/napari.yaml
 src/napari_ehooke.egg-info/PKG-INFO
 src/napari_ehooke.egg-info/SOURCES.txt
 src/napari_ehooke.egg-info/dependency_links.txt
 src/napari_ehooke.egg-info/entry_points.txt
 src/napari_ehooke.egg-info/requires.txt
@@ -19,9 +20,10 @@
 src/napari_ehooke/_tests/test_sample_data.py
 src/napari_ehooke/ehooke/__init__.py
 src/napari_ehooke/ehooke/cellaverager.py
 src/napari_ehooke/ehooke/cellcycleclassifier.py
 src/napari_ehooke/ehooke/cellprocessing.py
 src/napari_ehooke/ehooke/cells.py
 src/napari_ehooke/ehooke/colocmanager.py
+src/napari_ehooke/ehooke/mask.py
 src/napari_ehooke/ehooke/reports.py
 src/napari_ehooke/ehooke/segments.py
```

