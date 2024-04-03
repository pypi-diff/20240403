# Comparing `tmp/simlify-0.0.0.post73-py3-none-any.whl.zip` & `tmp/simlify-0.0.0.post74-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 25739 bytes, number of entries: 23
+Zip file size: 25734 bytes, number of entries: 23
 -rw-r--r--  2.0 unx     1482 b- defN 80-Jan-01 00:00 simlify/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 simlify/data/__init__.py
 -rw-r--r--  2.0 unx      456 b- defN 80-Jan-01 00:00 simlify/data/atomistic.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 simlify/data/backends/__init__.py
 -rw-r--r--  2.0 unx      460 b- defN 80-Jan-01 00:00 simlify/data/backends/_parquet.py
 -rw-r--r--  2.0 unx      368 b- defN 80-Jan-01 00:00 simlify/data/backends/_zarr.py
 -rw-r--r--  2.0 unx      792 b- defN 80-Jan-01 00:00 simlify/data/store.py
@@ -13,13 +13,13 @@
 -rw-r--r--  2.0 unx    12499 b- defN 80-Jan-01 00:00 simlify/simulation/amber/topo.py
 -rw-r--r--  2.0 unx    14822 b- defN 80-Jan-01 00:00 simlify/simulation/contexts.py
 -rw-r--r--  2.0 unx     6505 b- defN 80-Jan-01 00:00 simlify/simulation/prep.py
 -rw-r--r--  2.0 unx     4601 b- defN 80-Jan-01 00:00 simlify/simulation/topo.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 simlify/structure/__init__.py
 -rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 simlify/structure/solvent.py
 -rw-r--r--  2.0 unx      812 b- defN 80-Jan-01 00:00 simlify/utils.py
--rw-r--r--  2.0 unx    10357 b- defN 80-Jan-01 00:00 simlify-0.0.0.post73.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1685 b- defN 80-Jan-01 00:00 simlify-0.0.0.post73.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 simlify-0.0.0.post73.dist-info/WHEEL
--rw-r--r--  2.0 unx      156 b- defN 80-Jan-01 00:00 simlify-0.0.0.post73.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1944 b- defN 16-Jan-01 00:00 simlify-0.0.0.post73.dist-info/RECORD
-23 files, 72926 bytes uncompressed, 22557 bytes compressed:  69.1%
+-rw-r--r--  2.0 unx    10357 b- defN 80-Jan-01 00:00 simlify-0.0.0.post74.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1685 b- defN 80-Jan-01 00:00 simlify-0.0.0.post74.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 simlify-0.0.0.post74.dist-info/WHEEL
+-rw-r--r--  2.0 unx      156 b- defN 80-Jan-01 00:00 simlify-0.0.0.post74.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1944 b- defN 16-Jan-01 00:00 simlify-0.0.0.post74.dist-info/RECORD
+23 files, 72926 bytes uncompressed, 22552 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: simlify/structure/solvent.py
 Comment: 
 
 Filename: simlify/utils.py
 Comment: 
 
-Filename: simlify-0.0.0.post73.dist-info/LICENSE.md
+Filename: simlify-0.0.0.post74.dist-info/LICENSE.md
 Comment: 
 
-Filename: simlify-0.0.0.post73.dist-info/METADATA
+Filename: simlify-0.0.0.post74.dist-info/METADATA
 Comment: 
 
-Filename: simlify-0.0.0.post73.dist-info/WHEEL
+Filename: simlify-0.0.0.post74.dist-info/WHEEL
 Comment: 
 
-Filename: simlify-0.0.0.post73.dist-info/entry_points.txt
+Filename: simlify-0.0.0.post74.dist-info/entry_points.txt
 Comment: 
 
-Filename: simlify-0.0.0.post73.dist-info/RECORD
+Filename: simlify-0.0.0.post74.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `simlify-0.0.0.post73.dist-info/LICENSE.md` & `simlify-0.0.0.post74.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `simlify-0.0.0.post73.dist-info/METADATA` & `simlify-0.0.0.post74.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simlify
-Version: 0.0.0.post73
+Version: 0.0.0.post74
 Summary: Simplify your molecular simulation workflow.
 License: Apache-2.0
 Author: oasci
 Author-email: us@oasci.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: mdanalysis (>=2.6.1,<3.0.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: pint (>=0.23,<0.24)
-Requires-Dist: pyarrow (>=14.0.1,<15.0.0)
+Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: ray (>=2.8.1,<3.0.0)
 Requires-Dist: scipy (>=1.11.4,<2.0.0)
 Requires-Dist: xarray (>=2023.12.0,<2024.0.0)
 Requires-Dist: zarr (>=2.16.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">simlify</h1>
```

## Comparing `simlify-0.0.0.post73.dist-info/RECORD` & `simlify-0.0.0.post74.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 simlify/simulation/amber/topo.py,sha256=9DE6E7rl38f4tiHOaX8O8mXIhic_Ms5SH194Kayw9KA,12499
 simlify/simulation/contexts.py,sha256=I9ldf8YrwneGmnaRCJrCGz1wx9HqQeQiCObQ1OpJ9zU,14822
 simlify/simulation/prep.py,sha256=tg39YkDHU_EuBsIyfVY6PBAq1oIpvdV5AWO9BfhTKKw,6505
 simlify/simulation/topo.py,sha256=M6W35D5VhfkFi_8RylO1SiqzElpli6heilVr5muzNgk,4601
 simlify/structure/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 simlify/structure/solvent.py,sha256=6eRD6y5MvzUHr4DA_sDSwPZV6Ows2_rBay1Gu6sNUzQ,1785
 simlify/utils.py,sha256=kjWSFhr3YqjemxubHXGyuWa4ldnLjXAfS8VliSQaG-E,812
-simlify-0.0.0.post73.dist-info/LICENSE.md,sha256=TPdFRT9tT5cbS7PVfFe7EC3ArioMo8X-KfrbH7sKPIw,10357
-simlify-0.0.0.post73.dist-info/METADATA,sha256=eq-BrTvc9G7GedapP2Wzf73PQ3E96Ty-gzictQfnVBQ,1685
-simlify-0.0.0.post73.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-simlify-0.0.0.post73.dist-info/entry_points.txt,sha256=s3Ds3SE3dGS4I7jrSSg9xYSYtk3tTaUCtbMznGbO2UU,156
-simlify-0.0.0.post73.dist-info/RECORD,,
+simlify-0.0.0.post74.dist-info/LICENSE.md,sha256=TPdFRT9tT5cbS7PVfFe7EC3ArioMo8X-KfrbH7sKPIw,10357
+simlify-0.0.0.post74.dist-info/METADATA,sha256=tWEg_IdYiTsGasjz5HWCkCcsIOOIBtWleBqWmJvQVTI,1685
+simlify-0.0.0.post74.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+simlify-0.0.0.post74.dist-info/entry_points.txt,sha256=s3Ds3SE3dGS4I7jrSSg9xYSYtk3tTaUCtbMznGbO2UU,156
+simlify-0.0.0.post74.dist-info/RECORD,,
```

