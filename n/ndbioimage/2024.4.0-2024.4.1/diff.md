# Comparing `tmp/ndbioimage-2024.4.0.tar.gz` & `tmp/ndbioimage-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndbioimage-2024.4.0.tar", max compression
+gzip compressed data, was "ndbioimage-2024.4.1.tar", max compression
```

## Comparing `ndbioimage-2024.4.0.tar` & `ndbioimage-2024.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.4.0/LICENSE
--rw-r--r--   0        0        0     2608 2023-11-21 15:08:51.110664 ndbioimage-2024.4.0/README.md
--rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.4.0/ndbioimage/.DS_Store
--rw-r--r--   0        0        0  1333137 2022-09-20 11:13:05.926176 ndbioimage-2024.4.0/ndbioimage/AiryScan.xml
--rw-r--r--   0        0        0    39417 2022-08-02 08:12:58.529165 ndbioimage-2024.4.0/ndbioimage/Elyra_test.xml
--rw-r--r--   0        0        0    50692 2023-05-11 15:16:04.296888 ndbioimage-2024.4.0/ndbioimage/Elyra_test2.xml
--rwxr-xr-x   0        0        0    51234 2024-04-02 16:23:58.720136 ndbioimage-2024.4.0/ndbioimage/__init__.py
--rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.4.0/ndbioimage/jvm.py
--rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.4.0/ndbioimage/readers/__init__.py
--rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.4.0/ndbioimage/readers/bfread.py
--rw-r--r--   0        0        0    28629 2024-04-02 16:23:36.764150 ndbioimage-2024.4.0/ndbioimage/readers/cziread.py
--rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.4.0/ndbioimage/readers/fijiread.py
--rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.4.0/ndbioimage/readers/ndread.py
--rw-r--r--   0        0        0     6381 2024-03-29 16:56:03.400728 ndbioimage-2024.4.0/ndbioimage/readers/seqread.py
--rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.4.0/ndbioimage/readers/tifread.py
--rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.4.0/ndbioimage/transform.txt
--rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.4.0/ndbioimage/transforms.py
--rw-r--r--   0        0        0     1010 2024-04-02 16:19:40.692305 ndbioimage-2024.4.0/pyproject.toml
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 ndbioimage-2024.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.4.1/LICENSE
+-rw-r--r--   0        0        0     2608 2023-11-21 15:08:51.110664 ndbioimage-2024.4.1/README.md
+-rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.4.1/ndbioimage/.DS_Store
+-rw-r--r--   0        0        0  1333137 2022-09-20 11:13:05.926176 ndbioimage-2024.4.1/ndbioimage/AiryScan.xml
+-rw-r--r--   0        0        0    39417 2022-08-02 08:12:58.529165 ndbioimage-2024.4.1/ndbioimage/Elyra_test.xml
+-rw-r--r--   0        0        0    50692 2023-05-11 15:16:04.296888 ndbioimage-2024.4.1/ndbioimage/Elyra_test2.xml
+-rwxr-xr-x   0        0        0    51242 2024-04-03 08:49:48.656324 ndbioimage-2024.4.1/ndbioimage/__init__.py
+-rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.4.1/ndbioimage/jvm.py
+-rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.4.1/ndbioimage/readers/__init__.py
+-rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.4.1/ndbioimage/readers/bfread.py
+-rw-r--r--   0        0        0    28629 2024-04-02 16:23:36.764150 ndbioimage-2024.4.1/ndbioimage/readers/cziread.py
+-rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.4.1/ndbioimage/readers/fijiread.py
+-rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.4.1/ndbioimage/readers/ndread.py
+-rw-r--r--   0        0        0     6381 2024-03-29 16:56:03.400728 ndbioimage-2024.4.1/ndbioimage/readers/seqread.py
+-rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.4.1/ndbioimage/readers/tifread.py
+-rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.4.1/ndbioimage/transform.txt
+-rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.4.1/ndbioimage/transforms.py
+-rw-r--r--   0        0        0     1010 2024-04-03 08:52:04.192211 ndbioimage-2024.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 ndbioimage-2024.4.1/PKG-INFO
```

### Comparing `ndbioimage-2024.4.0/LICENSE` & `ndbioimage-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.0/README.md` & `ndbioimage-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.0/ndbioimage/.DS_Store` & `ndbioimage-2024.4.1/ndbioimage/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.0/ndbioimage/AiryScan.xml` & `ndbioimage-2024.4.1/ndbioimage/AiryScan.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.0/ndbioimage/Elyra_test.xml` & `ndbioimage-2024.4.1/ndbioimage/Elyra_test.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.0/ndbioimage/Elyra_test2.xml` & `ndbioimage-2024.4.1/ndbioimage/Elyra_test2.xml`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.0/ndbioimage/__init__.py` & `ndbioimage-2024.4.1/ndbioimage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         return super().__getitem__(n)
 
     @cached_property
     def yxczt(self) -> tuple[int, int, int, int, int]:
         return tuple(self[i] for i in 'yxczt')  # type: ignore
 
 
-class CachedPath(Path):
+class CachedPath(type(Path())):
     """ helper class for checking whether a file has changed, used by OmeCache """
 
     def __init__(self, path: Path | str) -> None:
         super().__init__(path)
         if self.exists():
             self._lstat = super().lstat()  # save file metadata like creation time etc.
         else:
```

### Comparing `ndbioimage-2024.4.0/ndbioimage/jvm.py` & `ndbioimage-2024.4.1/ndbioimage/jvm.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.0/ndbioimage/readers/bfread.py` & `ndbioimage-2024.4.1/ndbioimage/readers/bfread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.0/ndbioimage/readers/cziread.py` & `ndbioimage-2024.4.1/ndbioimage/readers/cziread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.0/ndbioimage/readers/fijiread.py` & `ndbioimage-2024.4.1/ndbioimage/readers/fijiread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.0/ndbioimage/readers/ndread.py` & `ndbioimage-2024.4.1/ndbioimage/readers/ndread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.0/ndbioimage/readers/seqread.py` & `ndbioimage-2024.4.1/ndbioimage/readers/seqread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.0/ndbioimage/readers/tifread.py` & `ndbioimage-2024.4.1/ndbioimage/readers/tifread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.0/ndbioimage/transforms.py` & `ndbioimage-2024.4.1/ndbioimage/transforms.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.0/pyproject.toml` & `ndbioimage-2024.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ndbioimage"
-version = "2024.4.0"
+version = "2024.4.1"
 description = "Bio image reading, metadata and some affine registration."
 authors = ["W. Pomp <w.pomp@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["bioformats", "imread", "numpy", "metadata"]
 include = ["transform.txt"]
 repository = "https://github.com/wimpomp/ndbioimage"
```

### Comparing `ndbioimage-2024.4.0/PKG-INFO` & `ndbioimage-2024.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndbioimage
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Bio image reading, metadata and some affine registration.
 Home-page: https://github.com/wimpomp/ndbioimage
 License: GPLv3
 Keywords: bioformats,imread,numpy,metadata
 Author: W. Pomp
 Author-email: w.pomp@nki.nl
 Requires-Python: >=3.8,<4.0
```

