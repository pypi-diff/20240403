# Comparing `tmp/quarkstudio-6.6.2.7-cp312-none-win_amd64.whl.zip` & `tmp/quarkstudio-6.6.2.8-cp312-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 99955 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-01 14:23 quarkstudio-6.6.2.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3210 b- defN 24-Apr-01 14:23 quarkstudio-6.6.2.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-01 14:23 quarkstudio-6.6.2.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       37 b- defN 24-Apr-01 14:23 quarkstudio-6.6.2.7.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-01 14:23 quarkstudio-6.6.2.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      517 b- defN 24-Apr-01 14:23 quarkstudio-6.6.2.7.dist-info/RECORD
--rw-rw-rw-  2.0 fat   144896 b- defN 24-Apr-01 14:23 quark/__init__.pyd
--rw-rw-rw-  2.0 fat    75776 b- defN 24-Apr-01 14:23 quark/setting.pyd
-8 files, 225622 bytes uncompressed, 98785 bytes compressed:  56.2%
+Zip file size: 157004 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-02 12:36 quarkstudio-6.6.2.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3210 b- defN 24-Apr-02 12:36 quarkstudio-6.6.2.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-02 12:36 quarkstudio-6.6.2.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       37 b- defN 24-Apr-02 12:36 quarkstudio-6.6.2.8.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-02 12:36 quarkstudio-6.6.2.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      517 b- defN 24-Apr-02 12:36 quarkstudio-6.6.2.8.dist-info/RECORD
+-rw-rw-rw-  2.0 fat   144384 b- defN 24-Apr-02 12:36 quark/__init__.pyd
+-rw-rw-rw-  2.0 fat   126464 b- defN 24-Apr-02 12:36 quark/cloud.pyd
+-rw-rw-rw-  2.0 fat    75776 b- defN 24-Apr-02 12:36 quark/setting.pyd
+9 files, 351574 bytes uncompressed, 155728 bytes compressed:  55.7%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
-Filename: quarkstudio-6.6.2.7.dist-info/LICENSE
+Filename: quarkstudio-6.6.2.8.dist-info/LICENSE
 Comment: 
 
-Filename: quarkstudio-6.6.2.7.dist-info/METADATA
+Filename: quarkstudio-6.6.2.8.dist-info/METADATA
 Comment: 
 
-Filename: quarkstudio-6.6.2.7.dist-info/WHEEL
+Filename: quarkstudio-6.6.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: quarkstudio-6.6.2.7.dist-info/entry_points.txt
+Filename: quarkstudio-6.6.2.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: quarkstudio-6.6.2.7.dist-info/top_level.txt
+Filename: quarkstudio-6.6.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: quarkstudio-6.6.2.7.dist-info/RECORD
+Filename: quarkstudio-6.6.2.8.dist-info/RECORD
 Comment: 
 
 Filename: quark/__init__.pyd
 Comment: 
 
+Filename: quark/cloud.pyd
+Comment: 
+
 Filename: quark/setting.pyd
 Comment: 
 
 Zip file comment:
```

## Comparing `quarkstudio-6.6.2.7.dist-info/LICENSE` & `quarkstudio-6.6.2.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `quarkstudio-6.6.2.7.dist-info/METADATA` & `quarkstudio-6.6.2.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quarkstudio
-Version: 6.6.2.7
+Version: 6.6.2.8
 Summary: description
 Author-email: YL <fengyl@pku.edu.cn>
 License: MIT License
         
         Copyright (c) 2021 YL Feng
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

## Comparing `quarkstudio-6.6.2.7.dist-info/RECORD` & `quarkstudio-6.6.2.8.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-quarkstudio-6.6.2.7.dist-info/LICENSE,sha256=C3Kj30P434KPtlRtTmqw8y310egFxXCp0sXadioePRs,1085
-quarkstudio-6.6.2.7.dist-info/METADATA,sha256=_FS4gdBepHFXU1_suBD_3zuy8dYYtUN51dyPEdQ7CJ0,3210
-quarkstudio-6.6.2.7.dist-info/WHEEL,sha256=b561VlO0FFA36s33ZiAcL1tul3l99V87_PXMBl3xyiU,100
-quarkstudio-6.6.2.7.dist-info/entry_points.txt,sha256=FeCgtGnAYHTU1GLSewHuHpp2BtExfrjz72bSRGWGfAc,37
-quarkstudio-6.6.2.7.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-quarkstudio-6.6.2.7.dist-info/RECORD,,
+quarkstudio-6.6.2.8.dist-info/LICENSE,sha256=C3Kj30P434KPtlRtTmqw8y310egFxXCp0sXadioePRs,1085
+quarkstudio-6.6.2.8.dist-info/METADATA,sha256=hR8I1c8MC5ry_H2uguaGD7hXYDzqThoXRI1aj3m8b_I,3210
+quarkstudio-6.6.2.8.dist-info/WHEEL,sha256=b561VlO0FFA36s33ZiAcL1tul3l99V87_PXMBl3xyiU,100
+quarkstudio-6.6.2.8.dist-info/entry_points.txt,sha256=FeCgtGnAYHTU1GLSewHuHpp2BtExfrjz72bSRGWGfAc,37
+quarkstudio-6.6.2.8.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+quarkstudio-6.6.2.8.dist-info/RECORD,,
```

