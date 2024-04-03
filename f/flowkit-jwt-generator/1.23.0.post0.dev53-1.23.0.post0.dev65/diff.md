# Comparing `tmp/flowkit_jwt_generator-1.23.0.post0.dev53-py3-none-any.whl.zip` & `tmp/flowkit_jwt_generator-1.23.0.post0.dev65-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8532 bytes, number of entries: 10
--rw-r--r--  2.0 unx      507 b- defN 24-Mar-27 09:00 flowkit_jwt_generator/__init__.py
--rw-r--r--  2.0 unx      510 b- defN 24-Mar-27 09:00 flowkit_jwt_generator/_version.py
--rw-r--r--  2.0 unx     1591 b- defN 24-Mar-27 09:00 flowkit_jwt_generator/cli.py
--rw-r--r--  2.0 unx     3405 b- defN 24-Mar-27 09:00 flowkit_jwt_generator/fixtures.py
--rw-r--r--  2.0 unx     9215 b- defN 24-Mar-27 09:00 flowkit_jwt_generator/jwt.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Mar-27 09:00 flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-27 09:00 flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/WHEEL
--rw-r--r--  2.0 unx      138 b- defN 24-Mar-27 09:00 flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 24-Mar-27 09:00 flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      967 b- defN 24-Mar-27 09:00 flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/RECORD
-10 files, 17781 bytes uncompressed, 6834 bytes compressed:  61.6%
+Zip file size: 8535 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      507 b- defN 24-Mar-27 16:31 flowkit_jwt_generator/__init__.py
+-rw-r--r--  2.0 unx      510 b- defN 24-Mar-27 16:31 flowkit_jwt_generator/_version.py
+-rw-r--r--  2.0 unx     1591 b- defN 24-Mar-27 16:31 flowkit_jwt_generator/cli.py
+-rw-r--r--  2.0 unx     3405 b- defN 24-Mar-27 16:31 flowkit_jwt_generator/fixtures.py
+-rw-r--r--  2.0 unx     9215 b- defN 24-Mar-27 16:31 flowkit_jwt_generator/jwt.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Mar-27 16:31 flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-27 16:31 flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/WHEEL
+-rw-r--r--  2.0 unx      138 b- defN 24-Mar-27 16:31 flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 24-Mar-27 16:31 flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      967 b- defN 24-Mar-27 16:31 flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/RECORD
+10 files, 17781 bytes uncompressed, 6837 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: flowkit_jwt_generator/fixtures.py
 Comment: 
 
 Filename: flowkit_jwt_generator/jwt.py
 Comment: 
 
-Filename: flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/METADATA
+Filename: flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/METADATA
 Comment: 
 
-Filename: flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/WHEEL
+Filename: flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/WHEEL
 Comment: 
 
-Filename: flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/entry_points.txt
+Filename: flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/entry_points.txt
 Comment: 
 
-Filename: flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/top_level.txt
+Filename: flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/top_level.txt
 Comment: 
 
-Filename: flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/RECORD
+Filename: flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/RECORD
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
- "date": "2024-03-27T08:57:50+0000",
+ "date": "2024-03-27T16:28:22+0000",
  "dirty": false,
  "error": null,
- "full-revisionid": "a0bf84a710c9d8e5639fe1087e1c1eadde802288",
- "version": "1.23.0.post0.dev53"
+ "full-revisionid": "b5b33a36a66685cc03fc4ec34f8da0b1c8a99fc3",
+ "version": "1.23.0.post0.dev65"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## Comparing `flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/METADATA` & `flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowkit-jwt-generator
-Version: 1.23.0.post0.dev53
+Version: 1.23.0.post0.dev65
 Summary: Common test JWT generator for FlowKit.
 Home-page: https://github.com/Flowminder/FlowKit
 Author: Flowminder Foundation
 Author-email: flowkit@flowminder.org
 Keywords: mobile telecommunications analysis
 Platform: MacOS X
 Platform: Linux
```

## Comparing `flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/RECORD` & `flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 flowkit_jwt_generator/__init__.py,sha256=Vqa2vcGLH7wfO7GXFiSQX2QXctRgwUuM-QG9DJ0HQqk,507
-flowkit_jwt_generator/_version.py,sha256=Gdp4xMRmKwnwI1dktnaEFg_Iq01vj3Yzq6IJouuD1Uc,510
+flowkit_jwt_generator/_version.py,sha256=BtQkZLXDbd4HaclkC_JBECIctRwlK6m8WuAT3kMPHXU,510
 flowkit_jwt_generator/cli.py,sha256=hx88rA2O7sqhQ0EHQTCVrZpcdBLW-qssaaodnpXV1DQ,1591
 flowkit_jwt_generator/fixtures.py,sha256=jVDYkagDNtu_m94ns2F6sDtqMmq1kBygS6DBaMqBGoo,3405
 flowkit_jwt_generator/jwt.py,sha256=R_IjXQwtq3eYOmEVcHp7bOCtBgoGUyUpmrJRKsp1MMc,9215
-flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/METADATA,sha256=0jmiJAHJ87wDywBWhCy4UPYmG33_rEjmb0tjuDN0G1Q,1334
-flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/entry_points.txt,sha256=dn2fWa3YIICO8NuUzecgAhZjHJqa_hCnJkRPdwdYW5I,138
-flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/top_level.txt,sha256=qNfUi5RerckeRiSkJOlGGv5098vruKE2Ck_3TbYyci4,22
-flowkit_jwt_generator-1.23.0.post0.dev53.dist-info/RECORD,,
+flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/METADATA,sha256=PLYsyl9gPJrJeh8H8Po2Ys6gGdRBqq-VbhqTRUq2-Ac,1334
+flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/entry_points.txt,sha256=dn2fWa3YIICO8NuUzecgAhZjHJqa_hCnJkRPdwdYW5I,138
+flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/top_level.txt,sha256=qNfUi5RerckeRiSkJOlGGv5098vruKE2Ck_3TbYyci4,22
+flowkit_jwt_generator-1.23.0.post0.dev65.dist-info/RECORD,,
```

