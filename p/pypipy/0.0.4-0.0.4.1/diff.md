# Comparing `tmp/pypipy-0.0.4-py3-none-any.whl.zip` & `tmp/pypipy-0.0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 2327 bytes, number of entries: 6
+Zip file size: 2529 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       19 b- defN 24-Apr-03 02:21 calc/__init__.py
 -rw-rw-rw-  2.0 fat      253 b- defN 24-Apr-03 01:48 calc/calculator.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-Apr-03 01:52 pypipy-0.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      479 b- defN 24-Apr-03 01:52 pypipy-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-03 01:52 pypipy-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-03 01:52 pypipy-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      453 b- defN 24-Apr-03 01:52 pypipy-0.0.4.dist-info/RECORD
-6 files, 2372 bytes uncompressed, 1505 bytes compressed:  36.6%
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-Apr-03 02:26 pypipy-0.0.4.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      483 b- defN 24-Apr-03 02:26 pypipy-0.0.4.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-03 02:26 pypipy-0.0.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Apr-03 02:26 pypipy-0.0.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      534 b- defN 24-Apr-03 02:26 pypipy-0.0.4.1.dist-info/RECORD
+7 files, 2476 bytes uncompressed, 1579 bytes compressed:  36.2%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
+Filename: calc/__init__.py
+Comment: 
+
 Filename: calc/calculator.py
 Comment: 
 
-Filename: pypipy-0.0.4.dist-info/LICENSE
+Filename: pypipy-0.0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: pypipy-0.0.4.dist-info/METADATA
+Filename: pypipy-0.0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: pypipy-0.0.4.dist-info/WHEEL
+Filename: pypipy-0.0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: pypipy-0.0.4.dist-info/top_level.txt
+Filename: pypipy-0.0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pypipy-0.0.4.dist-info/RECORD
+Filename: pypipy-0.0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pypipy-0.0.4.dist-info/LICENSE` & `pypipy-0.0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

