# Comparing `tmp/rg3py-0.0.3-py3-none-win_amd64.whl.zip` & `tmp/rg3py-0.0.4-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7949670 bytes, number of entries: 7
--rw-r--r--  2.0 unx      916 b- defN 24-Apr-02 19:25 rg3py/__init__.py
--rw-r--r--  2.0 unx 20607488 b- defN 24-Apr-02 19:26 rg3py/rg3py.pyd
--rw-r--r--  2.0 unx     8063 b- defN 24-Apr-02 19:26 rg3py/rg3py.pyi
--rw-r--r--  2.0 unx     4821 b- defN 24-Apr-02 19:26 rg3py-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       98 b- defN 24-Apr-02 19:26 rg3py-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-02 19:26 rg3py-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      510 b- defN 24-Apr-02 19:26 rg3py-0.0.3.dist-info/RECORD
-7 files, 20621902 bytes uncompressed, 7948782 bytes compressed:  61.5%
+Zip file size: 7949660 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      888 b- defN 24-Apr-03 16:23 rg3py/__init__.py
+-rw-r--r--  2.0 unx 20607488 b- defN 24-Apr-03 16:23 rg3py/rg3py.pyd
+-rw-r--r--  2.0 unx     8063 b- defN 24-Apr-03 16:23 rg3py/rg3py.pyi
+-rw-r--r--  2.0 unx     4821 b- defN 24-Apr-03 16:24 rg3py-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 24-Apr-03 16:24 rg3py-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-03 16:24 rg3py-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      510 b- defN 24-Apr-03 16:24 rg3py-0.0.4.dist-info/RECORD
+7 files, 20621874 bytes uncompressed, 7948772 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: rg3py/rg3py.pyd
 Comment: 
 
 Filename: rg3py/rg3py.pyi
 Comment: 
 
-Filename: rg3py-0.0.3.dist-info/METADATA
+Filename: rg3py-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: rg3py-0.0.3.dist-info/WHEEL
+Filename: rg3py-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: rg3py-0.0.3.dist-info/top_level.txt
+Filename: rg3py-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: rg3py-0.0.3.dist-info/RECORD
+Filename: rg3py-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rg3py/__init__.py

```diff
@@ -1,13 +1,12 @@
 from .rg3py import CppStandard
 from .rg3py import InheritanceVisibility
 from .rg3py import CppEnumEntry
 from .rg3py import CppTypeKind
 from .rg3py import CppEnum
-from .rg3py import CppAlias
 from .rg3py import CppIncludeKind
 from .rg3py import CppIncludeInfo
 from .rg3py import Location
 from .rg3py import CppNamespace
 from .rg3py import TagArgumentType
 from .rg3py import TagArgument
 from .rg3py import Tag
```

## Comparing `rg3py-0.0.3.dist-info/METADATA` & `rg3py-0.0.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rg3py
-Version: 0.0.3
+Version: 0.0.4
 Summary: RG3 is a C/C++ analyzer framework
 Author: DronCode
 Author-email: alexandrleutin@gmail.com
 Platform: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

