# Comparing `tmp/ByakuganVisualizer-0.1.0.tar.gz` & `tmp/ByakuganVisualizer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ByakuganVisualizer-0.1.0.tar", last modified: Thu Mar 28 18:13:12 2024, max compression
+gzip compressed data, was "ByakuganVisualizer-0.2.0.tar", last modified: Tue Apr  2 21:52:08 2024, max compression
```

## Comparing `ByakuganVisualizer-0.1.0.tar` & `ByakuganVisualizer-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:12.211190 ByakuganVisualizer-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-03-28 18:13:12.215190 ByakuganVisualizer-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-03-28 18:13:00.000000 ByakuganVisualizer-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-28 18:13:12.215190 ByakuganVisualizer-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-28 18:13:00.000000 ByakuganVisualizer-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:12.211190 ByakuganVisualizer-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:12.211190 ByakuganVisualizer-0.1.0/src/ByakuganVisualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-03-28 18:13:12.000000 ByakuganVisualizer-0.1.0/src/ByakuganVisualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-28 18:13:12.000000 ByakuganVisualizer-0.1.0/src/ByakuganVisualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 18:13:12.000000 ByakuganVisualizer-0.1.0/src/ByakuganVisualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-28 18:13:12.000000 ByakuganVisualizer-0.1.0/src/ByakuganVisualizer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 18:13:12.000000 ByakuganVisualizer-0.1.0/src/ByakuganVisualizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-28 18:13:12.000000 ByakuganVisualizer-0.1.0/src/ByakuganVisualizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-28 18:13:12.000000 ByakuganVisualizer-0.1.0/src/ByakuganVisualizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:13:12.211190 ByakuganVisualizer-0.1.0/src/byakuganvisualizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-28 18:13:00.000000 ByakuganVisualizer-0.1.0/src/byakuganvisualizer/ImageFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-28 18:13:00.000000 ByakuganVisualizer-0.1.0/src/byakuganvisualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-03-28 18:13:00.000000 ByakuganVisualizer-0.1.0/src/byakuganvisualizer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:52:08.243984 ByakuganVisualizer-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-02 21:52:08.243984 ByakuganVisualizer-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-02 21:51:58.000000 ByakuganVisualizer-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-02 21:52:08.247984 ByakuganVisualizer-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-02 21:51:58.000000 ByakuganVisualizer-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:52:08.243984 ByakuganVisualizer-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:52:08.243984 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-02 21:52:08.000000 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-02 21:52:08.000000 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:52:08.000000 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 21:52:08.000000 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:52:08.000000 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-02 21:52:08.000000 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 21:52:08.000000 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:52:08.243984 ByakuganVisualizer-0.2.0/src/byakuganvisualizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-02 21:51:58.000000 ByakuganVisualizer-0.2.0/src/byakuganvisualizer/ImageFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-02 21:51:58.000000 ByakuganVisualizer-0.2.0/src/byakuganvisualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-02 21:51:58.000000 ByakuganVisualizer-0.2.0/src/byakuganvisualizer/main.py
```

### Comparing `ByakuganVisualizer-0.1.0/README.md` & `ByakuganVisualizer-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,99 @@
 # ByakuganVisualizer
 
 <img src="logo/logo.jpeg" width="200">
 
-The ByakuganVisualizer repository hosts a Python tool designed to compare images and highlight their differences. 
+The ByakuganVisualizer repository hosts a Python tool designed to compare images and highlight their differences.
 It simplifies the process of identifying disparities between images, making it ideal for tasks like testing and quality 
-assurance. Additionally, it offers options for customization, which can be helpful for color-blind users.
+assurance.
+Moreover, it offers a color filter that can be used to correct images for **color-blind users**.
 
 
+## Installation
+
+```bash
+pip install byakuganvisualizer
+```
+
 ## Usage 
 
 ```
-usage: byakugan_vision [-h] [--version] --diff DIFF [--filter {red,blue,green,yellow}] [--out_dir OUT_DIR]
+usage: byakugan_vision [-h] [--version] [--diff DIFF] [--filter {red,blue,green,yellow}] [--images IMAGES] [--deuteranomaly DEUTERANOMALY]
+                       [--protanomaly PROTANOMALY] [--out_dir OUT_DIR]
 
-ByakuganVisualizer: Tool for comparing images and highlighting differences.
+ByakuganVisualizer: Tool for correcting the color palett for color blind people and highlighting differences of images.
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
-  --diff DIFF           String containing a list of tuples "Path_To_Image1a,Path_To_Image2a;Path_To_Image1b,Path_To_Image2b...". Each tuple contains two paths to images to be compared.
+  --diff DIFF           String containing a list of tuples "Path_To_Image1a,Path_To_Image2a;Path_To_Image1b,Path_To_Image2b...". Each tuple
+                        contains two paths to images to be compared.
   --filter {red,blue,green,yellow}
                         Filter type (red, blue, green, yellow)
+  --images IMAGES       List of image names to be manipulated by a filter. E.g.: A,B,C,D
+  --deuteranomaly DEUTERANOMALY
+                        Expresses your degree of deuteranomaly, which will be used to correct the image. Default is 1.
+  --protanomaly PROTANOMALY
+                        Expresses your degree of protanomaly, which will be used to correct the image. Default is 1.
   --out_dir OUT_DIR     Output directory for the difference images
+```
+
+## Image Correction for Color Blind People
+
+In the following examples the image is corrected for deuteranomaly and protanomaly. 
+
+**Note:** The float values for deuteranomaly and protanomaly are between 0 and 10. The default value is 1.
+The used algorithm is based on the following paper: https://arxiv.org/abs/1711.10662.
+
+The image used in the example is from the following source:
+https://www.anime2you.de/news/606180/naruto-feiert-20-anime-jubilaeum/
+
+<img src="tests/test_images/naruto.jpg" style="width: 200px">
+
+### Deuteranomaly Correction
+
+```bash
+byakugan_vision --images "tests/test_images/naruto.jpg" --deuteranomaly 2
+```
+
+<img src="tests/test_images/filtered/Filtered_naruto_deuteranomaly_2_protanomaly_0.jpg" style="width: 200px">
+
+### Protanomaly Correction
 
+```bash
+byakugan_vision --images "tests/test_images/naruto.jpg" --protanomaly 2
 ```
 
-## Example
+<img src="tests/test_images/filtered/Filtered_naruto_deuteranomaly_0_protanomaly_2.jpg" style="width: 200px">
+
+### Deuteranomaly and Protanomaly Correction
+
+```bash
+byakugan_vision --images "tests/test_images/naruto.jpg" --deuteranomaly 2 --protanomaly 2
+```
+
+<img src="tests/test_images/filtered/Filtered_naruto_deuteranomaly_2_protanomaly_2.jpg" style="width: 200px">
+
+
+```bash
+byakugan_vision --images "tests/test_images/naruto.jpg" --deuteranomaly 0.5 --protanomaly 0.5
+```
+
+<img src="tests/test_images/filtered/Filtered_naruto_deuteranomaly_0.5_protanomaly_0.5.jpg" style="width: 200px">
+
+### Filter an Image
+
+```bash
+byakugan_vision --images "tests/test_images/naruto.jpg" --filter red
+```
+
+<img src="tests/test_images/filtered/Filtered_naruto_red.jpg" style="width: 200px">
+
+
+## Differences between images
 
 The left image used in the example is from the following source:
 https://www.anime2you.de/news/606180/naruto-feiert-20-anime-jubilaeum/
 
 <div style="display: flex; flex-direction: row;">
     <img src="tests/test_images/naruto.jpg" alt="First Image" style="width: 200px; margin-right: 5px;">
     <img src="tests/test_images/naruto_modified.jpg" alt="Second Image" style="width: 200px; margin-left: 5px;">
```

### Comparing `ByakuganVisualizer-0.1.0/setup.cfg` & `ByakuganVisualizer-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ByakuganVisualizer-0.1.0/setup.py` & `ByakuganVisualizer-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 if __name__ == "__main__":
     try:
         setup(description="The ByakuganVisualizer repository hosts a Python tool designed to compare images and "
                           "highlight their differences. It simplifies the process of identifying disparities between "
                           "images, making it ideal for tasks like testing and quality assurance. Additionally, it "
                           "offers options for customization, which can be helpful for color-blind users.",
               long_description_content_type="text/markdown",
-              version="0.1.0"
+              version="0.2.0"
               )
     except:  # noqa
         print(
             "\n\nAn error occurred while building the project, "
             "please ensure you have the most updated version of setuptools, "
             "setuptools_scm and wheel with:\n"
-            "   pip install -U setuptools setuptools_scm wheel\n\n"
+            "   pip install -U setup tools setuptools_scm wheel\n\n"
         )
         raise
```

### Comparing `ByakuganVisualizer-0.1.0/src/byakuganvisualizer/__init__.py` & `ByakuganVisualizer-0.2.0/src/byakuganvisualizer/__init__.py`

 * *Files identical despite different names*

