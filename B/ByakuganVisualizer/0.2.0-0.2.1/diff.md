# Comparing `tmp/ByakuganVisualizer-0.2.0.tar.gz` & `tmp/ByakuganVisualizer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ByakuganVisualizer-0.2.0.tar", last modified: Tue Apr  2 21:52:08 2024, max compression
+gzip compressed data, was "ByakuganVisualizer-0.2.1.tar", last modified: Wed Apr  3 21:29:55 2024, max compression
```

## Comparing `ByakuganVisualizer-0.2.0.tar` & `ByakuganVisualizer-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:52:08.243984 ByakuganVisualizer-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-02 21:52:08.243984 ByakuganVisualizer-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-02 21:51:58.000000 ByakuganVisualizer-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-02 21:52:08.247984 ByakuganVisualizer-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-02 21:51:58.000000 ByakuganVisualizer-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:52:08.243984 ByakuganVisualizer-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:52:08.243984 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-02 21:52:08.000000 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-02 21:52:08.000000 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:52:08.000000 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 21:52:08.000000 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:52:08.000000 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-02 21:52:08.000000 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 21:52:08.000000 ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:52:08.243984 ByakuganVisualizer-0.2.0/src/byakuganvisualizer/
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-02 21:51:58.000000 ByakuganVisualizer-0.2.0/src/byakuganvisualizer/ImageFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-02 21:51:58.000000 ByakuganVisualizer-0.2.0/src/byakuganvisualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-04-02 21:51:58.000000 ByakuganVisualizer-0.2.0/src/byakuganvisualizer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:29:55.476952 ByakuganVisualizer-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-03 21:29:55.476952 ByakuganVisualizer-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-03 21:29:47.000000 ByakuganVisualizer-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-03 21:29:55.476952 ByakuganVisualizer-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-03 21:29:47.000000 ByakuganVisualizer-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:29:55.472952 ByakuganVisualizer-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:29:55.476952 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-03 21:29:55.000000 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-03 21:29:55.000000 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:29:55.000000 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 21:29:55.000000 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:29:55.000000 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 21:29:55.000000 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 21:29:55.000000 ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:29:55.476952 ByakuganVisualizer-0.2.1/src/byakuganvisualizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-03 21:29:47.000000 ByakuganVisualizer-0.2.1/src/byakuganvisualizer/Byakugan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-03 21:29:47.000000 ByakuganVisualizer-0.2.1/src/byakuganvisualizer/ImageFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-03 21:29:47.000000 ByakuganVisualizer-0.2.1/src/byakuganvisualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-03 21:29:47.000000 ByakuganVisualizer-0.2.1/src/byakuganvisualizer/main.py
```

### Comparing `ByakuganVisualizer-0.2.0/PKG-INFO` & `ByakuganVisualizer-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ByakuganVisualizer
-Version: 0.2.0
+Version: 0.2.1
 Summary: The ByakuganVisualizer repository hosts a Python tool designed to compare images and highlight their differences. It simplifies the process of identifying disparities between images, making it ideal for tasks like testing and quality assurance. Additionally, it offers options for customization, which can be helpful for color-blind users.
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: HokageM
 Author-email: m.trzaska663@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -27,14 +27,16 @@
 
 ```bash
 pip install byakuganvisualizer
 ```
 
 ## Usage 
 
+### Command Line Interface
+
 ```
 usage: byakugan_vision [-h] [--version] [--diff DIFF] [--filter {red,blue,green,yellow}] [--images IMAGES] [--deuteranomaly DEUTERANOMALY]
                        [--protanomaly PROTANOMALY] [--out_dir OUT_DIR]
 
 ByakuganVisualizer: Tool for correcting the color palett for color blind people and highlighting differences of images.
 
 options:
@@ -48,17 +50,29 @@
   --deuteranomaly DEUTERANOMALY
                         Expresses your degree of deuteranomaly, which will be used to correct the image. Default is 1.
   --protanomaly PROTANOMALY
                         Expresses your degree of protanomaly, which will be used to correct the image. Default is 1.
   --out_dir OUT_DIR     Output directory for the difference images
 ```
 
+### Python API
+
+Please read the API documentation for the classes `Byakugan` and `ImageFilter` for more information.
+You can simply import the classes as follows:
+
+```python
+from byakuganvisualizer.Byakugan import Byakugan
+from byakuganvisualizer.ImageFilter import ImageFilter
+```
+
+
 ## Image Correction for Color Blind People
 
 In the following examples the image is corrected for deuteranomaly and protanomaly. 
+Correction in this context means that the image is adjusted to be more distinguishable for color-blind people.
 
 **Note:** The float values for deuteranomaly and protanomaly are between 0 and 10. The default value is 1.
 The used algorithm is based on the following paper: https://arxiv.org/abs/1711.10662.
 
 The image used in the example is from the following source:
 https://www.anime2you.de/news/606180/naruto-feiert-20-anime-jubilaeum/
 
@@ -159,7 +173,18 @@
 ### Yellow Filtered Difference
 
 ```bash
 byakugan_vision --diff "tests/test_images/naruto.jpg,tests/test_images/naruto_modified.jpg" --filter yellow --out_dir tests/test_images/diff
 ```
 
 <img src="tests/test_images/diff/Diff_naruto_naruto_modified_yellow.jpg" style="width: 200px">
+
+## Byakugan
+
+The [Bykugan](https://naruto.fandom.com/wiki/Byakugan) from Naruto is a powerful ability that grants users the ability 
+to see through objects, detect chakra, and perceive long distances, but users are born blind, relying solely on this 
+special vision.
+
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `ByakuganVisualizer-0.2.0/README.md` & `ByakuganVisualizer-0.2.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 ```bash
 pip install byakuganvisualizer
 ```
 
 ## Usage 
 
+### Command Line Interface
+
 ```
 usage: byakugan_vision [-h] [--version] [--diff DIFF] [--filter {red,blue,green,yellow}] [--images IMAGES] [--deuteranomaly DEUTERANOMALY]
                        [--protanomaly PROTANOMALY] [--out_dir OUT_DIR]
 
 ByakuganVisualizer: Tool for correcting the color palett for color blind people and highlighting differences of images.
 
 options:
@@ -33,17 +35,29 @@
   --deuteranomaly DEUTERANOMALY
                         Expresses your degree of deuteranomaly, which will be used to correct the image. Default is 1.
   --protanomaly PROTANOMALY
                         Expresses your degree of protanomaly, which will be used to correct the image. Default is 1.
   --out_dir OUT_DIR     Output directory for the difference images
 ```
 
+### Python API
+
+Please read the API documentation for the classes `Byakugan` and `ImageFilter` for more information.
+You can simply import the classes as follows:
+
+```python
+from byakuganvisualizer.Byakugan import Byakugan
+from byakuganvisualizer.ImageFilter import ImageFilter
+```
+
+
 ## Image Correction for Color Blind People
 
 In the following examples the image is corrected for deuteranomaly and protanomaly. 
+Correction in this context means that the image is adjusted to be more distinguishable for color-blind people.
 
 **Note:** The float values for deuteranomaly and protanomaly are between 0 and 10. The default value is 1.
 The used algorithm is based on the following paper: https://arxiv.org/abs/1711.10662.
 
 The image used in the example is from the following source:
 https://www.anime2you.de/news/606180/naruto-feiert-20-anime-jubilaeum/
 
@@ -143,8 +157,19 @@
 
 ### Yellow Filtered Difference
 
 ```bash
 byakugan_vision --diff "tests/test_images/naruto.jpg,tests/test_images/naruto_modified.jpg" --filter yellow --out_dir tests/test_images/diff
 ```
 
-<img src="tests/test_images/diff/Diff_naruto_naruto_modified_yellow.jpg" style="width: 200px">
+<img src="tests/test_images/diff/Diff_naruto_naruto_modified_yellow.jpg" style="width: 200px">
+
+## Byakugan
+
+The [Bykugan](https://naruto.fandom.com/wiki/Byakugan) from Naruto is a powerful ability that grants users the ability 
+to see through objects, detect chakra, and perceive long distances, but users are born blind, relying solely on this 
+special vision.
+
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `ByakuganVisualizer-0.2.0/setup.cfg` & `ByakuganVisualizer-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ByakuganVisualizer-0.2.0/setup.py` & `ByakuganVisualizer-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 if __name__ == "__main__":
     try:
         setup(description="The ByakuganVisualizer repository hosts a Python tool designed to compare images and "
                           "highlight their differences. It simplifies the process of identifying disparities between "
                           "images, making it ideal for tasks like testing and quality assurance. Additionally, it "
                           "offers options for customization, which can be helpful for color-blind users.",
               long_description_content_type="text/markdown",
-              version="0.2.0"
+              version="0.2.1"
               )
     except:  # noqa
         print(
             "\n\nAn error occurred while building the project, "
             "please ensure you have the most updated version of setuptools, "
             "setuptools_scm and wheel with:\n"
             "   pip install -U setup tools setuptools_scm wheel\n\n"
```

### Comparing `ByakuganVisualizer-0.2.0/src/ByakuganVisualizer.egg-info/PKG-INFO` & `ByakuganVisualizer-0.2.1/src/ByakuganVisualizer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ByakuganVisualizer
-Version: 0.2.0
+Version: 0.2.1
 Summary: The ByakuganVisualizer repository hosts a Python tool designed to compare images and highlight their differences. It simplifies the process of identifying disparities between images, making it ideal for tasks like testing and quality assurance. Additionally, it offers options for customization, which can be helpful for color-blind users.
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: HokageM
 Author-email: m.trzaska663@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -27,14 +27,16 @@
 
 ```bash
 pip install byakuganvisualizer
 ```
 
 ## Usage 
 
+### Command Line Interface
+
 ```
 usage: byakugan_vision [-h] [--version] [--diff DIFF] [--filter {red,blue,green,yellow}] [--images IMAGES] [--deuteranomaly DEUTERANOMALY]
                        [--protanomaly PROTANOMALY] [--out_dir OUT_DIR]
 
 ByakuganVisualizer: Tool for correcting the color palett for color blind people and highlighting differences of images.
 
 options:
@@ -48,17 +50,29 @@
   --deuteranomaly DEUTERANOMALY
                         Expresses your degree of deuteranomaly, which will be used to correct the image. Default is 1.
   --protanomaly PROTANOMALY
                         Expresses your degree of protanomaly, which will be used to correct the image. Default is 1.
   --out_dir OUT_DIR     Output directory for the difference images
 ```
 
+### Python API
+
+Please read the API documentation for the classes `Byakugan` and `ImageFilter` for more information.
+You can simply import the classes as follows:
+
+```python
+from byakuganvisualizer.Byakugan import Byakugan
+from byakuganvisualizer.ImageFilter import ImageFilter
+```
+
+
 ## Image Correction for Color Blind People
 
 In the following examples the image is corrected for deuteranomaly and protanomaly. 
+Correction in this context means that the image is adjusted to be more distinguishable for color-blind people.
 
 **Note:** The float values for deuteranomaly and protanomaly are between 0 and 10. The default value is 1.
 The used algorithm is based on the following paper: https://arxiv.org/abs/1711.10662.
 
 The image used in the example is from the following source:
 https://www.anime2you.de/news/606180/naruto-feiert-20-anime-jubilaeum/
 
@@ -159,7 +173,18 @@
 ### Yellow Filtered Difference
 
 ```bash
 byakugan_vision --diff "tests/test_images/naruto.jpg,tests/test_images/naruto_modified.jpg" --filter yellow --out_dir tests/test_images/diff
 ```
 
 <img src="tests/test_images/diff/Diff_naruto_naruto_modified_yellow.jpg" style="width: 200px">
+
+## Byakugan
+
+The [Bykugan](https://naruto.fandom.com/wiki/Byakugan) from Naruto is a powerful ability that grants users the ability 
+to see through objects, detect chakra, and perceive long distances, but users are born blind, relying solely on this 
+special vision.
+
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `ByakuganVisualizer-0.2.0/src/byakuganvisualizer/ImageFilter.py` & `ByakuganVisualizer-0.2.1/src/byakuganvisualizer/ImageFilter.py`

 * *Files identical despite different names*

### Comparing `ByakuganVisualizer-0.2.0/src/byakuganvisualizer/__init__.py` & `ByakuganVisualizer-0.2.1/src/byakuganvisualizer/__init__.py`

 * *Files identical despite different names*

