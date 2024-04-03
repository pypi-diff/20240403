# Comparing `tmp/raw-image-converter-1.1.1.tar.gz` & `tmp/raw-image-converter-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raw-image-converter-1.1.1.tar", last modified: Thu Oct  5 22:18:40 2023, max compression
+gzip compressed data, was "raw-image-converter-1.1.2.tar", last modified: Wed Apr  3 20:55:53 2024, max compression
```

## Comparing `raw-image-converter-1.1.1.tar` & `raw-image-converter-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 22:18:40.109003 raw-image-converter-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-10-05 22:18:28.000000 raw-image-converter-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2023-10-05 22:18:40.109003 raw-image-converter-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2023-10-05 22:18:28.000000 raw-image-converter-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 22:18:40.109003 raw-image-converter-1.1.1/raw_image_converter/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-10-05 22:18:28.000000 raw-image-converter-1.1.1/raw_image_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2023-10-05 22:18:28.000000 raw-image-converter-1.1.1/raw_image_converter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2023-10-05 22:18:28.000000 raw-image-converter-1.1.1/raw_image_converter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 22:18:40.109003 raw-image-converter-1.1.1/raw_image_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2023-10-05 22:18:40.000000 raw-image-converter-1.1.1/raw_image_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-10-05 22:18:40.000000 raw-image-converter-1.1.1/raw_image_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 22:18:40.000000 raw-image-converter-1.1.1/raw_image_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-05 22:18:40.000000 raw-image-converter-1.1.1/raw_image_converter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-10-05 22:18:40.000000 raw-image-converter-1.1.1/raw_image_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-05 22:18:40.000000 raw-image-converter-1.1.1/raw_image_converter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-05 22:18:40.109003 raw-image-converter-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-10-05 22:18:28.000000 raw-image-converter-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 22:18:40.109003 raw-image-converter-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-10-05 22:18:28.000000 raw-image-converter-1.1.1/tests/test_utils_calculate_image_dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-10-05 22:18:28.000000 raw-image-converter-1.1.1/tests/test_utils_check_file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-10-05 22:18:28.000000 raw-image-converter-1.1.1/tests/test_utils_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2023-10-05 22:18:28.000000 raw-image-converter-1.1.1/tests/test_utils_split_file_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:55:53.238681 raw-image-converter-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-03 20:55:53.238681 raw-image-converter-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:55:53.234681 raw-image-converter-1.1.2/raw_image_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/raw_image_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/raw_image_converter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/raw_image_converter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:55:53.234681 raw-image-converter-1.1.2/raw_image_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-03 20:55:53.000000 raw-image-converter-1.1.2/raw_image_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-03 20:55:53.000000 raw-image-converter-1.1.2/raw_image_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:55:53.000000 raw-image-converter-1.1.2/raw_image_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 20:55:53.000000 raw-image-converter-1.1.2/raw_image_converter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 20:55:53.000000 raw-image-converter-1.1.2/raw_image_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 20:55:53.000000 raw-image-converter-1.1.2/raw_image_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:55:53.238681 raw-image-converter-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:55:53.234681 raw-image-converter-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/tests/test_utils_calculate_image_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/tests/test_utils_check_file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/tests/test_utils_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-03 20:55:49.000000 raw-image-converter-1.1.2/tests/test_utils_split_file_extension.py
```

### Comparing `raw-image-converter-1.1.1/LICENSE` & `raw-image-converter-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raw-image-converter-1.1.1/raw_image_converter/__main__.py` & `raw-image-converter-1.1.2/raw_image_converter/__main__.py`

 * *Files identical despite different names*

### Comparing `raw-image-converter-1.1.1/raw_image_converter/utils.py` & `raw-image-converter-1.1.2/raw_image_converter/utils.py`

 * *Files identical despite different names*

### Comparing `raw-image-converter-1.1.1/raw_image_converter.egg-info/SOURCES.txt` & `raw-image-converter-1.1.2/raw_image_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raw-image-converter-1.1.1/setup.py` & `raw-image-converter-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="raw-image-converter",
-    version="1.1.1",
+    version="1.1.2",
     description="Batch conversions of raw images",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/achimoraites/Python-Image-Converter",
     author="Achilles Moraites",
     author_email="achimoraites@yahoo.gr",
     license="MIT",
@@ -22,15 +22,15 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         'Topic :: Utilities',
     ],
     keywords='cli, converter, raw, images',
     packages=["raw_image_converter"],
-    install_requires=["numpy==1.22.3", "rawpy==0.17.1",
-                      "imageio==2.16.2", "Pillow==10.0.1", "colorama==0.4.6"],
+    install_requires=["numpy==1.26.4", "rawpy==0.19.1",
+                      "imageio==2.16.2", "Pillow==10.3.0", "colorama==0.4.6"],
     entry_points={
         "console_scripts": [
             "raw_image_converter=raw_image_converter.__main__:main",
         ]
     },
 )
```

### Comparing `raw-image-converter-1.1.1/tests/test_utils_calculate_image_dimension.py` & `raw-image-converter-1.1.2/tests/test_utils_calculate_image_dimension.py`

 * *Files identical despite different names*

### Comparing `raw-image-converter-1.1.1/tests/test_utils_check_file_type.py` & `raw-image-converter-1.1.2/tests/test_utils_check_file_type.py`

 * *Files identical despite different names*

### Comparing `raw-image-converter-1.1.1/tests/test_utils_message.py` & `raw-image-converter-1.1.2/tests/test_utils_message.py`

 * *Files identical despite different names*

### Comparing `raw-image-converter-1.1.1/tests/test_utils_split_file_extension.py` & `raw-image-converter-1.1.2/tests/test_utils_split_file_extension.py`

 * *Files identical despite different names*

