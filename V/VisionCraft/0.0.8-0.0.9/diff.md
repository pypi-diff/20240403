# Comparing `tmp/VisionCraft-0.0.8.tar.gz` & `tmp/VisionCraft-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisionCraft-0.0.8.tar", last modified: Thu Feb 29 18:07:30 2024, max compression
+gzip compressed data, was "VisionCraft-0.0.9.tar", last modified: Tue Mar 12 14:11:05 2024, max compression
```

## Comparing `VisionCraft-0.0.8.tar` & `VisionCraft-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-02-29 18:07:30.153123 VisionCraft-0.0.8/
--rw-rw-rw-   0        0        0     1090 2024-02-08 13:43:37.000000 VisionCraft-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    17601 2024-02-29 18:07:30.149653 VisionCraft-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    16590 2024-02-27 14:46:07.000000 VisionCraft-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-02-29 18:07:30.103695 VisionCraft-0.0.8/VisionCraft/
--rw-rw-rw-   0        0        0       25 2024-02-13 16:58:32.000000 VisionCraft-0.0.8/VisionCraft/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 18:07:30.114398 VisionCraft-0.0.8/VisionCraft/craft/
--rw-rw-rw-   0        0        0      312 2024-02-13 16:59:09.000000 VisionCraft-0.0.8/VisionCraft/craft/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-29 18:07:30.125597 VisionCraft-0.0.8/VisionCraft/help/
--rw-rw-rw-   0        0        0       30 2024-02-13 16:59:03.000000 VisionCraft-0.0.8/VisionCraft/help/__init__.py
--rw-rw-rw-   0        0        0     2342 2024-02-13 16:12:37.000000 VisionCraft-0.0.8/VisionCraft/help/exp1.py
--rw-rw-rw-   0        0        0        0 2024-02-13 14:34:10.000000 VisionCraft-0.0.8/VisionCraft/help/exp2.py
--rw-rw-rw-   0        0        0        0 2024-02-13 14:34:14.000000 VisionCraft-0.0.8/VisionCraft/help/exp3.py
--rw-rw-rw-   0        0        0     1338 2024-02-14 06:44:37.000000 VisionCraft-0.0.8/VisionCraft/help/exp4.py
--rw-rw-rw-   0        0        0    10224 2024-02-13 16:46:29.000000 VisionCraft-0.0.8/VisionCraft/help/exp5.py
-drwxrwxrwx   0        0        0        0 2024-02-29 18:07:30.143637 VisionCraft-0.0.8/VisionCraft/vision/
--rw-rw-rw-   0        0        0      777 2024-02-13 16:59:20.000000 VisionCraft-0.0.8/VisionCraft/vision/__init__.py
--rw-rw-rw-   0        0        0     9693 2024-02-29 18:01:52.000000 VisionCraft-0.0.8/VisionCraft/vision/filter.py
--rw-rw-rw-   0        0        0     6836 2024-02-14 18:18:57.000000 VisionCraft-0.0.8/VisionCraft/vision/processing.py
--rw-rw-rw-   0        0        0     9901 2024-02-14 19:09:26.000000 VisionCraft-0.0.8/VisionCraft/vision/transform.py
--rw-rw-rw-   0        0        0     9303 2024-02-15 14:47:33.000000 VisionCraft-0.0.8/VisionCraft/vision/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-29 18:07:30.148657 VisionCraft-0.0.8/VisionCraft.egg-info/
--rw-rw-rw-   0        0        0    17601 2024-02-29 18:07:29.000000 VisionCraft-0.0.8/VisionCraft.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      561 2024-02-29 18:07:29.000000 VisionCraft-0.0.8/VisionCraft.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-29 18:07:29.000000 VisionCraft-0.0.8/VisionCraft.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-02-29 18:07:29.000000 VisionCraft-0.0.8/VisionCraft.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-02-29 18:07:29.000000 VisionCraft-0.0.8/VisionCraft.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-29 18:07:30.153123 VisionCraft-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1275 2024-02-29 18:06:51.000000 VisionCraft-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:11:05.161012 VisionCraft-0.0.9/
+-rw-rw-rw-   0        0        0     1090 2024-02-08 13:43:37.000000 VisionCraft-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    17601 2024-03-12 14:11:05.150057 VisionCraft-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    16590 2024-02-27 14:46:07.000000 VisionCraft-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-12 14:11:05.090752 VisionCraft-0.0.9/VisionCraft/
+-rw-rw-rw-   0        0        0       25 2024-02-13 16:58:32.000000 VisionCraft-0.0.9/VisionCraft/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:11:05.116391 VisionCraft-0.0.9/VisionCraft/craft/
+-rw-rw-rw-   0        0        0      312 2024-02-13 16:59:09.000000 VisionCraft-0.0.9/VisionCraft/craft/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:11:05.133385 VisionCraft-0.0.9/VisionCraft/help/
+-rw-rw-rw-   0        0        0       30 2024-02-13 16:59:03.000000 VisionCraft-0.0.9/VisionCraft/help/__init__.py
+-rw-rw-rw-   0        0        0     2342 2024-02-13 16:12:37.000000 VisionCraft-0.0.9/VisionCraft/help/exp1.py
+-rw-rw-rw-   0        0        0        0 2024-02-13 14:34:10.000000 VisionCraft-0.0.9/VisionCraft/help/exp2.py
+-rw-rw-rw-   0        0        0        0 2024-02-13 14:34:14.000000 VisionCraft-0.0.9/VisionCraft/help/exp3.py
+-rw-rw-rw-   0        0        0     1338 2024-02-14 06:44:37.000000 VisionCraft-0.0.9/VisionCraft/help/exp4.py
+-rw-rw-rw-   0        0        0    10224 2024-02-13 16:46:29.000000 VisionCraft-0.0.9/VisionCraft/help/exp5.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:11:05.150057 VisionCraft-0.0.9/VisionCraft/vision/
+-rw-rw-rw-   0        0        0      777 2024-02-13 16:59:20.000000 VisionCraft-0.0.9/VisionCraft/vision/__init__.py
+-rw-rw-rw-   0        0        0     9720 2024-03-12 14:02:13.000000 VisionCraft-0.0.9/VisionCraft/vision/filter.py
+-rw-rw-rw-   0        0        0     6836 2024-02-14 18:18:57.000000 VisionCraft-0.0.9/VisionCraft/vision/processing.py
+-rw-rw-rw-   0        0        0     9901 2024-02-14 19:09:26.000000 VisionCraft-0.0.9/VisionCraft/vision/transform.py
+-rw-rw-rw-   0        0        0     9303 2024-02-15 14:47:33.000000 VisionCraft-0.0.9/VisionCraft/vision/utils.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:11:05.150057 VisionCraft-0.0.9/VisionCraft.egg-info/
+-rw-rw-rw-   0        0        0    17601 2024-03-12 14:11:04.000000 VisionCraft-0.0.9/VisionCraft.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      561 2024-03-12 14:11:04.000000 VisionCraft-0.0.9/VisionCraft.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-12 14:11:04.000000 VisionCraft-0.0.9/VisionCraft.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-03-12 14:11:04.000000 VisionCraft-0.0.9/VisionCraft.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-03-12 14:11:04.000000 VisionCraft-0.0.9/VisionCraft.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-12 14:11:05.161747 VisionCraft-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1275 2024-03-12 14:10:57.000000 VisionCraft-0.0.9/setup.py
```

### Comparing `VisionCraft-0.0.8/LICENSE` & `VisionCraft-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.0.8/PKG-INFO` & `VisionCraft-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionCraft
-Version: 0.0.8
+Version: 0.0.9
 Summary: Computer Vision Library to help do CV much faster, Updated Filters
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,CNN,cv
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VisionCraft-0.0.8/README.md` & `VisionCraft-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.0.8/VisionCraft/help/exp1.py` & `VisionCraft-0.0.9/VisionCraft/help/exp1.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.0.8/VisionCraft/help/exp4.py` & `VisionCraft-0.0.9/VisionCraft/help/exp4.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.0.8/VisionCraft/help/exp5.py` & `VisionCraft-0.0.9/VisionCraft/help/exp5.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.0.8/VisionCraft/vision/__init__.py` & `VisionCraft-0.0.9/VisionCraft/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.0.8/VisionCraft/vision/filter.py` & `VisionCraft-0.0.9/VisionCraft/vision/filter.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     filtered_img = np.zeros_like(img)
     for row in range(rows):
         for col in range(cols):
             replace = np.round(np.sum(img1[row:row+filter_size, col:col+filter_size])/(filter_size*filter_size))
             filtered_img[row,col]=  replace
     if show:
         plt.figure(figsize=(height, width))
-        imShow("Original Image",img, subplot=True, row=2,col=1, num=1)
-        imShow("Box Filter",filtered_img,subplot=True, row=2,col=1, num=2)
+        imShow("Original Image",img, subplot=True, row=1,col=2, num=1)
+        imShow("Box Filter",filtered_img,subplot=True, row=1,col=2, num=2)
         plt.show()  
         
     return filtered_img
 
 def weightedAvgFilter(img:np.ndarray = None, 
                       path: str = "", 
                       filter_size:int = 3, 
@@ -79,14 +79,15 @@
     - image (np.ndarray): Input image (grayscale).
     - image_path (str): Path to the input image file (if 'image' is not provided).
     - filter_size (int, optional): Size of the box filter. Should be an odd number for best results.
     - show_result (bool): If True, display the original and filtered images.
     - figure_height (int): Height of the Matplotlib figure (if 'show_result' is True).
     - figure_width (int): Width of the Matplotlib figure (if 'show_result' is True).
     - CONSTANT: Value to add in padding
+    - Sigma: blur factor
 
     Returns:
     - np.ndarray: Filtered image.
 
     If 'image' is not provided and 'image_path' is specified, it loads the image from the path.
     The weighted average filter is applied to the image using a 3x3 filter kernel.
     If 'show_result' is True, the original and filtered images are displayed using Matplotlib.
@@ -113,16 +114,16 @@
     filtered_img = np.zeros_like(img)
     for row in range(rows):
         for col in range(cols):
             replace = np.round(np.sum(img1[row:row+filter_size, col:col+filter_size] * filter))
             filtered_img[row,col]=  replace
     if show:
         plt.figure(figsize=(height, width))
-        imShow("Original Image",img, subplot=True, row=2,col=1, num=1)
-        imShow("Weighted Avg Filter",filtered_img,subplot=True, row=2,col=1, num=2)
+        imShow("Original Image",img, subplot=True, row=1,col=2, num=1)
+        imShow("Weighted Avg Filter",filtered_img,subplot=True, row=1,col=2, num=2)
         plt.show()  
         
     return filtered_img
     
 def medianFilter(img:np.ndarray = None, 
                  path: str = "", 
                  filter_size : int = 3,
@@ -164,16 +165,16 @@
     filtered_img = np.zeros_like(img)
     for row in range(rows):
         for col in range(cols):
             replace = np.median(img1[row:row+filter_size, col:col+filter_size])
             filtered_img[row,col]=  replace
     if show:
         plt.figure(figsize=(height, width))
-        imShow("Original Image",img, subplot=True, row=2,col=1, num=1)
-        imShow("Median Filter",filtered_img,subplot=True, row=2,col=1, num=2)
+        imShow("Original Image",img, subplot=True, row=1,col=2, num=1)
+        imShow("Median Filter",filtered_img,subplot=True, row=1, col=2, num=2)
         plt.show()  
         
     return filtered_img
 
 def minMaxFilter(img:np.ndarray = None, 
                  path: str = "",
                  minimum: bool = True, 
@@ -219,15 +220,15 @@
                 replace = np.min(img1[row:row+filter_size, col:col+filter_size])
                 filtered_img[row,col]=  replace
             else:
                 replace = np.max(img1[row:row+filter_size, col:col+filter_size])
                 filtered_img[row,col]=  replace
     if show:
         plt.figure(figsize=(height, width))
-        imShow("Original Image",img, subplot=True, row=2,col=1, num=1)
+        imShow("Original Image",img, subplot=True, row=1,col=2, num=1)
         if minimum:
-            imShow("Min Filter",filtered_img,subplot=True, row=2,col=1, num=2)
+            imShow("Min Filter",filtered_img,subplot=True, row=1,col=2, num=2)
         else:
-            imShow("Max Filter",filtered_img,subplot=True, row=2,col=1, num=2)
+            imShow("Max Filter",filtered_img,subplot=True, row=1,col=2, num=2)
         plt.show()  
         
     return filtered_img
```

### Comparing `VisionCraft-0.0.8/VisionCraft/vision/processing.py` & `VisionCraft-0.0.9/VisionCraft/vision/processing.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.0.8/VisionCraft/vision/transform.py` & `VisionCraft-0.0.9/VisionCraft/vision/transform.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.0.8/VisionCraft/vision/utils.py` & `VisionCraft-0.0.9/VisionCraft/vision/utils.py`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.0.8/VisionCraft.egg-info/PKG-INFO` & `VisionCraft-0.0.9/VisionCraft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisionCraft
-Version: 0.0.8
+Version: 0.0.9
 Summary: Computer Vision Library to help do CV much faster, Updated Filters
 Author: Prem Gaikwad
 Author-email: premgaikwad7a@gmail.com
 Keywords: python,CNN,cv
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VisionCraft-0.0.8/VisionCraft.egg-info/SOURCES.txt` & `VisionCraft-0.0.9/VisionCraft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VisionCraft-0.0.8/setup.py` & `VisionCraft-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Computer Vision Library to help do CV much faster, Updated Filters'
 LONG_DESCRIPTION = 'Simplifying computer vision tasks with Python. Visualize, transform, and analyze images effortlessly. Ideal for students, researchers, and developers. Enhance your computer vision projects!'
 
 # Setting up
 setup(
     name="VisionCraft",
     version=VERSION,
```

