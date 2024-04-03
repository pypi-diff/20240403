# Comparing `tmp/antimatter-0.1.8-py3-none-any.whl.zip` & `tmp/antimatter-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 348689 bytes, number of entries: 254
+Zip file size: 349565 bytes, number of entries: 255
 -rw-r--r--  2.0 unx      301 b- defN 20-Apr-16 12:00 antimatter/__init__.py
 -rw-r--r--  2.0 unx    11722 b- defN 20-Apr-16 12:00 antimatter/capsule.py
 -rw-r--r--  2.0 unx      928 b- defN 20-Apr-16 12:00 antimatter/cell_path.py
 -rw-r--r--  2.0 unx     3410 b- defN 20-Apr-16 12:00 antimatter/extra_helper.py
 -rw-r--r--  2.0 unx    10787 b- defN 20-Apr-16 12:00 antimatter/session.py
 -rw-r--r--  2.0 unx      847 b- defN 20-Apr-16 12:00 antimatter/builders/__init__.py
 -rw-r--r--  2.0 unx     1164 b- defN 20-Apr-16 12:00 antimatter/builders/capability.py
@@ -237,20 +237,21 @@
 -rw-r--r--  2.0 unx      935 b- defN 20-Apr-16 12:00 antimatter/session_mixins/encryption_mixin.py
 -rw-r--r--  2.0 unx     5530 b- defN 20-Apr-16 12:00 antimatter/session_mixins/fact_mixin.py
 -rw-r--r--  2.0 unx    10837 b- defN 20-Apr-16 12:00 antimatter/session_mixins/general_mixin.py
 -rw-r--r--  2.0 unx    10426 b- defN 20-Apr-16 12:00 antimatter/session_mixins/identity_provider_mixin.py
 -rw-r--r--  2.0 unx     5583 b- defN 20-Apr-16 12:00 antimatter/session_mixins/policy_rule_mixin.py
 -rw-r--r--  2.0 unx     5092 b- defN 20-Apr-16 12:00 antimatter/session_mixins/read_context_mixin.py
 -rw-r--r--  2.0 unx     2137 b- defN 20-Apr-16 12:00 antimatter/session_mixins/token.py
+-rw-r--r--  2.0 unx     1614 b- defN 20-Apr-16 12:00 antimatter/session_mixins/verification_mixin.py
 -rw-r--r--  2.0 unx     5065 b- defN 20-Apr-16 12:00 antimatter/session_mixins/write_context_mixin.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/session_mixins/serializers/__init__.py
 -rw-r--r--  2.0 unx      868 b- defN 20-Apr-16 12:00 antimatter/session_mixins/serializers/identity_details.py
 -rw-r--r--  2.0 unx       56 b- defN 20-Apr-16 12:00 antimatter/tags/__init__.py
 -rw-r--r--  2.0 unx     1458 b- defN 20-Apr-16 12:00 antimatter/tags/tag.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Apr-16 12:00 antimatter/tests/__init__.py
 -rw-r--r--  2.0 unx     8076 b- defN 20-Apr-16 12:00 antimatter/tests/test_capsule.py
 -rw-r--r--  2.0 unx      281 b- defN 20-Apr-16 12:00 antimatter/tests/test_cell_path.py
--rw-r--r--  2.0 unx     1685 b- defN 24-Mar-29 05:18 antimatter-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-29 05:18 antimatter-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Mar-29 05:18 antimatter-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    25952 b- defN 24-Mar-29 05:18 antimatter-0.1.8.dist-info/RECORD
-254 files, 1945403 bytes uncompressed, 306137 bytes compressed:  84.3%
+-rw-r--r--  2.0 unx     1685 b- defN 24-Mar-29 15:47 antimatter-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-29 15:47 antimatter-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Mar-29 15:47 antimatter-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    26056 b- defN 24-Mar-29 15:47 antimatter-0.1.9.dist-info/RECORD
+255 files, 1947121 bytes uncompressed, 306843 bytes compressed:  84.2%
```

## zipnote {}

```diff
@@ -720,14 +720,17 @@
 
 Filename: antimatter/session_mixins/read_context_mixin.py
 Comment: 
 
 Filename: antimatter/session_mixins/token.py
 Comment: 
 
+Filename: antimatter/session_mixins/verification_mixin.py
+Comment: 
+
 Filename: antimatter/session_mixins/write_context_mixin.py
 Comment: 
 
 Filename: antimatter/session_mixins/serializers/__init__.py
 Comment: 
 
 Filename: antimatter/session_mixins/serializers/identity_details.py
@@ -744,20 +747,20 @@
 
 Filename: antimatter/tests/test_capsule.py
 Comment: 
 
 Filename: antimatter/tests/test_cell_path.py
 Comment: 
 
-Filename: antimatter-0.1.8.dist-info/METADATA
+Filename: antimatter-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: antimatter-0.1.8.dist-info/WHEEL
+Filename: antimatter-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: antimatter-0.1.8.dist-info/top_level.txt
+Filename: antimatter-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: antimatter-0.1.8.dist-info/RECORD
+Filename: antimatter-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `antimatter-0.1.8.dist-info/METADATA` & `antimatter-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimatter
-Version: 0.1.8
+Version: 0.1.9
 Summary: library for interacting with capsules in various formats
 Author: Antimatter Team
 Author-email: support@antimatter.io
 Requires-Python: >=3.10
 Requires-Dist: annotated-types >=0.6
 Requires-Dist: packaging >=21.1
 Requires-Dist: pydantic >=2.0
```

## Comparing `antimatter-0.1.8.dist-info/RECORD` & `antimatter-0.1.9.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -236,19 +236,20 @@
 antimatter/session_mixins/encryption_mixin.py,sha256=U1BUoYTP-cu26cI3fDy__vPbMlWvSeotA9AqGPbUV6s,935
 antimatter/session_mixins/fact_mixin.py,sha256=glHJY7MsVQNCa4iTUaiAN1mcYd9sVS52eM2Y1KOJ9ig,5530
 antimatter/session_mixins/general_mixin.py,sha256=cGy-AVpgdFcB40IHNoPbC_dQ0RhEMMQ3IA4V38HqHnI,10837
 antimatter/session_mixins/identity_provider_mixin.py,sha256=62s3_XHrubKkEGseiojofSRmIIFy7vBkB7XLg7UWKtk,10426
 antimatter/session_mixins/policy_rule_mixin.py,sha256=2lj03Fl0u3ZZ6Vf-6ZuXYZmkdoGHwLbgKlh8xe10PLw,5583
 antimatter/session_mixins/read_context_mixin.py,sha256=plneC6JqMQRvJ1-WbqV_PIjmfpMLyFQX8iTO1bYnL6I,5092
 antimatter/session_mixins/token.py,sha256=HBmyhm71K8aHNLg6aFlMnZUiL448M72uKw95pbyWCkc,2137
+antimatter/session_mixins/verification_mixin.py,sha256=3Rq2lKQf0N-y_sqZIdHedP_5wEzlWIhwUWvAXruSWUM,1614
 antimatter/session_mixins/write_context_mixin.py,sha256=N-winYuRc9hJ6wYMCi8pJjviFs9F53-thGX7Qbpn8SM,5065
 antimatter/session_mixins/serializers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antimatter/session_mixins/serializers/identity_details.py,sha256=X3GgVc3wvg9cblPXadtQLlxSsqaQDENCURNGvgBdQmA,868
 antimatter/tags/__init__.py,sha256=8rV3j87stTslAEtTFLOPjhoQc57kN-gj-DjLtBfFslc,56
 antimatter/tags/tag.py,sha256=xROB-VxhTdveSuGysio61jui3-qsc9kiiV_KrLQNbyQ,1458
 antimatter/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 antimatter/tests/test_capsule.py,sha256=bJUvmSVd0Ifp1E7qFlJygt3n81D6ygo59pX-7DGQUf4,8076
 antimatter/tests/test_cell_path.py,sha256=r-PqBe3xlzvsAy6jZ6YFNh2ABHDEYH3gtcZeKWu3KUc,281
-antimatter-0.1.8.dist-info/METADATA,sha256=97-laIFMNtYtrlRic4KNYXnpe6dT1ynr6cPgIx1-AkU,1685
-antimatter-0.1.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-antimatter-0.1.8.dist-info/top_level.txt,sha256=YjU0PM1vIfQRPJOlRFZHrQLnLbJPOvjJ4McyOFnMGso,11
-antimatter-0.1.8.dist-info/RECORD,,
+antimatter-0.1.9.dist-info/METADATA,sha256=eLG6cyzuVvwu0Q4v-clHQk8w2I6oHY4ZQRslmyIoRw0,1685
+antimatter-0.1.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+antimatter-0.1.9.dist-info/top_level.txt,sha256=YjU0PM1vIfQRPJOlRFZHrQLnLbJPOvjJ4McyOFnMGso,11
+antimatter-0.1.9.dist-info/RECORD,,
```

