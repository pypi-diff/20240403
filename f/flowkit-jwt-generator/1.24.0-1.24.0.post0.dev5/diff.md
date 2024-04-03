# Comparing `tmp/flowkit_jwt_generator-1.24.0-py3-none-any.whl.zip` & `tmp/flowkit_jwt_generator-1.24.0.post0.dev5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8389 bytes, number of entries: 10
--rw-r--r--  2.0 unx      507 b- defN 24-Apr-03 13:45 flowkit_jwt_generator/__init__.py
--rw-r--r--  2.0 unx      498 b- defN 24-Apr-03 13:45 flowkit_jwt_generator/_version.py
--rw-r--r--  2.0 unx     1591 b- defN 24-Apr-03 13:45 flowkit_jwt_generator/cli.py
--rw-r--r--  2.0 unx     3405 b- defN 24-Apr-03 13:45 flowkit_jwt_generator/fixtures.py
--rw-r--r--  2.0 unx     9215 b- defN 24-Apr-03 13:45 flowkit_jwt_generator/jwt.py
--rw-r--r--  2.0 unx     1322 b- defN 24-Apr-03 13:45 flowkit_jwt_generator-1.24.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 13:45 flowkit_jwt_generator-1.24.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      138 b- defN 24-Apr-03 13:45 flowkit_jwt_generator-1.24.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-03 13:45 flowkit_jwt_generator-1.24.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      907 b- defN 24-Apr-03 13:45 flowkit_jwt_generator-1.24.0.dist-info/RECORD
-10 files, 17697 bytes uncompressed, 6811 bytes compressed:  61.5%
+Zip file size: 8523 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-03 17:24 flowkit_jwt_generator/__init__.py
+-rw-r--r--  2.0 unx      509 b- defN 24-Apr-03 17:24 flowkit_jwt_generator/_version.py
+-rw-r--r--  2.0 unx     1591 b- defN 24-Apr-03 17:24 flowkit_jwt_generator/cli.py
+-rw-r--r--  2.0 unx     3405 b- defN 24-Apr-03 17:24 flowkit_jwt_generator/fixtures.py
+-rw-r--r--  2.0 unx     9215 b- defN 24-Apr-03 17:24 flowkit_jwt_generator/jwt.py
+-rw-r--r--  2.0 unx     1333 b- defN 24-Apr-03 17:24 flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 17:24 flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/WHEEL
+-rw-r--r--  2.0 unx      138 b- defN 24-Apr-03 17:24 flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-03 17:24 flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      962 b- defN 24-Apr-03 17:24 flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/RECORD
+10 files, 17774 bytes uncompressed, 6835 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: flowkit_jwt_generator/fixtures.py
 Comment: 
 
 Filename: flowkit_jwt_generator/jwt.py
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.dist-info/METADATA
+Filename: flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/METADATA
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.dist-info/WHEEL
+Filename: flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/WHEEL
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.dist-info/entry_points.txt
+Filename: flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/entry_points.txt
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.dist-info/top_level.txt
+Filename: flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/top_level.txt
 Comment: 
 
-Filename: flowkit_jwt_generator-1.24.0.dist-info/RECORD
+Filename: flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flowkit_jwt_generator/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-04-03T14:07:56+0100",
+ "date": "2024-04-03T17:21:49+0000",
  "dirty": false,
  "error": null,
- "full-revisionid": "09a98be7da37396ebad8bf0f4bd82906e32fe59d",
- "version": "1.24.0"
+ "full-revisionid": "c66bdfecb07382c6b69d6f73153359b4c5f1bb22",
+ "version": "1.24.0.post0.dev5"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## Comparing `flowkit_jwt_generator-1.24.0.dist-info/METADATA` & `flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowkit-jwt-generator
-Version: 1.24.0
+Version: 1.24.0.post0.dev5
 Summary: Common test JWT generator for FlowKit.
 Home-page: https://github.com/Flowminder/FlowKit
 Author: Flowminder Foundation
 Author-email: flowkit@flowminder.org
 Keywords: mobile telecommunications analysis
 Platform: MacOS X
 Platform: Linux
```

## Comparing `flowkit_jwt_generator-1.24.0.dist-info/RECORD` & `flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 flowkit_jwt_generator/__init__.py,sha256=Vqa2vcGLH7wfO7GXFiSQX2QXctRgwUuM-QG9DJ0HQqk,507
-flowkit_jwt_generator/_version.py,sha256=YHWhct7t0X887kBtm8WTbeGW8qMssWoXSk0as4k5mSw,498
+flowkit_jwt_generator/_version.py,sha256=Sb7POz5GY9NBkNrj2tvLh6g_rQ9wuL_SysMbk_nQrao,509
 flowkit_jwt_generator/cli.py,sha256=hx88rA2O7sqhQ0EHQTCVrZpcdBLW-qssaaodnpXV1DQ,1591
 flowkit_jwt_generator/fixtures.py,sha256=jVDYkagDNtu_m94ns2F6sDtqMmq1kBygS6DBaMqBGoo,3405
 flowkit_jwt_generator/jwt.py,sha256=R_IjXQwtq3eYOmEVcHp7bOCtBgoGUyUpmrJRKsp1MMc,9215
-flowkit_jwt_generator-1.24.0.dist-info/METADATA,sha256=TUglrThCGnu_IY_GI1B36RfSo5pIBa0koO148RvXiQ8,1322
-flowkit_jwt_generator-1.24.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-flowkit_jwt_generator-1.24.0.dist-info/entry_points.txt,sha256=dn2fWa3YIICO8NuUzecgAhZjHJqa_hCnJkRPdwdYW5I,138
-flowkit_jwt_generator-1.24.0.dist-info/top_level.txt,sha256=qNfUi5RerckeRiSkJOlGGv5098vruKE2Ck_3TbYyci4,22
-flowkit_jwt_generator-1.24.0.dist-info/RECORD,,
+flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/METADATA,sha256=k4hvWBkXcKc1ZLMb2hCnOGQdVjVYH8PbkcyjN2UqPK4,1333
+flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/entry_points.txt,sha256=dn2fWa3YIICO8NuUzecgAhZjHJqa_hCnJkRPdwdYW5I,138
+flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/top_level.txt,sha256=qNfUi5RerckeRiSkJOlGGv5098vruKE2Ck_3TbYyci4,22
+flowkit_jwt_generator-1.24.0.post0.dev5.dist-info/RECORD,,
```

