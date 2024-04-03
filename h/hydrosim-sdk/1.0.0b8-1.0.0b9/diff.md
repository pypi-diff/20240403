# Comparing `tmp/hydrosim_sdk-1.0.0b8-py3-none-any.whl.zip` & `tmp/hydrosim_sdk-1.0.0b9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8670 bytes, number of entries: 11
+Zip file size: 8639 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Feb-02 06:07 hydrosim_sdk/__init__.py
 -rw-rw-rw-  2.0 fat     1591 b- defN 24-Jan-29 17:05 hydrosim_sdk/ctypes_json.py
 -rw-rw-rw-  2.0 fat     1345 b- defN 24-Jan-28 21:45 hydrosim_sdk/hydrosim_file.py
 -rw-rw-rw-  2.0 fat     4824 b- defN 24-Jan-30 16:36 hydrosim_sdk/hydrosim_sdk.py
--rw-rw-rw-  2.0 fat     3619 b- defN 24-Feb-02 06:52 hydrosim_sdk/hydrosim_struct_base.py
+-rw-rw-rw-  2.0 fat     3562 b- defN 24-Feb-02 07:02 hydrosim_sdk/hydrosim_struct_base.py
 -rw-rw-rw-  2.0 fat     7651 b- defN 24-Feb-02 06:27 hydrosim_sdk/hydrosim_structs.py
--rw-rw-rw-  2.0 fat     1069 b- defN 24-Feb-02 06:56 hydrosim_sdk-1.0.0b8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3039 b- defN 24-Feb-02 06:56 hydrosim_sdk-1.0.0b8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-02 06:56 hydrosim_sdk-1.0.0b8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Feb-02 06:56 hydrosim_sdk-1.0.0b8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      937 b- defN 24-Feb-02 06:56 hydrosim_sdk-1.0.0b8.dist-info/RECORD
-11 files, 24219 bytes uncompressed, 7072 bytes compressed:  70.8%
+-rw-rw-rw-  2.0 fat     1069 b- defN 24-Feb-02 07:04 hydrosim_sdk-1.0.0b9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3039 b- defN 24-Feb-02 07:04 hydrosim_sdk-1.0.0b9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-02 07:04 hydrosim_sdk-1.0.0b9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Feb-02 07:04 hydrosim_sdk-1.0.0b9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      937 b- defN 24-Feb-02 07:04 hydrosim_sdk-1.0.0b9.dist-info/RECORD
+11 files, 24162 bytes uncompressed, 7041 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: hydrosim_sdk/hydrosim_struct_base.py
 Comment: 
 
 Filename: hydrosim_sdk/hydrosim_structs.py
 Comment: 
 
-Filename: hydrosim_sdk-1.0.0b8.dist-info/LICENSE
+Filename: hydrosim_sdk-1.0.0b9.dist-info/LICENSE
 Comment: 
 
-Filename: hydrosim_sdk-1.0.0b8.dist-info/METADATA
+Filename: hydrosim_sdk-1.0.0b9.dist-info/METADATA
 Comment: 
 
-Filename: hydrosim_sdk-1.0.0b8.dist-info/WHEEL
+Filename: hydrosim_sdk-1.0.0b9.dist-info/WHEEL
 Comment: 
 
-Filename: hydrosim_sdk-1.0.0b8.dist-info/top_level.txt
+Filename: hydrosim_sdk-1.0.0b9.dist-info/top_level.txt
 Comment: 
 
-Filename: hydrosim_sdk-1.0.0b8.dist-info/RECORD
+Filename: hydrosim_sdk-1.0.0b9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hydrosim_sdk/hydrosim_struct_base.py

```diff
@@ -1,14 +1,12 @@
 import ctypes
 import json
 from uuid import UUID
 from dtypes.structify import structify
 
-from hydrosim_sdk.ctypes_json import CDataJSONEncoder
-
 
 class HydroSimStructure(ctypes.Structure):
     _pack_ = 1
 
     def __iter__(self):
         for prop in self.__properties__:
             val = getattr(self, prop)
```

## Comparing `hydrosim_sdk-1.0.0b8.dist-info/LICENSE` & `hydrosim_sdk-1.0.0b9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hydrosim_sdk-1.0.0b8.dist-info/METADATA` & `hydrosim_sdk-1.0.0b9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrosim_sdk
-Version: 1.0.0b8
+Version: 1.0.0b9
 Home-page: https://gitlab.com/hydrosim/shared-memory-api/hydrosim-sdk-python
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

