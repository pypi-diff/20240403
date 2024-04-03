# Comparing `tmp/stego-lsb-1.6.0.tar.gz` & `tmp/stego-lsb-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stego-lsb-1.6.0.tar", last modified: Fri Jan 26 02:37:33 2024, max compression
+gzip compressed data, was "stego-lsb-1.6.1.tar", last modified: Wed Apr  3 03:23:14 2024, max compression
```

## Comparing `stego-lsb-1.6.0.tar` & `stego-lsb-1.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-01-26 02:37:33.776782 stego-lsb-1.6.0/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      130 2022-06-05 03:00:51.000000 stego-lsb-1.6.0/AUTHORS.md
--rw-r--r--   0 ryan      (1000) ryan      (1000)     1077 2020-05-10 23:35:29.000000 stego-lsb-1.6.0/LICENSE.md
--rw-r--r--   0 ryan      (1000) ryan      (1000)     9256 2024-01-26 02:37:33.776782 stego-lsb-1.6.0/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     8044 2023-10-05 18:45:30.000000 stego-lsb-1.6.0/README.md
--rw-r--r--   0 ryan      (1000) ryan      (1000)       67 2024-01-26 02:37:33.776782 stego-lsb-1.6.0/setup.cfg
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1703 2024-01-26 02:34:15.000000 stego-lsb-1.6.0/setup.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-01-26 02:37:33.772783 stego-lsb-1.6.0/stego_lsb/
--rwxrwxr-x   0 ryan      (1000) ryan      (1000)     8095 2023-07-18 01:01:17.000000 stego-lsb-1.6.0/stego_lsb/LSBSteg.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1451 2023-07-18 01:00:24.000000 stego-lsb-1.6.0/stego_lsb/StegDetect.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     4038 2024-01-26 01:44:51.000000 stego-lsb-1.6.0/stego_lsb/WavSteg.py
--rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2020-05-10 23:35:29.000000 stego-lsb-1.6.0/stego_lsb/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     6449 2024-01-26 02:33:52.000000 stego-lsb-1.6.0/stego_lsb/bit_manipulation.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     4285 2023-07-18 00:12:47.000000 stego-lsb-1.6.0/stego_lsb/cli.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-01-26 02:37:33.776782 stego-lsb-1.6.0/stego_lsb.egg-info/
--rw-r--r--   0 ryan      (1000) ryan      (1000)     9256 2024-01-26 02:37:33.000000 stego-lsb-1.6.0/stego_lsb.egg-info/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      492 2024-01-26 02:37:33.000000 stego-lsb-1.6.0/stego_lsb.egg-info/SOURCES.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2024-01-26 02:37:33.000000 stego-lsb-1.6.0/stego_lsb.egg-info/dependency_links.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       48 2024-01-26 02:37:33.000000 stego-lsb-1.6.0/stego_lsb.egg-info/entry_points.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-09-01 14:21:06.000000 stego-lsb-1.6.0/stego_lsb.egg-info/not-zip-safe
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      115 2024-01-26 02:37:33.000000 stego-lsb-1.6.0/stego_lsb.egg-info/requires.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       10 2024-01-26 02:37:33.000000 stego-lsb-1.6.0/stego_lsb.egg-info/top_level.txt
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-01-26 02:37:33.776782 stego-lsb-1.6.0/tests/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2740 2024-01-26 02:14:46.000000 stego-lsb-1.6.0/tests/test_bit_manipulation.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3752 2023-10-05 19:02:44.000000 stego-lsb-1.6.0/tests/test_lsbsteg.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     3789 2024-01-26 02:16:51.000000 stego-lsb-1.6.0/tests/test_wavsteg.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-03 03:23:14.607091 stego-lsb-1.6.1/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      130 2022-06-05 03:00:51.000000 stego-lsb-1.6.1/AUTHORS.md
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     1077 2020-05-10 23:35:29.000000 stego-lsb-1.6.1/LICENSE.md
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     9269 2024-04-03 03:23:14.607091 stego-lsb-1.6.1/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     8044 2023-10-05 18:45:30.000000 stego-lsb-1.6.1/README.md
+-rw-r--r--   0 ryan      (1000) ryan      (1000)       67 2024-04-03 03:23:14.607091 stego-lsb-1.6.1/setup.cfg
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1716 2024-04-03 03:08:39.000000 stego-lsb-1.6.1/setup.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-03 03:23:14.607091 stego-lsb-1.6.1/stego_lsb/
+-rwxrwxr-x   0 ryan      (1000) ryan      (1000)     8111 2024-04-03 03:15:25.000000 stego-lsb-1.6.1/stego_lsb/LSBSteg.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1373 2024-04-03 03:18:50.000000 stego-lsb-1.6.1/stego_lsb/StegDetect.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     4038 2024-01-26 01:44:51.000000 stego-lsb-1.6.1/stego_lsb/WavSteg.py
+-rw-r--r--   0 ryan      (1000) ryan      (1000)        0 2020-05-10 23:35:29.000000 stego-lsb-1.6.1/stego_lsb/__init__.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     6449 2024-01-26 02:33:52.000000 stego-lsb-1.6.1/stego_lsb/bit_manipulation.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     4285 2023-07-18 00:12:47.000000 stego-lsb-1.6.1/stego_lsb/cli.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-03 03:23:14.607091 stego-lsb-1.6.1/stego_lsb.egg-info/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     9269 2024-04-03 03:23:14.000000 stego-lsb-1.6.1/stego_lsb.egg-info/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      492 2024-04-03 03:23:14.000000 stego-lsb-1.6.1/stego_lsb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2024-04-03 03:23:14.000000 stego-lsb-1.6.1/stego_lsb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       48 2024-04-03 03:23:14.000000 stego-lsb-1.6.1/stego_lsb.egg-info/entry_points.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-09-01 14:21:06.000000 stego-lsb-1.6.1/stego_lsb.egg-info/not-zip-safe
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      115 2024-04-03 03:23:14.000000 stego-lsb-1.6.1/stego_lsb.egg-info/requires.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       10 2024-04-03 03:23:14.000000 stego-lsb-1.6.1/stego_lsb.egg-info/top_level.txt
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-03 03:23:14.607091 stego-lsb-1.6.1/tests/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2740 2024-01-26 02:14:46.000000 stego-lsb-1.6.1/tests/test_bit_manipulation.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3832 2024-04-03 03:16:27.000000 stego-lsb-1.6.1/tests/test_lsbsteg.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3789 2024-01-26 02:16:51.000000 stego-lsb-1.6.1/tests/test_wavsteg.py
```

### Comparing `stego-lsb-1.6.0/LICENSE.md` & `stego-lsb-1.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stego-lsb-1.6.0/PKG-INFO` & `stego-lsb-1.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: stego-lsb
-Version: 1.6.0
+Version: 1.6.1
 Summary: Least Significant Bit Steganography for bitmap images (.bmp and .png), WAV sound files, and byte sequences. Simple LSB Steganalysis (LSB extraction) for bitmap images.
 Home-page: https://github.com/ragibson/Steganography
 Author: Ryan Gibson
 Author-email: ryan.alex.gibson@gmail.com
 License: MIT
 Keywords: steganography steganalysis
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `stego-lsb-1.6.0/README.md` & `stego-lsb-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `stego-lsb-1.6.0/setup.py` & `stego-lsb-1.6.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "numpy<1.25.0; python_version>='3.8' and python_version<'3.9'"
 ]
 
 setup(
     author="Ryan Gibson",
     author_email="ryan.alex.gibson@gmail.com",
     name="stego-lsb",
-    version="1.6.0",
+    version="1.6.1",
     description="Least Significant Bit Steganography for bitmap images (.bmp "
                 "and .png), WAV sound files, and byte sequences. Simple LSB "
                 "Steganalysis (LSB extraction) for bitmap images.",
     keywords="steganography steganalysis",
     license="MIT",
     long_description=readme,
     long_description_content_type="text/markdown",
@@ -30,15 +30,15 @@
     """,
     package_data={"stego_lsb": ["py.typed"]},
     include_package_data=True,
     packages=find_packages(include=["stego_lsb"]),
     zip_safe=False,
     python_requires=">=3.8",
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `stego-lsb-1.6.0/stego_lsb/LSBSteg.py` & `stego-lsb-1.6.1/stego_lsb/LSBSteg.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
     start = time()
     flattened_color_data = lsb_interleave_list(flattened_color_data, data, num_lsb)
     log.debug(f"{f'{message_size} bytes hidden':<30} in {time() - start:.2f}s")
 
     start = time()
     # PIL expects a sequence of tuples, one per pixel TODO: this expression is too complicated for typing to handle?
-    input_image.putdata(cast(List[int], list(zip(*[iter(flattened_color_data)] * num_channels))))
+    input_image.putdata(cast(List[int], list(zip(*[iter(flattened_color_data)] * num_channels))))  # type: ignore
     log.debug(f"{'Image overwritten':<30} in {time() - start:.2f}s")
     return input_image
 
 
 def hide_data(input_image_path: str, input_file_path: str, steg_image_path: str, num_lsb: int,
               compression_level: int, skip_storage_check: bool = False) -> None:
     """Hides the data from the input file in the input image."""
```

### Comparing `stego-lsb-1.6.0/stego_lsb/StegDetect.py` & `stego-lsb-1.6.1/stego_lsb/StegDetect.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,12 +32,11 @@
 
         image_data = cast(Iterable[Tuple[int, int, int]], image.getdata())
         color_data = [
             (255 * ((rgb[0] & mask) + (rgb[1] & mask) + (rgb[2] & mask)) // (3 * mask),) * 3
             for rgb in image_data
         ]
 
-        # TODO: image.putdata() appears to have buggy typing?
-        image.putdata(color_data)  # type: ignore
+        image.putdata(color_data)
         log.debug(f"Runtime: {time() - start:.2f}s")
         file_name, file_extension = os.path.splitext(image_path)
         image.save(f"{file_name}_{n}LSBs{file_extension}")
```

### Comparing `stego-lsb-1.6.0/stego_lsb/WavSteg.py` & `stego-lsb-1.6.1/stego_lsb/WavSteg.py`

 * *Files identical despite different names*

### Comparing `stego-lsb-1.6.0/stego_lsb/bit_manipulation.py` & `stego-lsb-1.6.1/stego_lsb/bit_manipulation.py`

 * *Files identical despite different names*

### Comparing `stego-lsb-1.6.0/stego_lsb/cli.py` & `stego-lsb-1.6.1/stego_lsb/cli.py`

 * *Files identical despite different names*

### Comparing `stego-lsb-1.6.0/stego_lsb.egg-info/PKG-INFO` & `stego-lsb-1.6.1/stego_lsb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: stego-lsb
-Version: 1.6.0
+Version: 1.6.1
 Summary: Least Significant Bit Steganography for bitmap images (.bmp and .png), WAV sound files, and byte sequences. Simple LSB Steganalysis (LSB extraction) for bitmap images.
 Home-page: https://github.com/ragibson/Steganography
 Author: Ryan Gibson
 Author-email: ryan.alex.gibson@gmail.com
 License: MIT
 Keywords: steganography steganalysis
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `stego-lsb-1.6.0/tests/test_bit_manipulation.py` & `stego-lsb-1.6.1/tests/test_bit_manipulation.py`

 * *Files identical despite different names*

### Comparing `stego-lsb-1.6.0/tests/test_lsbsteg.py` & `stego-lsb-1.6.1/tests/test_lsbsteg.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 import string
 import unittest
 
 
 class TestLSBSteg(unittest.TestCase):
     def write_random_image(self, filename: str, width: int, height: int, num_channels: int) -> None:
         image_data = np.random.randint(0, 256, size=(height, width, num_channels), dtype=np.uint8)
-        with Image.fromarray(image_data) as image:
+        # TODO: Image.fromarray() appears to have buggy typing?
+        with Image.fromarray(image_data) as image:  # type: ignore
             image.save(filename)
 
     def write_random_file(self, filename: str, num_bytes: int) -> None:
         with open(filename, "wb") as file:
             file.write(os.urandom(num_bytes))
 
     def check_random_interleaving(self, num_trials: int = 256, filename_length: int = 5, num_channels: int = 3,
```

### Comparing `stego-lsb-1.6.0/tests/test_wavsteg.py` & `stego-lsb-1.6.1/tests/test_wavsteg.py`

 * *Files identical despite different names*

